This is a clone of Reason's Subtractor synthesizer. It requires Pd-extended, but we are currently working on porting it to Vanilla.  Extended was used primarily for convenience.

It uses patches from Pd for LibPd, but it should have a copy of all the required patches in the Pd_for_LibPd_dependencies folder.  See the Pd-for-LibPd Repo for more info.

Subtractor.pd is the main patch.  It manages its state and will automatically save when necessary.  There are a few presets already, and you can easily add more with the "save" button.

All the presets are stored in the Subtractor-presets.pd patch.  If you want to use someone else's presets, you could import their version of Subtractor-presets.pd and it should work.  The patch also contains instructions on how to import an individual preset from another Subtractor-presets module.

The majority of the DSP is done in the Subtractor-voice.pd patch.  There are 16 voices in Subtractor.pd by default.

The midi folder contains example MIDI files you can play through the synth using the seq object from pd-extended.