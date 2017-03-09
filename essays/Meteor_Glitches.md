---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-03-09
labels:
  - Software Engineering
  - Meteor
---

## Problem 1: Why won't meteor run
The first problem I encountered with Meteor was while working through the Meteor in 50 mintues tutorial exercise.  Something was acting up and Meteor was returning a JScript compilation error that said I was missing a semicolon.  After reviewing the line of code the error message was referencing, I thought that maybe the error was a result of importing libraries into the meteor application.  After removing the libraries, the error continued to show up when trying to start the application.  This lead me to believe that the error had nothing to do with the procedure of my installations but rather to do with the line of code itself.

On a whim, I tried using var instead of let, and then ran meteor with no compilation errors.  Weird, I thought to myself, why would it accept var but not let?  The solution I eventually was given was that Windows Host Script was being used to compile the Javascript used by Meteor and was not using ECMASpript 6.  To fix this problem, I made IntelliJ the default program to run .js files.

## Problem 2: 6 days to install Meteor Template?
The second problem I encountered with Meteor came when I tried to configure Meteor settings during the Digits part 1 exercise. This problem was tricky to solve, because the solution was hidden from sight, literally.  After unzipping the Meteor template, there were hidden files that did not show up in my files explorer, similar to how the directory AppData is hidden in the Users directory.  To solve this problem, I made sure my files explorer was set to display all files and directories.