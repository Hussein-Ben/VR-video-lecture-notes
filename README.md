notes covering the entire course on 3D Virtual Environments and Animation (2018-19)

pdf, word and google docs is available in this repo (the google docs link is better)

http://www.vrglossary.org/glossary  - useful glossary
 
## Week 1
 
**What is VR?** 
 
*  The experience in which the user is effectively immersed in a responsive virtual world
*  VR Implies that the user has dynamic control of their viewpoint (very important)
 
**Why is VR different from other immersive media such as 3D cinema etc;**
 
* 3D Stereovision (camera for each eye)
* User dynamic control of viewpoint (display is updated to the viewpoint of one specific user, achieved via head tracking)
* Surrounding experience (full visual perception is surrounded by the device - the more of your field of view is covered by your device - the more immersed you will be - size of screen does not matter, for example google cardboard)
(you are trapped, when you look around you still see images from the virtual world)
* Experience is overwhelming and persistent - does not diminish over time.
 
### Uses of VR:
 
**Sport:** 360-degree video - watch events from the best seat (not interactive) can choose seat. Used in theatre too.
**VR for sports training** - Research papers show, training in the real world is still more effective. What you learn in VR, remains in VR. Skill are not yet transferable to the real world.
 
**Illusion of being someone else:**  need to give user a self-avatar where their actual body is.
**Proprioception (or kinaesthesia)** - someone's overall sense of their relative position of their own parts of their body.  Warning, if the user moves, but the model stays in the same place, then the illusion will break. 360 video - person can’t be changed. Important to have a static body where users expect their body to be. Mel Slater: VR can not only transform where you are, but who you are (useful in psychotherapy), we can choose someone else - long-lasting psychological effects on users.
 
**News & Documentaries:** Modal-based or 360-degree video can be used immerse the user in the news event - potential increase in empathy due to immersion.
 
**Scientific Data Visualisation:** as opposed to information visualization, refers to the use of computer graphics for the analysis and representation of simulated or real data. Common feature of scientific data is that it highly dimensional, VR allows you to view and interact with data in 3D space. Useful for education and training. Help to fully comprehend 3-dimensional data. Could help doctors explain scan results to patients.
 
**Medical Training:** used in immersive learning. 360 - video of surgery room. Surgical skill training, many problems - high end VR interaction devices. Can help Doctors improve their social skills, with challenging patients.
 
**Physical Rehabilitation and Psychotherapy:** EEG example, paralysed patient imagines moving their avatar. Interactive visual feedback plays important role in motivation for patient. Makes rehabilitation- less painful and less boring. You can control the difficulty of the rehabilitation - progress in steps. Treatment in psychotherapy - can be used to treat phobias such as heights and spiders - risk free and controlled environment. Can help soldiers revisit traumatic events to stop them over-reacting PTSD.
 
### Graphics:

* rendering: process of turning 3D representation into 2D images. (x, y, z) we only use points. Line get drawn between these points.
* Vertices => Edges => Polygons (2D shapes) => Surfaces (meshes)
* Skinned Mesh: Meshes that are rigged for animation
* Polygons are simple, many polygons can create a curve
* Photogrammetry: taking many pictures of an object, digitising it into a 3D model.
* Compound Objects = shared transforms, scale and move
* In 3D graphics, we have a virtual camera that does a perspective transform which maps the object into 2d. In VR you need two cameras for each eye for 3D stereo vision. Camera needs to transform as head turns - main reason for VR experience.
 
**VR technical framework:**
* HMD, VR interaction, VR content (images to display or 360 video).
 
**Model based VR and 360 video:**
* 360 video = video content generated in the real world
* Analogue or digital cameras - highly realistic - fast capture but you cannot modify
* Model Based = (CGI) computer generated 3D content - longer to generate - easy to modify - you can reuse - go beyond real-life - interactive in real-time - can be photorealistic.
 
*Skipped brief history of VR*
 
**Level of immersion in VR systems**
 
* Ideal system: display in all sensory systems. Vision, Sound (undirected, spatialized sound, modelled, reflected in environment), Haptics (sense of touch, force feedback) and smell.
* Haptics are currently specialized for certain application, no general haptic device. Currently no generalized smell, smell needs to linger or leave
* Vision and sound are supported currently and particular/specialist haptics and sound exist today.
 
### Measure immersion
 
Immersion: technical description of what a system can deliver (simulation on principal), technical specification (hardware and software) not the effect. If we take HMD A that can translate head, rotate with 6 degrees of freedom and another HMD B in which you can only rotate, you can say that HMD A is more immersive than HMD B, because you can use HMD A to simulate HMD B (HMD B is a subset of HMD A).
 
### Sensorimotor Contingency (SCs)

Definition: part of a theory of active vision. Describes how we use our bodies to perceive. We have a set of implicit rules we use to perceive the world. By implicit we mean that they are rules we do not have to think about (for example to look around). Vision is not passive (not simply light entering our eyes - we actually move our heads, turn around etc ...)  tactile feeling, reaching out your arms gives us a sense of distance for example. By sensorimotor contingency, that set of implicit rules whereby we use our bodies to perceive the world, across all the different senses.
 
*“sensorimotor contingencies (SCs) refer to the actions that we know to carry out in order to perceive”* - Mel Slater
 
**Sensorimotor Contingency (SCs) in VR**
 
* Immersion: the affordances the system gives you. More importantly, what does the system give you in terms of perception. Combination of how you perceive and what you perceive. The more that the How matches reality and the more what you perceive  matches what you expect to see in reality through the act of perception.  So you're getting closer to an actual sense of SCs. Brain beleives thar VR is real through natural SCs.
 
**Why do we need Immersive VR ?**
 
* You don’t - it depends on what you want to do. VR, gives you presence. Useful in clinical psychology. Treating fear of heights- gradual exposure to what they fear does work. Showing a movie of heights does not work, putting someone in a VR virtual height - same level of real height is induced. The immersion leads to an illusion of presence.  Brain does not know about VR, has to make a very fast decision. We are not in charge of all our reactions and actions. (Virtual height example)
 
**VR challenges**
 
* Realism (Graphics) : In training and therapy if the graphics do not reflect the real world (photo-realistic), then skills acquired in VR won’t be transferable.  In order to create photo-realistic environments, you need to know how lighting works in real life. 
 
* Diffuse: even looking reflection - reflects light equally in all directions, less computationally expensive.

* specular surface (metal): lights are reflected in a certain direction, giving it the shine look, more computationally expensive. Glossy and mirror surfaces are the most expensive.
* Local illumination: consider only lights that come directly from the light source.
* Global illumination:  inter-reflection between objects, like real life.
* 360 video: you cannot change lighting.
* Realism (animations): Humans are critical observers of animation, any slight mistake will be noticed.
* Navigation: position tracking - allows you to move your body- viewpoint will change. Mobile VR you can only rotate your head. Physical navigation problem - you are limited by the amount of physical space you have, does not work with mobile VR. Moving with a joystick can make you sick (nausea).
* 360 video, fixed position where you filmed but google street-view you can navigate.
* You can walk in space, does not cause nausea but no sense of acceleration.
* Teleporting can reduce nausea too, but user can be disoriented when teleporting to a new location.
* 3D navigation that relies on interfaces (such as the keyboard) is not encouraged.
 
**Nausea (simulation sickness)**
 
* Discomfort induced by simulated environments
* Mainly caused by the conflict between information received in the brain from our vestibular system and our visual system.
* In this situation, you are physically moving but are looking at someone that is relatively  still. The vestibular system tells the brain that you are moving, but the visual system says that you are not => feeling sick
* Simulation sickness is opposite to this. Vestibular: you are not physically moving but your visual system says you are (immersed in VR) = causes nausea.
* Best way to avoid this, physical movements similar to real life cause less nausea, walk-in place and teleporting also reduce nausea.
*  Worst method is to use the default 1st person camera (keyboard, mouse joystick) => causes sickness.
* Eye strain, as displays are close to eyes
* Frame rates below 90fps
* Flashing and High-Contrast images
* Some people are less prone to simulation sickness.
 
**Meeting other people:**
 
In person we are better at negotiation than in video conferencing.
-        Relationship building
-        Trust
-        Body language
-        Facial expressions
-        Timing
 
 ----
* We rely on social skills acquired over years that operate on the unconscious level.
 
* Facial expression is hard to track due to HMD covering face.
 
* Eye gaze, pupil dilation, Subtle emotion changes: blushing, sweating, Subtle facial muscle movements all need to be tracked for realism.
 
Volumetric capturing can work but it relies on post-processing, it is not real-time.
Current tech does not support meaningful physical contact with another person (cannot shake someone hands etc...)
 

**Haptic feedback**
 
* Ability to interact with objects in a naturalistic way is still poor with current technology. We need VR gloves, good tracking but no haptic or tactile feedback. Exoskeleton gloves provides haptic feedback. Force and tactile feedback still available with VR suits.
 
What is the difference between tactile feedback and haptic feedback?
Tactile Feedback is a type of Haptic Feedback. Haptic feedback is generally divided into two different classes: Tactile and Kinaesthetic. The difference between the two is quite complex, but at a high level:
 
*  **Kinaesthetic:** The things you feel from sensors in your muscles, joints, tendons. Weight, stretch, joint angles of your arm, hand, wrist, fingers, etc. Imagine holding a coffee-mug  in your hand. Kinaesthetic feedback tells your brain the approximate size of the mug, it's weight, and how you are holding it relative to your body.
 
* **Tactile:** The things you feel in your 'fingers' etc., or on the surface. The tissue (for example in your fingers), has a number of different sensors embedded in the skin and right underneath it. They allow your brain to feel things such as vibration, pressure, touch, texture etc.
 
Haptic Feedback is a combination of both Tactile and Kinaesthetic Feedback.
https://www.quora.com/Robotics-What-is-the-difference-between-tactile-feedback-and-haptic-feedback
 
*Skipped history of VR*
 
## Week 2: VR Graphics
 
We see objects through the light that is reflected off them. Real objects have many details, colour, rough, smooth - properties of the surface of the object. How light reflects of the surface fundamentally shapes what it would look like - refer to this as material.
 
Skipped most videos this week, a lot of it is not theory just practical, less likely to come up in the exam.
 
Two cameras must render the same scene, post-processing is required. For VR to work when you move your head the frames need to update fast.
 
Motion to Photon time: From the moment the you move your head through to the moment the image is rendered. Needs to be less than 20ms. Lot of processing in a short amount of time - high end PCs are required.
Global illumination: very expensive, natural light that bounces off other objects. Global illumination can be baked(pre-computed) before rendering, works well with static objects.
 
Ambient lighting: very cheap
 
**What’s the difference between Graphics in VR and games & films?**

* Same graphic techniques that is used in games (both real-time)
* Animations and films are not real-time
*  VR is more computationally intensive
* Presence and comfort more important in VR
* Rendering two screens at under 20ms - limited by what you can do.
* Bump mapping (creates effect of “bumbs”) on surface, does not work in VR
* Parallax mapping works better
* Place illusion, plausibility illusion and embodiment illusion together these form presence
* Graphics can support or fail to support place and plausibility
* Better graphics does not improve presence, graphics did not make a big difference.
* However, some techniques work well such as real-time shadows.
* High frequency movement can cause nausea. Aliasing - seeing the pixels of object can be disturbing, anti-aliasing can avoid this.
* VR is like the real-world, you should use the real-world as your reference.
* VR scale is more noticeable than in games. Sensitive to even small inconsistencies
*  In VR, environments need to be a size that you can comfortably move around in, unlike in games in which you move at 30mph.
* VR, there is no frame, you can look around everywhere, you can't control the users but you can guide them. Do not make assumptions, keep testing in VR - you need to check if the environment you have made works.
 
 
### The Three illusions of VR
 
* Place illusion: a feeling of being in a virtual place even though you know that you are not there. When you have visual sensorimotor contingencies that more or less like real life, this affords the possibility for the brain to make a decision that this is where I am, the virtual place rather than the real place.
Place illusion: can occur if nothing else is happening in the environment, as long as you can look around.
* Plausibility illusion: how real do I take the events around me to be. It is separate from place illusion. For example if you are driving a car and you see a policeman from a distance you begin slow down, but as get closer, you see that the policeman is actually a cardboard cutout - plausibility breaks, you know it is not a real policeman. Plausibility: The events that I am perceiving are really happening.
* Embodiment: sensorimotor contingency in the real world when I look down I see my body. In VR,  If you look down and see a virtual body = embodiment illusion (body ownership) form and shape of body can be quite powerful.
 
Place illusion Examples: public speaking VR, the Bystander problem…
 
Does immersion cause Place Illusion (PI)?:
 
* **Immersion** = what the system offers, the technology. **PI** = response of the individual. Immersion provides a framework basis in which place illusion can occur. Immersion does not cause place illusion, it's on the basis on which PI can arise. (different people can respond differently in the same VR world)
 


## Week 3
 
Interaction in VR is completely different than in other media.

You have an HMD covering your face - you can’t see the interaction devices in the virtual world. You can’t see the keyboard. Mouse and touchscreen is mostly designed for 2D interfaces, you can’t interact with depth.

VR is all about creating the three illusions that make up presence.

Embodiment is about linking your body to the interaction, by visual representation of your body as well as physically moving your body.

Computer interface are based on metaphors - for example the desktop.
When developing in VR you should think about how you interact with the real world.
 
**Natural Interaction:**
Allows us to use the same skills used in real life and apply them in the virtual world. You don’t have to know about tennis to play Wii tennis.
 
Interface need to show you what you can do and give you feedback when you carry out an action. Gestural interfaces do not do any of these things, you don’t know which gestures you need to do - hard for software to recognise. VR interaction should be close to the real world, but there needs to be feedback, gestures need to be clear.
 
**Magic Interaction:**
Interaction should be realistic as possible, close to the real world. Because VR is not the real world you can do things you can’t do in the real world - magical interaction, like reaching out to grab an item, magical interfaces can be better than natural interaction, you shouldn’t limit yourself to real world interactions.
 
### Active and passive interaction:
 
**Active interaction -** consciously deciding to interact, like using a mouse to click on an icon.
 
**Passive interaction -** not consciously interacting. Not doing anything, detecting what you’re doing and reacting, for example a fitness tracker. Unlikely to be aware.
 
Turning your head to look around in VR is a passive interaction. You don’t have to think about turning around, HMD responds to you. 
 
Passive interaction can be bad/creepy - software collecting data on you. Not clear how it works for the user. Use passive interaction for indirect things.
 
**Affordances:**
 
Interaction design. Affordance is the relationship of an object and our ability to act on it. For example, a door handle (object) = pulling with our hand (ability to act on it). Affordances are not always designed. Affordances in VR are closer to the real world. Affordances depend on the properties of an object and your ability to act. False affordances = bad design, pull on a door handle that you must push. Make sure you have good signalling of affordances.
 
**VR interaction theory:**
 
All interaction should be based on the real world - not in games or films. Interaction must be useable - make it clear how the user should interact with the world. Design your objects so that the actions you can carry out on the object are obvious. We can see what actions we can do to an object just by looking at it (affordances). A well-designed object has clear affordances. Keep testing with different people.
 
### Introduction to Plausibility Illusion
 
Bystander situation is an example. If an aggressor does not respond to you shouting or if the characters ignore you then this is a failure of plausibility. Bar example in video - animations were repetitive, users noticed this.
 
**Necessary conditions for Psi (Place Illusion & Plausibility Illusion):**
 
* Events occur in relation to you personally, the subject of an action by another part of the visual environment.
 
* World responds to you, you walk through a crowd - the crowd moves out of the way.
 
* Credibility, environment needs to respond to people's expectation - If you are depicting something in reality than it should conform to that. We don't know how the credibility part of plausibility works.
  
**Break of presence:**
 
Because place illusion is perceptual and because it relies on the Sensorimotor-contingency, sensorimotor-contingency is provided by the system/immersion, they don’t change. When place illusion breaks it comes back again.
                
When plausibility breaks it never comes back again, because Plausibility is more cognitive and place illusion is more perceptual.
 
## Week 4
 
HMD = User Input
 
Inputs:
 
**HR** = Head Rotation (3 degrees of Freedom- does not update when we move our head sideways)
 
**HP** = Head Position (you look forward, sideways, move around - 6 degrees of freedom)
 
**CR** = Controller Rotation
 
**CP** = Controller Position
 
VR interaction is supposed to be cognitively less demanding.


### Navigation in VR:
High-end VR with precision tracking supports physical navigation. 
 
Room-scale VR (Physical Navigation) is the most natural form of movement, physical motion powerfully aids illusion of presence, actual walking allows you to feel how large a place is. Less likely to cause simulation sickness. Limitation of physical space. Health & Safety issues. Require user to state how much physical space they have. We use the same body, as we do in real life.
 
Redirected walking manipulates users into believing that they are walking on a straight line, whereas in the physical reality they are walking in a curved line. Causes users to change their direction of walking without them noticing. Walk around a circle thinking they are walking on straight line. The angle of rotation should be a function of the users velocity, so if the users moves faster, the world rotates quicker. Angular velocity, when the user turns around, we can make Virtual world turn to one direction, resulting in them actually turning bigger or smaller angle in the physical world than in the virtual world. A combination of adding rotation distortion, using both linear and angular rotation could quite dramatically increase the perception of the physical space available. Requires a lot of programming and creativity.
 
Walk-in-Place- Navigation in VR by engaging fully body movement without moving forward. Head tracker position will dictate position 
 
**Virtual Navigation:**
 
Using a joystick to move just like in games can cause nausea. In real life, you would mostly be looking at the direction of travelling. Secondly, too many changes in speed and acceleration can also cause nausea. You need to give users control of their speed.
 
**Teleporting:**
 
Target location = the new place users wish to travel to.  All methods discussed previously only apply to model-based VR (what we did with unity).
 
### Travel in VR - Quality Factors
 
* Speed: how much control does the user have in terms of speed? Sense of control, not actual control. Constant speed is better for the user instead of a there being constant speed changes.
* Accuracy: Is the user able to arrive at the desired target? How likely is the user to overshoot the target?
* Spatial awareness: the users implicit knowledge of their position and orientation within the environment during and after travel. Does the user feel disorientated after travel? do they have a good sense of scale? after exploring the VR scenario can they draw an accurate map of the virtual world they visited?
* Ease of Learning: Is this something easy for a novice user to use? How long would it take on average for the user to get a hand on it? cognitive load?
* Information gathering: the users ability to actively obtain information from the environment during their travel. After their experience can they remember objects they saw?
* How comfortable is the experience for the user?
 
## Week 5
 
Best VR experiences use techniques from games, films and immersive theatre. The Three illusions are key for VR experiences. Plausibility is the most important in terms of interaction. You need to maintain plausibility. VR is about simulating reality, you are trying to get user to use their body and brain in the same way they do in real life, doesn’t matter if the experience is fantasy or abstract, you still need to understand as human beings, how we interpret external signals and internalise using our body and mind. We can beyond real life. Avoid 2D menus. User comfort is important, no one wants to stay in experience if it makes them sick.

**User Evaluation:**
 
User testing takes a long time, data analysis is required. A/B testing. Quantitative data- numbers, measurements, 1 to 5 scale - objective data - allows comparisons. Qualitative data, subjective, opinion based, useful for measuring plausibility. Film user testing.
 
Testing is useful to decide which feature to keep or change in a game.
 
*The Pinocchio Illusion:* watch the video
 
* Brain has a contradiction to resolve, the brain doesn’t like contradiction it likes solutions, it believes its nose is that long.
 
*The Rubber Hand Illusion:*
 
* Brain can quickly give you an illusion that its body has changed.
 
**Psychological Effects of Embodiment Illusion:**
 
* Brain doesn’t actually have access to knowing what's part of our bodies, it can only rely on the signals it receives.
* Vision overrides other sense, such as proprioception (where your hand is in space)
* VR allows opportunities not possible in the real world, like a virtual body part.
 
### Visual-Tactile and Visual-Motor Synchrony
 
Rubber-hand (the Visual-tactile synchrony) experiment in VR had the same results as the same experiment in real life. In VR you can go beyond the rubber hand, virtual arm could be programmed for different movements.
 
**Visual-tactile synchrony** - the virtual hand moving caused increases electrical activity in the real arm - dependent on the subjective strength of the illusion. The stronger the illusion, the more electrical activity.
 
**Visuo-motor synchrony**:  
visual motor is when you move your body and you see the virtual body move synchronously, it's simply the fact of looking down and seeing a body, substitute your own body is already enough to give you the illusion
 
“The vast amount of research on the rubber hand illusion uses visuotactile synchronous stimulation to induce the illusion. This means that sight of the rubber hand being touched is synchronous temporally and spatially with the tactile stimulation felt on the corresponding (hidden) real hand. (seeing the hand)
 
It has also been shown that the illusion can be induced with visuomotor stimulation - meaning that (in this case) the virtual hand moves synchronously with the movements of the corresponding (hidden) real hand. (moving the Hand)” mel slaters blog
 
We know that we are in this world, because we can see our bodies.
 
Technical setup: http://journal.frontiersin.org/article/10.3389/frobt.2014.00009/full
* Wide field of display
* tracked HMD
* Head tracked using a body tracker
 
Change in Attitude, Behaviour and Cognition: (main reason VR is being pushed)
 
Change of the body in VR altered the participants perception. Empathy. Racial bias. Unconscious mimicry. Behaviour changed subconsciously.
 
https://pure.royalholloway.ac.uk/portal/files/26296788/Maister_et_al_TICS_authors_version_Figures.pdf
 
Self-counselling and treating depression:
 
You can give better advice to a friend than to yourself. 
http://bjpo.rcpsych.org/content/2/1/74
https://www.nature.com/articles/srep13899.
 
 
### Comparing CGI and 360 Video
 
Embodiment illusion works best with modal based VR. 360 Video: problems with position of body. Good to capture large spaces, things that are far away. 360 video does not provide a sense that you were in that place, with video you know its video - it’s not real, it can't interact with you.
 
This is where Prof Mel Slater's theory on the three illusions was first published:
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2781884/
 
Embodiment is the most important aspect of VR, it is completely unique.
 
 
### Physics Interaction:
 
* Physics (programmed, objects respond to force)(great for dynamic animation like balls works well for non-complex objects - infinite responses)


* Key-Frame animation (hand animation, not very interactive, play animation clips depending on what the user does - state machines)(more complex movements but only allows a small number of responses)
 
 
## Week 6
 
Our ability to interact with objects in the virtual world is essential for creating the plausibility illusion in VR. Direct control or agent control. Positioning of an object. Rotation, change orientation of an object. User could change scale too.
 
**DoF (Degrees of Freedom)**
 
Position: 3 degree of freedom:
*  X, Y and Z axis rotation
Rotation: 3 degree of freedom:
*  Pitch (moving up and down), Roll (sideways) and Yaw (left - right)
 
Position and Rotation: 6 degree of freedom
 
 
Immersive systems need to provide to user this framework:
* Indication of object
* Confirmation of selection
* Feedback
 
Object interaction within reach of real arm, this is what people naturally do in real life. Important for;
*  Physical rehabilitation
* Training and therapy
* Sports games
 
The most naturalistic way to represent object interaction in VR is to use a simplistic virtual hand. Low cognitive load, anyone can do it. You do not want your hand to be gender, age specific.
 
Problems: users can only interact with objects within reach without having to travel. Frustration can occur when they cannot interact with certain items, problems with clipping - you cannot stop your hand from dragging an item through a table - can break plausibility illusion.
 
### Hyper-natural interaction:
 
Interacting with objects beyond our arm length. Go-Go technique allows virtual arm to be longer than the real arm.
 
### Magic Interaction:
 
Recasting a virtual pointer. Reach objects out of reach, not something we do in real life. Natural and Hyper-natural is better, magic interaction can break plausibility. You can do a hybrid approach of both natural and magic interaction. Occlusion framing. Eye- hand visibility mismatch. You can scale down the word, and move around in it.


### Evaluation metrics:
 
* Task performance: how long does it take for a user to perform a task and how accurate are they at performing it?
* Usability related issues: how easy it uses the techniques, is it cognitively demanding?
* How natural and immersive the experience is.
* Expressiveness: flexibility user has with a given technique
* User comfort, does the user suffer from simulation sickness or tiredness
 
In application such as simulation and training you need the interaction to be as realistic as possible, so the users can apply their skills to the real world.
 
If developing a game, ease of learning is important to get as many people as possible involved.
 
If you are developing a tool for experts, for example a data visualization tool for neuroscientists to visualise MRI data. It needs to unsophisticated enough that once they have learned the interaction it engages fairly low cognitive load, so they can use it as a tool to solve more cognitively demanding tasks.
 
## Week 7 - no video lectures
 
## Week 8
 
### Introduction to Social VR and characters:
 
Verbal (speech) and non-verbal (body language) signals. Emoticons were designed to express non-verbal signals such as emotions. Online communication often over-simplifies or removes real-time social signal exchanges. VR is normally between real and digital social interaction, can combine both.
 
### Virtual characters:
 
Photorealistic and cartoon like characters. Anthropomorphic, non-humans having human features. Visual fidelity how real does a character look. Motion fidelity, more important, how does a character move. Avoid high visual fidelity and low motion fidelity. The visual fidelity sets the expectation.
 
### Agents and Avatars:
 
PC (player character or player) directly controlled, also called avatars. Agents (NPC) cannot be controlled but the player can interact with, NPC are controlled by algorithms.
 
### Applications of Virtual Characters:
 
In VR we interact with virtual characters.
 
### Introduction to character animation:
 
Unlike other animated objects, humans are very attuned to human animations, we can easily notice any mistakes or poor quality in human animations.
 
### Two basic ways to animate characters for VR:
 
* **Pre-recorded animations**:
Sequences of poses of a character that can be played back to create movement. Hand animation using keyframe animations or recorded from a real person using motion capture. This type of animation is not flexible, cannot be adapted to the moment, uses state machines. Can achieve complex movements.
 
* **Procedural simulations**:
Generating movement in real-time using code, such as eye-ball movement.
 
Most Body language is subconscious it’s not directly controlled by the person.
 
Uncanny Valley: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4428060/
 
Human conversation is highly complex, body language, speech, tone, personal space, posture etc …
 
**FK** = Forward kinematics takes longer to animates (for example, to move hand you first move arm => forearm => wrist => hand)
 
**IK** = Inverse kinematics (algorithm, much quicker to animate, you move hand - algorithm handles the rest)
 
Mocap is much faster, requires no artistic skills.
 
Facial expressions - we need to animate face and head movement.
 
**Facial Action Coding System (FACS)** - based on minimal facial movements we can make called action units
 
Facial bones is used to animate the face. Harder for animators. Animators normally use blend shapes (a complete copy of the face mesh with a different facial expression, animations are created by combining face meshes to form new expressions based on FACS)
 
Visemes - mouth shapes, the visual versions of the basic sounds (phonemes)
 
Importance of gaze in social interaction, eye contact shows that we are paying attention to someone, can indicate a range of social meanings, from intimacy to aggression.  We use eyes in very complex ways, not just for vision. Most part in VR we are controlling whether the character is looking at the player or not. Eyes are normally procedurally animated using inverse kinematics.
 
Blushing is easier with virtual characters, but not with humans - happens subconsciously (even the best actors cannot make themselves blush). The effect on participants happens on a subconscious level (try adding pale, gaze, small facial expressions to a virtual character) 
 
## Week 9
 
Abstract interfaces: we can try to keep the interaction, body based and use gestures to interact, can be tiring and hard to remember.
 
GUI are touchscreen interfaces in VR, real world is full of GUI, so it will probably feel natural to the user.
 
### Diegetic and non-diegetic UI
 
Non-diegetic interface: like health bars in games, not part of the game world- overlaid onto the screen. Works best in screen-based games.
 
### Diegetic interface:
Appears in the VR world, attached to objects or floating. Also known as spatial UI. On-body UI.

**Gesture Interaction:**
More likely to feel natural, if they are close to real world actions, easier to learn. Hard to implement, remember some cultures gestures have different meaning (nodding your head means yes in the west, but in some cultures, it may mean something else)
 
VR needs diegetic interfaces. UI can become pixelated, harder to read, small text won’t work. VR controllers are great for 3D interaction but not for complex detailed interaction. UI should be simple and big. UI in VR does not have a physical surface, needs to a have wide tolerance for interacting. UI should not be transparent, otherwise the user keeps staring at objects nearby and far away will cause and headache. Curved interfaces are better than flat interfaces.
 
Without testing the VR app, you are going to make the wrong assumption.
Some good advice for VR testing app: User Evaluation https://learn.gold.ac.uk/mod/helixmedia/view.php?id=606986&forceview=1
 
*The rest of videos are non-theory based, just advice.*
