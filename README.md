# polyphonic-FM-synth
### Overview:

***Max***, also known as Max/MSP/Jitter, is a visual **programming language** for music/ audio development. It is built upon the JUCE framework written in C++.

***Max for Live*** is a **platform** to build custom instruments and audio effects/ tools for audio production, visuals, and much more. Max devices are open source and highly customizable and can built from scratch or on top of other devices using the same components.

***Max for Live devices*** can be configured as standalone applications, but are generally used as a **plugin** in a Digital Audio Workstation(DAW), which in the case of Max for Live devices is **Ableton Live**.

Max for Live can completely change how Live interacts with all things external. Reconfigure connections to hardware controllers & synthesizers. Route audio to multiple sets of speakers from your Live project. Use Live to control physical objects like motors and lights using Arduino, OSC and other technologies—there are infinite possibilities for connection and control between Live and the world surrounding it.

### The Synth Instrument:

The Polyphonic FM Audio Instrument looks like this:

![Poly Synth](https://user-images.githubusercontent.com/110298158/183830142-34f4615b-fae8-46a6-9ded-6807e003d5e4.png)

It contains the following parts:

- ***Carrier*** :
- ***Modulator*** :
- ***Mixer Tools*** :
- ***Master Filter*** :
- ***Master Volume*** :
- ***Modulation Matrix*** :

### Steps:

- The [**.amxd**](https://github.com/av-neesh/polyphonic-FM-synth/blob/main/poly_avneesh_synth.amxd) Ableton Max Device file is the master file for running the device as a plugin in Ableton Live.
- Locate the path of Max Instruments from the Ableton Live directory and drag drop the .amxd file into the folder.
- Then refresh the browser and reload the project

            Ableton Browser -> Categories -> Max for Live -> Max Instrument -> **poly_avneesh_synth.amxd**
            
- Drag and Drop the .amxd file into the **instrument rack**. The sample project workspace would look something like:

![Sample workspace](https://user-images.githubusercontent.com/110298158/183826747-2ecc340b-e646-4acf-a2ca-0377612c144c.png)

- Click on **Edit Button** in top right corner of the instrument.
- The Max Editor will open in a few seconds. The editor would look something like this:

![Max Editor](https://user-images.githubusercontent.com/110298158/183827300-d455aa23-cb86-4a45-93a9-8b750fbd000f.png)

- Click again on Presentation Mode, to return to the Edir Mode. Unfreeze the scenario if needed. The editor would look like this:

![Edit Mode](https://user-images.githubusercontent.com/110298158/183827635-452f7a20-d9f6-471e-9143-58563b83352e.png)

- Follow the path:
            
            Options -> File Preferences -> userpath

, note the path into the file explorer and paste the [**.maxpat**](https://github.com/av-neesh/polyphonic-FM-synth/blob/main/poly_avneesh_patch.maxpat) Max patch file into the directory.
- The previous step is very important to ensure polyphony in the synthesizer.
- Ensure that the Max patch file when opened in Max Editor looks like this:

![Max Patch file](https://user-images.githubusercontent.com/110298158/183829022-4c22c59a-64ca-4854-b289-1b43a68b997d.png)

- **NOTE**: If the polyphonic synth, doesn't produced modulated sound, or any other issues occur, use the Monophonic synth only: [**mono_avneesh_synth.amxd**](https://github.com/av-neesh/polyphonic-FM-synth/blob/main/mono_avneesh_synth.amxd).
- The monophonic synth doesn't need a patch file to be loaded, and can be directly used as a Max instrument repaeating the above steps (excluding loading the patch file).
