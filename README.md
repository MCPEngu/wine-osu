# wine-osu

Original PKGBUILD from ThePooN and Geno: https://gitlab.com/telastrus/wine-osu & https://blot.thepoon.fr/osuLinuxAudioLatency
Original Patches from gonX, openglfreak and tdeo
**Join ThePooN's Discord Server for any questions and problems regarding running osu! using Wine https://discord.com/invite/thepoon**

The `master` branch uses stable wine and seems to work the best, but the `staging` branch is available if you want to play around. 

**NOTE: CURRENTLY AUDIO COMPATIBILITY MUST BE TURNED ON IN osu! FOR THIS TO WORK** (probably a bug, still investigating)

**NOTE: MUST BE BUILT WITH GCC UNDER 10 AS IT BREAKS ONE OF THE DLL FILES, WILL FIND THE FIX LATER AS THIS IS A WORKAROUND**

Environment variables:

- `DEFAULT_MINREQ` - set this flag to use winepulse's default PulseAudio minimum request
- `PULSE_TLENGTH` - override the default (1000) target length for Pulse
- `PULSE_OVERRIDE_MIN` - set this to keep wine from forcing the minimum and default period; I've had success with this flag
- `STAGING_AUDIO_DURATION` - set the staging audio duration; I've had success with this being set to 10000, but this varies from PC to PC, so I recommend tweaking this to your liking
- `STAGING_AUDIO_PERIOD` - set the staging audio period; I use 3000, but same disclaimer from above applies
