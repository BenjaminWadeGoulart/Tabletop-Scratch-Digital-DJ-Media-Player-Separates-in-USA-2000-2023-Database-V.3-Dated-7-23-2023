Categories and variables presently included:
Brand, Model, and Year are self-explanatory, but announcements of a new product in December of a year may be coded for the next year if there is no evidence of the product being sold or even reviewed until the next year.
MaxKhz: The maximum supported sampling rate of the audio files that can be played. This is independent of what the SPDIF output runs at. The higher the sample rates supported, the more aggressive the real-time sample rate conversion (SRC) that is necessary to play any format. Higher quality SRC requires more processing throughput for a given max supported sampling rate.
TruDigOut: Digital SPDIF output is only counted if it is an actual in-situ digital signal to a coax that functions at all times and has no additional stages of DA to AD conversions. A few early units disable their SPDIF when the pitch fader or scratch mode is active, and the original CDJ-1000 had analog conversion in the path. In most cases, the next model resolved this in each brand’s lineup.
CD, MP3CD, USBplay, and SDplay all refer to source media that can be played from.
Bay is whether a hard drive can be installed into a bay inside the player.
SDcues: Storing cue and memo points on SD cards. Some allow this storage of bookmarks in the tracks while not allowing playback of actual music from the card.
Dual: Has dual or layers mode where two tracks can be played at once from a single deck separate. This capability requires more processing throughput to handle, and obviously double the audio outputs on the back.
MultiCue: More than one cue point can be temporarily set.
ASIO: Has the ability to function as a USB audio device or soundcard output when connected to a computer with proper software drivers. Useful with MIDI & HID.
MIDI: Can send older-style musical instrument instructions to a computer, either over MIDI cable or USB. Instructions back to the unit are mostly limited to LEDs and timecode.
HID: Two-way controller communications with computer over USB, which includes not only MIDI-style commands but complex info back to the unit’s screen.
Touch: Jog wheel platter is touch-activated, which simulates holding the record.
Motor: Platter has a motor like a turntable and rotates when motor or vinyl mode is activated.
JogZone: When no motor is active, jog wheel platter rotation has a deadzone whereby no pitch bend is registered until velocity, time, or distance past a certain rotation threshold is reached.
Ramp: Jog bend is time-based, rather than rate-based and thus is cumulative or progressive as jog bending continues. This necessitates brief nudges to use effectively for bending, but may improve some scratch emulations.
Digits: Number of pitch percentage digits to the right of the decimal place displayed.
PitchLow: Pitch increments for lowest pitch range.
PitchMed: Pitch increments for medium pitch range, usually about the 10-25% range.
PitchHigh: Pitch increments for the highest pitch range, usually 50-100%. If the highest range on a player is much lower than 50%, this may need to be left blank and the unit’s highest relegated in PitchMed.
Ranges: The number of available unique pitch fader ranges that can be switched between. Players with crude PitchHigh increments can compensate with more available pitch ranges to choose from such that the lowest range that will still allow the required speed change to sufficiently beatmatch can instead be chosen, and thereby maximize pitch resolution and shrink the size of the increments.
RandInc: In some players, pitch fader positional increments are not discrete and always repeatable, but rather are slightly randomized in how the position is sampled and registered. This can spoof a higher effective pitch fader resolution as the user wiggles over the same spot to choose a different value.
Sync: This is auto sync, but just because the unit has it, does not mean the function is reliable, which requires either reliable waveform analysis on the unit or preparation software. Older BeatKeeper-style functionality meant for smart loops may reliably detect the BPM or timing alone, but may not detect the correct downbeat to keep things in alignment for sync to work sufficiently between decks.
FullFFA: Unit has onboard, full Fast Fourier Analysis of audio waveforms.
PrepSoft: Preparation software is available from the branding for use with the unit. This could be rudimentary software just for building a searchable database or setting cue points, or it may also include its own FFA waveform analysis and library system.
Samp: Onboard audio sampler for playing back brief sections of music that does not simply store the data on a removable media.
Filter: Sweepable audio filter.
Effects: This includes audio effects besides filter or the basic vinyl emulation effects (scratching, braking, and reverse) that are already a requirement for inclusion in this data set of tabletop digital DJ media players with some turntable simulation. These acceptable effects often includes flanger, echo, or optional vinyl ‘warmth’ sound quality simulators.
KeyCh: Unit allows key to be changed to something other than original key and independent of the pitch fader. All units evaluated already have the ability to optionally lock to the original key even when the pitch fader is away from zero.
AdvKey: Uses sophisticated interpolation keylock or key change beyond the old, simple technique. The old style is excellent with the key locked lower than the pitch warrants, or rather the key locked to original and the speed increased, but breaks up in the reverse situation (key locked to original and speed slowed) as the disparity from original speed occurs. Newer techniques require greater processing throughput to achieve, have less dependence on key & speed shift direction, but also may degrade fidelity simply turning the processing on without deviating the key or speed from original.
Link: At least a pair of these tabletop scratch DJ players can be linked to each other to at least share source media. Linking that can only share timecode or cue & memo points are not counted. This source sharing may be done using daisy-chained USB cables, crossover cable, or Ethernet cables, and may do more than just source sharing.
Auto: A proxy for beat sync automation that requires the use of sync, preparation software ahead of time, and link, but that does not require onboard, full FFA. It is a composite binary/Boolean value using the formula:
Auto=Sync*PrepSoft*Link
