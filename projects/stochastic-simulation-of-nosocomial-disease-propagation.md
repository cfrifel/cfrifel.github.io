---
layout: project
type: project
image: images/netlogo.png
title: Stochastic Simulation of Nosocomial Disease Propagation
permalink: projects/stochastic-simulation-of-nosocomial-disease-propagation
date: 2017
labels:
  - Netlogo
  - Monte Carlo
  - Hospital Simulation
summary: Program a simulation to study HAI propagation characteristics
---
  <img class="ui centered image" src="../images/nlogo-simulation.jpg">

### Background
Hospital Associated Infections (HAIs) are defined as an infection that one contracts from being in a health-care facility.  HAIs account for billions of dollars in health-care costs and are responsible for roughly 99,000 deaths every year within the US [1].  This project focused on developing a computer simulation to model the propagation of HAIs in a hospital setting based on adjustable parameters.

### Overview
We used a programmable modeling environment called NetLogo to construct our hospital simulation.  The layout of the NetLogo model was based off the John A. Burns School of Medicine (JABSOM) SimTiki Simulation Center in order to model an accurate health-care facility.  To model the activities of health-care workers, visitors, and patients in a hospital, we programmed a movement script for these agents in the simulation.  On top of the movement script, we programmed an SIR model to track the infectious state of each agent in the simulation.  In our model, we record the contacts that each agent has with another agent.  If an agent comes within a predetermined distance from another agent in the model, we define this interaction as a contact.  To see the propagation characteristics of HAIs in our model, we introduced a random chance that an agent can become infected after having a contact with an infected agent.  We then conducted Monte Carlo simulations by running our model many times while varying the distance in which we define a contact and the probability of transfer.

Our NetLogo code is hosted on Github <a href="https://github.com/cfrifel/ee496-senior-project">here</a>.


### References
[1] "AHRQ's Efforts to Prevent and Reduce Health Care-Associated Infections." *AHRQ—Agency for Healthcare Research and Quality: Advancing Excellence in Health Care.* U.S. HHS:
Agency for Healthcare Research and Quality, 02 Oct. 2014. Web. 10 May. 2017.
