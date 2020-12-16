# mannion-makecents
Repo to collect all data for MakeCents and affiliated git repos and data

The purpose of using submodules is to freeze the repos at the time of submission, but to allow me to continue to work on them. The repos here will be 
updated to the latest commit at the time of submission, and wont update unless I push the latest commits to them.

## How to test MakeCents for grading purposes

Click on the makecents submodule above and clone it, follow the directions in the README

Both repos have an `Issues` tab detailing known bugs and projects I would like to improve on.

## MakeCents submodule

The MakeCents submodule contains all files necessary for running and testing MakeCents, including the Rasa files and the coin prices database. Please
look at the submodule or navigate to [the MakeCents repo](https://github.com/ryanamannion/makecents) for instructions on configuring your environment and
testing MakeCents. Since MakeCents relies on a number of different packages, including `pcgs_scraper` (which I have not yet released on PyPi), I made a
few shell scripts to make it easier to run.

	* `latest-release` handles downloading the latest tarball for pcgs_scraper
	* `makecents-test` handles launching the actions server and rasa x, as well as killing the processes afterwards

## PCGS Scraper submodule

The pscgs_scraper submodule was built from the ground up to scrape and store data on coin desriptions and prices. It is not necessary to clone and install
it for the purposes of grading, and running it to get all the information necessary to run MakeCents takes upwards of 24 hours, so I have supplied the
data in the MakeCents repo
