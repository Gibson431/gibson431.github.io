---
title: 'UTS Rocketry - Meerkat Ground Station'
date: 2019-07-18T17:18:05+01:00
draft: false
cover:
    image : "projects/meerkat/cover.png"
---

## Description

The Meerkat ground station is a ground operations centre for centralising data on a rocketry site.

The system comprises of a physical box that hosts several web UIs that provide data on various subsystems involved in the ground operations.

## Components

### User Interface

#### V1

The first version involved a screen that displayed the status of the systems and a map of personell in the field.

This worked as a static display bust was not flexible enough for the desired use case as there was no way to interact with the system beyond the buttons that were pre-programmed.

| | |
|-|-|
|![real1](/projects/meerkat/real-meerkat.jpeg) | ![real2](/projects/meerkat/real-meerkat2.jpeg)|

#### V2

The second version removed the screen and utilised the wifi card on the Jetson to host an access point.

This access point was used to connect to a [Grafana](https://grafana.com/grafana/) visualiser and a custom map viewer.

By changing it to this version, new pages could be added the the nginx router and functionality could be added in a significantly more modular way.

### RF Network

The network between the ground station and any in-field devices is facilitated by a set of LoRa modules operating in the 915 MHz band.

These devices include any rocket flight computers (eg. [Ibis](/projects/ibis)) and any [recovery trackers](/projects/meerkat-recovery) for personnel.
