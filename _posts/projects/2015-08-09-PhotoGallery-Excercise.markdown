---
layout:     project
title:      "Weld"
date:       2015-09-08 23:10:02
categories: private
permalink: /private/photo-gallery/


---

## Photo Gallery UI

I decided to focus on the user orientation of the interaction. This felt like the place the "designer" was having the toughest time. Since the photo gallery is a common design pattern we've been seeing since 2007, I wanted to focus on the nuts and blots of the interaction more than the underlying code.

## The Ask

A designer on the team delivers mockups for a grid view and detailed photo view and asks you to help define the transition between the two states.

##### How might you build a smooth transition from the grid view to the detail view?

I did this by expanding the image from the grid view to the detail view. Keeping the image as the focus allows the user to grasp that this new state of the view is composed of the same objects.

##### How could you use gestures to enhance the interactivity? e.g. should users swipe to move between images?

I think that gestures strengthen the understanding of the model in this example. The lightbox is a representation of the list in a new orientation. Allowing the transition between the states to imply that fact is a big part of the end goal. Users should know, or at least have hints at what is coming next.

##### Feel free to use any technologies, libraries, or frameworks you like to build the prototype.

I took this as technologies, not code. I feel like communicating this type of state change is clearer in a more visual format for all involved. Once the hand-off from the prototype to "real code" happens we have artifacts from working out the animations that can support replication of the visual style.

## My Approach

The above scenario seems to be more of "figure out the animation" than "build a working prototype". I usually prefer to just write code for these kinds of elements in the language they'll be implemented in (js, Objective-C, etc.). If there is time or it saves someone on the engineering team some headaches I think that is the best route.

I made some assumptions about the designer and the team:

* The designer was unfamiliar with modern prototyping tools
* The team really wanted to find the states between these comps
* The team had a hard time deciding on deliverables in the past

This felt like a great opportunity to play with a new tool - [Principle](http://principleformac.com/). It doesn't focus on giving you working code. Principle does however do a great job of doing down-and-dirty interaction animations. It also gives you the option to tweak the animations quite a bit with real values (easing, springs, etc.).

## The Prototype

I focused on the interactions more than the code (literally no code). I tried to make the user feel like the lightbox was an extension of the list itself. I accomplished this by having the images animate from the tap-origin in the list up into the lightbox.

There are swipe gestures to "page" the images in the gallery. I also added a swipe down to close. This is a common interaction pattern and I really like the natural feel.

<figure class="sketch video" id="fig1">
  <video src="{{ site.url }}/img/google/PhotoGalleryEx2.mp4" controls></video>
  <figcaption>
    <p><em>(fig. 1)</em></p>
    <p>This was a pretty quick exercise, but it was fun to play with a new tool!</p>
  </figcaption>
</figure>

## Aside

In the real world this could just be built with an off-the-shelf js library. Heck, there are ~10 js lightboxes that could be re-purposed for the project. The best of which is [PhotoSwipe](http://photoswipe.com/), it does this exact thing really well. Since it is a design exercise I thought that'd be cheating ;).




