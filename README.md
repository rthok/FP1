# Final Project Assignment 1: Exploration (FP1) 
DUE March 25, 2015 Wednesday (2015-03-25)

### My Library: Stickman Icons

* a narrative of what you did

I worked with the Stickman Icons library. I first created the original standing stickman icon that is used in Racket. Next, I created a two more standing stickman icon, changing the colors and height of each. I then created two running stickman icons. Each of the running stickman icons shows a different frames from when it is running. Lastly, I changed the running stickman icons' colors and height and created a list showing all the 12 different frames of it running.

* the code that you wrote

```
#lang racket
(require images/icons/stickman)

(standing-stickman-icon)

(standing-stickman-icon #:body-color "blue"
                        #:arm-color "red"
                        #:head-color "white"
                        #:height 50)

(standing-stickman-icon #:body-color "pink"
                        #:arm-color "green"
                        #:head-color "purple"
                        #:height 100) 

(running-stickman-icon 1)
(running-stickman-icon .3)
                                     
(for/list([t (in-range 0 1 1/12)])
(running-stickman-icon t  
                       #:body-color "blue"
                       #:arm-color "yellow"
                       #:head-color "blue"
                       #:height 45))
```

* output from your code demonstrating what it produced


[A screenshot of my output](https://github.com/rthok/image/issues/1)


* any diagrams or figures explaining your work 
 
The narrative itself should be no longer than 350 words. Yes, you can add more files and link or refer to them. This is github, handling files is awesome and easy!

Ask questions publicly in the Piazza group.

### How to Do and Submit this assignment

1. To start, [**fork** this repository][forking].
1. You might want to [**Clone**][ref-clone] this repository to your computer
  2. (This assignment is just one README.md file, so you can edit it right in github without cloning if you like)
1. Modify the README.md file and [**commit**][ref-commit] changes to complete your solution.
1. [**Push**][ref-push]/sync the changes up to your GitHub (skip this if you didn't clone)
1. [Create a **pull request**][pull-request] on the original repository to turn in the assignment.

<!-- Links -->
[piazza]: https://piazza.com/class/i55is8xqqwhmr?cid=411
[markdown]: https://help.github.com/articles/markdown-basics/
[forking]: https://guides.github.com/activities/forking/
[ref-clone]: http://gitref.org/creating/#clone
[ref-commit]: http://gitref.org/basic/#commit
[ref-push]: http://gitref.org/remotes/#push
[pull-request]: https://help.github.com/articles/creating-a-pull-request
