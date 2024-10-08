# EXP-FX
EXP-FX, Il Sole e la Luna (eg. The Sun and the Moon) is an expansion module for [Sibilla](https://github.com/Clatters/Sibilla/tree/main), aiming to let you admire the same panorama under two different glows.

Depending on the Sibilla uploaded firmware, EXP-FX can either act as an actual Sibilla expander, giving you direct control on more Sibilla’s parameters, or can turn your module into a stereo pitchshifting droning effect, allowing you to process your favourite oscillator the same way Sibilla processes its internal waveforms.

## Table of contents

- [EXP (il Sole)](#EXP-il-Sole)
- [FX (la Luna)](#FX-la-Luna)
- [Firmware](#Firmware)

<br/><br/><br/>

## EXP (il Sole)
<h3 align="center">
Everything regarding EXP is written with golden graphics on the module faceplate.
</h3> <br/>

Expand your Sibilla by adding more control on the internal AR envelope and filter resonant frequency.
With the help of this firmware, Sibilla's controls stay untouched and the following EXP commands are added:
- **ATTACK**: sets the duration of the envelope attack stage. This is the time it takes for the envelope level to go from zero to the maximum level when a gate signal is received on   Sibilla’s trigger input. The duration is nearly zero with the knob fully closed, and 5 seconds when the knob is fully clockwise;
- **RELEASE**: sets the duration of the envelope release stage. This is the time it takes for the envelope to go from its maximum level back to 0 after the gate is released (max length is 5 seconds);
- **Q**: sets the peak level of Sibilla’s resonant LP filter (Resonance). When fully counterclockwise, resonant peak will be rounded and become more apparent with higher settings, depending on the harmonics created by Rise and Fall parameters of Sibilla.

#### Current draw
- +12V: 140mA;
- -12V: 33mA;
- +5V: 0mA;

## FX (la Luna)
<h3 align="center">
Everything regarding FX is written with white (black panel) or black (silver panel) graphics 
on the module faceplate.
</h3>
<br/>
With configurable eurorack/line stereo inputs, turns your Sibilla into an intricate stereo pitch shifting delay effect. Splits your incoming sound in two separate pitch shifted tracks whose stereophony is affected by LFOs movements, white noise, delay lines and sampled bits of audio.

When installing this firmware, the whole duo (FX + Sibilla) turns into an intricate stereo pitchshifting droning module with Sibilla's parameters performing the same functionalities as always, but applied to the incoming input audio signals:
- **RISE**: pitch-shifts (from low to high pitch) the incoming sound on the left channel;
- **FALL**: pitch-shifts (from high to low pitch) the incoming sound on the right channel;

As for Sibilla, the stereophony of these pitch-shifted tracks is affected by the movement of two free running LFOs with configurable waveforms and can be altered by a resonant LPF and the addition of a white noise source. Sibilla's sampling delay network is now open and can by directly modified by the user:
- **BUFFER SIZE**: controls the real time sampling window length. It’s nearly 100ms when the knob is fully closed and goes up to 1s with the knob fully clockwise;
- **FEEDBACK**: controls the amount of sampled and pitch shifted audio sent back into the sampler;
- **FREEZE**: manually freezes the audio buffer to the last recorded bit of audio. While freezed, the buffer size can still be modified;
- **GRAINS**: sets the starting position of the audio bits to be recorded into the buffer size (this feature still needs to be activated with a double tap on Sibilla's center button);

#### Current draw
- +12V: 142mA;
- -12V: 35mA;
- +5V: 0mA;

  ----

More information on both firmwares behavious are available by downloading the product manual pdf in the [downloads](https://clattersmachines.com/users-manual/) section of Clatters Machines website.

## Firmware

Regardless on the desired EXP or FX application, Sibilla needs to be reprogrammed n order to accept EXP-FX as an expansion module. The programming procedure is very similar to the one used to update Sibilla, but with a few extra steps. Please visit the dedicated section on the [Sibilla Setup and Programming page](https://github.com/Clatters/Sibilla/tree/main/Official%20firmwares).

