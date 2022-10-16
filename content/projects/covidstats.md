---
title: "Covidstats"
type: page
draft: false
---

Android application that makes two separate requests to an open data regularly updated daily (around 6:00 pm) the number of COVID-19 contagions.

REQUEST 1: Number of contagions in a certain province from pandemic start until today.

REQUEST 2: Number of contagions from the beginning of the pandemic to today's day from all Italian provinces.

The data is saved to a file in the system so that we avoid redoing the request to the github repository used:
https://github.com/pcm-dpc/COVID-19

When changing activity the first time, this data is saved to a system file called config.csv.

An intent is then used that sends a bundle containing a string to verify that it is saved correctly.

The first time the application is started in any case a request is made to the repository where the file (about 10MB large) will be downloaded.

Dynamic spinners and a datePickerDialog are used to have a more interactive look and feel, at the same time limiting possible user input errors in case the user is given complete freedom with simple EditTexts

Here is the source code on [github.com](https://github.com/CCCorrado/CovidStats)

