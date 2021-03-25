# Piano technique

Let's make piano exercises e.g. scales and arpeggios more fun!

## todo

* Convert this list into a project plan.
* Design diagrams.
* Minimal API example: /hello returns "Hello World"
  * API endpoint in server.
  * Connect via Router in Express.
  * Client side just display plaintext.
* Two phases (expanded below):
  1. MIDI input (easier, but limited to digital pianos)
  2. Raw audio input (extra step: convert to note on/off timings)
* Convert time from absolute to elapsed, with first note on defining t=0.
* Generate exercises starting with C major scale.
  * Add other scales and arpeggios in order of [Trinity book](https://shop.trinitycollege.com/shop/prod/Trinity-College-London-Piano-Scales-Arpeggios-from-2015-Initial-Grade-5/2104331).
* Given an exercise and a performance of it, assign a score accounting for:
  * Tempo consistency.
  * Volume consistency (from note velocity).
  * Missing notes.
  * Extra notes.
* Track progress:
  * Scores over time, grouped by exercise.
  * Database? Cache? User accounts?
  * Pick up where you left off.
* Choose useful libraries e.g. for MIDI, FFT.

### todo: MIDI

* Extend [Web MIDI](https://www.w3.org/TR/webmidi/) examples.
* Pair note off events with note on events, determine time on.
* Piano emulator to test without hardware available? (Just emit MIDI messages.)

### todo: raw audio

* Convert raw audio to note on/off timings.
* Piano emulator to test without hardware available?

## Useful links

* [spectro](https://github.com/calebj0seph/spectro): real-time audio spectrogram generator for the web. It can visualise sound from your microphone or audio files on your device. Stack: React, Node.
* [MERN project setup: medium.com](https://medium.com/how-to-react/setup-mern-mongodb-express-js-react-js-and-node-js-environment-and-create-your-first-mern-7774df0fff19)
* [MERN part 1 JS Mastery](https://www.youtube.com/watch?v=ngc9gnGgUdA&t=0s)