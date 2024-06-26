---
layout: default
title: Building This Website
nav_order: 2
parent: General
---

## Github Pages
I built this website using the Github Pages feature. The theme itself is taken from [this template](https://github.com/vsoch/notes-jekyll)
There were some hurdles I had to overcome once I cloned the repo, and most of them had to do with building the website via Github actions. I used the included `build.yml` in the repo but I needed to add in the following lines:
```
permissions:
  contents: write
```
under the build job. This gives the Github bot permission to push the pages into the repo, or something like that.

Another change I had to make was getting rid of this line:
```
git commit -m "Build $(git rev-parse source | grep -o '^.\{10\}')"
```
Something about that `git rev-parse source` would break. It gave message:
```
fatal: ambiguous argument 'source': unknown revision or path not in the working tree.
```
It's unclear what this was trying to accomplish (I think it was trying to automatically update the build number but I'm not sure from what). 

It looks like I have to manually create a `gh-pages` branch, since that's what the deploy command seems to be looking for.

Okay actually what the hell is this build file doing. This makes no sense. Need to look up workflow stuff in the morning.

Another massive problem I just saw is that all the links so far are to ``/notes-jekyll/`` mirroring the repository name from the creator. Our repo is just named ``/notes/`` so this will cause issues. Figure out how to fix.

I'd bet some stuff has changed with actions since this was written. Go read the documentation for GitHub actions and see if you can fix.

## Just The Docs
All of the above was written specifically for the `notes-jekyll` distribution or theme. I think I'm going to switch over to Just the Docs, which is slightly cleaner and gives me the layout that I like better. 

To get this to work, I needed to do the following.

#### Front Matter
On each post, I needed a front matter that looked like
```
---
layout: default
title: Building This Website
nav_order: 2
---
```
without which the pages didn't compile correctly.

#### Github Actions
Letting the github actions run normally deploys this right to pages. 

#### Posts
All posts are just located in the `docs` folder, just like the original repo is set up.