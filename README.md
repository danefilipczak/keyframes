# Composition experiments using [MusicVAE](https://magenta.tensorflow.org/music-vae).  
In Progress. 

MusicVAE is a new model from the Magenta team at Google that affords some neat tricks. I'm going to explore what forms these new tools suggest, starting with the ability to smoothly interpolate between melodic fragments. 

For now, I'm taking bits of easily recognizable tunes and interpolating between them, then using the best results as cantus firmi for polyphonic compositions. For now, I'm not editing or modifying the MusicVAE output, except for octave displacement (basic orchestration). I'll be as transparent as possible about what arises from the VAE and what from my hands.



# Frère Jacques (C) -> La Marseillaise (G) -> Frère Jacques (A). Woodwind Quintet

[Full Audio](https://dfilipczak.github.io/keyframes/audio/1/keyframes1.wav)

[Score](https://dfilipczak.github.io/keyframes/scores/keyframes1.pdf), MusicVAE contribution shown in blue.


[Loop 0](https://dfilipczak.github.io/keyframes/audio/1/0.wav), Frère Jacques in C Major.

[Loop 1](https://dfilipczak.github.io/keyframes/audio/1/1.wav), La Marseillaise in G Major.

[Loop 2](https://dfilipczak.github.io/keyframes/audio/1/2.wav), Frère Jacques in A Major.

[Interpolation of 0 to 1](https://dfilipczak.github.io/keyframes/audio/1/0to1.wav), over 7 repetitions

[Interpolation of 1 to 2](https://dfilipczak.github.io/keyframes/audio/1/1to2.wav), over 10 repetitions

[Combined MusicVAE contribution](https://dfilipczak.github.io/keyframes/audio/1/0to2.wav)

## Notes

MusicVAE output is consistently musical throughout the interpolation, even when it makes bold decisions. Some interesting moves are the staccato figure it introduces at measure 13 and the detached quarter notes starting at measure 38. In both cases I tried to highlight rather than mask these interesting maneuvers and developed them as motifs. 

MusicVAE's manner of interpolation is "correct", for lack of a better word, and makes good musical sense - however, it isn't necessarily intuitive. Both input melodies are legato with no rests, and the interpolation includes lots of staccato and sometimes jarring gaps. If I were to interpolate by hand, it would seem most obvious to maintain legato throughout. 

