# For Patricia - overview

For now there are four interconnected modules to work on: 

- AI
- Visuals
- Choreography
- Music

## [AI](./AI-notes.md)

An AI agent is trained on a base text, which is the poem "À ma mère" by Mahmoud Darwich (translated into French). Using one or more semantic schemes, the poem is segmented and, according to different scenario parameters, can be generatively sequenced. The segmented text serves as the basis for a visual score, which is read by the dancers and musicians, who perform corresponding choreographed movements and music. 

> **Tools:** Max, DICY2 package

### Basic workflow: 
- Text is manually analyzed, and lines/sections/phrases/etc. given semantic labels (i.e., 'emotions', 'objects', 'actions')
- Parameters for scenarios are created, based on... TBD. 
- DICY2 receives labeled text as input (the model) and based on a given scenario outputs reordered text. 
- Text is associated with visual score objects (icons? glyphs?) that are associated with movement and music instructions

## 2. [Visuals](./Visuals-notes.md)

The main visual element is a virtual dancer, animated and projected on the rear wall of the stage. The dancer performs the "correct" or "ideal" version of the dance, based on the output of the AI and generative score. The visual score elements may also be projected in some visually interesting way. 

> **Tools TBD:** Mocap (Freemocap.org or similar for cheap/easy capture in studio); Blender for rigging and animation; Max/Jitter for projecting, or something else? (Processing, Resolume, TouchDesigner, ...)

### Basic workflow
- A motion capture is taken of a dancer (two dancers?) performing the fixed version of the choreography (roughly three minutes in length). 
- The capture is segmented based on... TBD, 
- An avatar is rigged based on the mocap data and given an appropriate form (also TBD), resulting in a short animated segment for each segment of the dance. 
- An algorithm is created that can output, loop, and sequence segments together, with appropriate connecting animations between them. 

## 3. [Choreography](./Choreography-notes.md)

A ~3 minute fixed choreography for two dancers is created, corresponding with the selected text (À ma mère). The choreography is segmented in correspondence with the schema for the text, and performed live according to the new sequences and directions provided by the AI (and displayed as a visual score). There will, or should be, a correlation between the dancers onstage and the animated dancer(s) projected behind them. 

> **Tools:** none, but need to figure out the visual score system

### Workflow
- Basic choreography creation, in conjunction with text and music
- Motion capture of fixed choreography for visualization
- Segmentation according to agreed-upon schema
- Notate segments via visual score
- Perform according to live-generated score

## 4. [Music](./Music-notes.md)

Like the choreography, a ~3 minute fixed composition is created to accompany the dance, and to be performed by 2 musicians. The music is segmented to match the text and choreography, so that it can be performed in a modular fashion, based on the new generated sequences provided by the AI. 

> **Tools:** For music, Max, Ableton Live (maybe, to keep things on a consistent timeline if needed), VCV Rack. Acoustic piano, drumkit.

### Workflow
- Same as choreography: create a ~3 minute composition that corresponds with the dance and text
- Segmentation to match text and choreo
- Notate segments via visual score
- Perform according to live-generated score

