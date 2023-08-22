# wasp-2023-summer-school

## Welcome

This repository hosts the full pipeline code for the WASP summer school 2023 group assignments. The system contains three major components, with corresponding resources broken down into the following folders:

- Generating text with a text prompt : [`./subsystem1_text-generation/`](https://github.com/Svito-zar/wasp-2023-summer-school/tree/main/subsystem1_text-generation)
- Synthesizing speech from text : [`./subsystem2_text-to-speech/`](https://github.com/Svito-zar/wasp-2023-summer-school/tree/main/subsystem2_text-to-speech)
- Generating gesture animations from audio : [`./subsystem3_gesture-generation/`](https://github.com/Svito-zar/wasp-2023-summer-school/tree/main/subsystem3_gesture-generation)

The Monday student assignment presentation is in file `student-assignment.pptx`.

The demo video for the student assignment shown on Monday can be found [on YouTube](https://www.youtube.com/watch?v=by40aaCbLpY).

## Agenda
In the assignment you will be dealing with various systems. The primary goal is to first familiarize you with these systems, and then to use what you learned before making your final submissions.

The information below is derived from the original agenda [here](https://internal.wasp-sweden.org/event/wasp-summer-school-synthesis-of-human-communication-2023/). It will likely not be updated in case of any changes, but you will be notified on Slack (in the `general` channel for now).

- Monday 15:30 - Presentation of assignment
- Tuesday 14:00 - 16:00 - Work on [text generation tutorial](https://github.com/Svito-zar/wasp-2023-summer-school/tree/main/subsystem1_text-generation)
- Wednesday 10:00 - 12:00 - Work on [text to speech tutorial](https://github.com/Svito-zar/wasp-2023-summer-school/tree/main/subsystem2_text-to-speech)
- Wednesday 14:20 - 16:00 - Work on [gesture generation tutorial](https://github.com/Svito-zar/wasp-2023-summer-school/tree/main/subsystem3_gesture-generation)
- Wednesday 16:00 - 17:00 - Work on the tutorials
- Thursday 09:00 - 12:00 - Work on final assignment
- **Thursday 12:00 - Submission deadline**
- Friday 09:00 - 12:00 - Demo of your submissions in the 3D dome

## Assignment
The goal of the student assignment is for you to be creative and tell your own story by using the tools you interacted with during the tutorial sessions. Last year, the students completed a similar assignment, in which they created stories in a "free-for-all" theme. You can view the result of their submissions online:
- [Team 1 submission](https://www.youtube.com/watch?v=IyaEcUJp6G8)
- [Team 2 submission](https://www.youtube.com/watch?v=OJMNvtoPsfk)
- [Team 3 submission](https://www.youtube.com/watch?v=3mwK3OCXH9k)
- [Team 4 submission](https://www.youtube.com/watch?v=h8z85fxWz10)

This year we are changing the theme to "participation in a popular talent show". The stories that you craft and submit are encouraged to fit into the "talent show" theme, but do not feel overly constrained by it; use it primarily for inspiration.

You can expect to follow this process when completing the assignment:
1. You use LLMs to generate a script for your story
2. You use Text2Speech to generate audio for the script
3. You use Speech2Gestures to generate animations
4. You iterate on the above steps
5. When satisfied, you submit to us

For the audio files, you are free to use any AI generated voice or even your own voice. You can stich multiple audio files or add silence if you wish to control pacing. Please make sure that you re-generate your animations when making changes.

When you send us your submission, we will put together a video sequence showcasing what you created. We will put a brief intro / outro at the beginning / end of your story, similar to how we did with the white avatars during the Assignment Demo. (*TODO: Upload the demo and presentation after day is over*)

### Submission instructions
To submit, send an email to `tnikolov@hotmail.com` OR `tsakovm@gmail.com`.

Your submission should be **2-5 minutes** long and be composed of the following files:
- a `.zip` of `.fbx` files
- a `.zip` of `.wav` files
- a `.txt` file

The `.fbx` and `.wav` files should be named in ascending order, starting from 0, in the order that they should be played back. Append `A`, `B`, `C`, `D` or `E` to each file to indicate which avatar you wish to use for the animation. The `.fbx` files are extracted using the gesture generation system.

<p align="center">
  <img src="https://github.com/Svito-zar/wasp-2023-summer-school/blob/main/avatars.png" alt="The 5 avatars to choose from.">
  <br>
  <i>The 5 avatars to choose from.</i>
</p>

*Example:*
- fbx.zip
    - 0A.fbx
    - 1C.fbx
    - 2C.fbx
    - 3B.fbx
    - 4C.fbx
    - 5D.fbx
- wav.zip
    - 0A.wav
    - 1C.wav
    - 2C.wav
    - 3B.wav
    - 4C.wav
    - 5D.wav

The `.txt` file should contain the following information:
- Team name or ID
- World

*Example:*
- Jackal.txt
    - Team "Jackal"
    - World "Tropical island"

We have the following teams this year:
1. *Algorithmic Amigos*
2. *VR WASP Wizards*
3. *Artificial Four*
4. *Quebec*
5. *Lucasfilm Ltd TM*

We offer 5 worlds to choose from:

**Egypt**
<p align="center">
  <img src="https://github.com/Svito-zar/wasp-2023-summer-school/blob/main/Images/Egypt2.png" alt="Egtpy.">
</p>

**Asian village**
<p align="center">
  <img src="https://github.com/Svito-zar/wasp-2023-summer-school/blob/main/Images/AsianVillage2.png" alt="Asian village.">
</p>

**Tropical island**
<p align="center">
  <img src="https://github.com/Svito-zar/wasp-2023-summer-school/blob/main/Images/Tropical2.png" alt="Tropical island">
</p>

**Venice**
<p align="center">
  <img src="https://github.com/Svito-zar/wasp-2023-summer-school/blob/main/Images/Venice2.png" alt="Venice.">
</p>

**ForestLevel**
<p align="center">
  <img src="https://github.com/Svito-zar/wasp-2023-summer-school/blob/main/Images/ForestLevel2.png" alt="Forest level">
</p>

You can find more examples in the [images](https://github.com/Svito-zar/wasp-2023-summer-school/blob/main/Images/) folder.
