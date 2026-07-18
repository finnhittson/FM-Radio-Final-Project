# Stanford EE 251 - High Frequency Circuit Design

This repo documents the completed labs in EE 251 that were used to make an FM radio receiver. The radio itself was made using FR4 boards, copper tape, discrete BJTS, and passive components like capacitors, resistors, and inductors. The circit was simulated in blocks using LTSpice to validate our design before building nad to help debug our boards after we built them. The first block of our radio (i.e. the front end) freatured a cascaded broadband and narrowband amplifier. This was to boost the antenna signal and selectively amplify frequencies of interest. The second block was our mixer oscillator combo. This amplified signal are fed to a mixer, driven by a Colpitts oscillator, which mixed the signal down to an intermediate frequency. The final block was then an IF amplifier for selective filtering and gain, followed by a democulation stage to extract the audio signal for the speaker.


## First Block - Broadband and Narrowband Amplifier

The front end of our radio consists of a narrowband and broadband amplifier. The signal recieved off of the antenna is very small and needs to be gained up in order to do any signal processing and eventually hear a signal through a speaker. The broadband amplifier amplifies everything from DC to daylight and is used as a quick and easy way to get gain at the expense of gaining everything including the noise floor. The narrow band amplifier is used to selectivly gain the frequencies of interest and attenuate everything else.

### Broadband Amplifier

The broadband amplifier used the common emitter topology with feedback. To help get a wide bandwith the feedback is rolled off with a parallel capacitor which helps the amplifier have a flatter higher gain at higher frequencies. A detailed discussion of our design choises and the performance of our built broadband amplifier can be found in `Lab2/`. Below our schematic and an image of our assembled board.
![Broadband schematic and photo of assembled board.](lab2/images/broadband_schematic_and_board.png)

## Second Block - Mixer and Colpitts Oscillator



## Third Block - IF Amplifier and Demodulation


