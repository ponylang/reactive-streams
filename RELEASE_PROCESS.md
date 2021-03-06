# How to cut a reactive_streams release

This document is aimed at members of the Pony team who might be cutting a release of reactive_streams. It serves as a checklist that can take you through doing a release step-by-step.

## Prerequisites

You must have commit access to the reactive_streams repository

## Releasing

Please note that this document was written with the assumption that you are using a clone of the `reactive_streams` repo. You have to be using a clone rather than a fork. It is advised that you do this by making a fresh clone of the `reactive_streams` repo from which you will release.

```bash
git clone git@github.com:ponylang/reactive_streams.git reactive_streams-release-clean
cd reactive_streams-release-clean
```

Before getting started, you will need a number for the version that you will be releasing as well as an agreed upon "golden commit" that will form the basis of the release.

The "golden commit" must be `HEAD` on the `main` branch of this repository. At this time, releasing from any other location is not supported.

In this document, we pretend that the new release version is `0.3.1`. Wherever you see those values, please substitute with your own version.

```bash
git tag release-0.3.1
git push origin release-0.3.1
```
