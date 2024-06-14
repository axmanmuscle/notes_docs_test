---
layout: default
title: Intro and To Do
nav_order: 2
---

Let's make a to-do list of what we want to do here.

## Introduction
I'd really love to spend some time actually writing out optimization notes. This will help my own writing be more clear and serve as a resource to look back on (besides just generally being a good thing to spend time on). I'm choosing to do Markdown/Github Pages over Overleaf so that writing and contributing is slightly easier at the cost of the math being slightly more annoying to write. I think this is a small price to pay.

Where do I even start with the field of numerical optimization. I'm very biased but I really do believe this is the most useful/applicable field of applied mathematics. The number of problems that can be posed as a standard optimization program and solved using classical methods seems nearly boundless---there are examples from aeronautical engineering and space to magnetic resonance imaging to RADAR to signal processing. Nearly every field of engineering has problems that can be solved via optimization techniques.

It seems I can write markdown on Overleaf so I'll have a way to contribute remotely. This package also lets me upload papers so this will serve as a repository and get my ass in gear to start doing citations better.

## To Do (Website)
 1. Gotta learn how to make categories and make the website look cleaner.
 2. Probably just get rid of the other layouts and focus on this one, I think this looks the best.
 3. Figure out how to host PDFs on here? Could make up a citation thing as well but that may not be necessary.
 4. Figure out if math is gonna render

## To Do (Math)
 1. Introduction to numerical optimization/calculus?
 2. Norms/Vectors/Matrices
 3. Convexity, strong and strict, Lipschitz, Gradients, these things
 4. *Monotone Operators * 
	 1. __This should be a big section. Focus on this for now__
	 2. Properties
	 3. Resolvents
	 4. Reflected Resolvents
	 5. Connection to Euler
 5. Gradient Descent and step size/Lipschitz things
	 1. Stuff to prove here: optimal step size given strong and strict convexity
 6. Proximal operators
 7. Proximal gradient descent/forward backward splitting
 8. Algorithms
	 1. Newton and Quasi Newton
 9. Line Searches

### Towards This
#### Gradient Descent
Let's talk about the simplest possible first order method - gradient descent. In fact we'll start even simpler and talk about this in one-dimension, so this is just derivative descent or the optiizmation that we all learned in our first calculus classes.

Let $f$ be a function that is differentiable.