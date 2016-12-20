

# This repository contains the source code for the cc-revisionlog solution.

### For being able to run these docker images locally you might need to follow this tutorial: [DED0033 - CC Development Environment Installation Manual](https://bitbucket/projects/ENET/repos/environment/browse/docs/DED0033-Development-environment-installation-manual.md)

The app will be running at [http://localhost:5000](http://localhost:5000), and the results will be at [http://localhost:5001](http://localhost:5001).

Architecture
-----

![Architecture diagram](architecture.png)

* A Python webapp which lets you vote between two options
* A Redis queue which collects new votes
* A .NET worker which consumes votes and stores them in…
* A Postgres database backed by a Docker volume
* A Node.js webapp which shows the results of the voting in real time

