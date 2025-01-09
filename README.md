## Idea

Create a music visualizer on an LED ring. Different color patterns are implemented based on the frequency spectrum from a fast Fourier transform (FFT). Digital audio is passed to the microcontroller using a Bluetooth device.

## Materials Required
- **LED Ring:** Used for the visualization of music.
- **Bluetooth Device:** Used to get digital audio on the microcontroller.
- **Tiva Launchpad:** Microcontroller used to control the LED ring.

## Schematic

![Block Diagram](schematic.png)
*Figure 1: Block Diagram*

## Working
- Audio file format `.ogg` is used. The file is decoded to retrieve audio samples and metadata.
- These samples are transmitted via Bluetooth to the microcontroller.
- The microcontroller performs digital signal processing techniques, such as FFT and filtering, to obtain the frequency representation of the audio.
- This frequency representation is translated into LED ring visuals, and appropriate signals are passed to the LED ring.

## References

- Code Reference: [Music Visualizer](https://www.youtube.com/playlist?list=PLpM-Dvs8t0Vak1rrE2NJn8XYEJ5M7-BqT)
- Bluetooth Module Reference: [Bluetooth Module](https://github.com/mtayyip/Tiva-C-Series-TM4C123G-LaunchPad-HC06-Bluetooth-Module)

## Members

- Ayush Singhi (210020048)
- Kushal Mohta (210020023)
