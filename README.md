# ICSE Talk

- A brief history of VR
- Demo without VR
- What is VR?
- Why use VR with Software Engineering?
- Affordances
    - Spatial Cognition
    - Manipulation and Motion
    - Feedback
- RiftSketch
    - Debug window
    - Leap motion integraiton
    - Flocking algorithm
- Open questions (cut if needed)
- Future work

## A brief history of VR

Virtual reality has been a staple of science fiction for decades but, from the nineteen sixties to the nineteen nineties, there was a flurry of activity around the topic. Research exploded and hardware companies actually tried to produce VR headsets. Unfortunately, the technology of the time couldn't meet expectations. VR was abandoned shortly after and laid dormant for almost twenty years.

That is until two thousand twelve, when a kid in a garage took advantage of mobile phone hardware and reignited a new generation of VR. A rapid series of events lead the formation of a company and to a kickstarter campaign that raised 2.4 million dollars. Only a couple of years later, the company was bought by Facebook for 2 billion dollars. Today VR is spreading in the entertainment and computing industries. Giants like Google, Microsoft, Samsung and HTC, amongst others, are making moves into VR. And the first consumer devices are scheduled to hit shelves around the end of this year.

## Demo without VR

## What is VR?
There are many definitions of virtual reality, but we will use a casual definition that virtual reality is a combination of innate human abilities and the malleability provided by digital technology.

Humans are amazing creatures with all sorts of amazing abilities.  However, current programming environments only take advantage of a few of these abilities.  We have built VR prototypes that take more fully take advantage of the innate human abilities of spatial cognition, manipulation and motion, and feedback.

## Why use VR with SE?
VR enables more natural programming solutions.

### More familiar
These solutions can be more familiar to users than traditional solutions which we expect would increase task speed and decrease cognitive load (ex: looking around in 3D via head vs. mouse).

### New techniques
These solutions could also enable techniques that have been previously impossible. For example, VR enables video game developers to be *inside* their game while creating it.

## Affordances

In that vein, our research suggests several affordances that VR can provide to software engineering and provides rudimentary examples of how they might be implemented.

The first affordance we considered was spatial cognition. Unlike any other computing interface, VR can fully engage your brain's inherent sense of space through head tracking and stereoscopy. Our research considers that unlocking this capability can lead to improvements in comprehension and recall. When learning a codebase, one could view the structure of an application laid out around you or while reviewing a code change, you could toss irrelevant code into a pile at your feet or pin interesting snippets front and center.

The second affordance, manipulation and motion, speaks about using VR perhiperals to track the movement of your limbs in order to interact with virtual objects as you would with physical ones. This affordance would allow improved perception and retention. For example, you'd be able to crank a handle in a mechanical simulation and have a visceral experience of the software's behaviour or you'd be able to walk along a row of commit histories while attempting to find where a bug was introduced in code.

Finally, we consider feedback in VR. Although live-coding has existed in 2D software systems for decades, real-time feedback is especially effective in VR when your software has a visual 3D analog. Allowing developers to experience and edit the software and the world around them in a short cycle can improve productivity, experimentation and learning.

## Demo

- RiftSketch
    - Debug window
    - Leap motion integraiton
    - Flocking algorithm

## Open Questions
There are still some big questions that would benefit from research.

### Degrees of Immersion
It is easy to imagine VR helping with 3D software. Could VR be helpful when building software that lacks a 3D analog?  Would augmented reality be more helpful?

### Input forms
How can software engineers immersed in a virtual environment instruct the computer on what to do?  Voice? Gestures? Text?

## Future work
* more powerful 3D editor
* as needed info visualizations
* 3D visual programming languages
