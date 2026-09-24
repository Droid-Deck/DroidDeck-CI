# DroidDeck CI Releases

This repository is the release target for automated DroidDeck CI builds.

## Purpose

GitHub Actions in the main DroidDeck repository publish an APK here for every pull request, so each pull request has its own release page with the build attached.

## What You Will Find Here

- A prerelease for each pull request, tagged `pr-<number>`
- The APK built from the pull request's latest commit
- Release notes linking back to the source pull request

## Installing

Every build is signed with the same key, so a newer build installs over an older one, whichever pull request it came from, without uninstalling first.

## Notes

- Releases in this repository are generated automatically.
- The APK is replaced each time new commits are pushed to the same pull request.
- The file name carries the pull request number and the first five characters of the commit it was built from.

## Source Repository

Source changes are developed in the main DroidDeck repository and published here as CI release artifacts.
