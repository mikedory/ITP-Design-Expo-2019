# Design Expo 2017
**Mike Dory**  
**Thursdays, 9:30-12 (2/23 - 4/13)**

## OVERVIEW

Design Expo is an eight-week design challenge for students of [NYU ITP](http://itp.nyu.edu) — seven weeks during the semester, and one after. Students will work in groups to understand, and then respond to, a brief from Microsoft Research (MSR), and then present their work for feedback and iteration. 

---

## Installing

This app is built on [Cactus](https://github.com/koenbok/Cactus), so it's assumed you've already either installed that, or aren't planning on using the handy tools. To install, run:

    sudo pip install cactus

I mean, they say to use `easy_install`, but doing so via Pip in a Virtualenv sucks less.  `¯\_(ツ)_/¯`.


## Using

Your options for building and designing this are the standard Cactus ones.

To build:

    cactus build

When developing:

    cactus watch

To deploy

    cactus deploy

Deploy, in this case, assumes an s3 bucket. You could do this on [Surge](http://surge.sh) or something if that were your jam instead, I bet.


## Requirements

Aside from Python and Cactus, this app uses YUICSSOptimizer for CSS. You can install that with Homebrew:

    brew install yuicompressor

Cactus likes to use the Clojure Compiler for JS, which you could install thusly:

    brew install closure-compiler

That would have made me install Java again on my poor machine, so I have opted to pass, but add `.js` to the `optimize` array in `config.json` if you decide you're braver than I.
