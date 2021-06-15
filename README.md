/*
 * SPDX-FileCopyrightText: 2021 Stefan Begerad <stefan@begerad.de>
 *
 * SPDX-License-Identifier: GPL-3.0-or-later
 */
# dede-obc-adapter
The Dede On-board Computer Adapter translates the JSON object from the Dede On-board Computer to the model supported by the data base of the Dede Server. At the end of the day the Dede Map is served at: https://dedriver.org

## Overview
This repository provides a command line interface service for Linux based operating system. As a back end service, this server interacts between Dede On-board Computer and the Dede Map.

## Preparation
Run the following command in your favorite GNU/Linux shell to install dependenies.
```
npm i
```
Checkout the following git repository into this project root directory to enable access to MongoDB data base.
```
git clone https://github.com/dancesWithCycles/dede-mongo.git
```
## Development setup
Run the following command in your favorite GNU/Linux shell if you fancy log messages for debugging.
```
export DEBUG=$DEBUG,dede-obc-adapter
```
Run the following command in your favorite GNU/Linux shell to start the service in development mode.
```
npm run dev
```
## Production deployment
Run the following command in your favorite GNU/Linux shell to start the service for production mode.
```
npm run start
```
