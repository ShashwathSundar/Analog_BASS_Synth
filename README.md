This Bass Synth is basically a single voice synth that can be powered by 5V USB.
I am achieving this by faking a bi-polar sypply by first, boosting the 5V to 10V using a boost converter.
Mid-rail voltage is 5V generated using a 7905 (not 7805!! ) negative voltage regulator.
7905 regulator acts as a current sink for all the circuits that need to be connected to the mid rail ground.

There are 4 circuits for building the synth:
VCO - Voltage controlled oscillator made with a CD4046 PLL VCO chip (exponential converter by Rene Schmittz).
VCF - Voltage controlled filter inspired by Korg monotron's filter design.
VCA - Voltage controlled amplifier inspired by Korg MS10's VCA design.
ENV - Simple envelope generator inspired by Roland TB-303 controls (it just has Decay control ;P ).

Since the outside world's GND is -V for the synthesizer, the CV/gate inputs and audio output are referenced to GND (-V) and not the internal 5V mid rail reference.

A Demo for the Synth and its build process is on Instagram (might do a youtube vid soon ;) ).

NOTE: The "Signal Flow" and "Supply Loading" Sheets are only for reference and not a part of the synth schematic.
