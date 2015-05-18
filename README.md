# ICSE Talk

- A brief history of VR
- Demo without VR
- Demo with VR
- What is VR?
- Why use VR with Software Engineering?
- Affordances
    - Spatial Cognition
    - Manipulation and Motion
    - Feedback
- Dev Benefits
- Persuade Researchers
- Resources
- Open questions (cut if needed)
- Future work

## A brief history of VR

Virtual reality has been a staple of science fiction for decades but, from the nineteen sixties to the nineteen nineties, there was a flurry of activity around the topic. Research exploded and hardware companies actually tried to produce VR headsets. Unfortunately, the technology of the time couldn't meet expectations. VR was abandoned shortly after and laid dormant for almost twenty years.

That is until two thousand twelve, when a kid in a garage took advantage of mobile phone hardware and reignited a new generation of VR. A rapid series of events lead the formation of a company and to a kickstarter campaign that raised 2.4 million dollars. Only a couple of years later, the company was bought by Facebook for 2 billion dollars. Today VR is spreading in the entertainment and computing industries. Giants like Google, Microsoft, Samsung and HTC, amongst others, are making moves into VR. And the first consumer devices are scheduled to hit shelves around the end of this year.

## Demo without VR

So, given the rise of this new generation of VR, we wanted to show you an example of the types of problems we think VR can address. To that end, we've arranged a demo. And although it may be somewhat contrived, hopefully it gives you an idea of what we're talking about. We'll start with a typical development environment. Web devs will recognize this setup, with your favorite editor side-by-side with a browser. In this case the code we're working on implements a simple 3D application, written in JavaScript, that includes a flocking algorithm.

The first thing we'd like to point out is the problem of file management. Most editors have moved towards tab-based interfaces, which is certainly helpful, but dealing with multiple files in can still slow you down. At best you might be able to spread your files across a few screens. Anyway, lets move on to the actual application.

The code constructs a 3D world containing boids which behave according to a flocking algorithm. Lets edit the code a bit to generate more of these boids. As soon as we do that, we run into the second problem we'd like to solve. This one is particular to 3D applications but it is quite a serious problem. As you can see, it is difficult to tell these boids apart, despite their contrasting colors, without manually rotating your point of view.

Now let's take a look at this flocking algorithm. It's got a bug in it that we'd like to fix. The code has a few magic numbers that we may have to tweak. One of them controls the interpolation between two quaternions during the separation step of the algorithm. We can keep editing this number to find the right balance but let's turn to VR and see if there's a better way.

Before we do that though, one last thing we want to point out is that the traditional development process involves this tedious edit, switch and refresh cycle. Maybe we can solve that in VR as well.

## Demo with VR

- inside world
- editors in world
- move editors
- depth
- position self
- fix bug: gestures to change number
- returnToOrigin

The first thing you'll notice in the VR version of this demo is that we are no longer just looking at the demo application from the outside but that we are actually inhabiting the world itself. [Look around the world] To our right, our JavaScript files appear in free-floating editors. [Look at the editors]

Thanks to hand-tracking provided by the Leap Motion sensor, we can use our hands in VR and grab the editors and position them as we choose in this 360 degree virtual screen space. [Grab one of the editors and move it around a bit] Since we're not interested in the World and Boid files right now, we can just move them out of the way. [Move the two editors behind]

Secondly, we can perceive the depth of 3D objects in our application, this makes it much easier to understand what we're looking at. [Look back at boids, shift around to show parallax] We can even position ourselves at an ideal vantage point as needed. [Step a few paces around the boids]

Let's try to fix that bug we were looking at. Using a gesture, we can tweak the number directly in the code and immediately see the effects of our changes. [Scrub the number and show it change while also looking at the boid react]

Let's expand on this code for a bit longer to give you an idea of what it feels like to code in this environment. [Makes the boids actually move around and add a behaviour for them to return back to origin]

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

## Dev Benefits

We've considered a few other benefits that VR could provide to developers. The first screenshot here shows a prototype of a code review tool. This tool gives you the best of both worlds, the physical and the virtual. So you could search for a piece of code in your codebase, just like you would with any digital text, but you'd also be able to pin that it up to the space in front of you or throw it down into piles below you depending on how relevant they were to the code that you're reviewing.

The second screenshot shows an existing 2D tool which lets you visualize the flow of a program through methods and the callstack as you debug it. Similar tool in VR that takes advantage of an unlimited 3D space and surrounds you, instead of one that only gives you a small window into the visualization, so that you could always have that spatial context.

VR would also be extremely useful when combined with simulation software. Imagine you were a developer for Boeing, working on avionics software for their next line of aircraft. You could debug your code in a virtual simulation with a miniature 3D model of the aircraft in the palm of your hand. As your code runs, you could watch the visualization of the software's commands propagate through the aircraft's control circuits. Then could blow the aircraft up to larger than life-size and walk into the guts of the wing's flight surface mechanism and watch behavior of the hydraulic actuators.

## Persuade Researchers

## Resources

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
