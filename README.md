# How to Merge Changes from an Upstream Fork

For some projects at Lambda School you may start with a starter iOS project. We recommend that you create branches for work from each cohort (so you don't need to delete a fork and recreate).

You'll need to manually keep your fork up to date with changes in Swift / bug fixes in the starter project.

1. Clone your fork (rename it "<project>-starter"):

		git clone git@github.com:<YOUR-USERNAME>/<YOUR-FORKED-REPO>.git
	
2. Add remote from original repository in your forked repository:

		cd into/cloned/fork-repo
		git remote add upstream git://github.com/LambdaSchool/<STARTER-REPO-YOU-FORKED-FROM>.git
		git fetch upstream
		
3. Updating your fork from original repo to keep up with changes:

		git pull upstream master

## How to Merge Changes from a Fork (Real Links)

1. Clone a forked repository (renamed: "dependency-starter")

		git clone git@github.com:PaulSolt/ios-guided-project-third-party-libraries-and-dependency-management-starter.git dependency-starter

2. Add a remote and fetch upstream changes

		cd dependency-starter
		git remote add upstream git@github.com:LambdaSchool/ios-guided-project-third-party-libraries-and-dependency-management-starter.git
		git fetch upstream

3. Pull upstream changes into master

		git pull upstream master

## New Branches for New Cohorts

At this point you can now create a new branch from `master` and you will have any Xcode project updates or bug fixes to the starter project.

	git checkout master

Checkout a branch for a new cohort 

	git checkout -b iOS9

Push the branch to Github and share URL with students

	git push -u origin iOS9
