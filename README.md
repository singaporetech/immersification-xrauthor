# XRAuthor

An open source tool to create learning content of multiple formats by using a simple webcam.

A short demonstration of XRAuthor is as seen below.

[demo.webm](https://github.com/singaporetech/immersification-xrauthor/assets/3720988/9de13d89-6aa1-429f-afbe-76113f737830)

## Research Question

> How to design an authoring tool that allows educators to effectively create learning content based on a particular physical learning activity to be delivered in multiple formats of different immersion levels (i.e., video, interactive and VR formats)?

## Usable Artifact

### Live Demo

[Author app (tree sort)](https://xredu.dev/author/tree%20sort)

[Learner app (tree sort)](https://xredu.dev/learn/tree%20sort)

[Author app (new session)](https://xredu.dev/author/)

## Prototype Design

The core design of the tool is to help educators create interactive learning content in multiple formats via a simple and familiar process. It lets users record demonstration videos with markers and only requires minimal user inputs of video segmentation to generate the following three formats (see Fig. 1) of interactive learning content automatically:

- Video Format: footages recorded by webcam, augmented with virtual object overlay, segmented into steps, having multiple-choice questions for each step, used on a computer;
- Interactive Format: animations of virtual objects with/without video background, having interactive tasks for each step, used on a computer;
- VR Format: animations and tasks in immersive VR environments (classroom or some relevant surroundings), being able to show/hide the recorded video.

![learner-task](https://user-images.githubusercontent.com/3720988/183364397-20722d23-c27b-40be-a898-d9106d6c5ace.png)
Fig. 1. (A) Video Format: a participant answering a multiple-choice question in a standalone web app, (B) Interactive Format: a participant interacting with cubes to complete a step of the learning content embedded in the Wikipedia page of tree sort, and (C) VR Format: a participant completing a step in VR.

Considering accessibility, we implemented the tool to run in a web browser on a computer without any installation. It has a minimalist UI (see Fig. 2), having four buttons for the tool's major modes at the top, a viewing area for displaying authored content in the middle and a progress bar with editing and playing controls at the bottom.

![author-ui](https://user-images.githubusercontent.com/3720988/183364641-08e08d7e-2273-4975-96ff-53d475573c27.png)\
Fig. 2. A video recording is being edited in the tool.

After setting up the markers, the authoring process could start with recording a regular demonstration video and afterwards have an edit-review loop on the video footage until the author is satisfied with the content and upload it to the server (see Fig. 3). The content could be used as a standalone web app or be embedded into existing web pages. Learners could access the content online in the preferred format (see Fig. 1).

![author-process](https://user-images.githubusercontent.com/3720988/183364600-3c816646-19c8-4967-ad85-45e45225c33c.png)\
Fig. 3. Tool Authoring Process

The following describes the detailed steps of the process:

1. Launch the app in the browser and click "Set up'' button to show video inputs from the camera;
2. Show cards (or other physical objects) with markers in front of the camera and check if the app show the augmented video (overlaying virtual objects at the positions of the markers);
3. Click virtual objects on the screen to change their visual settings and text labels;
4. Click "Complete setup'' after the markers are ready for recording;
5. Click "Record'' to start recording the augmented video and generating the animation;
6. Use cards to demonstrate learning contents (e.g., computer sorting algorithms);
7. Click "Complete recording'' after the demonstration (clicking "Record'' again could start to record another footage for a new session or just replacing the current one);
8. Click "Edit'' to show and review the recorded video and animation;
9. Click "Video Format'', "Interactive Format'' or "VR Format'' to show the content in different formats;
10. Use the progress bar with editing controls to segment the video and animation into steps (the app generates interactive tasks and questions after the steps are created);
11. Click the step buttons to replay and review the video and animation of steps;
12. Review and complete the step tasks in the Interactive or VR Format (using mouse to move virtual objects to required positions after step animations are played);
13. Review and complete the multiple choice questions for steps in the Video Format;
14. Use the progress bar to adjust the start or end positions of the steps (the app regenerate the tasks and questions accordingly), add or remove steps, if necessary;
15. Click "Complete editing'' when the content is satisfying;
16. Click "Publish'' to upload the content to the server for generating the webpage of the learning contents with multiple formats.

**Markers:**

![3x4mb-1](https://user-images.githubusercontent.com/3720988/212082838-3d77819e-c782-489c-8a14-eadfc64bae28.png)

## Papers

### The Paper Motivating the Tool Design

- [Full access at Frontiers in Virtual Reality](https://www.frontiersin.org/articles/10.3389/frvir.2021.597487)

- The bibtex:

```bibtex
@ARTICLE{10.3389/frvir.2021.597487,
  
AUTHOR={Shen, Songjia and Chen, Hsiang-Ting and Raffe, William and Leong, Tuck Wah},   
  
TITLE={Effects of Level of Immersion on Virtual Training Transfer of Bimanual Assembly Tasks},      
 
JOURNAL={Frontiers in Virtual Reality},      
 
VOLUME={2},           
 
YEAR={2021},      
   
URL={https://www.frontiersin.org/articles/10.3389/frvir.2021.597487},       
 
DOI={10.3389/frvir.2021.597487},      
 
ISSN={2673-4192},   
   
ABSTRACT={The availability of consumer-facing virtual reality (VR) headsets makes virtual training an attractive alternative to expensive traditional training. Recent works showed that virtually trained workers perform bimanual assembly tasks equally well as ones trained with traditional methods. This paper presents a study that investigated how levels of immersion affect learning transfer between virtual and physical bimanual gearbox assembly tasks. The study used a with-in subject design and examined three different virtual training systems i.e., VR training with direct 3D inputs (HTC VIVE Pro), VR training without 3D inputs (Google Cardboard), and passive video-based training. 23 participants were recruited. The training effectiveness was measured by participant’s performance of assembling 3D-printed copies of the gearboxes in two different timings: immediately after and 2 weeks after the training. The result showed that participants preferred immersive VR training. Surprisingly, despite being less favourable, the subjects’ performance of video-based training were similar to training on HTC VIVE Pro. However, video training led to a significant performance decrease in the retention test session 2 weeks after the training.}
}

```

- The formatted text (Chicago Manual of Style 17th edition):

```text
Shen, Songjia, Hsiang-Ting Chen, William Raffe, and Tuck Wah Leong. 2021. “Effects of Level of Immersion on Virtual Training Transfer of Bimanual Assembly Tasks.” Frontiers in Virtual Reality 2. https://doi.org/10.3389/frvir.2021.597487.
```
