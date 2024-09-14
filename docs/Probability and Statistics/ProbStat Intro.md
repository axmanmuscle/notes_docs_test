---
layout: default
title: Intro and To Do
nav_order: 1
math: mathjax3
parent: Prob&Stats
---

## Introduction to Probability and Statistics
This will be about _Probability and Statistics_, where I will detail some stuff I find interesting in the probability and statistics region.

## To Do
 1. Introduction to Prob/Stat
 1. Use some stuff from Jem's book esp. difference between probability and statistics
 1. Useful ideas/theorems (LOTUS, Kolmogorov, etc)
 1. MGF/Characteristic Function
 1. Tables of distributions
 1. Tests/likelihood/GLRT?

## Introduction
Probability and statistics play an important role in almost every engineering discipline and application. Noise is present at every level of measurement for every type of application, so estimating parameters from noisy measurements is used everywhere. Just in electrical engineering, this is present in e.g. communications, radar, and imaging.

What I think a lot of books miss is _what_ is the difference between probability and statistics? In my opinion, the answer is simple:

__Probability is about the future. Statistics is about the past.__

By way of example - suppose we have a fair coin. We toss it three times. What is the _probability_ that we get _at least_ two heads? We can enumerate all eight possible outcomes:

 - HHH
 - HHT
 - HTH
 - HTT
 - THH
 - THT
 - TTH
 - TTT

How many of these outcomes have at least two heads? Four! In this case we had information about the _generating phenomenon_ and used it to infer what the future might hold. This was a _probability_ question.

The reverse question might be: A coin was tossed ten times and it was heads 8 times. Do you believe the coin is fair? This is a _statistics_ question. We were given the data and asked to make deductions about the generating phenomenon.

Herein lies the nuance that most probability and statistics courses miss. If you want to do _statistics_ you have to have a firm grasp of _probability_ in the first place.