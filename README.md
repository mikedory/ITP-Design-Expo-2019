# Design Expo 2019
**Mike Dory**  
**Wednesdays, 9:30-12 (2/20 - 4/10)**

## OVERVIEW

Design Expo is an eight-week design challenge for students of [NYU ITP](http://itp.nyu.edu) — seven weeks during the semester, and one after. Students will work in groups to understand, and then respond to, a brief from Microsoft Research (MSR), and then present their work for feedback and iteration. 

---

## Installing

This app is built on [Cactus](https://github.com/koenbok/Cactus), so it's assumed you've already either installed that, or aren't planning on using the handy tools. To install, run:

    sudo pip install cactus


## Using

Your options for building and designing this are the standard Cactus ones.

To build:

    cactus build

When developing:

    cactus watch

To deploy

    cactus deploy

Deploy, in this case, assumes an s3 bucket. You could do this on pretty much anything that does nice static hosting tho.


## Requirements

Aside from Python and Cactus, this app uses YUICSSOptimizer for CSS. You can install that with Homebrew:

    brew install yuicompressor

Cactus likes to use the Clojure Compiler for JS, which you could install thusly:

    brew install closure-compiler

I have opted to pass, but add `.js` to the `optimize` array in `config.json` if you like.
