# EXP-FX
EXP-FX, Il Sole e la Luna (eg. The Sun and the Moon) is an expansion module for [Sibilla](https://github.com/Clatters/Sibilla/tree/main), aiming to let you admire the same panorama under two different glows.

Depending on the Sibilla uploaded firmware, EXP-FX can either act as an actual Sibilla expander, giving you direct control on more Sibilla’s parameters, or can turn your module into a stereo pitchshifting droning effect, allowing you to process your favourite oscillator the same way Sibilla processes its internal waveforms.

![EXP-FX](EXP-FX_black&silver_render.png)

## Table of contents

- [Installation and firmware upload](#Installation-and-firmware-upload)
- [EXP (il Sole)](#EXP-il-Sole)
- [FX (la Luna)](#FX-la-Luna)
- [Power consumption](#power-consumption)




<br/><br/><br/>

## Installation and firmware upload

### Installation

EXP-FX connects to Sibilla with a small 12 contacts, 0.635mm pitch ribbon cable following the same rules of Eurorack power ribbon cables.
> [!WARNING]
> Cable's red stripe is indicated on the module pcb by a white line (EXP-FX) and small white dot (Sibilla).
Please watch carefully the manual's illustration before connecting EXP-FX to Sibilla.

### Firmware upload

> [!IMPORTANT]
> Regardless on the desired EXP or FX application, **Sibilla needs to be reprogrammed in order to accept EXP-FX as an expansion module.**

The programming procedure is very similar to the one used to update Sibilla, but with a few extra steps; it doesn't require any external program nor file to be downloaded and it can be entirely performed on Clatters Machines' website. Please visit the dedicated section on the [Sibilla Setup and Programming page](https://github.com/Clatters/Sibilla/tree/main/Official%20firmwares).

## EXP (il Sole)
<h3 align="center">
Everything regarding EXP is written with golden graphics on the module faceplate.
</h3> <br/>

Expand your Sibilla by adding more control on the internal AR envelope and filter resonant frequency.
With the help of this firmware, Sibilla's controls stay untouched and the following EXP commands are added:
- **ATTACK**: sets the duration of the envelope attack stage. This is the time it takes for the envelope level to go from zero to the maximum level when a gate signal is received on   Sibilla’s trigger input. The duration is nearly zero with the knob fully closed, and 5 seconds when the knob is fully clockwise;
- **RELEASE**: sets the duration of the envelope release stage. This is the time it takes for the envelope to go from its maximum level back to 0 after the gate is released (max length is 5 seconds);
- **Q**: sets the peak level of Sibilla’s resonant LP filter (Resonance). When fully counterclockwise, resonant peak will be rounded and become more apparent with higher settings, depending on the harmonics created by Rise and Fall parameters of Sibilla.

## FX (la Luna)
<h3 align="center">
Everything regarding FX is written with white (black panel) or black (silver panel) graphics 
on the module faceplate.
</h3> <br/>

With configurable eurorack/line stereo inputs, turns the whole duo (FX + Sibilla) into an intricate stereo pitch shifting delay droning effect. Splits your incoming sound in two separate pitch shifted tracks whose stereophony is affected by LFOs movements, white noise, delay lines and sampled bits of audio.

When installing this firmware, Sibilla's parameters perform the same functionalities as always, but applied to the incoming input audio signals:
- **RISE**: pitch-shifts (from low to high pitch) the incoming sound on the left channel;
- **FALL**: pitch-shifts (from high to low pitch) the incoming sound on the right channel;

As for Sibilla, the stereophony of these pitch-shifted tracks is affected by the movement of two free running LFOs with configurable waveforms and can be altered by a resonant LPF and the addition of a white noise source.

In addition, Sibilla's sampling delay network is now open and can be directly modified by the user:
- **BUFFER SIZE**: controls the real time sampling window length. It’s nearly 100ms when the knob is fully closed and goes up to 1s with the knob fully clockwise;
- **FEEDBACK**: controls the amount of sampled and pitch shifted audio sent back into the sampler;
- **FREEZE**: manually freezes the audio buffer to the last recorded bit of audio. While freezed, the buffer size can still be modified;
- **GRAINS**: sets the starting position of the audio bits to be recorded into the buffer size (this feature still needs to be activated with a double tap on Sibilla's center button);

A small switch on the back of the module is used to shift between Eurorack and Line input signal. When **Line inputs** are configured, the **Line Gain** knob can be used to tame the incoming audio signal.

  ----

Every knob but the Line Gain is CV controllable and accepts ±5V while the Freeze button can be activated with external triggers.

  ----

More information on both firmwares behavious are available by downloading the product manual pdf in the [downloads](https://clattersmachines.com/users-manual/) section of Clatters Machines website.

## Power consumption

EXP-FX doesn't draw current directly from your system but relies on Sibilla's power; for this reason, depending on the uploaded firmware, Sibilla's power consumption will change as follows:

- **EXP**
  - +12V: 140mA;
  - -12V: 33mA;
  - +5V: 0mA;

- **FX**
  - +12V: 142mA;
  - -12V: 35mA;
  - +5V: 0mA;

