---
layout:     project-hidden
title:      "Earnest"
date:       2016-08-16 1:02:02
categories: campaign
img:        img/projects/analyze/0.0-hero.png
thumb:      img/projects/analyze/1-Analyze2.png
type:       Case Study
roles:
  - User Experience
  - Design Patterns
  - React

---

Earnest is a bank that wants to democratize access to world-class financial services. That mission is predicated upon having the tools to assess our clients risk with radically different results than traditional banks. We take into account many more indicators of financial health than any of our competitors.

Having this much data means we can serve more diverse clients &mdash; it also means that we need to make better decisions with more data. That is where I come in - I design tools for our internal teams to make the mission a reality. I get to help amplify my coworker's skills and happiness; that is fun.

## If it works how bad could it be?

Before I arrived at Earnest the majority of internal tools had been built hastily to serve the needs of a rapidly growing business. Earnest had grown more than 5x in the 6 months preceding my arrival. And the tools looked the part. They were built for and mutated from earlier processes. The initial cry from the teams was "fix the tools".

It was clear that we'd need to do more than put a veneer on these old tools. We needed a radical rethinking of how we stored data and transformed it throughout the application process (immutability anyone?). The executive team realized this and allocated the proper resources to tackle the problem.

## What to break first?

First, we needed to improve our risk team's tools. Risk encompasses the verifiers and the underwriters. They've got access to tools, models, and all of the data that bleed out into the rest of the business, including the client application. Myself, a product manager, and one of my favorite engineers mapped out the future vision of the entire suite of tools that we would need in a previous project. All of the tools flow from having the right clients and the right data.

We started with some whiteboard sessions that lead to a flow diagram that was monolithic and confusing - a good outcome as it lead us to a flow diagram. Then another [(fig. 1)](#fig1) that was even right-er[sic]. Getting this part of the process nailed is really important to me, the engineers, and the product team as it informs the entire software making process. Using the same words or pointing to the same blob on a flowchart does a lot of the job for us when making hard decisions.

<figure id="fig1">
  <img src="{{ site.url }}/img/projects/analyze/0.1-Flowdocs.png" alt="Analyze flow documents">
  <figcaption>
    <p><em>(fig. 1)</em></p>
    <p>The whiteboard sketches and the final google drawing. I like google drawings because everyone on the team can get access to comment and edit. Like a stack of post-its or a whiteboard where everyone can interact and design.</p>
  </figcaption>
</figure>

We started to head toward agreement on what needed to be built and in what phases we could accomplish our goals. I started to think in sketches and wireframes. As the thinking in one fidelity starts to gel, I am compelled to move onto the next level of fidelity to validate assumptions and make sure we've got any obvious issues dealt with at the earliest possible stage.

I try to get all of the data on one screen &ndash; starting to push and pull at what is needed and what can be combined away. The goal is to try to tease out the essence of the problem through brute force. This is usually frustrating but rewarding. I feel like you can shave days off the proper design process with a few hours of ugly, low-fi sketching in this phase of design.

<figure id="fig2">
  <img src="{{ site.url }}/img/projects/analyze/0.2-Pass1.png" alt="">
  <figcaption>
    <p><em>(fig. 2)</em></p>
    <p>Data dumps are funny &amp; extremely helpful. Trying to match the fidelity to the thinking is hard, but when you find it you just know.</p>
  </figcaption>
</figure>

## Up the fidelity

The next exercise was in Sketch. Improving usability and accessibility of the analyze tool were "non goals", but they were an important part of the process to me. I wanted to make this simple for anyone to use, even on a small screen. Making it feel consumer-y held a lot of weight for me &mdash; I don't want my coworkers to feel like they were being punished because we had a looming deadline while making their tools. Some of these explorations were fruitful and some were junk, but that is the process.

<figure id="fig3">
  <img src="{{ site.url }}/img/projects/analyze/0.3-Pass3.png" alt="">
  <figcaption>
    <p><em>(fig. 3)</em></p>
    <p>I tried to leverage a design language another team was working toward and augment it with a simplified feel. That -- - 0 + ++ was one of the hardest things to work out. It is not a standard UI pattern to rank the middle as best.</p>
  </figcaption>
</figure>

Once I was circling the solution we started another round of User and Engineering feedback about what I was planning. The engineering feedback is less conventional at this stage, but they were already building infrastructure that could impact the deadline. I typically try to get some technical feedback, but it is usually around understanding the limitations; this felt way more collaborative.

The feedback was incredibly valuable to get in unison - the technical _and_ the emotional. I love having great engineers and product folks in the room as we talk with users on these internal tools. It creates a feedback loop that allows new ideas to surface and unconventional questions to be asked.

## Conclusion

The simple part of this project was improving the UI design from a spreadsheet to a set of dedicated components. The harder part was garnering the good will in the organization to tackle this project with the set of resources we pulled together to accomplish the task in the set time.

## Design Details

The result of the project was a pretty minimal tool that allowed for the scoping of future tools that will be "plugged into" this tool over time. We really scaled back what it meant to analyze a loan. Simplifying a job without removing the feeling of agency from the user is a huge win.

<figure id="fig4">
  <img src="{{ site.url }}/img/projects/analyze/0.4-Components.png" alt="">
  <figcaption>
    <p><em>(fig. 4)</em></p>
    <p>Spec'ing components</p>
    <p>Components were a huge part of the new design system. We composed discrete components to tackle the jobs bing done in this interface. They can also be composed to accomplish other tasks that happen later in the work flow of an application becoming a loan.</p>
  </figcaption>
</figure>

<figure id="fig5">
  <img src="{{ site.url }}/img/projects/analyze/0.5-CreditAdmin.png" alt="">
  <figcaption>
    <p><em>(fig. 5)</em></p>
    <p>The Credit Admin tool</p>
    <p>This project was really 2 primary applications that combine to allow our underwrtiters to decide a loan <em>and</em> our scoring model to improve rapidly.</p>
  </figcaption>
</figure>

<figure id="fig6">
  <img src="{{ site.url }}/img/projects/analyze/0.6-AllScreens.png" alt="">
  <figcaption>
    <p><em>(fig. 6)</em></p>
    <p><em>Almost</em> all of the screens</p>
    <p>There were lots of permutations of screens, but with the component architecture we could limit the number of screens that needed to be designed.</p>
  </figcaption>
</figure>

<figure id="fig7">
  <img src="{{ site.url }}/img/projects/analyze/0.7-Whimsy.png" alt="">
  <figcaption>
    <p><em>(fig. 7)</em></p>
    <p>Whimsey cannot be shoehorned</p>
    <p>These didn't work out for scoring feedback, but if you read all the way to this point I hope you feel the biggest of the smiles.</p>
  </figcaption>
</figure>
