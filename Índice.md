# Índice 
## Contenidos 

[[Prólogo]]. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .ix 

[[Prefacio]]. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . xi

1. [[Sinusoides, amplitud y frecuencia]] . . . . . . . . . . . . . . . . . . . . . . . .1
	1.1 [[Medidas de Amplitud]] . . . . . . . . . . . . . . . . . . . . . . . . 3
	1.2 [[Unidades de Amplitud]] . . . . . . . . . . . . . . . . . . . . . . . . . . 4
	1.3 [[Control de Amplitud]] . . . . . . . . . . . . . . . . . . . . . . . . 6
	1.4 [[Frecuencia]] . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
	1.5 [[Sintetizando Ondas Sinusoidales]] . . . . . . . . . . . . . . . . . . . . 8
	1.6 [[Superposición de señales]] . . . . . . . . . . . . . . . . . . . . . . . . . 10
	1.7 [[Señales periódicas]] . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12
	1.8 [[Ejemplos acerca del Software]] . . . . . . . . . . . . . . . . . . . . 15 
		[[Introducción Rápida a Pd]] . . . . . . . . . . . . . . . . . . . . . . 15 
		[[Cómo encontrar y ejecutar los ejemplos]] . . . . . . . . . . . . . . . . . 17
	1.9 [[Ejemplos]] . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 17 
		[[Escalador de amplitud constante]] . . . . . . . . . . . . . . . . . . . . . . 17 
		[[Control de amplitud en decibeles]] . . . . . . . . . . . . . . . . . . . . 18 
		[[Control de amplitud suavizado con un generador de envolvente]] . . . . . 21 
		[[Tríada mayor]] . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 22 
		[[Conversión entre frecuencia y tono]] . . . . . . . . . . . . . . 22 
		[[Más síntesis aditiva]] . . . . . . . . . . . . . . . . . . . . . . . 23 
	[[Ejercicios]] . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 24

2 Wavetables and samplers 27

1. The Wavetable Oscillator . . . . . . . . . . . . . . . . . . . . . . 29
1. Sampling . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 32
1. Enveloping samplers . . . . . . . . . . . . . . . . . . . . . . . . . 36
1. Timbre stretching . . . . . . . . . . . . . . . . . . . . . . . . . . . 37
1. Interpolation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 43
1. Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 47 Wavetable oscillator . . . . . . . . . . . . . . . . . . . . . . . . . 47 Wavetable lookup in general . . . . . . . . . . . . . . . . . . . . . 48 Using a wavetable as a sampler . . . . . . . . . . . . . . . . . . . 50

iii

iv CONTENTS

Looping samplers . . . . . . . . . . . . . . . . . . . . . . . . . . . 52 Overlapping sample looper . . . . . . . . . . . . . . . . . . . . . . 54 Automatic read point precession . . . . . . . . . . . . . . . . . . 56 Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 57

3 Audio and control computations 59

1. The sampling theorem . . . . . . . . . . . . . . . . . . . . . . . . 59
1. Control . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 61
1. Control streams . . . . . . . . . . . . . . . . . . . . . . . . . . . . 63
1. Converting from audio signals to numeric control streams . . . . 67
1. Control streams in block diagrams . . . . . . . . . . . . . . . . . 68
1. Event detection . . . . . . . . . . . . . . . . . . . . . . . . . . . . 69
1. Audio signals as control . . . . . . . . . . . . . . . . . . . . . . . 71
1. Operations on control streams . . . . . . . . . . . . . . . . . . . . 74
1. Control operations in Pd . . . . . . . . . . . . . . . . . . . . . . . 77
1. Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 78 Sampling and foldover . . . . . . . . . . . . . . . . . . . . . . . . 78 Converting controls to signals . . . . . . . . . . . . . . . . . . . . 80 Non-looping wavetable player . . . . . . . . . . . . . . . . . . . . 81 Signals to controls . . . . . . . . . . . . . . . . . . . . . . . . . . 82 Analog-style sequencer . . . . . . . . . . . . . . . . . . . . . . . . 83 MIDI-style synthesizer . . . . . . . . . . . . . . . . . . . . . . . . 83 Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 86

4 Automation and voice management 89

1. Envelope Generators . . . . . . . . . . . . . . . . . . . . . . . . . 89
1. Linear and Curved Amplitude Shapes . . . . . . . . . . . . . . . 92
1. Continuous and discontinuous control changes . . . . . . . . . . . 94
1. Muting . . . . . . . . . . . . . . . . . . . . . . . . . . . . 95
1. Switch-and-ramp . . . . . . . . . . . . . . . . . . . . . . . 96
4. Polyphony . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 98
5. Voice allocation . . . . . . . . . . . . . . . . . . . . . . . . . . . . 98
5. Voice tags . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 99
5. Encapsulation in Pd . . . . . . . . . . . . . . . . . . . . . . . . . 102
5. Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 103 ADSR envelope generator . . . . . . . . . . . . . . . . . . . . . . 103 Transfer functions for amplitude control . . . . . . . . . . . . . . 106 Additive synthesis: Risset's bell . . . . . . . . . . . . . . . . . . . 107 Additive synthesis: spectral envelope control . . . . . . . . . . . 110 Polyphonic synthesis: sampler . . . . . . . . . . . . . . . . . . . . 111 Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 117

CONTENTS v

5 Modulation 119

1. Taxonomy of spectra . . . . . . . . . . . . . . . . . . . . . . . . . 119
1. Multiplying audio signals . . . . . . . . . . . . . . . . . . . . . . 122
1. Waveshaping . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 126
1. Frequency and phase modulation . . . . . . . . . . . . . . . . . . 132
1. Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 134 Ring modulation and spectra . . . . . . . . . . . . . . . . . . . . 134 Octave divider and formant adder . . . . . . . . . . . . . . . . . 135 Waveshaping and di®erence tones . . . . . . . . . . . . . . . . . . 138 Waveshaping using Chebychev polynomials . . . . . . . . . . . . 139 Waveshaping using an exponential function . . . . . . . . . . . . 140 Sinusoidal waveshaping: evenness and oddness . . . . . . . . . . 141 Phase modulation and FM . . . . . . . . . . . . . . . . . . . . . . 141 Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 146

6 Designer spectra 147

1. Carrier/modulator model . . . . . . . . . . . . . . . . . . . . . . 148
1. Pulse trains . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 151
1. Pulse trains via waveshaping . . . . . . . . . . . . . . . . 151
1. Pulse trains via wavetable stretching . . . . . . . . . . . . 152
1. Resulting spectra . . . . . . . . . . . . . . . . . . . . . . . 154
3. Movable ring modulation . . . . . . . . . . . . . . . . . . . . . . 156
4. Phase-aligned formant (PAF) generator . . . . . . . . . . . . . . 158
4. Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 163 Wavetable pulse train . . . . . . . . . . . . . . . . . . . . . . . . 163 Simple formant generator . . . . . . . . . . . . . . . . . . . . . . 164 Two-cosine carrier signal . . . . . . . . . . . . . . . . . . . . . . . 167 The PAF generator . . . . . . . . . . . . . . . . . . . . . . . . . . 169 Stretched wavetables . . . . . . . . . . . . . . . . . . . . . . . . . 172 Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 172

7 Time shifts and delays 175

1. Complex numbers . . . . . . . . . . . . . . . . . . . . . . . . . . 176

   7\.1.1 Complex sinusoids . . . . . . . . . . . . . . . . . . . . . . 178

2. Time shifts and phase changes . . . . . . . . . . . . . . . . . . . 179
3. Delay networks . . . . . . . . . . . . . . . . . . . . . . . . . . . . 180
3. Recirculating delay networks . . . . . . . . . . . . . . . . . . . . 184
3. Power conservation and complex delay networks . . . . . . . . . 189
3. Arti¯cial reverberation . . . . . . . . . . . . . . . . . . . . . . . . 193

   7\.6.1 Controlling reverberators . . . . . . . . . . . . . . . . . . 196

7. Variable and fractional shifts . . . . . . . . . . . . . . . . . . . . 196
8. Fidelity of interpolating delay lines . . . . . . . . . . . . . . . . . 201
8. Pitch shifting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 202
8. Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 208 Fixed, noninterpolating delay line . . . . . . . . . . . . . . . . . . 208 Recirculating comb ¯lter . . . . . . . . . . . . . . . . . . . . . . . 209

vi CONTENTS

Variable delay line . . . . . . . . . . . . . . . . . . . . . . . . . . 209

Order of execution and lower limits on delay times . . . . . . . . 211

Order of execution in non-recirculating delay lines . . . . . . . . 214

Non-recirculating comb ¯lter as octave doubler . . . . . . . . . . 215

Time-varying complex comb ¯lter: shakers . . . . . . . . . . . . . 216

Reverberator . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 218

Pitch shifter . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 218 Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 221

8 Filters 223

1. Taxonomy of ¯lters . . . . . . . . . . . . . . . . . . . . . . . . . . 224
1. Low-pass and high-pass ¯lters . . . . . . . . . . . . . . . . 224
1. Band-pass and stop-band ¯lters . . . . . . . . . . . . . . . 226
1. Equalizing ¯lters . . . . . . . . . . . . . . . . . . . . . . . 227
2. Elementary ¯lters . . . . . . . . . . . . . . . . . . . . . . . . . . . 229
1. Elementary non-recirculating ¯lter . . . . . . . . . . . . . 229
1. Non-recirculating ¯lter, second form . . . . . . . . . . . . 231
1. Elementary recirculating ¯lter . . . . . . . . . . . . . . . . 232
1. Compound ¯lters . . . . . . . . . . . . . . . . . . . . . . . 232
1. Real outputs from complex ¯lters . . . . . . . . . . . . . . 233
1. Two recirculating ¯lters for the price of one . . . . . . . . 234
3. Designing ¯lters . . . . . . . . . . . . . . . . . . . . . . . . . . . . 235
1. One-pole low-pass ¯lter . . . . . . . . . . . . . . . . . . . 236
1. One-pole, one-zero high-pass ¯lter . . . . . . . . . . . . . 237
1. Shelving ¯lter . . . . . . . . . . . . . . . . . . . . . . . . . 238
1. Band-pass ¯lter . . . . . . . . . . . . . . . . . . . . . . . . 239
1. Peaking and stop-band ¯lter . . . . . . . . . . . . . . . . 240
1. Butterworth ¯lters . . . . . . . . . . . . . . . . . . . . . . 240
1. Stretching the unit circle with rational functions . . . . . 243
1. Butterworth band-pass ¯lter . . . . . . . . . . . . . . . . 244
1. Time-varying coe±cients . . . . . . . . . . . . . . . . . . 245
1. Impulse responses of recirculating ¯lters . . . . . . . . . . 246
1. All-pass ¯lters . . . . . . . . . . . . . . . . . . . . . . . . 249
4. Applications . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 249
1. Subtractive synthesis . . . . . . . . . . . . . . . . . . . . . 250
1. Envelope following . . . . . . . . . . . . . . . . . . . . . . 252
1. Single Sideband Modulation . . . . . . . . . . . . . . . . . 254
5. Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 255 Prefabricated low-, high-, and band-pass ¯lters . . . . . . . . . . 256 Prefabricated time-varying band-pass ¯lter . . . . . . . . . . . . 256 Envelope followers . . . . . . . . . . . . . . . . . . . . . . . . . . 257 Single sideband modulation . . . . . . . . . . . . . . . . . . . . . 259 Using elementary ¯lters directly: shelving and peaking . . . . . . 259 Making and using all-pass ¯lters . . . . . . . . . . . . . . . . . . 261 Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 262

CONTENTS vii

9 Fourier analysis and resynthesis 263

1. Fourier analysis of periodic signals . . . . . . . . . . . . . . . . . 263
1. Periodicity of the Fourier transform . . . . . . . . . . . . 264
1. Fourier transform as additive synthesis . . . . . . . . . . . 265
2. Properties of Fourier transforms . . . . . . . . . . . . . . . . . . 265
1. Fourier transform of DC . . . . . . . . . . . . . . . . . . . 266
1. Shifts and phase changes . . . . . . . . . . . . . . . . . . 267
1. Fourier transform of a sinusoid . . . . . . . . . . . . . . . 269
3. Fourier analysis of non-periodic signals . . . . . . . . . . . . . . . 269
4. Fourier analysis and reconstruction of audio signals . . . . . . . . 274
1. Narrow-band companding . . . . . . . . . . . . . . . . . . 276
1. Timbre stamping (classical vocoder) . . . . . . . . . . . . 278
5. Phase . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 279

   9\.5.1 Phase relationships between channels . . . . . . . . . . . . 283

6. Phase bashing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 284
7. Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 286 Fourier analysis and resynthesis in Pd . . . . . . . . . . . . . . . 286 Narrow-band companding: noise suppression . . . . . . . . . . . 290 Timbre stamp (\vocoder") . . . . . . . . . . . . . . . . . . . . . . 291 Phase vocoder time bender . . . . . . . . . . . . . . . . . . . . . 292 Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 294

10 Classical waveforms 295

1. Symmetries and Fourier series . . . . . . . . . . . . . . . . . . . . 297

   10\.1.1 Sawtooth waves and symmetry . . . . . . . . . . . . . . . 298

2. Dissecting classical waveforms . . . . . . . . . . . . . . . . . . . . 300
3. Fourier series of the elementary waveforms . . . . . . . . . . . . . 302
1. Sawtooth wave . . . . . . . . . . . . . . . . . . . . . . . . 303
1. Parabolic wave . . . . . . . . . . . . . . . . . . . . . . . . 304
1. Square and symmetric triangle waves . . . . . . . . . . . . 304
1. General (non-symmetric) triangle wave . . . . . . . . . . . 305
4. Predicting and controlling foldover . . . . . . . . . . . . . . . . . 307
1. Over-sampling . . . . . . . . . . . . . . . . . . . . . . . . 307
1. Sneaky triangle waves . . . . . . . . . . . . . . . . . . . . 309
1. Transition splicing . . . . . . . . . . . . . . . . . . . . . . 309
5. Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 313 Combining sawtooth waves . . . . . . . . . . . . . . . . . . . . . 313 Strategies for band-limiting sawtooth waves . . . . . . . . . . . . 314 Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 316

Index 319 Bibliography 323

viii CONTENTS


Foreword

The Theory and Technique of Electronic Music is a uniquely complete source of information for the computer synthesis of rich and interesting musical timbres. The theory is clearly presented in a completely general form. But in addition, examples of how to synthesize each theoretical aspect are presented in the Pd language so the reader ofthe book can immediately use the theory for his musical purposes. I know of no other book which combines theory and technique so usefully.

By far the most popular music and sound synthesis programs in use today are block diagram compilers with graphical interfaces. These allow the composer to design instruments by displaying the \ob jects" of his instrument on a computer screen and drawing the connecting paths between the objects. The resulting graphical display is very congenial to musicians. A naive user can design a simple instrument instantly. He can rapidly learn to design complex instruments. He can understand how complex instruments work by looking at their graphical images.

The ¯rst graphical compiler program, Max, was written by Miller Puckette in 1988. Max dealt only with control signals for music synthesis because the computers available at the time were not fast enough to deal with sound. As soon as faster computers which could compute soundwave samples in real-time were available, Puckette and David Zicarelli appended MSP to Max (Max/MSP) thus making the computer, usually a laptop computer, into a complete musical instrument capable of live performance.

Development of Max/MSP was done by Puckette and Zicarelli at IRCAM in the period 1993 to 1994 . Both have now moved to California. Zicarelli com- mercialized and sells Max, MSP, and JITTER (an extension to video synthesis) as products. Puckette, now a professor at UCSD, wrote Pd (Pure Data). It is an open source program which is a close equivalent to Max/MSP.

Max and Pd allow almost anyone to synthesize uninteresting timbres almost instantly. Making interesting timbres is much more di±cult and requires much additional knowledge. The Theory and Technique of Electronic Music is that body of knowledge. The theory is important for any synthesis program. The Theory and Technique of Electronic Music gives copious examples of how to apply the theory using Pd. The combination of theory plus Pd examples makes this book uniquely useful. It also contains problem sets for each chapter so it is a ¯ne textbook.

ix
x CONTENTS

I expect Puckette's book to become THE essential book in any electronic musician's library.

Max Mathews



Preface

This is a book about using electronic techniques to record, synthesize, process, and analyze musical sounds, a practice which came into its modern form in the years 1948-1952, but whose technological means and artistic uses have under- gone several revolutions since then. Nowadays most electronic music is made using computers, and this book will focus exclusively on what used to be called \computer music", but which should really now be called \electronic music using a computer".

Most of the computer music tools available today have antecedents in earlier generations of equipment. The computer, however, is relatively cheap and the results of using one are easy to document and re-create. In these respects at least, the computer makes the ideal electronic music instrument|it is hard to see what future technology could displace it.

The techniques and practices of electronic music can be studied (at least in theory) without making explicit reference to the current state of technology. Still, it's important to provide working examples. So each chapter starts with theory (avoiding any reference to implementation) and ends with a series of examples realized in a currently available software package.

The ideal reader of this book is anyone who knows and likes electronic music of any genre, has plenty of facility with computers in general, and who wants to learn how to make electronic music from the ground up, starting with the humble oscillator and continuing through sampling, FM, ¯ltering, waveshaping, delays, and so on. This will take plenty of time.

This book doesn't take the easy route of recommending pre-cooked software to try out these techniques; instead, the emphasis is on learning how to use a general-purpose computer music environment to realize them yourself. Of the several such packages available, we'll use Pd, but that shouldn't stop you from using these same techniques in other environments such as Csound or Max/MSP.

To read this book you must understand mathematics through intermediate algebra and trigonometry; starting in Chapter 7, complex numbers also make an appearance, although not complex analyis. (For instance, complex numbers are added, multiplied, and conjugated, but there are no complex exponentials.) A review of mathematics for computer music by F. Richard Moore appears in [Str85, pp. 1-68].

Although the \level" of mathematics is not high, the mathematics itself is sometimes quite challenging. All sorts of cool mathematics is in the reach

xi
xii CONTENTS

of any student of algebra or geometry. In the service of computer music, for instance, we'll run into Bessel functions, Chebychev polynomials, the Central Limit Theorem, and, of course, Fourier analysis.

You don't need much background in music as it is taught in the West; in particular, Western written music notation is not needed. Some elementary bits of Western music theory are used, such as the tempered scale, the A-B- C system of naming pitches, and terms like \note" and \chord". Also you should be familiar with terms of musical acoustics such as sinusoids, amplitude, frequency, and the overtone series.

Each chapter starts with a theoretical discussion of some family of techniques or theoretical issues, followed by a series of examples realized in Pd to illustrate them. The examples are included in the Pd distribution, so you can run them and/or edit them into your own spino®s. In addition, all the ¯gures were created using Pd patches, which appear in an electronic supplement. These aren't care- fully documented but in principle could be used as an example of Pd's drawing capabilities for anyone interested in that.

I would like to thank some people who have made it possible for me to write this. Barry Vercoe is almost entirely responsible for my music education. Mean- while I was taught mathematics by Wayne Holman, Samuel Greitzer, Murray Klamkin, Gian-Carlo Rota, Frank Morgan, Michael Artin, Andrew Gleason, and many others. Phil White taught me English and Rosie Paschall visual com- position. Finally, my parents (one deceased) are mighty patient; I'm now 47. Thank you.



Chapter 1

Sinusoids, amplitude and frequency

Electronic music is usually made using a computer, by synthesizing or processing digital audio signals. These are sequences of numbers,

:::;x[n ¡ 1];x[n];x[n + 1];:::

where the index n, called the sample number, may range over some or all the integers. A single number in the sequence is called a sample. An example of a digital audio signal is the Sinusoid :

x[n] = a cos(!n + Á)

where a is the amplitude, ! is the angular frequency, and Áis the initial phase. The phase is a function of the sample number n, equal to !n + Á. The initial phase is the phase at the zeroth sample (n = 0).

Figure 1.1 (part a) shows a sinusoid graphically. The horizontal axis shows successive values of n and the vertical axis shows the corresponding values of x[n]. The graph is drawn in such a way as to emphasize the sampled nature of the signal. Alternatively, we could draw it more simply as a continuous curve (part b). The upper drawing is the most faithful representation of the (digital audio) sinusoid, whereas the lower one can be considered an idealization of it.

Sinusoids play a key role in audio processing because, if you shift one of them left or right by any number of samples, you get another one. This makes it easy to calculate the e®ect of all sorts of operations on sinusoids. Our ears use this same special property to help us parse incoming sounds, which is why sinusoids, and combinations of sinusoids, can be used to achieve many musical e®ects.

Digital audio signals do not have any intrinsic relationship with time, but to listen to them we must choose a sample rate, usually given the variable name R, which is the number of samples that ¯t into a second. The time t is related to

1
2 CHAPTER 1. SINUSOIDS, AMPLITUDE AND FREQUENCY

x[n] (a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.001.png)

1  

49  n  -1 0  

x(n)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.002.png)

(b)

1  

50 -1 

Figure 1.1: A digital audio signal, showing its discrete-time nature (part a), and idealized as a continuous function (part b). This signal is a (real-valued) sinusoid, ¯fty points long, with amplitude 1, angular frequency 0.24, and initial phase zero.



1. MEASURES OF AMPLITUDE 3

the sample number n by Rt = n, or t = n=R. A sinusoidal signal with angular frequency ! has a real-time frequency equal to

!R f =

2¼

in Hertz (i.e., cycles per second), because a cycle is 2¼radians and a second is R samples.

A real-world audio signal's amplitude might be expressed as a time-varying voltage or air pressure, but the samples of a digital audio signal are unitless numbers. We'll casually assume here that there is ample numerical accuracy so that we can ignore round-o® errors, and that the numerical format is unlimited in range, so that samples may take any value we wish. However, most digital audio hardware works only over a ¯xed range of input and output values, most often between -1 and 1. Modern digital audio processing software usually uses a °oating-point representation for signals. This allows us to use whatever units are most convenient for any given task, as long as the ¯nal audio output is within the hardware's range [Mat69, pp. 4-10].

1. Measures of Amplitude

The most fundamental property of a digital audio signal is its amplitude. Unfor- tunately, a signal's amplitude has no one canonical de¯nition. Strictly speaking, all the samples in a digital audio signal are themselves amplitudes, and we also spoke of the amplitude a of the sinusoid as a whole. It is useful to have measures of amplitude for digital audio signals in general. Amplitude is best thought of as applying to a window, a ¯xed range of samples of the signal. For instance, the window starting at sample M of length N of an audio signal x[n] consists of the samples,

x[M];x[M + 1];:::;x[M + N ¡ 1]

The two most frequently used measures of amplitude are the peak amplitude, which is simply the greatest sample (in absolute value) over the window:

Apeak fx[n]g = max jx[n]j; n = M;:::;M + N ¡ 1 and the root mean square (RMS) amplitude:

p ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.003.png)

ARMS fx[n]g = P fx[n]g

where P fx[n]g is the mean power, de¯ned as:

- ´

P fx[n]g = 1 jx[M]j2 + ¢¢¢+ jx[M + N ¡ 1]j2

N

(In this last formula, the absolute value signs aren't necessary at the moment since we're working on real-valued signals, but they will become important later

1) peak RMS![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.004.png)
1) peak RMS![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.005.png)

Figure 1.2: Root mean square (RMS) and peak amplitudes of signals compared. Fpor a sinusoid (part a), the peak amplitude is higher than RMS by a factor of![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.006.png)

2\.

when we consider complex-valued signals.) Neither the peak nor the RMS am- plitude of any signal can be negative, and either one can be exactly zero only if the signal itself is zero for all n in the window.

The RMS amplitude of a signal mapy equal the peak amplitude but never exceeds it; and it may be as little as 1= N times the peak amplitude, but never less than that.

Under reasonable conditions|if the window contains at least several periods and if the angular frequency is well under one radian per sample|the peak amplitudepof the sinusoid of Page 1 is approximately a and its RMS amplitude ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.007.png)about a= 2. Figure 1.2 shows the peak and RMS amplitudes of two digital audio signals.

2. Units of Amplitude

Two amplitudes are often better compared using their ratio than their di®erence. Saying that one signal's amplitude is greater than another's by a factor of two might be more informative than saying it is greater by 30 millivolts. This is true for any measure of amplitude (RMS or peak, for instance). To facilitate comparisons, we often express amplitudes in logarithmic units called decibels. If a is the amplitude of a signal (either peak or RMS), then we can de¯ne the

2. UNITS OF AMPLITUDE 5 1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.008.png)

   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.009.png)

ampli-

tude

0\.1

0  

-20 -10 0  

decibels![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.010.png)

Figure 1.3: The relationship between decibel and linear scales of amplitude. The linear amplitude 1 is assigned to 0 dB.

decibel (dB) level d as:

d = 20 ¢log10 (a=a0)

where a0 is a reference amplitude. This de¯nition is set up so that, if we increase thepsignal power by a factor of ten (so that the amplitude increases by a factor of![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.011.png) 10), the logarithm will increase by 1=2, and so the value in decibels goes

up (additively) by ten. An increase in amplitude by a factor of two corresponds to an increase of about 6.02 decibels; doubling power is an increase of 3.01 dB. The relationship between linear amplitude and amplitude in decibels is graphed in Figure 1.3.

Still using a0 to denote the reference amplitude, a signal with linear ampli- tude smaller than a0 will have a negative amplitude in decibels: a0=10 gives -20 dB, a0=100 gives -40, and so on. A linear amplitude of zero is smaller than that of any value in dB, so we give it a dB level of ¡1.

In digital audio a convenient choice of reference, assuming the hardware has a maximum amplitude of one, is

a0 = 10¡5 = 0:00001

so that the maximum amplitude possible is 100 dB, and 0 dB is likely to be inaudibly quiet at any reasonable listening level. Conveniently enough, the dynamic range of human hearing|the ratio between a damagingly loud sound and an inaudibly quiet one|is about 100 dB.

Amplitude is related in an inexact way to the perceived loudness of a sound. In general, two signals with the same peak or RMS amplitude won't necessarily have the same loudness at all. But amplifying a signal by 3 dB, say, will fairly

440 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.012.png)330 220 

110![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.013.png)

0  

45  57  69 frequency pitch

Figure 1.4: The relationship between \MIDI" pitch and frequency in cycles per second (Hertz). The span of 24 MIDI values on the horizontal axis represents two octaves, over which the frequency increases by a factor of four.

reliably make it sound about one \step" louder. Much has been made of the supposedly logarithmic nature of human hearing (and other senses), which may partially explain why decibels are such a useful scale of amplitude [RMW02, p. 99].

Amplitude is also related in an inexact way to musical dynamic. Dynamic is better thought of as a measure of e®ort than of loudness or power. It ranges over nine values: rest, ppp, pp, p, mp, mf, f, ®,®f. These correlate in an even looser way with the amplitude of a signal than does loudness [RMW02, pp. 110-111].

3. Controlling Amplitude

Perhaps the most frequently used operation on electronic sounds is to change their amplitudes. For example, a simple strategy for synthesizing sounds is by combining sinusoids, which can be generated by evaluating the formula on Page 1, sample by sample. But the sinusoid has a constant nominal amplitude a, and we would like to be able to vary that in time.

In general, to multiply the amplitude of a signal x[n] by a factor y ¸ 0, you can just multiply each sample by y, giving a new signal y ¢x[n]. Any measurement of the RMS or peak amplitude of x[n] will be greater or less by the factor y. More generally, you can change the amplitude by an amount y[n] which varies sample by sample. If y[n] is nonnegative and if it varies slowly enough, the amplitude of the product y[n]¢x[n] (in a ¯xed window from M to M + N ¡ 1) will be that of x[n], multiplied by the value of y[n] in the window

4. FREQUENCY 7

(which we assume doesn't change much over the N samples in the window).

In the more general case where both x[n]and y[n]are allowed to take negative and positive values and/or to change quickly, the e®ectofmultiplying them can't be described as simply changing the amplitude of one of them; this is considered later in Chapter 5.

4. Frequency

Frequencies, like amplitudes, are often measured on a logarithmic scale, in order to emphasize proportions between them, which usually provide a better descrip- tion of the relationship between frequencies than do di®erences between them. The frequency ratio between two musical tones determines the musical interval between them.

The Western musical scale divides the octave (the musical interval associated with a ratio of 2:1) into twelve equal sub-intervals, each of which therefore corresponds to a ratio of 21=12 . For historical reasons this sub-interval is called a half-step. A convenient logarithmic scale for pitch is simply to count the number of half-steps from a reference pitch|allowing fractions to permit us to specify pitches which don't fall on a note of the Western scale. The most commonly used logarithmic pitch scale is \MIDI pitch", in which the pitch 69 is assigned to a frequency of 440 cycles per second|the A above middle C. To convert between a MIDI pitch m and a frequency in cycles per second f , apply the Pitch/Frequency Conversion formulas:

m = 69 + 12 ¢log2(f =440)

f = 440 ¢2(m¡69)=12

Middle C, corresponding to MIDI pitch m = 60, comes to f = 261:626 cycles per second.

MIDI itself is an old hardware protocol which has unfortunately insinuated itself into a great deal of software design. In hardware, MIDI allows only integer pitches between 0 and 127. However, the underlying scale is well de¯ned for any \MIDI" number, even negative ones; for example a \MIDI pitch" of -4 is a decent rate of vibrato. The pitch scale cannot, however, describe frequencies less than or equal to zero cycles per second. (For a clear description of MIDI, its capabilities and limitations, see [Bal03, ch.6-8]).

A half-step comes to a ratio of about 1.059 to 1, or about a six percent increase in frequency. Half-steps are further divided into cents, each cent being one hundredth of a half-step. As a rule of thumb, it might take about three cents to make a discernible change in the pitch of a musical tone. At middle C this comes to a di®erence of about 1/2 cycle per second. A graph of frequency as a function of MIDI pitch, over a two-octave range, is shown in Figure 1.4.

FREQUENCY FREQUENCY

OUT y[n]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.014.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.015.png)

OUT

1) (b)

Figure 1.5: Block diagrams for (a) a sinusoidal oscillator; (b) controlling the amplitude using a multiplier and an amplitude signal y[n].

5. Synthesizing a sinusoid

In most widely used audio synthesis and processing packages (Csound, Max/MSP, and Pd, for instance), the audio operations are speci¯ed as networks of unit generators [Mat69] which pass audio signals among themselves. The user of the software package speci¯es the network, sometimes called a patch, which essen- tially corresponds to the synthesis algorithm to be used, and then worries about how to control the various unit generators in time. In this section, we'll use ab- stract block diagrams to describe patches, but in the \examples" section (Page 17), we'll choose a speci¯c implementation environment and show some of the software-dependent details.

To show how to produce a sinusoid with time-varying amplitude we'll need to introduce two unit generators. First we need a pure sinusoid which is made with an oscillator. Figure 1.5 (part a) shows a pictorial representation of a sinusoidal oscillator as an icon. The input is a frequency (in cycles per second), and the output is a sinusoid of peak amplitude one.

Figure 1.5 (part b) shows how to multiply the output ofa sinusoidal oscillator by an appropriate scale factor y[n]to control its amplitude. Since the oscillator's peak amplitude is 1, the peak amplitude of the product is about y[n], assuming y[n] changes slowly enough and doesn't become negative in value.

Figure 1.6 shows how the sinusoid of Figure 1.1 is a®ected by amplitude change by two di®erent controlling signals y[n]. The controlling signal shown in part (a) has a discontinuity, and so therefore does the resulting amplitude- controlled sinusoid shown in (b). Parts (c) and (d) show a more gently-varying possibility for y[n]and the result. Intuition suggests that the result shown in (b)

5. SYNTHESIZING A SINUSOID 9

1   y[n]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.016.png)

(a)

n  0   50 

-1 

1   x[n]y[n]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.017.png)

(b)

-1 

1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.018.png)

y[n]

(c)

-1 

1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.019.png)

x[n]y[n]

(d)

-1 

Figure 1.6: Two amplitude functions (parts a, c), and (parts b, d), the result of multiplying them by the pure sinusoid of Figure 1.1.

won't sound like an amplitude-varying sinusoid, but instead like a sinusoid in- terrupted by an audible \pop" after which it continues more quietly. In general, for reasons that can't be explained in this chapter, amplitude control signals y[n] which ramp smoothly from one value to another are less likely to give rise to parasitic results (such as that \pop") than are abruptly changing ones.

For now we can state two general rules without justifying them. First, pure sinusoids are the signals most sensitive to the parasitic e®ectsof quick amplitude change. So when you want to test an amplitude transition, if it works for sinusoids it will probably work for other signals as well. Second, depending on the signal whose amplitude you are changing, the amplitude control will need between 0 and 30 milliseconds of \ramp" time|zero for the most forgiving signals (such as white noise), and 30 for the least (such as a sinusoid). All this also depends in a complicated way on listening levels and the acoustic context.

Suitable amplitude control functions y[n] may be made using an envelope generator. Figure 1.7 shows a network in which an envelope generator is used to control the amplitude of an oscillator. Envelope generators vary widely in design, but we will focus on the simplest kind, which generates line segments as shown in Figure 1.6 (part c). If a line segment is speci¯ed to ramp between two output values a and b over N samples starting at sample number M, the output is:

n ¡ M

y[n] = a + (b¡ a)~~ ; M · n · M + N ¡ 1:

N

The output may have any number of segments such as this, laid end to end, over the entire range of sample numbers n; °at, horizontal segments can be made by setting a = b.

In addition to changing amplitudes of sounds, amplitude control is often used, especially in real-time applications, simply to turn sounds on and o®: to turn one o®, ramp the amplitude smoothly to zero. Most software synthesis packages also provide ways to actually stop modules from computing samples at all, but here we'll use amplitude control instead.

The envelope generator dates from the analog era [Str95, p.64] [Cha80, p.90], as does the rest of Figure 1.7; oscillators with controllable frequency were called voltage-controlled oscillators or VCOs, and the multiplication step was done using a voltage-controlled ampli¯er or VCA [Str95, pp.34-35] [Cha80, pp.84-89]. Envelope generators are described in more detail in Section 4.1.

6. Superposing Signals

If a signal x[n] has a peak or RMS amplitude A (in some ¯xed window), then the scaled signal k ¢x[n] (where k ¸ 0) has amplitude kA. The mean power of the scaled signal changes by a factor of k2. The situation gets more complicated when two di®erent signals are added together; just knowing the amplitudes of the two does not su±ce to know the amplitude of the sum. The two amplitude measures do at least obey triangle inequalities; for any two signals x[n] and y[n],

Apeak fx[n]g + Apeak fy[n]g ¸ Apeak fx[n]+ y[n]g

6. SUPERPOSING SIGNALS 11 FREQUENCY

OUT![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.020.png)

Figure 1.7: Using an envelope generator to control amplitude. ARMS fx[n]g + ARMS fy[n]g ¸ ARMS fx[n]+ y[n]g

If we ¯x a window from M to N + M ¡ 1 as usual, we can write out the mean power of the sum of two signals:

P fx[n]+ y[n]g = P fx[n]g + P fy[n]g + 2 ¢COVfx[n];y[n]g

where we have introduced the covariance of two signals:

x[M]y[M]+ ¢¢¢+ x[M + N ¡ 1]y[M + N ¡ 1] COVfx[n];y[n]g =

N

The covariance may be positive, zero, or negative. Over a su±ciently large window, the covariance of two sinusoids with di®erent frequencies is negligible compared to the mean power. Two signals which have no covariance are called uncorrelated (the correlation is the covariance normalized to lie between -1 and 1). In general, for two uncorrelated signals, the power of the sum is the sum of the powers:

P fx[n]+ y[n]g = P fx[n]g + P fy[n]g; whenever COVfx[n];y[n]g = 0 Put in terms of amplitude, this becomes:

(ARMS fx[n]+ y[n]g)2 = (ARMS fx[n]g)2 + (ARMS fy[n]g)2:

This is the familiar Pythagorean relation. So uncorrelated signals can be thought of as vectors at right angles to each other; positively correlated ones as having an acute angle between them, and negatively correlated as having an obtuse angle between them.

For example, if two uncorrelatedp signals both have RMS amplitude a, the sum![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.021.png) will have RMS amplitude 2a. On the other hand if the two signals happen to be equal|the most correlated possible|the sum will have amplitude 2a, which is the maximum allowed by the triangle inequality.

7. Periodic Signals

A signal x[n] is said to repeat at a period ¿ if

x[n + ¿] = x[n]

for all n. Such a signal would also repeat at periods 2¿ and so on; the smallest ¿ if any at which a signal repeats is called the signal's period. In discussing periods of digital audio signals, we quickly run into the di±culty of describing signals whose \period" isn't an integer, so that the equation above doesn't make sense. For now we'll e®ectively ignore this di±culty by supposing that the signal x[n] may somehow be interpolated between the samples so that it's well de¯ned whether n is an integer or not.

A sinusoid has a period (in samples) of 2¼=! where ! is the angular fre- quency. More generally, any sum of sinusoids with frequencies 2¼k=!, for inte- gers k, will repeat after 2¼=! samples. Such a sum is called a Fourier Series :

x[n] = a0 + a1 cos(!n + Á1) + a2 cos(2!n + Á2) + ¢¢¢+ ap cos(p!n + Áp)

Moreover, if we make certain technical assumptions (in e®ect that signals only contain frequencies up to a ¯nite bound), we can represent any periodic signal as such a sum. This is the discrete-time variant of Fourier analysis which will reappear in Chapter 9.

The angular frequencies of the sinusoids above are all integer multiples of !. They are called the harmonics of !, which in turn is called the fundamental. In terms of pitch, the harmonics !;2!;::: are at intervals of 0, 1200, 1902, 2400, 2786, 3102, 3369, 3600, ..., cents above the fundamental; this sequence of pitches is sometimes called the harmonic series. The ¯rst six of these are all quite close to multiples of 100; in other words, the ¯rst six harmonics of a pitch in the Western scale land close to (but not always exactly on) other pitches of the same scale; the third and sixth miss only by 2 cents and the ¯fth misses by 14.

Put another way, the frequency ratio 3:2 (a perfect ¯fth in Western termi- nology) is almost exactly seven half-steps, 4:3 (a perfect fourth) is just as near to ¯ve half-steps, and the ratios 5:4 and 6:5 (perfect major and minor thirds) are fairly close to intervals of four and three half-steps, respectively.

A Fourier series (with only three terms) is shown in Figure 1.8. The ¯rst three graphs are ofsinusoids, whose frequencies are in a 1:2:3 ratio. The common period is marked on the horizontal axis. Each sinusoid has a di®erent amplitude and initial phase. The sum of the three, at bottom, is not a sinusoid, but it still maintains the periodicity shared by the three component sinusoids.

Leaving questions of phase aside, we can use a bank of sinusoidal oscillators to synthesize periodic tones, or even to morph smoothly through a succession of periodic tones, by specifying the fundamental frequency and the (possibly time-varying) amplitudes of the partials. Figure 1.9 shows a block diagram for doing this.

7. PERIODIC SIGNALS 13

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.022.png)

+ ` `![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.023.png)
+ ` `![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.024.png)
- ` `![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.025.png)

Figure 1.8: A Fourier series, showing three sinusoids and their sum. The three component sinusoids have frequencies in the ratio 1:2:3.

FREQUENCY

(more)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.026.png)

3  

2  

OUT

Figure 1.9: Using many oscillators to synthesize a waveform with desired har- monic amplitudes.

8. ABOUT THE SOFTWARE EXAMPLES 15

This is an example of additive synthesis ; more generally the term can be applied to networks in which the frequencies of the oscillators are independently controllable. The early days of computer music rang with the sound of additive synthesis.

8. About the Software Examples

The examples for this book use Pure Data (Pd), and to understand them you will have to learn at least something about Pd itself. Pd is an environment for quickly realizing computer music applications, primarily intended for live music performances. Pd can be used for other media as well, but we won't go into that here.

Several other patchable audio DSP environments exist besides Pd. The most widely used one is certainly Barry Vercoe's Csound [Bou00], which di®ers from Pd in being text-based (not GUI-based). This is an advantage in some respects and a disadvantage in others. Csound is better adapted than Pd for batch processing and it handles polyphony much better than Pd does. On the other hand, Pd has a better developed real-time control structure than Csound. Genealogically, Csound belongs to the so-called Music N languages [Mat69, pp.115-172].

Another open-source alternative in wide use is James McCartney's SuperCol- lider, which is also more text oriented than Pd, but like Pd is explicitly designed for real-time use. SuperCollider has powerful linguistic constructs which make

it a more suitable tool than Csound for tasks like writing loops or maintaining complex data structures.

Finally, Pd has a widely-used sibling, Cycling74's commercial program Max/MSP (the others named here are all open source). Both beginners and system man- agers running multi-user, multi-purpose computer labs will ¯nd Max/MSP bet-

ter supported and documented than Pd. It's possible to take knowledge of Pd

and apply it in Max/MSP and vice versa, and even to port patches from one to the other, but the two aren't truly compatible.

Quick Introduction to Pd

Pd documents are called patches. They correspond roughly to the boxes in the abstract block diagrams shown earlier in this chapter, but in detail they are quite di®erent, because Pd is an implementation environment, not a speci¯cation language.

A Pd patch, such as the ones shown in Figure 1.10, consists of a collection of boxes connected in a network. The border of a box tells you how its text is interpreted and how the box functions. In part (a) of the ¯gure we see three types of boxes. From top to bottom they are:

- a message box. Message boxes, with a °ag-shaped border, interpret the text as a message to send whenever the box is activated (by an incoming

9. EXAMPLES 16

21  message box![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.027.png)

+ 13 object box

34  number

(GUI) box

(a)

440 frequency

osc~ sinusoidal oscillator![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.028.png)

amplitude

0\.1 0   (on/off)

\*~  multiplier

dac~ output

(b)

9. EXAMPLES 19

Figure 1.10: (a) three types of boxes in Pd (message, object, and GUI); (b) a simple patch to output a sinusoid.

message or with a pointing device). The message in this case consists simply of the number \21".

- an object box. Object boxes have a rectangular border; they interpret the text to create objects when you load a patch. Object boxes may hold hundreds of di®erent classes of objects|including oscillators, envelope generators, and other signal processing modules to be introduced later| depending on the text inside. In this example, the box holds an adder. In most Pd patches, the majority of boxes are of type \ob ject". The ¯rst word typed into an object box speci¯es its class, which in this case is just \+". Any additional (blank-space-separated) words appearing in the box are called creation arguments, which specify the initial state of the object when it is created.
- a number box. Number boxes are a particular type of GUI box. Others include push buttons and toggle switches; these will come up later in the examples. The number box has a punched-card-shaped border, with a nick out of its top right corner. Whereas the appearance of an object or message box is ¯xed when a patch is running, a number box's contents (the text) changes to re°ect the current value held by the box. You can also use a number box as a control by clicking and dragging up and down, or by typing values in it.

In Figure 1.10 (part a) the message box, when clicked, sends the message \21" to an object box which adds 13 to it. The lines connecting the boxes carry data from one box to the next; outputs of boxes are on the bottom and inputs on top.

Figure 1.10 (part b) shows a Pd patch which makes a sinusoid with con- trollable frequency and amplitude. The connecting patch lines are of two types

here; the thin ones are for carrying sporadic messages, and the thicker ones (connecting the oscillator, the multiplier, and the output dac~ object) carry digital audio signals. Since Pd is a real-time program, the audio signals °ow in a continuous stream. On the other hand, the sporadic messages appear at speci¯c but possibly unpredictable instants in time.

Whether a connection carries messages or signals depends on the box the connection comes from; so, for instance, the + object outputs messages, but the \*~ object outputs a signal. The inputs of a given object may or may not accept signals (but they always accept messages, even if only to convert them to signals). As a convention, object boxes with signal inputs or outputs are all named with a trailing tilde (\~") as in \\*~" and \osc~".

How to ¯nd and run the examples

To run the patches, you must ¯rst download, install, and run Pd. Instructions for doing this appear in Pd's on-line HTML documentation, which you can ¯nd at http://crca.ucsd.edu/~msp/software.htm.

This book should appear at http:/crca/ucsd/edu/~msp/techniques.htm, pos- sibly in several revisions. Choose the revision that corresponds to the text you're reading (or perhaps just the latest one) and download the archive containing the associated revision of the examples (you may also download an archive of the HTML version of this book for easier access on your machine). The examples should all stay in a single directory, since some of them depend on other ¯les in that directory and might not load them correctly if you have moved things around.

If you do want to copy one of the examples to another directory so that you can build on it (which you're welcome to do), you should either include the examples directory in Pd's search path (see the Pd documentation) or else ¯gure out what other ¯les are needed and copy them too. A good way to ¯nd this out is just to run Pd on the relocated ¯le and see what Pd complains it can't ¯nd.

There should be dozens of ¯les in the \examples" folder, including the ex- amples themselves and the support ¯les. The ¯lenames of the examples all begin with a letter (A for chapter 1, B for 2, etc.) and a number, as in \A01.sinewave.pd".

The example patches are also distributed with Pd, but beware that you may ¯nd a di®erent version of the examples which might not correspond to the text you're reading.

9. Examples

Constant amplitude scaler

Example A01.sinewave.pd, shown in Figure 1.11, contains essentially the sim- plest possible patch that makes a sound, with only three object boxes. (There

are also comments, and two message boxes to turn Pd's \DSP" (audio) process- ing on and o®.) The three object boxes are:

osc » : sinusoidal oscillator. The left hand side input and the output are dig- ital![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.029.png) audio signals. The input is taken to be a (possibly time-varying) frequency in Hertz. The output is a sinusoid at the speci¯ed frequency. If nothing is connected to the frequency inlet, the creation argument (440 in this example) is used as the frequency. The output has peak amplitude one. You may set an initial phase by sending messages (not audio signals) to the right inlet. The left (frequency) inlet may also be sent messages to set the frequency, since any inlet that takes an audio signal may also be sent messages which are automatically converted to the desired audio signal.

- » : multiplier. This exists in two forms. If a creation argument is speci¯ed![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.030.png)

(as in this example; it's 0.05), this box multiplies a digital audio signal (in the left inlet) by the number; messages to the right inlet can update the number as well. If no argument is given, this box multiplies two incoming digital audio signals together.

dac » : audio output device. Depending on your hardware, this might not actually![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.031.png) be a Digital/Analog Converter as the name suggests; but in general, it allows you to send any audio signal to your computer's audio output(s). If there are no creation arguments, the default behavior is to output to channels one and two of the audio hardware; you may specify alternative channel numbers (one or many) using the creation arguments. Pd itself may be con¯gured to use two or more output channels, or may not have the audio output device open at all; consult the Pd documentation for details.

The two message boxes show a peculiarity in the way messages are parsed in message boxes. Earlier in Figure 1.10 (part a), the message consisted only of the number 21. When clicked, that box sent the message \21" to its outlet and hence to any objects connected to it. In this current example, the text of the message boxes starts with a semicolon. This is a terminator between messages (so the ¯rst message is empty), after which the next word is taken as the name of the recipient of the following message. Thus the message here is \dsp 1" (or \dsp 0") and the message is to be sent, not to any connected objects|there aren't any anyway|but rather, to the object named \pd". This particular object is provided invisibly by the Pd program and you can send it various messages to control Pd's global state, in this case turning audio processing on (\1") and o® (\0").

Many more details about the control aspects of Pd, such as the above, are explained in a di®erent series of example patches (the \control examples") in the Pd release, but they will only be touched on here as necessary to demonstrate the audio signal processing techniques that are the subject of this book.

Amplitude control in decibels

Example A02.amplitude.pd shows how to make a crude amplitude control; the active elements are shown in Figure 1.12 (part a). There is one new object class:

MAKING A SINE WAVE

Audio computation in Pd is done using "tilde objects" such as the three below. They use continuous audio streams to intercommunicate, and also communicate with other ("control") Pd objects using messages.

osc~ 440 440 Hz. sine wave at full blast \*~ 0.05![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.032.png) reduce amplitude to 0.05

dac~ send to the audio output device

Audio computation can be turned on and off by sending messages to the global "pd" object as follows:

- ;![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.033.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.034.png)

pd dsp 1 pd dsp 0 <-- click these

ON  OFF

You should see the Pd ("main") window change to reflect whether audio is on or off. You can also turn audio on and off using the "audio" menu, but the buttons are provided as a shortcut.

When DSP is on, you should hear a tone whose pitch is A 440 and whose amplitude is 0.05. If instead you are greeted with silence, you might want to read the HTML documentation on setting up audio.

In general when you start a work session with Pd, you will want to choose "test audio and MIDI" from the help window, which opens a more comprehensive test patch than this one.

Figure 1.11: The contents of the ¯rst Pd example patch: A01.sinewave.pd.

9. EXAMPLES 20

osc~ 440![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.035.png)

0  dbtorms

0  

\*~ 0 dac~

(a)

osc~ 440

0\.1 2000 <-- slow on![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.036.png)

0\.1 50 <-- fast on

0\.1 <-- instant on

0 2000 <-- slow off 0 50 <-- fast off

0   <-- instant off line~ <--- ramp generator

\*~  <-- multiplier: this time

taking a signal in dac~ on both sides.

(b)

osc~ 440

osc~ 550![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.037.png)

+~ 

osc~ 660 +~ 

output~

dB 0

mute

(c)

9. EXAMPLES 25

Figure 1.12: The active ingredients to three patches: (a) A02.amplitude.pd; (b) A03.line.pd; (c) A05.output.subpatch.pd.

dbtorms : Decibels to linear amplitude conversion. The \RMS" is a misnomer; it![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.038.png) should have been named \dbtoamp", since it really converts from decibels to any linear amplitude unit, be it RMS, peak, or other. An input of 100 dB is normalized to an output of 1. Values greater than 100 are ¯ne (120 will give 10), but values less than or equal to zero will output zero (a zero input would otherwise have output a small positive number). This is a control object, i.e., the numbers going in and out are messages, not signals. (A corresponding

object, dbtorms » , is the signal correlate. However, as a signal object this is ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.039.png)expensive in CPU time and most often we'll ¯nd one way or another to avoid using it.)

The two number boxes are connected to the input and output of the dbtorms object. The input functions as a control; \mouse" on it (click and drag upward or downward) to change the amplitude. It has been set to range from 0 to 80; this is protection for your speakers and ears, and it's wise to build such guardrails into your own patches.

The other number box shows the output of the dbtorms object. It is useless to mouse on this number box, since its outlet is connected nowhere; it is here purely to display its input. Number boxes may be useful as controls, displays, or both, although if you're using it as both there may be some extra work to do.

Smoothed amplitude control with an envelope generator

As Figure 1.6 shows, one way to make smooth amplitude changes in a signal without clicks is to multiply it by the output of an envelope generator as shown in block diagram form in Figure 1.7. This may be implemented in Pd using the line~ object:

line » : envelope generator. The output is a signal which ramps linearly from one![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.040.png) value to another over time, as determined by the messages received. The inlets take messages to specify target values (left inlet) and time delays (right inlet). Because of a general rule of Pd messages, a pair of numbers sent to the left inlet su±ces to specify a target value and a time together. The time is in milliseconds (taking into account the sample rate), and the target value is unitless, or in other words, its output range should conform to whatever input it may be connected to.

Example A03.line.pd demonstrates the use of a line~ object to control the amplitude of a sinusoid. The active part is shown in Figure 1.12 (part b). The six message boxes are all connected to the line~ object, and are activated by clicking on them; the top one, for instance, speci¯es that the line~ ramp (starting at wherever its output was before receiving the message) to the value 0.1 over two seconds. After the two seconds elapse, unless other messages have arrived in the meantime, the output remains steady at 0.1. Messages may arrive before the two seconds elapse, in which case the line~ object abandons its old tra jectory and takes up a new one.

Two messages to line~ might arrive at the same time or so close together

in time that no DSP computation takes place between the two; in this case, the earlier message has no e®ect, since line~ won't have changed its output yet to follow the ¯rst message, and its current output, unchanged, is then used as a starting point for the second segment. An exception to this rule is that, if line~ gets a time value of zero, the output value is immediately set to the new value and further segments will start from the new value; thus, by sending two pairs, the ¯rst with a time value of zero and the second with a nonzero time value, one can independently specify the beginning and end values of a segment in line~'s output.

The treatment of line~'s right inlet is unusual among Pd objects in that

it forgets old values; a message with a single number such as \0.1" is always equivalent to the pair, \0.1 0". Almost any other object will retain the previous value for the right inlet, instead of resetting it to zero.

Example A04.line2.pd shows the line~ object's output graphically. Using the various message boxes, you can recreate the e®ects shown in Figure 1.6.

Ma jor triad

Example A05.output.subpatch.pd, whose active ingredients are shown in Figure 1.12 (part c), presents three sinusoids with frequencies in the ratio 4:5:6, so that the lower two are separated by a major third, the upper two by a minor third, and the top and bottom by a ¯fth. The lowest frequency is 440, equal to A above middle C, or MIDI 69. The others are approximately four and seven half-steps higher, respectively. The three have equal amplitudes.

The amplitude control in this example is taken care of by a new object called output~. This isn't a built-in object of Pd, but is itself a Pd patch which lives in a ¯le, \output.pd". (You can see the internals of output~ by opening the properties menu for the box and selecting \open".) You get two controls, one for amplitude in dB (100 meaning \unit gain"), and a \mute" button. Pd's audio processing is turned on automatically when you set the output level|this might not be the best behavior in general, but it's appropriate for these example patches. The mechanism for embedding one Pd patch as an object box inside another is discussed in Section 4.7.

Conversion between frequency and pitch

Example A06.frequency.pd (Figure 1.13) shows Pd's object for converting pitch to frequency units (mtof, meaning \MIDI to frequency") and its inverse ftom. We also introduce two other object classes, send and receive.

mtof , ftom : convert MIDI pitch to frequency units according to the Pitch/Frequency ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.041.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.042.png)Conversion Formulas (Page 7). Inputs and outputs are messages (\tilde" equiv-

alents of the two also exist, although like dbtorms~ they're expensive in CPU

time). The ftom object's output is -1500 if the input is zero or negative; and likewise, if you give mtof -1500 or lower it outputs zero.

receive , r : Receive messages non-locally. The receive object, which may![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.043.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.044.png)

r frequency r pitch![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.045.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.046.png)

set $1 set $1

0   <−− set frequency 0   <−− set MIDI pitch

s frequency s pitch

ftom <−− convert frequency mtof <−− convert "MIDI" pitch

to "MIDI" pitch to frequency s pitch s frequency

Figure 1.13: Conversion between pitch and frequency in A06.frequency.pd.

be abbreviated as \r", waits for non-local messages to be sent by a send ob- ject (described below) or by a message box using redirection (the \;" feature discussed in the earlier example, A01.sinewave.pd). The argument (such as \fre- quency" and \pitch" in this example) is the name to which messages are sent. Multiple receive objects may share the same name, in which case any message sent to that name will go to all of them.

send , s : The send object, which may be abbreviated as \s", directs mes- sages![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.047.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.048.png) to receive objects.

Two new properties of number boxes are used here. Earlier we've used them as controls or as displays; here, the two number boxes each function as both. If a number box gets a number in its inlet, it not only displays the number but also repeats the number to its output. However, a number box may also be sent a \set" message, such as \set 55" for example. This would set the value of the number box to 55 (and display it) but not cause the output that would result from the simple \55" message. In this case, numbers coming from the two receive objects are formatted (using message boxes) to read \set 55" instead of just \55", and so on. (The special word \$1" is replaced by the incoming number.) This is done because otherwise we would have an in¯nite loop: frequency would change pitch which would change frequency and so on forever, or at least until something broke.

More additive synthesis

The major triad (Example A06.frequency.pd, Page 22) shows one way to com- bine several sinusoids together by summing. There are many other possible ways to organize collections of sinusoids, of which we'll show two. Example A07.fusion.pd (Figure 1.14) shows four oscillators, whose frequencies are tuned in the ratio 1:2:3:4, with relative amplitudes 1, 0.1, 0.2, and 0.5. The amplitudes are set by multiplying the outputs of the oscillators (the \*~ objects below the oscillators).

0   <-- choose a pitch mtof![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.049.png)

* 2 \* 3 \* 4frequencies of harmonics

osc~ osc~ osc~ osc~ four oscillators

\*~ 0.1 \*~ 0.2 \*~ 0.5 adjust amplitudes

+~ 

+~  add the three overtones together +~  \*~  <-- overtones ON/OFF

(OUT)

Figure 1.14: Additive synthesis using harmonically tuned oscillators.

The second, third, and fourth oscillator are turned on and o®using a toggle switch. This is a graphical control, like the number box introduced earlier. The

toggle switch puts out 1 and 0 alternately when clicked on with the mouse.

This value is multiplied by the sum of the second, third, and fourth oscillators, e®ectively turning them on and o®.

Even when all four oscillators are combined (with the toggle switch in the \1" position), the result fuses into a single tone, heard at the pitch of the leftmost oscillator. In e®ect this patch sums a four-term Fourier series to generate a complex, periodic waveform.

Example A08.beating.pd (Figure 1.15) shows another possibility, in which

six oscillators are tuned into three pairs of neighbors, for instance 330 and 330.2

Hertz. These pairs slip into and out of phase with each other, so that the amplitude of the sum changes over time. Called beating, this phenomenon is frequently used for musical e®ects.

Oscillators may be combined in other ways besides simply summing their

output, and a wide range ofresulting sounds is available. Example A09.frequency.mod.pd (not shown here) demonstrates frequency modulation synthesis, in which one oscillator controls another's frequency. This will be more fully described in

Chapter 5.

Exercises

1. A sinusoid (Page 1) has initial phase Á = 0 and angular frequency ! = ¼=10. What is its period in samples? What is the phase at sample number

osc~ 330 osc~ 440 osc~ 587![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.050.png)

osc~ 330.2 osc~ 440.33 osc~ 587.25 +~  +~  +~ 

+~ 

+~ 

(OUT)

Figure 1.15: Additive synthesis: six oscillators arranged into three beating pairs.

n = 10?

2. Two sinusoids have periods of 20 and 30 samples, respectively. What is the period of the sum of the two?
2. If 0 dB corresponds to an amplitude of 1, how many dB corresponds to amplitudes of 1.5, 2, 3, and 5?
2. Two uncorrelated signals of RMS amplitude 3 and 4 are added; what's the RMS amplitude of the sum?
2. How many uncorrelated signals, all of equal amplitude, would you have to add to get a signal that is 9 dB greater in amplitude?
2. What is the angular frequency of middle C at 44100 samples per second?
2. Two sinusoids play at middle C (MIDI 60) and the neighboring C sharp (MIDI 61). What is the di®erence, in Hertz, between their frequencies?
2. How many cents is the interval between the seventh and the eighth har- monic of a periodic signal?
2. If an audio signal x[n];n = 0;:::;N ¡ 1 has peak amplitude 1, what is the minimum possible RMS amplitude? What is the maximum possible?

26 CHAPTER 1. SINUSOIDS, AMPLITUDE AND FREQUENCY


Chapter 2

Wavetables and samplers

In Chapter 1 we treated audio signals as if they always °owed by in a continuous stream at some sample rate. The sample rate isn't really a quality of the audio signal, but rather it speci¯es how fast the individual samples should °ow into or out of the computer. But audio signals are at bottom just sequences of numbers, and in practice there is no requirement that they be \played" sequentially. Another, complementary view is that they can be stored in memory, and, later, they can be read back in any order|forward, backward, back and forth, or totally at random. An inexhaustible range of new possibilities opens up.

For many years (roughly 1950-1990), magnetic tape served as the main stor- age medium for sounds. Tapes were passed back and forth across magnetic pickups to play the signals back in real time. Since 1995 or so, the predominant way of storing sounds has been to keep them as digital audio signals, which are read back with much greater freedom and facility than were the magnetic tapes. Many modes of use dating from the tape era are still current, including cutting, duplication, speed change, and time reversal. Other techniques, such as waveshaping, have come into their own only in the digital era.

Suppose we have a stored digital audio signal, which is just a sequence of samples (i.e., numbers) x[n] for n = 0;:::;N ¡ 1, where N is the length of the sequence. Then if we have an input signal y[n] (which we can imagine to be °owing in real time), we can use its values as indices to look up values of the stored signal x[n]. This operation, called wavetable lookup, gives us a new signal, z[n], calculated as:

z[n] = x[y[n]]

Schematically we represent this operation as shown in Figure 2.1.

Two complications arise. First, the input values, y[n], might lie outside the range 0;:::;N ¡ 1, in which case the wavetable x[n] has no value and the expression for the output z[n] is unde¯ned. In this situation we might choose to clip the input, that is, to substitute 0 for anything negative and N ¡ 1 for anything N or greater. Alternatively, we might prefer to wrap the input around end to end. Here we'll adopt the convention that out-of-range samples

27

1. THE WAVETABLE OSCILLATOR 31

IN 

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.051.png)

OUT

Figure 2.1: Diagram for wavetable lookup. The input is in samples, ranging approximately from 0 to the wavetable's size N, depending on the interpolation scheme.

are always clipped; when we need wraparound, we'll introduce another signal processing operation to do it for us.

The second complication is that the input values need not be integers; in other words they might fall between the points of the wavetable. In general, this is addressed by choosing some scheme for interpolating between the points of the wavetable. For the moment, though, we'll just round down to the nearest integer below the input. This is called non-interpolating wavetable lookup, and its full de¯nition is:

8

- x[by[n]c] if 0 · y[n] < N ¡ 1

z[n] = x[0] if y[n] < 0

: x[N ¡ 1] if y[n] ¸ N ¡ 1

(where by[n]c means, \the greatest integer not exceeding y[n]").

Pictorally, we use y[0](a number) as a location on the horizontal axis of the wavetable shown in Figure 2.1, and the output, z[0], is whatever we get on the vertical axis; and the same for y[1] and z[1] and so on. The \natural" range for the input y[n] is 0 · y[n] < N. This is di®erent from the usual range of an audio signal suitable for output from the computer, which ranges from -1 to 1 in our units. We'll see later that the usable range of input values, from 0 to N for non-interpolating lookup, shrinks slightly if interpolating lookup is used.

Figure 2.2 (part a) shows a wavetable and the result of using two di®erent input signals as lookup indices into it. The wavetable contains 40 points, which are numbered from 0 to 39. In part (b), a sawtooth wave is used as the input signal y[n]. A sawtooth wave is nothing but a ramp function repeated end to end. In this example the sawtooth's range is from 0 to 40 (this is shown in the vertical axis). The sawtooth wave thus scans the wavetable from left to right|from the beginning point 0 to the endpoint 39|and does so every time it repeats. Over the ¯fty points shown in Figure 2.2 (part b) the sawtooth wave

makes two and a half cycles. Its period is twenty samples, or in other words the frequency (in cycles per second) is R=20.

Part (c) of Figure 2.2 shows the result of applying wavetable lookup, using the table x[n], to the signal y[n]. Since the sawtooth input simply reads out the contents of the wavetable from left to right, repeatedly, at a constant rate of precession, the result will be a new periodic signal, whose waveform (shape) is derived from x[n] and whose frequency is determined by the sawtooth wave y[n].

Parts (d) and (e) show an example where the wavetable is read in a nonuni- form way; since the input signal rises from 0 to N and then later recedes to 0, we see the wavetable appear ¯rst forward, then frozen at its endpoint, then backward. The table is scanned from left to right and then, more quickly, from right to left. As in the previous example the incoming signal controls the speed of precession while the output's amplitudes are those of the wavetable.

1. The Wavetable Oscillator

Figure 2.2 suggests an easy way to synthesize any desired ¯xed waveform at any desired frequency, using the block diagram shown in Figure 2.3. The upper block is an oscillator|not the sinusoidal oscillator we saw earlier, but one that produces sawtooth waves instead. Its output values, as indicated at the left of the block, should range from 0 to the wavetable size N. This is used as an index into the wavetable lookup block (introduced in Figure 2.1), resulting in a periodic waveform. Figure 2.3 (part b) adds an envelope generator and a multiplier to control the output amplitude in the same way as for the sinusoidal oscillator shown in Figure 1.7 (Page 11). Often, one uses a wavetable with (RMS or peak) amplitude 1, so that the amplitude of the output is just the magnitude of the envelope generator's output.

Wavetable oscillators are often used to synthesize sounds with speci¯ed, static spectra. To do this, you can pre-compute N samples of any waveform of period N (angular frequency 2¼=N) by adding up the elements of the Fourier Series (Page 12). The computation involved in setting up the wavetable at ¯rst might be signi¯cant, but this may be done in advance of the synthesis process, which might take place in real time.

While direct additive synthesis of complex waveforms, as shown in Chapter 1, is in principle in¯nitely °exible as a technique for producing time-varying timbres, wavetable synthesis is much less expensive in terms of computation but requires switching wavetables to change the timbre. An intermediate technique, more °exible and expensive than simple wavetable synthesis but less °exible and less expensive than additive synthesis, is to create time-varying mixtures between a small number of ¯xed wavetables. If the number of wavetables is only two, this is in e®ect a cross-fade between the two waveforms, as diagrammed in Figure 2.4. Suppose we wish to use some signal 0 · x[n] · 1 to control the relative strengths of the two waveforms, so that, if x[n] = 0, we get the ¯rst one and if x[n] = 1 we get the second. Denoting the two signals to be cross-faded

1   x[n]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.052.png)

(a) 0   40  n  

−1 

40  y[n]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.053.png)

0~~   (b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.054.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.055.png)

50 

1   z[n]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.056.png)

(c) −1 

40  y2[n]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.057.png)

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.058.png) 0   ~~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.059.png)~~ (d)

1   z2[n]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.060.png)

(e) −1 

Figure 2.2: Wavetable lookup: (a) a wavetable; (b) and (d) signal inputs for lookup; (c) and (e) the corresponding outputs.

frequency frequency ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.061.png)

N  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.062.png)

N  

0  0   1  1  

-1 

-1 

OUT

OUT (a)

(b)

Figure 2.3: Block diagrams: (a) for a wavetable lookup oscillator; (b) with amplitude control by an envelope generator.

by y[n] and z[n], we compute the signal

(1 ¡ x[n])y[n]+ x[n]z[n] or, equivalently and usually more e±cient to calculate, y[n]+ x[n](z[n]¡ y[n])

This computation is diagrammed in Figure 2.4.

When using this technique to cross-fade between wavetable oscillators, it might be desirable to keep the phases of corresponding partials the same across the wavetables, so that their amplitudes combine additively when they are mixed. On the other hand, if arbitrary wavetables are used (borrowed, for instance, from a recorded sound) there will be a phasing e®ect as the di®erent waveforms are mixed.

This scheme can be extended in a daisy chain to move along a continuous path between a succession of timbres. Alternatively, or in combination with daisy-chaining, cross-fading may be used to interpolate between two di®erent timbres, for example as a function of musical dynamic. To do this you would prepare two or even several waveforms of a single synthetic voice played at di®erent dynamics, and interpolate between successive ones as a function of the output dynamic you want.

2. SAMPLING 35

frequency

N  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.063.png)

0  1  

-1 

OUT

Figure 2.4: Block diagram for cross-fading between two wavetables.

2. Sampling

\Sampling" is nothing more than recording a live signal into a wavetable, and then later playing it out again. (In commercial samplers the entire wavetable is usually called a \sample" but to avoid confusion we'll only use the word \sample" here to mean a single number in an audio signal.)

At its simplest, a sampler is simply a wavetable oscillator, as was shown in Figure 2.3. However, in the earlier discussion we imagined playing the oscillator back at a frequency high enough to be perceived as a pitch, at least 30 Hertz or so. In the case of sampling, the frequency is usually lower than 30 Hertz, and so the period, at least 1/30 second and perhaps much more, is long enough that you can hear the individual cycles as separate events.

Going back to Figure 2.2, suppose that instead of 40 points the wavetable x[n] is a one-second recording, at an original sample rate of 44100, so that it has 44100 points; and let y[n] in part (b) of the ¯gure have a period of 22050 samples. This corresponds to a frequency of 2 Hertz. But what we hear is not a pitched sound at 2 cycles per second (that's too slow to hear as a pitch) but rather, we hear the original recording x[n] played back repeatedly at double speed. We've just reinvented the sampler.

In general, if we assume the sample rate R of the recording is the same as the output sample rate, if the wavetable has N samples, and if we index it with a sawtooth wave of period M, the sample is sped up or slowed down by a factor of

N=M, equal to Nf =R if f is the frequency in Hertz of the sawtooth. If we denote the transposition factor by t (so that, for instance, t = 3=2 means transposing upward a perfect ¯fth), and if we denote the transposition in half-steps by h, then we get the Transposition Formulas for Looping Wavetables:

t = N=M = Nf =R

µ ¶ µ ¶ h = 12log2 M = 12log2 NRf

N

Frequently the desired transposition in half-steps (h) is known and the formula must be solved for either f or N:

2h=12 R f =

N 2h=12 R

N =

f

So far we have used a sawtooth as the input wave y[t], but, as suggested in parts (d) and (e) of Figure 2.2, we could use anything we like as an input signal. In general, the transposition may be time dependent and is controlled by the rate of change of the input signal.

The transposition multiple t and the transposition in half-steps h are then given by the Momentary Transposition Formulas for Wavetables:

t[n] = jy[n]¡ y[n ¡ 1]j
h[n] = 12log2 jy[n]¡ y[n ¡ 1]j

(Here the enclosing bars \j" mean absolute value.) For example, if y[n] = n, then z[n] = x[n] so we hear the wavetable at its original pitch, and this is what the formula predicts since, in that case,

y[n]¡ y[n ¡ 1] = 1

On the other hand, if y[n] = 2n, then the wavetable is transposed up an octave, consistent with

y[n]¡ y[n ¡ 1] = 2

If values of y[n] are decreasing with n, you hear the sample backward, but the transposition formula still gives a positive multiplier. This all agrees with the earlier Transposition Formula for Looping Wavetables; if a sawtooth ranges from 0 to N, f times per second, the di®erence of successive samples is just Nf =R|except at the sample at the beginning of each new cycle.

It's well known that transposing a recording also transposes its timbre|this

is the \chipmunk" e®ect. Not only are any periodicities (such as might give rise to pitch) transposed, but so are the frequencies of the overtones. Some timbres, notably those of vocal sounds, have characteristic frequency ranges in which overtones are stronger than other nearby ones. Such frequency ranges

are also transposed, and this is is heard as a timbre change. In language that will be made more precise in Section 5.1, we say that the spectral envelope is transposed along with the pitch or pitches.

In both this and the preceding section, we have considered playing wavetables periodically. In Section 2.1 the playback repeated quickly enough that the repetition gives rise to a pitch, say between 30 and 4000 times per second, roughly the range of a piano. In the current section we assumed a wavetable one second long, and in this case \reasonable" transposition factors (less than four octaves up) would give rise to a rate of repetition below 30, usually much lower, and going down as low as we wish.

The number 30 is signi¯cant for another reason: it is roughly the maximum number of separate events the ear can discern per second; for instance, 30 vocal phonemes, or melodic notes, or attacks of a snare drum are about the most we can hope to crowd into a second before our ability to distinguish them breaks down.

A continuum exists between samplers and wavetable oscillators, in that the patch of Figure 2.3 can either be regarded as a sampler (if the frequency of rep- etition is less than about 20 Hertz) or as a wavetable oscillator (if the frequency is greater than about 40 Hertz). It is possible to move continuously between the two regimes. Furthermore, it is not necessary to play an entire wavetable in a loop; with a bit more arithmetic we can choose sub-segments of the wavetable, and these can change in length and location continuously as the wavetable is played.

The practice of playing many small segments of a wavetable in rapid suc- cession is often called granular synthesis. For much more discussion of the possibilities, see [Roa01].

Figure 2.5 shows how to build a very simple looping sampler. In the ¯gure, if the frequency is f and the segment size in samples is s, the output transposition factor is given by t = f s=R, where R is the sample rate at which the wavetable was recorded (which need not equal the sample rate the block diagram is working at.) In practice, this equation must usually be solved for either f or s to attain a desired transposition.

In the ¯gure, a sawtooth oscillator controls the location of wavetable lookup, but the lower and upper values of the sawtooth aren't statically speci¯ed as they were in Figure 2.3; rather, the sawtooth oscillator simply ranges from 0 to 1 in value and the range is adjusted to select a desired segment of samples in the wavetable.

It might be desirable to specify the segment's location l either as its left- hand edge (its lower bound) or else as the segment's midpoint; in either case we specify the length s as a separate parameter. In the ¯rst case, we start by multiplying the sawtooth by s, so that it then ranges from 0 to s; then we add l so that it now ranges from l to l + s. In order to specify the location as the segment's midpoint, we ¯rst subtract 1=2 from the sawtooth (so that it ranges from ¡1=2 to 1=2), and then as before multiply by s (so that it now ranges from ¡s=2 to s=2) and add l to give a range from l ¡ s=2 to l + s=2.

In the looping sampler, we will need to worry about maintaining continuity

frequency 1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.064.png)

0  

optional - for 1/2

centered segments segment size

segment location

1  -1 

OUT

Figure 2.5: A simple looping sampler, as yet with no amplitude control. There are inputs to control the frequency and the segment size and location. The \-" operation is included if we wish the segment location to be speci¯ed as the segment's midpoint; otherwise we specify the location of the left end of the segment.

4. TIMBRE STRETCHING 41

between the beginning and the end of segments of the wavetable; we'll take this up in the next section.

A further detail is that, if the segment size and location are changing with time (they might be digital audio signals themselves, for instance), they will a®ect the transposition factor, and the pitch or timbre ofthe output signal might waver up and down as a result. The simplest way to avoid this problem is to synchronize changes in the values ofs and l with the regular discontinuities ofthe sawtooth; since the signal jumps discontinuously there, the transposition is not really de¯ned there anyway, and, if you are enveloping to hide the discontinuity, the e®ects of changes in s and l are hidden as well.

3. Enveloping samplers

In the previous section we considered reading a wavetable either sporadically or repeatedly to make a sampler. In most real applications we must deal with getting the samples to start and stop cleanly, so that the output signal doesn't jump discontinuously at the beginnings and ends of samples. This discontinuity can sound like a click or a thump depending on the wavetable.

The easiest way to do this, assuming we will always play a wavetable com- pletely from beginning to end, is simply to prepare it in advance so that it fades in cleanly at the beginning and out cleanly at the end. This may even be done when the wavetable is sampled live, by multiplying the input signal by a line segment envelope timed to match the length of the recording.

In many situations, however, it is either inconvenient or impossible to pre- envelope the wavetable|for example, we might want to play only part of it back, or we may want to change the sharpness of the enveloping dynamically. In Section 1.5 we had already seen how to control the amplitude of sinusoidal oscillators using multiplication by a ramp function (also known as an envelope generator), and we built this notion into the wavetable oscillators of Figures

3. and 2.4. This also works ¯ne for turning samplers on and o® to avoid discontinuities, but with one major di®erence: whereas in wavetable synthesis, we were free to assume that the waveform lines up end to end, so that we may choose any envelope timing we want, in the case of sampling using unprepared waveforms, we are obliged to get the envelope generator's output to zero by the time we reach the end of the wavetable for the ¯rst time. This situation is pictured in Figure 2.6.

   In situations where an arbitrary wavetable must be repeated as needed, the simplest way to make the looping work continuously is to arrange for amplitude change to be synchronized with the looping, using a separate wavetable (the envelope). This may be implemented as shown in Figure 2.7. A single sawtooth oscillator is used to calculate lookup indices for two wavetables, one holding the recorded sound, and the other, an envelope shape. The main thing to worry about is getting the inputs of the two wavetables each into its own appropriate range.

In many situations it is desirable to combine two or more copies ofthe looping

(a) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.065.png)

new periods 

(b)

Figure 2.6: Di®ering envelope requirements for oscillators and samplers: (a) in an oscillator, the envelope can be chosen to conform to any desired timescale;

2) when the wavetable is a recorded sound, it's up to you to get the envelope to zero before you hit the end of the wavetable for the ¯rst time.

   wavetable sampler at the same frequency and at a speci¯ed phase relationship. This may be done so that when any particular one is at the end of its segment, one or more others is in the middle of the same segment, so that the aggregate is continuously making sound. To accomplish this, we need a way to generate two or more sawtooth waves at the desired phase relationship that we can use in place of the oscillator at the top of Figure 2.7. We can start with a single sawtooth wave and then produce others at ¯xed phase relationships with the ¯rst one. If we wish a sawtooth which is, say, a cycles ahead of the ¯rst one, we simply add the parameter a and then take the fractional part, which is the desired new sawtooth wave, as shown in Figure 2.8.

4. Timbre stretching

The wavetable oscillator of Section 2.1, which we extended in Section 2.2 to en- compass grabbing waveforms from arbitrary wavetables such as recorded sounds, may additionally be extended in a complementary way, that we'll refer to as timbre stretching, for reasons we'll develop in this section. There are also many other possible ways to extend wavetable synthesis, using for instance frequency modulation and waveshaping, but we'll leave them to later chapters.

The central idea oftimbre stretching is to reconsider the idea ofthe wavetable

frequency 1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.066.png)

0  

size

N  location

1   1  0  

-1 

0   N  

OUT

Figure 2.7: A sampler as in Figure 2.5, but with an additional wavetable lookup for enveloping.

frequency![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.067.png)

1   1  

0  

1\.3 a  

0\.3

WRAP

OUT

1  

0\.3

Figure 2.8: A technique for generating two or more sawtooth waves with ¯xed phase relationships between them. The relative phase is controlled by the pa- rameter a (which takes the value 0.3 in the graphed signals). The \wrap" operation computes the fractional part of its input.

(a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.068.png)

20  40  50 

10  30 

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.069.png)

15  25 

(c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.070.png)

20  40  60 0  

Figure 2.9: A waveform is played at a period of 20 samples: (a) at 100 percent duty cycle; (b) at 50 percent; (c) at 200 percent

oscillator as a mechanism for playing a stored wavetable (or part of one) end to end. There is no reason the end of one cycle has to coincide with the beginning of another. Instead, we could ask for copies of the waveform to be spaced with alternating segments of silence; or, going in the opposite direction, the waveform copies could be spaced more closely together so that they overlap. The single parameter available in Section 2.1|the frequency|has been heretofore used to control two separate aspects of the output: the period at which we start new copies of the waveform, and also the length of each individual copy. The idea of timbre stretching is to control the two independently.

Figure 2.9 shows the result of playing a wavetable in three ways. In each case the output waveform has period 20; in other words, the output frequency is R=20 if R is the output sample rate. In part (a) of the ¯gure, each copy of the waveform is played over 20 samples, so that the wave form ¯ts exactly into the cycle with no gaps and no overlap. In part (b), although the period is still 20, the waveform is compressed into the middle half of the period (10 samples); or in other words, the duty cycle|the relative amount of time the waveform ¯lls the cycle|equals 50 percent. The remaining 50 percent of the time, the output is zero.

In part (c), the waveform is stretched to 40 samples, and since it is still repeated every 20 samples, the waveforms overlap two to one. The duty cycle is thus 200 percent.

Suppose now that the 100 percent duty cycle waveform has a Fourier series

(Section 1.7) equal to:

x100 [n] = a0 + a1 cos(!n + Á1) + a2 cos(2!n + Á2) + ¢¢¢

where ! is the angular frequency (equal to ¼=10 in our example since the period is 20.) To simplify this example we won't worry about where the series must end, and will just let it go on forever.

We would like to relate this to the Fourier series of the other two waveforms in the example, in order to show how changing the duty cycle changes the timbre of the result. For the 50 percent duty cycle case (calling the signal x50 [n]), we observe that the waveform, if we replicate it out of phase by a half period and add the two, gives exactly the original waveform at twice the frequency:

¼ x [2n] = x [n]+ x [n + ]

100 50 50 !

where ! is the angular frequency (and so ¼=! is half the period) of both signals. So if we denote the Fourier series of x50[n] as:

x50[n] = b0 + b1 cos(!n + µ1) + b2 cos(2!n + µ2) + ¢¢¢ and substitute the Fourier series for all three terms above, we get: a0 + a1 cos(2!n + Á1) + a2 cos(4!n + Á2) + ¢¢¢

- b0 + b1 cos(!n + µ1) + b2 cos(2!n + µ2) + ¢¢¢

+b0 + b1 cos(!n + ¼+ µ1) + b2 cos(2!n + 2¼+ µ2) + ¢¢¢

- 2b0 + 2b2 cos(2!n + µ2) + 2b4 cos(4!n + µ4) + ¢¢¢

and so

a0 = 2b0; a1 = 2b2; a2 = 2b4

and so on: the even partials of x50 , at least, are obtained by stretching the partials of x100 out twice as far. (We don't yet know about the odd partials of x50 , and these might be in line with the even ones or not, depending on factors we can't control yet. Su±ce it to say for the moment, that if the waveform connects smoothly with the horizontal axis at both ends, the odd partials will act globally like the even ones. To make this more exact we'll need Fourier analysis, which is developed in Chapter 9.)

Similarly, x100 and x200 are related in exactly the same way:

¼

x [2n] = x [n]+ x [n + ]

200 100 100 !

so that, if the amplitudes of the fourier series of x200 are denoted by c0, c1, :::, we get:

c0 = 2a0;c1 = 2a2;c2 = 2a4;:::

so that the partials of x200 are those of x100 shrunk, by half, to the left.

5. INTERPOLATION 45

200%![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.071.png)

ampli-

tude 100% 50%

1   2   3   4   5  

partial number

Figure 2.10: The Fourier series magnitudes for the waveforms shown in Figure 2.9. The horizontal axis is the harmonic number. We only \hear" the coe±cients for integer harmonic numbers; the continuous curves are the \ideal" contours.

We see that squeezing the waveform by a factor of 2 has the e®ect of stretch- ing the Fourier series out by two, and on the other hand stretching the waveform by a factor of two squeezes the Fourier series by two. By the same sort of ar- gument, in general it turns out that stretching the waveform by a factor of any positive number f squeezes the overtones, in frequency, by the reciprocal 1=f|at least approximately, and the approximation is at least fairly good if the waveform \behaves well" at its ends. (As we'll see later, the waveform can always be forced to behave at least reasonably well by enveloping it as in Figure 2.7.)

Figure 2.10 shows the spectra of the three waveforms|or in other words the one waveform at three duty cycles|of Figure 2.9. The ¯gure emphasizes the relationship between the three spectra by drawing curves through each, which, on inspection, turn out to be the same curve, only stretched di®erently; as the duty cycle goes up, the curve is both compressed to the left (the frequencies all drop) and ampli¯ed (stretched upward).

The continuous curves have a very simple interpretation. Imagine squeezing the waveform into some tiny duty cycle, say 1 percent. The contour will be stretched by a factor of 100. Working backward, this would allow us to inter- polate between each pair of consecutive points of the 100 percent duty cycle contour (the original one) with 99 new ones. Already in the ¯gure the 50 per- cent duty cycle trace de¯nes the curve with twice the resolution of the original

one. In the limit, as the duty cycle gets arbitrarily small, the spectrum is ¯lled in more and more densely; and the limit is the \true" spectrum of the waveform.

This \true" spectrum is only audible at suitably low duty cycles, though. The 200 percent duty cycle example actually misses the peak in the ideal (con- tinuous) spectrum because the peak falls below the ¯rst harmonic. In general, higher duty cycles sample the ideal curve at lower resolutions.

Timbre stretching is an extremely powerful technique for generating sounds with systematically variable spectra. Combined with the possibilities of mix- tures of waveforms (Section 2.1) and of snatching endlessly variable waveforms from recorded samples (Section 2.2), it is possible to generate all sorts of sounds. For example, the block diagram of Figure 2.7 gives us a way to to grab and stretch timbres from a recorded wavetable. When the \frequency" parameter f is high enough to be audible as a pitch, the \size" parameter s can be thought of as controlling timbre stretch, via the formula t = f s=R from Section 2.2, where we now reinterpret t as the factor by which the timbre is to be stretched.

5. Interpolation

As mentioned before, interpolation schemes are often used to increase the ac- curacy of table lookup. Here we will give a somewhat simpli¯ed account of the e®ects of table sizes and interpolation schemes on the result of table lookup.

To speak of error in table lookup, we must view the wavetable as a sampled version of an underlying function. When we ask for a value of the underlying function which lies between the points ofthe wavetable, the error is the di®erence between the result of the wavetable lookup and the \ideal" value of the function at that point. The most revealing study of wavetable lookup error assumes that the underlying function is a sinusoid (Page 1). We can then understand what happens to other wavetables by considering them as superpositions (sums) of sinusoids.

The accuracy of lookup from a wavetable containing a sinusoid depends on two factors: the quality of the interpolation scheme, and the period of the sinusoid. In general, the longer the period of the sinusoid, the more accurate the result.

In the case of a synthetic wavetable, we might know its sinusoidal com- ponents from having speci¯ed them|in which case the issue becomes one of choosing a wavetable size appropriately, when calculating the wavetable, to match the interpolation algorithm and meet the desired standard of accuracy. In the case of recorded sounds, the accuracy analysis might lead us to adjust the sample rate of the recording, either at the outset or else by resampling later.

Interpolation error for a sinusoidal wavetable can have two components: ¯rst, the continuous signal (the theoretical result of reading the wavetable continu- ously in time, as if the output sample rate were in¯nite) might not be a pure sinusoid; and second, the amplitude might be wrong. (It is possible to get phase errors as well, but only through carelessness.)

In this treatment we'll only consider polynomial interpolation schemes such

as rounding, linear interpolation, and cubic interpolation. These schemes amount to evaluating polynomials (of degree zero, one, and three, respectively) in the interstices between points of the wavetable. The idea is that, for any index x, we choose a nearby reference point x0, and let the output be calculated by some polynomial:

yINT (x) = a0 + a1(x ¡ x0) + a2(x ¡ x0)2 + ¢¢¢+ an (x ¡ x0)n

Usually we choose the polynomial which passes through the n + 1 nearest points of the wavetable. For 1-point interpolation (a zero-degree polynomial) this means letting a0 equal the nearest point of the wavetable. For two-point inter- polation, we draw a line segment between the two points of the wavetable on either side of the desired point x. We can let x0 be the closest integer to the left of x (which we write as bxc) and then the formula for linear interpolation is:

yINT (x) = y[x0]+ (y[x0 + 1]¡ y[x0]) ¢(x ¡ x0)

which is a polynomial, as in the previous formula, with

a0 = y[x0]

a1 = y[x0 + 1]¡ y[x0]

In general, you can ¯t exactly one polynomial of degree n ¡ 1 through any n points as long as their x values are all di®erent.

Figure 2.11 shows the e®ect of using linear (two-point) interpolation to ¯ll in a sinusoid of period 6. At the top are three traces: the original sinusoid, the linearly-interpolated result of using 6 points per period to represent the sinusoid, and ¯nally, another sinusoid, of slightly smaller amplitude, which bet- ter matches the six-segment waveform. The error introduced by replacing the original sinusoid by the linearly interpolated version has two components: ¯rst, a (barely perceptible) change in amplitude, and second, a (very perceptible) distortion of the wave shape.

The bottom graph in the ¯gure shows the di®erence between the interpolated waveform and the best-¯tting sinusoid. This is a residual signal all of whose en- ergy lies in overtones of the original sinusoid. As the number of points increases, the error decreases in magnitude. Since the error is the di®erence between a sinusoid and a sequence of approximating line segments, the magnitude of the error is roughly proportional to the square of the phase di®erence between each pair of points, or in other words, inversely proportional to the square of the number of points in the wavetable. Put another way, wavetable error decreases by 12 dB each time the table doubles in size. (This rule of thumb is only good for tables with 4 or more points.)

original best fit interpolated![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.072.png)

error![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.073.png)

Figure 2.11: Linear interpolation of a sinusoid: (upper graph) the original sinu- soid, the interpolated sinusoid, and the best sinusoidal ¯t back to the interpo- lated version; (lower graph) the error, rescaled vertically.

6. EXAMPLES 51

period interpolation points![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.074.png)

1  2 4
2  -1.2 -17.1 -20.2
2  -2.0 -11.9 -15.5
2  -4.2 -17.1 -24.8

8 -10.0 -29.6 -48.4

16 -15.9 -41.8 -72.5

32 -21.9 -53.8 -96.5

64 -27.9 -65.9 -120.6

128 -34.0 -77.9 -144.7

Table 2.1: RMS error for table lookup using 1, 2, and 4 point interpolation at various table sizes.

Four-point (cubic) interpolation works similarly. The interpolation formula is:

yINT (x) =

¡f (f ¡ 1)(f ¡ 2)=6 ¢y[x0 ¡ 1]+ (f + 1)(f ¡ 1)(f ¡ 2)=2 ¢y[x0]

¡(f + 1)f (f ¡ 2)=2 ¢y[x0 + 1]+ (f + 1)f (f ¡ 1)=6 ¢y[x0 + 2]

where f = x ¡ x0 is the fractional part of the index. For tables with 4 or more points, doubling the number of points on the table tends to improve the RMS error by 24 dB. Table 2.1 shows the calculated RMS error for sinusoids at various periods for 1, 2, and 4 point interpolation. (A slightly di®erent quantity is measured in [Moo90, p.164]. There, the errors in amplitude and phase are also added in, yielding slightly more pessimistic results. See also [Har87].)

The allowable input domain for table lookup depends on the number of points of interpolation. In general, when using k-point interpolation into a table with N points, the input may range over an interval of N + 1 ¡ k points. If k = 1 (i.e., no interpolation at all), the domain is from 0 to N (including the endpoint at 0 but excluding the one at N) assuming input values are truncated (as is done for non-interpolated table lookup in Pd). The domain is from -1=2 to N ¡ 1=2 if, instead, we round the input to the nearest integer instead of interpolating. In either case, the domain stretches over a length of N points.

For two-point interpolation, the input must lie between the ¯rst and last points, that is, between 0 and N ¡ 1. So the N points su±ce to de¯ne the function over a domain of length N ¡ 1. For four-point interpolation, we cannot get values for inputs between 0 and 1 (not having the required two points to the left of the input) and neither can we for the space between the last two points (N ¡ 2 and N ¡ 1). So in this case the domain reaches from 1 to N ¡ 2 and has length N ¡ 3.

Periodic waveforms stored in wavetables require special treatment at the ends of the table. For example, suppose we wish to store a pure sinusoid of length N. For non-interpolating table lookup, it su±ces to set, for example,

x[n] = cos(2¼n=N); n = 0;:::;N ¡ 1

table10

0   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.075.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.076.png)mtof 0   

tabosc4~ table10 |   

(OUT) 

Figure 2.12: A wavetable oscillator: B01.wavetables.pd.

For two-point interpolation, we need N + 1 points:

x[n] = cos(2¼n=N); n = 0;:::;N

In other words, we must repeat the ¯rst (n = 0) point at the end, so that the last segment from N ¡ 1 to N reaches back to the beginning value.

For four-point interpolation, the cycle must be adjusted to start at the point n = 1, since we can't get properly interpolated values out for inputs less than one. If, then, one cycle of the wavetable is arranged from 1 to N, we must supply extra points for 0 (copied from N), and also N + 1 and N + 2, copied from 1 and 2, to make a table of length N + 3. For the same sinusoid as above, the table should contain:

x[n] = cos(2¼(n ¡ 1)=N); n = 0;:::;N + 2

6. Examples

Wavetable oscillator

Example B01.wavetables.pd, shown in Figure 2.12, implements a wavetable os- cillator, which plays back from a wavetable named \table10". Two new Pd primitives are shown here. First is the wavetable itself, which appears at right in the ¯gure. You can \mouse" on the wavetable to change its shape and hear the sound change as a result. Not shown in the ¯gure but demonstrated in the patch is Pd's facility for automatically calculating wavetables with speci¯ed partial amplitudes, which is often preferable to drawing waveforms by hand. You can also read and write tables to (text or sound) ¯les for interchanging data with other programs. The other novelty is an object class:

tabosc4 » : a wavetable oscillator. The \4" indicates that this class uses 4- ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.077.png)point (cubic) interpolation. In the example, the table's name, \table10", is

speci¯ed as a creation argument to the tabosc4~ object. (You can also switch between wavetables dynamically by sending appropriate messages to the object.)

Wavetables used by tabosc4~ must always have a period equal to a power of two; but as shown above, the wavetable must have three extra points wrapped around the ends. Allowable table lengths are thus of the form 2m + 3, such as 131, 259, 515, etc.

Wavetable oscillators are not limited to use as audio oscillators. Patch B02.wavetable.FM.pd (not pictured here) uses a pair of wavetable oscillators in series. The ¯rst one's output is used as the input of the second one, and thus controls its frequency which changes periodically in time.

Wavetable lookup in general

The tabosc4~ class, while handy and e±cient, is somewhat specialized and for many of the applications described in this chapter we need something more gen- eral. Example B03.tabread4.pd (Figure 2.13) demonstrates the timbre stretch- ing technique discussed in Section 2.4. This is a simple example of a situation where tabosc4~ would not have su±ced. There are new classes introduced here:

tabread4 » : wavetable lookup. As in tabosc4~ the table is read using 4- ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.078.png)point interpolation. But whereas tabosc4~ takes a frequency as input and automatically reads the waveform in a repeating pattern, the simpler tabread4~ expects the table lookup index as input. If you want to use it to do something repetitious, as in this example, the input itself has to be a repeating waveform. Like tabosc4~ (and all the other table reading and writing objects), you can send messages to select which table to use.

tabwrite » : record an audio signal into a wavetable. In this example the tabwrite~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.079.png) is used to display the output (although later on it will be used for all sorts of other things.) Whenever it receives a \bang" message from the pushbutton icon above it, tabwrite~ begins writing successive samples of its input to the named table.

Example B03.tabread4.pd shows how to combine a phasor~ and a tabread4~ object to make a wavetable oscillator. The phasor~'s output ranges from 0 to 1 in value. In this case the input wavetable, named \waveform12", is 131 elements long. The domain for the tabread4~ object is thus from 1 to 129. To adjust the range of the phasor~ accordingly, we multiply it by the length of the domain (128) so that it reaches between 0 and 128, and then add 1, e®ectively sliding the interval to the right by one point. This rescaling is accomplished by the \*~ and +~ objects between the phasor~ and the tabread4~.

With only these four boxes we would have essentially reinvented the tabosc4~ class. In this example, however, the multiplication is not by a constant 128 but by a variable amount controlled by the \squeeze" parameter. The function of the four boxes at the right hand side of the patch is to supply the \*~ object with values to scale the phasor~ by. This makes use of one more new object class:

frequency squeeze 162 206![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.080.png)

phase

generation --> phasor~ pack 0 50

range

adjustment --> \*~  line~

+~ 1 +~ 128 tabread4~ waveform12

<--click to graph

tabwrite~ wave-out12

waveform12

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.081.png)

wave-out12

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.082.png)

Figure 2.13: A wavetable oscillator with variable duty cycle: B03.tabread4.pd.

pack : compose a list of two or more elements. The creation arguments es- tablish![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.083.png) the number of arguments, their types (usually numbers) and their initial values. The inlets (there will be as many as you speci¯ed creation arguments) update the values of the message arguments, and, if the leftmost inlet is changed (or just triggered with a \bang" message), the message is output.

In this patch the arguments are initially 0 and 50, but the number box will update the value of the ¯rst argument, so that, as pictured, the most recent message to leave the pack object was \206 50". The e®ect of this on the line~ object below is to ramp to 206 in 50 milliseconds; in general the output of the line~ object is an audio signal that smoothly follows the sporadically changing values of the number box labeled \squeeze".

Finally, 128 is added to the \squeeze" value; if \squeeze" takes non-negative values (as the number box in this patch enforces), the range-setting multiplier ranges the phasor by 128 or more. If the value is greater than 128, the e®ect is that the rescaled phasor spends some fraction of its cycle stuck at the end of the wavetable (which clips its input to 129). The result is that the waveform is scanned over some fraction of the cycle. As shown, the waveform is squeezed into 128/(128+206) of the cycle, so the spectrum is stretched by a factor of about 1/2.

For simplicity, this patch is subtly di®erent from the example of Section 2.4 in that the waveforms are squeezed toward the beginning of each cycle and not toward the middle. This has the e®ect of slightly changing the phase of the various partials of the waveform as it is stretched and squeezed; if the squeezing factor changes quickly, the corresponding phase drift will sound like a slight wavering in pitch. This can be avoided by using a slightly more complicated arrangement: subtract 1/2 from the phasor~, multiply it by 128 or more, and then add 65 instead of one.

Using a wavetable as a sampler

Example B04.sampler.pd (Figure 2.14) shows how to use a wavetable as a sam- pler. In this example the index into the sample (the wavetable) is controlled by mousing on a number box at top. A convenient scaling for the number box is hundredths of a second; to convert to samples (as the input of tabread4~ re- quires) we multiply by 44100 samples/sec times 0.01 sec to get 441 samples per unit, before applying pack and line~ in much the same way as they were used in the previous example. The transposition you hear depends on how quickly you mouse up and down. This example has introduced one new object class:

hip » : simple high-pass (low-cut) ¯lter. The creation argument gives the ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.084.png)roll-o®frequency in cycles per second. We use it here to eliminate the constant (zero-frequency) output when the input sits in a single sample (whenever you aren't actively changing the wavetable reading location with the mouse). Filters are discussed in Chapter 8.

The pack and line~ in this example are not included merely to make the sound more continuous, but are essential to making the sound intelligible at

0   <-- read point, 0-100![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.085.png)

* 441 convert to SAMPLES pack 0 100

  line~

  tabread4~ sample-table

  hip~ 5 high pass filter to cut DC |  

(OUT)

sample-table![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.086.png)

--- 44103 samples ---

Figure 2.14: A sampler with mouse-controlled index: B04.sampler.pd.

6. EXAMPLES

53

all. If the index into the wavetable lookup simply changed every time the mouse moved a pixel (say, twenty to ¯fty times a second) the overwhelming majority of samples would get the same index as the previous sample (the other 44000+ samples, not counting the ones where the mouse moved.) So the speed of precession would almost always be zero. Instead of changing transpositions, you would hear 20 to 50 cycles-per-second grit. (Try it to ¯nd out what that sounds like!)

Looping samplers

In most situations, you'll want a more automated way than moving the mouse to specify wavetable read locations; for instance, you might want to be able to play a sample at a steady transposition; you might have several samples playing back at once (or other things requiring attention), or you might want to switch quickly between samples or go to prearranged locations. In the next few examples we'll develop an automated looping sample reader, which, although only one of many possible approaches, is a powerful and often-used one.

Patches B05.sampler.loop.pd and B06.sampler.loop.smooth.pd show how to

do this: the former in the simplest possible way and the latter (pictured in Figure 2.15, part a) incorporating a second waveshape to envelope the sound as described in Section 2.3. One new object class is introduced here:

cos » : compute the cosine of 2¼times the input signal (so that 0 to 1 makes a![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.087.png) whole cycle). Unlike the table reading classes in Pd, cos~ handles wraparound so that there is no range limitation on its input.

In Figure 2.15 (part a), a phasor~ object supplies both indices into the wavetable (at right) and phases for a half-cosine-shaped envelope function at left. These two are multiplied, and the product is high-pass ¯ltered and output.

Reading the wavetable is straightforward; the phasor is multiplied by a \chunk size" parameter, added to 1, and used as an index to tabread4~The\_ chunk size

parameter is multiplied by 441 to convert it from hundredths of a second to samples. This corresponds exactly to the block diagram shown in Figure 2.5, with a segment location of 1. (The segment location can't be 0 because 1 is the minimum index for which tabread4~ works.)

The left-hand signal path in the example corresponds to the enveloping wavetable lookup technique shown in Figure 2.7. Here the sawtooth wave is adjusted to the range (-1/4, 1/4) (by subtracting and multiplying by 0.5), and then sent to cos~. This reads the cosine function in the range (¡¼=2, ¼=2), thus giving only the positive half of the waveform.

Part (b) of Figure 2.15 introduces a third parameter, the \read point", which speci¯es where in the sample the loop is to start. (In part (a) we always started at the beginning.) The necessary change is simple enough: add the \read point" control value, in samples, to the wavetable index and proceed as before. To avoid discontinuities in the index we smooth the read point value using pack and line~ objects, just as we did in the ¯rst sampler example (Figure 2.14).

This raises an important, though subtle, issue. The Momentary Transpo-

6. EXAMPLES



frequency (Hz.)

0  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.088.png)

chunk size
phasor~ (hundredths of a

second)

0  

* 441

-~ 0.5 \*~ 

\*~ 0.5 +~ 1

cos~ tabread4~ table18 \*~ 

hip~ 5

|  (OUT)

(a)

frequency 0  phasor~ 0

-~ 0.5![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.089.png)

\*~ 0.5 chunk size

0  

cos~

* 441

samphold~

\*~  read point +~ 1 0  

* 441

pack 0 100

line~ samphold~

+~ 

tabread4~ table20

\*~ 

hip~ 5

|  

(OUT)

(b)

6. EXAMPLES

54

Figure 2.15: (a) a looping sampler with a synchronized envelope (B06.sampler.loop.smooth.pd); (b) the same, but with a control for read lo- cation (B08.sampler.nodoppler.pd).

sition Formula (Page 33) predicts that, as long as the chunk size and read point aren't changing in time, the transposition is just the frequency times the chunk size (as always, using appropriate units; Hertz and seconds, for example, so that the product is dimensionless). However, varying the chunk size and read point in time will a®ect the momentary transposition, often in very no- ticeable ways, as can be heard in Example B07.sampler.scratch.pd. Example B08.sampler.nodoppler.pd (the one shown in the ¯gure) shows one possible way of controlling this e®ect, while introducing a new object class:

samphold » : a sample and hold unit. (This will be familiar to analog syn- thesizer![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.090.png) users, but with a digital twist; for more details see Section 3.7.) This stores a single sample of the left-hand-side input and outputs it repeatedly, until caused by the right-hand-side input (also a digital audio signal, called the trigger) to overwrite the stored sample with a new one|again from the left-hand-side input. The unit acquires a new sample whenever the trigger's numerical value falls from one sample to the next. This is designed to be easy to pair with phasor~ objects, to facilitate triggering on phase wraparounds.

Example B08.sampler.nodoppler.pd uses two samphold~ objects to update the values of the chunk size and read point, exactly when the phasor~ wraps around, at which moments the cosine envelope is at zero so the e®ect of the instantaneous changes can't be heard. In this situation we can apply the simpler Transposition Formula for Looping Wavetables to relate frequency, chunk size, and transposition. This is demonstrated in Example B09.sampler.transpose.pd (not shown).

Overlapping sample looper

As described in Section 2.3, it is sometimes desirable to use two or more over- lapping looping samplers to produce a reasonably continuous sound without having to envelope too sharply at the ends of the loop. This is especially likely in situations where the chunk that is looped is short, a tenth of a second or less. Example B10.sampler.overlap.pd, shown in Figure 2.16 (part a), realizes two looping samplers a half-cycle out of phase from each other. New object classes are:

loadbang : output a \bang" message on load. This is used in this patch to make![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.091.png) sure the division of transposition by chunk size will have a valid transpo- sition factor in case \chunk size" is moused on ¯rst.

expr : evaluate mathematical expressions. Variables appear as $f1, $f2, and so![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.092.png) on, corresponding to the object's inlets. Arithmetic operations are allowed, with parentheses for grouping, and many library functions are supplied, such as exponentiation, which shows up in this example as \pow" (the power function).

wrap » : wrap to the interval from 0 to 1. So, for instance, 1.2 becomes 0.2;![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.093.png)

0\.5 remains unchanged; and -0.6 goes to 0.4.

send » , s » , receive » , r » : signal versions of send and receive. An![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.094.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.095.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.096.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.097.png) audio signal sent to a send~ object appears at the outlets of any and all

6. EXAMPLES

55

loadbang![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.098.png)

0  <-- transposition,

(tenths of a halftone)

expr pow(2, $f1/120)

r chunk-size

t b f

/  phasor~

+~ 0.5 s~ phase wrap~

s~ phase2

(chunk size and read point controls not shown)

r chunk-size-samples samphold~ r~ phase

r~ phase

\*~  r~ read-pt r~ phase +~ 1 r~ phase -~ 0.5

+~  samphold~ \*~ 0.5 tabread4~ table22 cos~

\*~ 

+~  <- (second reader

not shown) hip~ 5

|  

(OUT)

(a)

0   <-- transposition

r chunk-size r precession t b f![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.099.png) t b f

expr (pow(2, $f1/120)-$f3)/$f2

+~ 0.5

phasor~ wrap~

s~ phase s~ phase2

0   <-- precession loadbang

(percent)

* 0.01 chunk / 0.9 s precession 1010  <-(msec)size

  phasor~ \* 0.001

  \*~ 0.9 s chunk-size s~ read-pt

  r chunk-size

  samphold~ r~ phase

  \*~  r~ phase

  +~  r~ read-pt r~ phase \*~ 44100 -~ 0.5 +~ 1 \*~ 0.5

  tabread4~ table23 cos~

  \*~ 

  +~  <- (second reader

  not shown) hip~ 5

|  

(OUT)

(b)

6. EXAMPLES

56

Figure 2.16: (a) two overlapped looping samplers (B10.sampler.overlap.pd); (b) the same, but with a phasor-controlled read point (B11.sampler.rockafella.pd).


receive~ objects of the same name. Unlike send and receive, you may not have more than one send~ object with the same name (in that connection, see the throw~ and catch~ objects).

In the example, part of the wavetable reading machinery is duplicated, using identical calculations of \chunk-size-samples" (a message stream) and \read-pt" (an audio signal smoothed as before). However, the \phase" audio signal, in the other copy, is replaced by \phase2". The top part of the ¯gure shows the calculation of the two phase signals: the ¯rst one as the output of a phasor~ object, and the second by adding 0.5 and wrapping, thereby adding 0.5 cycles (¼ radians) to the phase. The two phase signals are each used, with the same range adjustments as before, to calculate indices into the wavetable and the cos~ object, and to control the two samphold~ objects. Finally, the results of the two copies are added for output.

Automatic read point precession

Example B11.sampler.rockafella.pd, shown in part (b) of Figure 2.16, adapts the ideas shown above to a situation where the read point is computed automati- cally. Here we precess the read-point through the sample in a loop, permitting us to speed up or slow down the playback independently of the transposition.

This example addresses a weakness of the preceding one, which is that, if the relative precession speed is anywhere near one (i.e., the natural speed oflistening to the recorded wavetable), and if there is not much transposition either, it becomes preferable to use larger grains and lower the frequency of repetition accordingly (keeping the product constant to achieve the desired transposition.) However, if the grain size is allowed to get large, it is no longer convenient to quantize control changes at phase wrappings, because they might be too far apart to allow for a reasonable response time to control changes.

In this patch we remove the samphold~ object that had controlled the read point (but we leave in the one for chunk size which is much harder to change in mid-loop). Instead, we use the (known) rate of precession of the read point to correct the sawtooth frequency, so that we maintain the desired transposition.

It turns out that, when transposition factor and precession are close to each other (so that we are nearly doing the same thing as simple speed change) the frequency will drop to a value close to zero, so we will have increased the naturalness of the result at the same time.

In this patch we switch from managing read points, chunk sizes, etc., in samples and use seconds instead, converting to samples (and shifting by one) only just before the tabread4~ object. The wavetable holds one second of sound, and we'll assume here that the nominal chunk size will not exceed 0.1 second, so that we can safely let the read point range from 0 to 0.9; the \real" chunk size will vary, and can become quite large, because of the moving read pointer.

The precession control sets the frequency of a phasor of amplitude 0.9, and therefore the precession must be multiplied by 0.9 to set the frequency of the phasor (so that, for a precession of one for instance, the amplitude and fre-

2\.6. EXAMPLES 57

quency of the read point are both 0.9, so that the slope, equal to amplitude over frequency, is one). The output of this is named \read-pt" as before, and is used by both copies of the wavetable reader.

The precession p and the chunk size c being known, and if we denote the frequency of the upper (original) phasor~ by f , the transposition factor is given by:

t = p + cf

and solving for f gives:

t ¡ p 2h=12 ¡ p

f = =

c c

where h is the desired transposition in half-steps. This is the formula used in the expr object.

Exercises

1. If a wavetable with 1000 samples is played back at unit transposition, at a sample rate of 44100 Hertz, how long does the resulting sound last?
1. A one-second wavetable is played back in 0.5 seconds. By what interval is the sound transposed?
1. Still assuming a one-second wavetable, if we play it back periodically (in a loop), at how many Hertz should we loop the wavetable to transpose the original sound upward one half-step?
1. We wish to play a wavetable (recorded at R = 44100), looping ten times per second, so that the original sound stored in the wavetable is transposed up a perfect ¯fth (see Page 12). How large a segment of the wavetable, in samples, should be played back?
1. Suppose you wish to use waveform stretching on a wavetable that holds a periodic waveform of period 100. You wish to hear the untransposed spectrum at a period of 200 samples. By what duty factor should you squeeze the waveform?
1. The ¯rst half of a wavetable contains a cycle of a sinusoid of peak am- plitude one. The second half contains zeros. What is the strength of the second partial of the wavetable?
1. A sinusoid is stored in a wavetable with period 4 so that the ¯rst four elements are 0, 1, 0, and -1, corresponding to indices 0, 1, 2, and 3. What value do we get for an input of 1.5: (a) using 2-point interpolation? (b) using 4-point interpolation? (c) What's the value of the original sinusoid there?
1. If a wavetable's contents all fall between -1 and 1 in value, what is the range of possible outputs of wavetable lookup using 4-point interpolation?


Chapter 3

Audio and control computations

1. The sampling theorem

So far we have discussed digital audio signals as ifthey were capable ofdescribing any function of time, in the sense that knowing the values the function takes on the integers should somehow determine the values it takes between them. This isn't really true. For instance, suppose some function f (de¯ned for real numbers) happens to attain the value 1 at all integers:

f (n) = 1; n = :::;¡1;0;1;:::

We might guess that f (t) = 1 for all real t. But perhaps f happens to be one for integers and zero everywhere else|that's a perfectly good function too, and nothing about the function's values at the integers distinguishes it from the simpler f (t) = 1. But intuition tells us that the constant function is in the spirit of digital audio signals, whereas the one that hides a secret between the samples isn't. A function that is \possible to sample" should be one for which we can use some reasonable interpolation scheme to deduce its values on non-integers from its values on integers.

It is customary at this point in discussions of computer music to invoke the famous Nyquist theorem. This states (roughly speaking) that if a function is a ¯nite or even in¯nite combination ofsinusoids, none ofwhose angular frequencies exceeds ¼, then, theoretically at least, it is fully determined by the function's values on the integers. One possible way of reconstructing the function would be as a limit of higher- and higher-order polynomial interpolation.

The angular frequency ¼, called the Nyquist frequency, corresponds to R=2 cycles per second if R is the sample rate. The corresponding period is two samples. The Nyquist frequency is the best we can do in the sense that any real sinusoid of higher frequency is equal, at the integers, to one whose fre- quency is lower than the Nyquist, and it is this lower frequency that will get

59

0   7  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.100.png)

Figure 3.1: Two real sinusoids, with angular frequencies ¼=2 and 3¼=2, showing that they coincide at integers. A digital audio signal can't distinguish between the two.

reconstructed by the ideal interpolation process. For instance, a sinusoid with angular frequency between ¼and 2¼, say ¼+ !, can be written as

cos((¼+ !)n + Á) = cos((¼+ !)n + Á¡ 2¼n)

- cos((! ¡ ¼)n + Á)
- cos((¼¡ !)n ¡ Á)

for all integers n. (If n weren't an integer the ¯rst step would fail.) So a sinusoid with frequency between ¼and 2¼is equal, on the integers at least, to one with frequency between 0 and ¼; you simply can't tell the two apart. And since any conversion hardware should do the \right" thing and reconstruct the lower- frequency sinusoid, any higher-frequency one you try to synthesize will come out your speakers at the wrong frequency|speci¯cally, you will hear the unique frequency between 0 and ¼ that the higher frequency lands on when reduced in the above way. This phenomenon is called foldover, because the half-line of frequencies from 0 to 1 is folded back and forth, in lengths of ¼, onto the interval from 0 to ¼. The word aliasing means the same thing. Figure 3.1 shows that sinusoids of angular frequencies ¼=2 and 3¼=2, for instance, can't be distinguished as digital audio signals.

We conclude that when, for instance, we're computing values of a Fourier series (Page 12), either as a wavetable or as a real-time signal, we had better leave out any sinusoid in the sum whose frequency exceeds ¼. But the picture in general is not this simple, since most techniques other than additive synthesis don't lead to neat, band-limited signals (ones whose components stop at some limited frequency). For example, a sawtooth wave of frequency !, of the form put out by Pd's phasor~ object but considered as a continuous function f (t), expands to:

µ ¶

1  1 sin(2!t) sin(3!t)

f (t) = ¡ sin(!t) +~~ +~~ + ¢¢¢

2  ¼ 2 3

which enjoys arbitrarily high frequencies; and moreover the hundredth partial is only 40 dB weaker than the ¯rst one. At any but very low values of !,

3\.2. CONTROL 61

the partials above ¼ will be audibly present|and, because of foldover, they will be heard at incorrect frequencies. (This does not mean that one shouldn't use sawtooth waves as phase generators|the wavetable lookup step magically corrects the sawtooth's foldover|but one should think twice before using a sawtooth wave itself as a digital sound source.)

Many synthesis techniques, even if not strictly band-limited, give partials which may be made to drop o® more rapidly than 1=n as in the sawtooth example, and are thus more forgiving to work with digitally. In any case, it is always a good idea to keep the possibility of foldover in mind, and to train your ears to recognize it.

The ¯rst line of defense against foldover is simply to use high sample rates; it is a good practice to systematically use the highest sample rate that your computer can easily handle. The highest practical rate will vary according to whether you are working in real time or not, CPU time and memory constraints, and/or input and output hardware, and sometimes even software-imposed lim- itations.

A very non-technical treatment of sampling theory is given in [Bal03]. More detail can be found in [Mat69, pp. 1-30].

2. Control

So far we have dealt with audio signals, which are just sequences x[n] de¯ned for integers n, which correspond to regularly spaced points in time. This is often an adequate framework for describing synthesis techniques, but real elec- tronic music applications usually also entail other computations which have to be made at irregular points in time. In this section we'll develop a framework for describing what we will call control computations. We will always require that any computation correspond to a speci¯c logical time. The logical time controls which sample of audio output will be the ¯rst to re°ect the result of the computation.

In a non-real-time system (such as Csound in its classical form), this means that logical time proceeds from zero to the length of the output sound¯le. Each \score card" has an associated logical time (the time in the score), and is acted upon once the audio computation has reached that time. So audio and control calculations (grinding out the samples and handling note cards) are each handled in turn, all in increasing order of logical time.

In a real-time system, logical time, which still corresponds to the time of the next a®ected sample of audio output, is always slightly in advance of real time, which is measured by the sample that is actually leaving the computer. Control and audio computations still are carried out in alternation, sorted by logical time.

The reason for using logical time and not real time in computer music com- putations is to keep the calculations independent of the actual execution time of the computer, which can vary for a variety of reasons, even for two seemingly identical calculations. When we are calculating a new value of an audio signal

3. CONTROL STREAMS 65

audio output![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.101.png)

1) 0   1   2  
- . . control![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.102.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.103.png)

0   1  1   2  2   3   audio

logical time

2) 0   1   2   3   4   5   6   7  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.104.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.105.png)
- . .

0   4   4   8   8  

Figure 3.2: Timeline for digital audio and control computation: (a) with a block size of one sample; (b) with a block size of four samples.

or processing some control input, real time may pass but we require that the logical time stay the same through the whole calculation, as if it took place instantaneously. As a result of this, electronic music computations, if done cor- rectly, are deterministic: two runs of the same real-time or non-real-time audio computation, each having the same inputs, should have identical results.

Figure 3.2 (part a) shows schematically how logical time and sample com- putation are lined up. Audio samples are computed at regular periods (marked as wavy lines), but before the calculation of each sample we do all the control calculations that might a®ect it (marked as straight line segments). First we do the control computations associated with logical times starting at zero, up to but not including one; then we compute the ¯rst audio sample (of index zero), at logical time one. We then do all control calculations up to but not including logical time 2, then the sample of index one, and so on. (Here we are adopt- ing certain conventions about labeling that could be chosen di®erently. For instance, there is no fundamental reason control should be pictured as coming \before" audio computation but it is easier to think that way.)

Part (b) of the ¯gure shows the situation if we wish to compute the audio output in blocks of more than one sample at a time. Using the variable B to denote the number of elements in a block (so B = 4 in the ¯gure), the ¯rst audio computation will output samples 0;1;:::B ¡ 1 all at once in a block computed at logical time B. We have to do the relevant control computations for all B periods of time in advance. There is a delay of B samples between logical time and the appearance of audio output.

Most computer music software computes audio in blocks. This is done to increase the e±ciency of individual audio operations (such as Csound's unit

time![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.106.png)

Figure 3.3: Graphical representation of a control stream as a sequence of points in time.

generators and Max/MSP and Pd's tilde objects). Each unit generator or tilde object incurs overhead each time it is called, equal to perhaps twenty times the cost of computing one sample on average. If the block size is one, this means an overhead of 2,000%; if it is sixty-four (as in Pd by default), the overhead is only some 30%.

3. Control streams

Control computations may come from a variety of sources, both internal and external to the overall computation. Examples of internally engendered con- trol computations include sequencing (in which control computations must take place at pre-determined times) or feature detection of the audio output (for instance, watching for zero crossings in a signal). Externally engendered ones may come from input devices such as MIDI controllers, the mouse and keyboard, network packets, and so on. In any case, control computations may occur at irregular intervals, unlike audio samples which correspond to a steadily ticking sample clock.

We will need a way of describing how information °ows between control and audio computations, which we will base on the notion of a control stream. This is simply a collection of numbers|possibly empty|that appear as a re- sult of control computations, whether regularly or irregularly spaced in logical time. The simplest possible control stream has no information other than a time sequence:

:::;t[0];t[1];t[2];:::

Although the time values are best given in units of samples, their values aren't quantized; they may be arbitrary real numbers. We do require them to be sorted in nondecreasing order:

¢¢¢· t[0]· t[1]· t[2]· ¢¢¢

Each item in the sequence is called an event.

Control streams may be shown graphically as in Figure 3.3. A number line shows time and a sequence of arrows points to the times associated with each event. The control stream shown has no data (it is a time sequence). If we want to show data in the control stream we will write it at the base of each arrow.

A numeric control stream is one that contains one number per time point, so that it appears as a sequence of ordered pairs:

:::; (t[0];x[0]); (t[1];x[1]); :::

where the t[n] are the time points and the x[n] are the signal's values at those times.

A numeric control stream is roughly analogous to a \MIDI controller", whose values change irregularly, for example when a physical control is moved by a performer. Other control stream sources may have higher possible rates of change and/or more precision. On the other hand, a time sequence might be a sequence of pedal hits, which (MIDI implementation notwithstanding) shouldn't be considered as having values, just times.

Numeric control streams are like audio signals in that both are just time- varying numeric values. But whereas the audio signal comes at a steady rate (and so the time values need not be speci¯ed per sample), the control stream comes unpredictably|perhaps evenly, perhaps unevenly, perhaps never.

Let us now look at what happens when we try to convert a numeric control stream to an audio signal. As before we'll choose a block size B = 4. We will consider as a control stream a square wave of period 5.5:

(2;1);(4:75;0);(7:5;1);(10:25;0);(13;1);:::

and demonstrate three ways it could be converted to an audio signal. Figure

4. (part a) shows the simplest, fast-as-possible, conversion. Each audio sample of output simply re°ects the most recent value of the control signal. So samples 0 through 3 (which are computed at logical time 4 because of the block size) are 1 in value because of the point (2, 1). The next four samples are also one, because of the two points, (4.75, 0) and (7.5, 1), the most recent still has the value 1.

   Fast-as-possible conversion is most appropriate for control streams which do not change frequently compared to the block size. Its main advantages are simplicity of computation and the fastest possible response to changes. As the ¯gure shows, when the control stream's updates are too fast (on the order of the block size), the audio signal may not be a good likeness of the sporadic one. (If, as in this case, the control stream comes at regular intervals of time, we can use the sampling theorem to analyze the result. Here the Nyquist frequency associated with the block rate R=B is lower than the input square wave's fre- quency, and so the output is aliased to a new frequency lower than the Nyquist frequency.)

   Part (b) shows the result of nearest-sample conversion. Each new value of the control stream at a time t a®ects output samples starting from index btc (the greatest integer not exceeding t). This is equivalent to using fast-as-possible conversion at a block size of 1; in other words, nearest-sample conversion hides the e®ect of the larger block size. This is better than fast-as-possible conversion in cases where the control stream might change quickly.

a   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.107.png)

0  1  2  3  4   8   12  16 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.108.png)

- . .

0   4   8   12  16 

(2, 1) (7.5, 1) (13, 1) (18.5, 1)

(4.75, 0) (10.25, 0) (15.75, 0)

b   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.109.png)

0  1  2  3  4   8   12  16 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.110.png)

- . .

0   4   8   12  16 

c   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.111.png)

0  1  2  3  4   8   12  16 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.112.png)

- . .

0   4   8   12  16 

Figure 3.4: Three ways to change a control stream into an audio signal: (a) as fast as possible; (b) delayed to the nearest sample; (c) with two-point interpo- lation for higher delay accuracy.


Part (c) shows sporadic-to-audio conversion, again at the nearest sample, but now also using two-point interpolation to further increase the time accuracy. Conceptually we can describe this as follows. Suppose the value of the control stream was last equal to x, and that the next point is (n + f;y), where n is an integer and f is the fractional part of the time value (so 0 · f < 1). The ¯rst point a®ected in the audio output will be the sample at index n. But instead of setting the output to y as before, we set it to

f x + (1 ¡ f )y;

in other words, to a weighted average of the previous and the new value, whose weights favor the new value more if the time of the sporadic value is earlier, closer to n. In the example shown, the transition from 0 to 1 at time 2 gives

0 ¢x + 1 ¢y = 1; while the transition from 1 to 0 at time 4.75 gives:

0:75 ¢x + 0:25 ¢y = 0:75:

This technique gives a still closer representation of the control signal (at least, the portion of it that lies below the Nyquist frequency), at the expense of more computation and slightly greater delay.

Numeric control streams may also be converted to audio signals using ramp functions to smooth discontinuities. This is often used when a control stream is used to control an amplitude, as described in Section 1.5. In general there are three values to specify to set a ramp function in motion: a start time and target value (speci¯ed by the control stream) and a target time, often expressed as a delay after the start time.

In such situations it is almost always accurate enough to adjust the start and ending times to match the ¯rst audio sample computed at a later logical time, a choice which corresponds to the fast-as-possible scenario above. Figure

5. (part a) shows the e®ect of ramping from 0, starting at time 3, to a value of 1 at time 9, immediately starting back toward 0 at time 15, with block size B = 4. The times 3, 9, and 15 are truncated to 0, 8, and 12, respectively.

   In real situations the block size might be on the order of a millisecond, and adjusting ramp endpoints to block boundaries works ¯ne for controlling amplitudes; reaching a target a fraction of a millisecond early or late rarely makes an audible di®erence. However, other uses of ramps are more sensitive to time quantization of endpoints. For example, if we wish to do something repetitively every few milliseconds, the variation in segment lengths will make for an audible aperiodicity.

   For situations such as these, we can improve the ramp generation algorithm to start and stop at arbitrary samples, as shown in Figure 3.5 (part b), for example. Here the endpoints of the line segments line up exactly with the requested samples 3, 9, and 15. We can go even further and adjust for fractional samples, making the line segments touch the values 0 and 1 at exactly speci¯able points on a number line.

3\.4. CONVERTING FROM AUDIO SIGNALS TO NUMERIC CONTROL STREAMS67

a   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.113.png)

0   4   8   12 

b   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.114.png)

3   9   15 

- . .![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.115.png)

3   9   15 

Figure 3.5: Line segment smoothing of numeric control streams: (a) aligned to block boundaries; (b) aligned to nearest sample.

For example, suppose we want to repeat a recorded sound out of a wavetable 100 times per second, every 441 samples at the usual sample rate. Rounding errors due to blocking at 64-sample boundaries could detune the playback by as much as a whole tone in pitch; and even rounding to one-sample boundaries could introduce variations up to about 0.2%, or three cents. This situation would call for sub-sample accuracy in sporadic-to-audio conversion.

4. Converting from audio signals to numeric control streams

We sometimes need to convert in the other direction, from an audio signal to a sporadic one. To go in this direction, we somehow provide a series of logical times (a time sequence), as well as an audio signal. For output we want a control stream combining the time sequence with values taken from the audio signal. We do this when we want to incorporate the signal's value as part of a control computation.

For example, we might be controlling the amplitude of a signal using a line~ object as in Example A03.line.pd (Page 21). Suppose we wish to turn o®the sound at a ¯xed rate of speed instead of in a ¯xed amount of time. For instance, we might want to re-use the network for another sound and wish to mute it as quickly as possible without audible artifacts; we probably can ramp it o® in less time if the current amplitude is low than if it is high. To do this we must confect a message to the line~ object to send it to zero in an amount of time we'll calculate on the basis of its current output value. This will require, ¯rst of all, that we \sample" the line~ object's output (an audio signal) into a control stream.

The same issues of time delay and accuracy appear as for sporadic to audio conversion. Again there will be a tradeo® between immediacy and accuracy.

trigger![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.116.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.117.png)

signal snapshot

1) (b)

Figure 3.6: Conversion between control and audio: (a) control to signal; (b) signal to control by snapshots.

Suppose as before that we are calculating audio in blocks of 4 samples, and suppose that at logical time 6 we want to look at the value of an audio signal, and use it to change the value of another one. As shown in Figure 3.2 (part b), the most recently calculated value of the signal will be for index 3 and the earliest index at which our calculation can a®ect a signal is 4. We can therefore carry out the whole a®air with a delay of only one sample. However, we can't choose exactly which sample|the update can occur only at a block boundary.

As before, we can trade immediacy for increased time accuracy. If it matters exactly at which sample we carry out the audio-to-control-to-audio computation, we read the sample of index 2 and update the one at index 6. Then if we want to do the same thing again at logical time 7, we read from index 3 and update at index 7, and so on. In general, if the block size is B, and for any index n, we can always read the sample at index n ¡ B and a®ect the one at index n. There is thus a round-trip delay of B samples in going from audio to control to audio computation, which is the price incurred for being able to name the index n exactly.

If we wish to go further, to being able to specify a fraction of a sample, then (as before) we can use interpolation|at a slight further increase in delay. In general, as in the case of sporadic-to-audio conversion, in most cases the simplest solution is the best, but occasionally we have to do extra work.

5. Control streams in block diagrams

Figure 3.6 shows how control streams are expressed in block diagrams, using control-to-signal and signal-to-control conversion as examples. Control streams are represented using dots (as opposed to audio signals which appear as solid arrows).

The signal block converts from a numeric control stream to an audio signal. The exact type of conversion isn't speci¯ed at this level of detail; in the Pd

3\.6. EVENT DETECTION 69 examples the choice of conversion operator will determine this.

The snapshot block converts from audio signals back to numeric control streams. In addition to the audio signal, a separate, control input is needed to specify the time sequence at which the audio signal is sampled.

6. Event detection

Besides taking snapshots, a second mode of passing information from audio sig- nals to control computations is event detection. Here we derive time information from the audio signal. An example is threshold detection, in which the input is an audio signal and the output is a time sequence. We'll consider the example of threshold detection in some detail here.

A typical reason to use threshold detection is to ¯nd out when some kind of activity starts and stops, such as a performer playing an instrument. We'll suppose we already have a continuous measure of activity in the form of an audio signal. (This can be done, for example, using an envelope follower). What we want is a pair of time sequences, one which marks times in which activity starts, and the other marking stops.

Figure 3.7 (part a) shows a simple realization of this idea. We assume the signal input is as shown in the continuous graph. A horizontal line shows the constant value of the threshold. The time sequence marked \onsets" contains one event for each time the signal crosses the threshold from below to above; the one marked \turno®s" marks crossings in the other direction.

In many situations we will get undesirable onsets and turno®s caused by small ripples in the signal close to the threshold. This is avoided by debouncing, which can be done in at least two simple ways. First, as shown in part (b) of the ¯gure, we can set two thresholds: a high one for marking onsets, and a lower one for turno®s. In this scheme the rule is that we only report the ¯rst onset after each turno®, and, vice versa, we only report one turno® after each onset. Thus the third time the signal crosses the high threshold in the ¯gure, there is no reported onset because there was no turno® since the previous one. (At startup, we act as if the most recent output was a turno®, so that the ¯rst onset is reported.)

A second approach to ¯ltering out multiple onsets and turno®s, shown in part

(c) of the ¯gure, is to associate a dead period to each onset. This is a constant interval of time after each reported onset, during which we refuse to report more onsets or turno®s. After the period ends, if the signal has dropped below the threshold in the meantime, we belatedly report a turno®. Dead periods may also be associated with turno®s, and the two time periods may have di®erent values.

The two ¯ltering strategies may be used separately or simultaneously. It is usually necessary to tailor the threshold values and/or dead times by hand to each speci¯c situation in which thresholding is used.

Thresholding is often used as a ¯rst step in the design of higher-level strate- gies for arranging computer responses to audible cues from performers. A simple

7. AUDIO SIGNALS AS CONTROL 73

onsets![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.118.png)

threshold (a)

turnoffs

time

2) high threshold low threshold![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.119.png)

(c) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.120.png)

dead periods

Figure 3.7: Threshold detection: (a) with no debouncing; (b) debounced using two threshold levels; (c) debounced using dead periods.

example could be to set o®a sequence of pre-planned processes, each one to be set o®by an onset of sound after a speci¯ed period of relative silence, such as you would see if a musician played a sequence of phrases separated by rests.

More sophisticated detectors (built on top of threshold detection) could de- tect continuous sound or silence within an expected range of durations, or se- quences of quick alternation between playing and not playing, or periods of time in which the percentage of playing time to rests is above or below a threshold, or many other possible features. These could set o®predetermined reactions or ¯gure in an improvisation.

7. Audio signals as control

From the tradition of analog synthesis comes an elegant, old-fashioned approach to control problems that can be used as an alternative to the control streams we have been concerned with so far in this chapter. Instead, or in addition to using control streams, we can use audio signals themselves to control the production of other audio signals. Two speci¯c techniques from analog synthesis lend themselves well to this treatment: analog sequencing and sample-and-hold.

The analog sequencer [Str95, pp. 70-79] [Cha80, pp. 93,304-308] was often used to set o®a regularly or semi-regularly repeating sequence of sounds. The sequencer itself typically put out a repeating sequence of voltages, along with a trigger signal which pulsed at each transition between voltages. One used the voltages for pitches or timbral parameters, and the trigger to control one or more envelope generators. Getting looped sequences of predetermined values in digital audio practice is as simple as sending a phasor~ object into a non- interpolating table lookup. If you want, say, four values in the sequence, scale the phasor~ output to take values from 0 to 3:999::: so that the ¯rst fourth of the cycle reads point 0 of the table and so on.

To get repeated triggering, the ¯rst step is to synthesize another sawtooth that runs in synchrony with the phasor~ output but four times as fast. This is done using a variant of the technique of Figure 2.8, in which we used an adder and a wraparound operator to get a desired phase shift. Figure 3.8 shows the e®ect of multiplying a sawtooth wave by an integer, then wrapping around to get a sawtooth at a multiple of the original frequency.

From there is is easy to get to a repeated envelope shape by wavetable lookup for example (using an interpolating table lookup this time, unlike the sequence voltages). All the waveform generation and altering techniques used for making pitched sounds can also be brought to use here.

The other standard control technique from analog synthesizer control is the sample and hold unit [Str95, pp. 80-83] [Cha80, p. 92]. This takes an incoming signal, picks out certain instantaneous values from it, and \freezes" those values for its output. The particular values to pick out are selected by a secondary, \trigger" input. At points in time speci¯ed by the trigger input a new, single value is taken from the primary input and is output continuously until the next time point, when it is replaced by a new value of the primary input.

1  frequency![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.121.png) 4  

1  

0  

* 4  

WRAP

OUT 1  

Figure 3.8: Multiplying and wrapping a sawtooth wave to generate a higher frequency.

IN ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.122.png)

trigger

S/H

OUT

Figure 3.9: Sample and hold (\S/H"), using falling edges of the trigger signal.


In digital audio it is often useful to sample a new value on falling edges of the trigger signal, i.e., whenever the current value ofthe trigger signal is smaller than its previous value, as shown in Figure 3.9. This is especially convenient for use with a sawtooth trigger, when we wish to sample signals in synchrony with an oscillator-driven process. Pd's sample and hold object was previously introduced in the context of sampling (Example B08.sampler.nodoppler.pd, Page 53).

8. Operations on control streams

So far we've discussed how to convert between control streams and audio streams. In addition to this possibility, there are four types of operations you can per- form on control streams to get other control streams. These control stream operations have no corresponding operations on audio signals. Their existence explains in large part why it is useful to introduce a whole control structure in parallel with that of audio signals.

The ¯rst type consists of delay operations, which o®set the time values associated with a control stream. In real-time systems the delays can't be negative in value. A control stream may be delayed by a constant amount, or alternatively, you can delay each event separately by di®erent amounts.

Two di®erent types of delay are used in practice: simple and compound. Examples of each are shown in Figure 3.10. A simple delay acting on a control stream schedules each event, as it comes in, for a time in the future. However, if another event arrives at the input before the ¯rst event is output, the ¯rst event is forgotten in favor of the second. In a compound delay, each event at the input produces an output, even if other inputs arrive before the output appears.

A second operation on control steams is merging: taking two control streams and combining all the events into a new one. Figure 3.11 (part a) shows how this and the remaining operations are represented in block diagrams.

Part (b) of the ¯gure shows the e®ect of merging two streams. Streams may contain more than one event at the same time. If two streams to be merged contain events at the same time, the merged stream contains them both, in a well-de¯ned order.

A third type of operation on control streams is pruning. Pruning a control stream means looking at the associated data and letting only certain elements through. Part (c) shows an example, in which events (which each have an associated number) are passed through only if the number is positive.

Finally, there is the concept ofresynchronizing one control stream to another, as shown in part (d). Here one control stream (the source) contributes values which are put onto the time sequence of a second one (the sync). The value given the output is always the most recent one from the source stream. Note that any event from the source may appear more than once (as suggested in the ¯gure), or, on the other hand, it might not appear at all.

Again, we have to consider what happens when the two streams each contain an event at the same time. Should the sync even be considered as happening before the source (so that the output gets the value ofthe previous source event)?

8. OPERATIONS ON CONTROL STREAMS 75

in  delay time delay![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.123.png) (a)

out

time

(input)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.124.png)

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.125.png) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.126.png) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.127.png)

(b) (c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.128.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.129.png)

Figure 3.10: Delay as an operation on a control stream: (a) block diagram; (b) e®ect of a simple delay on a control stream; (c) e®ect of a compound delay.

sync data merge![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.130.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.131.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.132.png) prune resync

(a)

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.133.png)

1   -2  3   -4  (c) 1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.134.png) 3  

1   3  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.135.png)

(d)

1  1   3  

Figure 3.11: Operations on control streams (besides delay): (a) block diagrams; (b) merging; (c) pruning; (d) resynchronizing.

9. CONTROL OPERATIONS IN PD 77 0 0![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.136.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.137.png)

0

delay (a)

0  (b)

0 0 0 0 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.138.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.139.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.140.png)moses select (c) float (d) 0 0

Figure 3.12: The four control operations in Pd: (a) delay; (b) merging; (c) pruning; (d) resynchronizing.

Or should the source event be considered as being ¯rst so that its value goes to the output at the same time? How this should be disambiguated is a design question, to which various software environments take various approaches. (In Pd it is controlled explicitly by the user.)

9. Control operations in Pd

So far we have used Pd mostly for processing audio signals, although as early as Figure 1.10 we have had to make the distinction between Pd's notion of audio signals and of control streams: thin connections carry control streams and thick ones carry audio. Control streams in Pd appear as sequences of messages. The messages may contain data (most often, one or more numbers), or not. A numeric control stream (Section 3.3) appears as a (thin) connection that carries numbers as messages.

Messages not containing data make up time sequences. So that you can see messages with no data, in Pd they are given the (arbitrary) symbol \bang".

The four types of control operations described in the previous section can be expressed in Pd as shown in Figure 3.12. Delays are accomplished using two explicit delay objects:

del , delay : simple delay. You can specify the delay time in a creation![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.141.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.142.png)

argument or via the right inlet. A \bang" in the left inlet sets the delay, which then outputs \bang" after the speci¯ed delay in milliseconds. The delay is simple in the sense that sending a bang to an already set delay resets it to a new output time, canceling the previously scheduled one.

pipe : compound delay. Messages coming in the left inlet appear on the![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.143.png)

10. EXAMPLES 81

output after the speci¯ed delay, which is set by the ¯rst creation argument. If there are more creation arguments, they specify one or more inlets for numeric or symbolic data the messages will contain. Any number of messages may be stored by pipe simultaneously, and messages may be reordered as they are output depending on the various delay times given for them.

Merging of control streams in Pd is accomplished not by explicit objects but by Pd's connection mechanism itself. This is shown in part (b) of the ¯gure with number boxes as an example. In general, whenever more than one connection is made to a control inlet, the control streams are merged.

Pd o®ersseveral objects for pruning control streams, of which two are shown in part (c) of the ¯gure:

moses : prune for numeric range. Numeric messages coming in the left inlet ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.144.png)appear on the left output if they are smaller than a threshold value (set by a creation argument or by the right inlet), and out the right inlet otherwise.

select , sel : prune for speci¯c numbers. Numeric messages coming in the![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.145.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.146.png)

left inlet produce a \bang" on the output only if they match a test value exactly. The test value is set either by creation argument or from the right inlet.

Finally, Pd takes care of resynchronizing control streams implicitly in its connection mechanism, as illustrated by part (d) of the ¯gure. Most objects with more than one inlet synchronize all other inlets to the leftmost one. So the float object shown in the ¯gure resynchronizes its right-hand-side inlet (which takes numbers) to its left-hand-side one. Sending a \bang" to the left inlet outputs the most recent number float has received beforehand.

10. Examples

Sampling and foldover

Example C01.nyquist.pd (Figure 3.13, part a) shows an oscillator playing a wavetable, sweeping through frequencies from 500 to 1423. The wavetable con- sists of only the 46th partial, which therefore varies from 23000 to 65458 Hertz. At a sample rate of 44100 these two frequencies theoretically sound at 21100 and 21358 Hertz, but sweeping from one to the other folds down through zero and back up.

Two other waveforms are provided to show the interesting e®ects of beat- ing between partials which, although they \should" have been far apart, ¯nd themselves neighbors through foldover. For instance, at 1423 Hertz, the second harmonic is 2846 Hertz whereas the 33rd harmonic sounds at 1423\*33-44100 = 2859 Hertz|a rude dissonance.

Other less extreme examples can still produce audible foldover in less strik- ing forms. Usually it is still objectionable and it is worth learning to hear it. Example C02.sawtooth-foldover.pd (not pictured here) demonstrates this for a sawtooth (the phasor~ object). For wavetables holding audio recordings, inter- polation error can create extra foldover. The e®ects of this can vary widely; the

500, 1423 4000![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.147.png)

line~

tabosc4~ table24 (OUT)

table24![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.148.png)

(a)

pd metro![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.149.png)

1 300 0 300

pd metro![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.150.png)

line line~ 1 2 0 2

osc~ 880

line~ vline~

\*~  \*~ 

output~ output~ output~ output~ dB0 dB0 dB0 dB0 mute mute mute mute

(b) (c)

Figure 3.13: (a) sending an oscillator over the Nyquist frequency; (b) zipper noise from the line (control) object; (c) the line~ and vline~ objects com- pared.

sound is sometimes described as \crunchy" or \splattering", depending on the recording, the transposition, and the interpolation algorithm.

Converting controls to signals

Example C03.zipper.noise.pd (Figure 3.13, part b) demonstrates the e®ect of converting a slowly-updated control stream to an audio signal. This introduces a new object:

line : a ramp generator with control output. Like line~, line takes pairs of ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.151.png)numbers as (target, time) pairs and ramps to the target in the given amount of time; however, unlike line~, the output is a numeric control stream, appearing, by default, at 20 msec time intervals.

In the example you can compare the sound of the rising and falling amplitude controlled by the line output with one controlled by the audio signal generated by line~.

The output of line is converted to an audio signal at the input of the \*~ object. The conversion is implied here by connecting a numeric control stream into a signal inlet. In Pd, implicit conversions from numeric control streams to audio streams is done in the fast-as-possible mode shown in Figure 3.4 (part a). The line output becomes a staircase signal with 50 steps per second. The result is commonly called \zipper noise".

Whereas the limitations of the line object for generating audio signals were clearly audible even over such long time periods as 300 msec, the signal variant, line~, does not yield audible problems until the time periods involved become much shorter. Example C04.control.to.signal.pd (Figure 3.13, part c) demon- strates the e®ect of using line~ to generate a 250 Hertz triangle wave. Here the e®ects shown in Figure 3.5 come into play. Since line~ always aligns line segments to block boundaries, the exact durations of line segments vary, and in this example the variation (on the order of a millisecond) is a signi¯cant fraction of their length.

A more precise object (and a more expensive one, in terms of computation time) is provided for these situations:

vline » : exact line segment generator. This third member of the \line" family outputs![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.152.png) an audio signal (like line~), but aligns the endpoints of the signal to the desired time points, accurate to a fraction of a sample. (The accuracy is limited only by the °oating-point numerical format used by Pd.) Further, many line segments may be speci¯ed withing a single audio block; vline~ can generate waveforms at periods down to two samples (beyond which you will just get foldover instead).

The vline~ object can also be used for converting numeric control streams to audio streams in the nearest-sample and two-point-interpolation modes as shown in Figure 3.4 (parts b and c). To get nearest-sample conversion, simply give vline~ a ramp time of zero. For linear interpolation, give it a ramp time of one sample (0.0227 msec if the sample rate is 44100 Hertz).

bang <-- play the sample![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.153.png)

- cut the cutoff 0 5 sound off

Wait for the delay 5 cutoff to finish

- set the upper line~ to start phase 1, 4.41e+08 1e+07; at the first sample and play cutoff 1 forever (or until next trigger)

start new playback

10. EXAMPLES 

r phase![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.154.png)

vline~ tabread4~ tab28

r cutoff \*~  vline~

|  

(OUT)

<-- record

adc~ 1 del 3990 hip~ 5![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.155.png) 0 10

0, 1 5

line~ \*~ 

tabwrite~ tab28

10. EXAMPLES 87

Figure 3.14: Non-looping sampler.

Non-looping wavetable player

One application area requiring careful attention to the control stream/audio signal boundary is sampling. Until now our samplers have skirted the issue by looping perpetually. This allows for a rich variety of sound that can be accessed by making continuous changes in parameters such as loop size and envelope shape. However, many uses of sampling require the internal features of a wavetable to emerge at predictable, synchronizable moments in time. For example, recorded percussion sounds are usually played from the beginning, are not often looped, and are usually played in a determined time relationship with the rest of the music.

In this situation, control streams are better adapted than audio signals as triggers. Example C05.sampler.oneshot.pd (Figure 3.14) shows one possible way to accomplish this. The four tilde objects at bottom left form the signal processing network for playback. One vline~ object generates a phase signal (actually just a table lookup index) to the tabread4~ object; this replaces the phasor~ of Example B03.tabread4.pd (Page 49) and its derivatives.

The amplitude of the output of tabread4~ is controlled by a second vline~

object, in order to prevent discontinuities in the output in case a new event is started while the previous event is still playing. The \cuto®" vline~ object ramps the output down to zero (whether or not it is playing) so that, once the output is zero, the index of the wavetable may be changed discontinuously.

In order to start a new \note", ¯rst, the \cuto®" vline~ object is ramped to zero; then, after a delay of 5 msec (at which point vline~ has reached zero) the phase is reset. This is done with two messages: ¯rst, the phase is set to 1 (with no time value so that it jumps to 1 with no ramping). The value \1" speci¯es the ¯rst readable point of the wavetable, since we are using 4-point interpolation. Second, in the same message box, the phase is ramped to 441,000,000 over a time period of 10,000,000 msec. (In Pd, large numbers are shown using exponential notation; these two appear as 4.41e+08 and 1e+07.) The quotient is 44.1 (in units per millisecond) giving a transposition of one. The upper vline~ object (which generates the phase) receives these messages via the \r phase" object above it.

The example assumes that the wavetable is ramped smoothly to zero at ei- ther end, and the bottom right portion of the patch shows how to record such a wavetable (in this case four seconds long). Here a regular (and computationally cheaper) line~ object su±ces. Although the wavetable should be at least 4 sec- onds long for this to work, you may record shorter wavetables simply by cutting the line~ object o®earlier. The only caveat is that, if you are simultaneously reading and writing from the same wavetable, you should avoid situations where read and write operations attack the same portion of the wavetable at once.

The vline~ objects surrounding the tabread4~ were chosen over line~ be- cause the latter's rounding of breakpoints to the nearest block boundary (typi- cally 1.45 msec) can make for audible aperiodicities in the sound if the wavetable is repeated more than 10 or 20 times per second, and would prevent you from getting a nice, periodic sound at higher rates of repetition.

We will return to vline~-based sampling in the next chapter, to add trans- position, envelopes, and polyphony.

Signals to controls

Example C06.signal.to.control.pd (not pictured) demonstrates conversion from audio signals back to numeric control streams, via a new tilde object introduced here.

snapshot » : convert audio signal to control messages. This always gives the most![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.156.png) recently computed audio sample (fast-as-possible conversion), so the exact sampling time varies by up to one audio block.

It is frequently desirable to sense the audio signal's amplitude rather than peek at a single sample; Example C07.envelope.follower.pd (also not pictured) introduces another object which does this:

env » : RMS envelope follower. Outputs control messages giving the short- term![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.157.png) RMS amplitude (in decibels) of the incoming audio signal. A creation

argument allows you to select the number of samples used in the RMS compu- tation; smaller numbers give faster (and possibly less stable) output.

Analog-style sequencer

Example C08.analog.sequencer.pd (Figure 3.15) realizes the analog sequencer and envelope generation described in Section 3.7. The \sequence" table, with nine elements, holds a sequence of frequencies. The phasor~ object at top cycles through the sequence table at 0.6 Hertz. Non-interpolating table lookup (tabread~ instead of tabread4~) is used to read the frequencies in discrete steps. (Such situations, in which we prefer non-interpolating table lookup, are rare.)

The wrap~ object converts the amplitude-9 sawtooth to a unit-amplitude one as described earlier in Figure 3.8, which is then used to obtain an envelope function from a second wavetable. This is used to control grain size in a looping sampler (from Section 2.6). Here the wavetable consists of six periods of a sinusoid. The grains are smoothed by multiplying by a raised cosine function (cos~ and + 1).

Example C09.sample.hold.pd (not pictured here) shows a sample-and-hold unit, another useful device for doing control tasks in the audio signal domain.

MIDI-style synthesizer

Example C10.monophonic.synth.pd (Figure 3.16) also implements a monophonic, note-oriented synthesizer, but in this case oriented toward MIDI controllability. Here the tasks of envelope generation and sequencing pitches are handled using control streams instead of audio signals. New control objects are needed for this example:

notein : MIDI note input. Three outlets give the pitch, velocity, and channel of![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.158.png) incoming MIDI note-on and note-o® events (with note-o® events appearing as velocity-zero note-on events). The outputs appear in Pd's customary right- to-left order.

stripnote : ¯lter out note-o® messages. This passes (pitch, velocity) pairs through![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.159.png) whenever the velocity is nonzero, dropping the others. Unlike notein, stripnote does not directly use hardware MIDI input or output.

trigger , t : copy a message to outlets in right to left order, with type con-![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.160.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.161.png)

version. The creation arguments (\b" and \f" in this example) specify two outlets, one giving \bang" messages, the other \°oat" (i.e., numbers). One out- let is created for each creation argument. The outputs appear in Pd's standard right-to-left order.

The patch's control objects feed frequencies to the phasor~ object whenever a MIDI note-on message is received. Controlling the amplitude (via the line~ object) is more di±cult. When a note-on message is received, the sel 0 object outputs the velocity at right (because the input failed to match 0); this is divided

phasor~ 0.6![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.162.png)

\*~ 9 main loop: sawtooth of amplitude 9 tabread~ sequence read frequency sequence phasor~ wrap~ 9x original frequency sawtooth -~ 0.5 \*~ 100 adjust for reading

+~ 1 envelope sample tabread4~ envelope

\*~  multiply by audio-frequency sawtooth \*~ 128 adjust amplitude

cos~ and center for wavetable

+~ 129

+~ 1

tabread4~ sample

\*~  multiply by raised-cosine smoothing function |   envelope![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.163.png)

(OUT)

sequence sample![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.164.png)

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.165.png)

Figure 3.15: An analog-synthesizer-style sequencer.

notein![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.166.png)

f - store pitch below

pit vel t b f

b - bang to recall velocity

float velocity stored here note-on

filter sel 0 test for note on or off

stripnote off on 

float recall pitch

pitch

mtof / 127 select test against latest

phasor~ note-on pitch

$1 100 0 1000

-~ 0.5 line~

envelope generator now controls amplitude as well as grain size

cos~ +~ 0.5

+~ 1 \*~ 

\*~  \*~ 2

\*~  cos~ This replaces the tabread4~

|   in the previous patch.

(OUT)

Figure 3.16: A MIDI-style monophonic synthesizer.

by the maximum MIDI velocity of 127 and packed into a message for line~ with a time of 100 msec.

However, when a note-o® is received, it is only appropriate to stop the sound if the note-o® pitch actually matches the pitch the instrument is playing. For example, suppose the messages received are \60 127", \72 127", \60 0", and \72 0". When the note-on at pitch 72 arrives the pitch should change to 72, and then the \60 0" message should be ignored, with the note playing until the \72 0" message.

To accomplish this, ¯rst we store the velocity in the upper float object. Second, when the pitch arrives, it too is stored (the lower float object) and then the velocity is tested against zero (the \bang" outlet of t b f recalls the velocity which is sent to sel 0). If this is zero, the second step is to recall the pitch and test it (the select object) against the most recently received note-on pitch. Only if these are equal (so that \bang" appears at the left-hand-side outlet of select) does the message \0 1000" go to the line~ object.

Exercises

1. How many partials of a tone at A 440 can be represented digitally at a sample rate of 44100 Hertz?
1. What frequency would you hear if you synthesized a sinusoid at 88000 Hertz at a sample rate of 44100?
1. Suppose you are synthesizing sound at 44100 Hertz, and are computing 64- sample audio blocks. A control event is scheduled to happen at an elapsed time of exactly one second, using the fast-as-possible update scheme. At what sample does the update actually occur?
1. Sampling at 44100, we wish to approximately play a tone at middle C by repeating a ¯xed waveform every N samples. What value of N should we choose, and how many cents (Page 7) are we o®from the \true" middle C?
1. Two sawtooth waves, of unit amplitude, have frequencies 200 and 300 Hertz, respectively. What is the periodicity of the sum of the two? What if you then wrapped the sum back to the range from 0 to 1? Does this result change depending on the relative phase of the two?
1. Two sawtooth waves, of equal frequency and amplitude and one half cycle out of phase, are summed. What is the waveform of the sum, and what are its amplitude and frequency?
1. What is the relative level, in decibels, of a sawtooth wave's third harmonic (three times the fundamental) compared to that of the fundamental?
1. Suppose you synthesize a 44000-Hertz sawtooth wave at a sample rate of 44100 Hertz. What is the resulting waveform?
9. Using the techniques of Section 3.7, draw a block diagram for generating two phase-locked sinusoids at 500 and 700 Hertz.
9. Draw a block diagram showing how to use thresholding to detect when one audio signal exceeds another one in value. (You might want to do this to detect and ¯lter out feedback from speakers to microphones.)

88 CHAPTER 3. AUDIO AND CONTROL COMPUTATIONS


Chapter 4


Automation management

and voice


It is often desirable to control musical objects or events as aggregates rather than individually. Aggregates might take the form of a series of events spaced in time, in which the details of the events follow from the larger arc (for instance, notes in a melody). Or the individuals might sound simultaneously, as with voices in a chord, or partials in a complex tone. Often some or all properties of the individual elements are best inferred from those of the whole.

A rich collection of tools and ideas has arisen in the electronic music reper- tory for describing individual behaviors from aggregate ones. In this chapter we cover two general classes of such tools: envelope generators and voice banks. The envelope generator automates behavior over time, and the voice bank over aggregates of simultaneous processes (such as signal generators).

1. Envelope Generators

An envelope generator (sometimes, and more justly, called a transient generator ) makes an audio signal that smoothly rises and falls as if to control the loudness of a musical note. Envelope generators were touched on earlier in Section 1.5. Amplitude control by multiplication (Figure 1.4) is the most direct, ordinary way to use one, but there are many other possible uses.

Envelope generators have come in many forms over the years, but the sim- plest and the perennial favorite is the ADSR envelope generator. \ADSR" is an acronym for \Attack, Decay, Sustain, Release", the four segments of the ADSR generator's output. The ADSR generator is turned on and o®by a con- trol stream called a \trigger". Triggering the ADSR generator \on" sets o®its attack, decay, and sustain segments. Triggering it \o®" starts the release seg- ment. Figure 4.1 shows the block diagram representation of an ADSR envelope generator.

There are ¯ve parameters controlling the ADSR generator. First, a level

89

trigger![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.167.png)

Figure 4.1: ADSR envelope as a block diagram, showing the trigger input (a control stream) and the audio output.

parameter sets the output value at the end of the attack segment (normally the highest value output by the ADSR generator). Second and third, the attack and decay parameters give the time duration of the attack and decay segments. Fourth, a sustain parameter gives the level of the sustain segment, as a fraction of the level parameter. Finally, the release parameter gives the duration of the release segment. These ¯ve values, together with the timing of the \on" and \o®" triggers, fully determines the output of the ADSR generator. For example, the duration of the sustain portion is equal to the time between \on" and \o®" triggers, minus the durations of the attack and decay segments.

Figure 4.2 graphs some possible outputs of an ADSR envelope generator. In part (a) we assume that the \on" and \o®" triggers are widely enough separated that the sustain segment is reached before the \o®" trigger is received. Parts (b) and (c) of Figure 4.2 show the result of following an \on" trigger quickly by an \o®" one: (b) during the decay segment, and (c) even earlier, during the attack. The ADSR generator reacts to these situations by canceling whatever remains of the attack and decay segments and continuing straight to the release segment. Also, an ADSR generator may be retriggered \on" before the release segment is ¯nished or even during the attack, decay, or sustain segments. Part (d) of the ¯gure shows a reattack during the sustain segment, and part (e), during the decay segment.

The classic application of an ADSR envelope is using a voltage-control key- board or sequencer to make musical notes on a synthesizer. Depressing and re- leasing a key (for example) would generate \on" and \o®" triggers. The ADSR generator could then control the amplitude of synthesis so that \notes" would start and stop with the keys. In addition to amplitude, the ADSR generator can (and often is) used to control timbre, which can then be made to evolve naturally over the course of each note.

1. ENVELOPE GENERATORS 91

attack![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.168.png)

decay

sustain

1) release on  off time

(b) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.169.png)

on  off (c) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.170.png)

on off

(d) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.171.png)

on  on (e) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.172.png)

on  on 

Figure 4.2: ADSR envelope output: (a) with \on" and \o®" triggers separated; (b), (c) with early \o®" trigger; (d), (e) re-attacked.

2. Linear and Curved Amplitude Shapes

Suppose you wish to fade a signal in over a period of ten seconds|that is, you wish to multiply it by an amplitude-controlling signal y[n] which rises from 0 to 1 in value over 10R samples, where R is the sample rate. The most obvious choice would be a linear ramp: y[n] = n=(10R). But this will not turn out to yield a smooth increase in perceived loudness. Over the ¯rst second y[n] rises from ¡1 dB to -20 dB, over the next four by another 14 dB, and over the remaining ¯ve, only by the remaining 6 dB. Over most of the ten second period the rise in amplitude will be barely perceptible.

Another possibility would be to ramp y[n] exponentially, so that it rises at a constant rate in dB. You would have to ¯x the initial amplitude to be inaudible, say 0 dB (if we ¯x unity at 100 dB). Now we have the opposite problem: for the ¯rst ¯ve seconds the amplitude control will rise from 0 dB (inaudible) to 50 dB (pianissimo); this part of the fade-in should only have taken up the ¯rst second or so.

A more natural progression would perhaps have been to regard the fade-in as a timed succession of dynamics, 0-ppp-pp-p-mp-mf-f-®-®f, with each step taking roughly one second.

A fade-in ideally should obey some scale in between logarithmic and linear. A somewhat arbitrary choice, but useful in practice, is the quartic curve:

- n ´4

y[n] = ;

N

where N is the number of samples to fade in over (in the example above, it's 10R). So, after the ¯rst second of the ten we would have risen to -80 dB, after ¯ve seconds to -24 dB, and after nine, about -4 dB.

Figure 4.3 shows three amplitude transfer functions:

f1(x) = x (linear);

f2(x) = 102(x¡1) (dB to linear);

f3(x) = x4 (quartic):

The second function converts from dB to linear, arranged so that the input range, from 0 to 1, corresponds to 40 dB. (This input range of 40 dB corresponds to a reasonable dynamic range, allowing 5 dB for each of 8 steps in dynamic.) The quartic curve imitates the exponential (dB) curve fairly well for higher amplitudes, but drops o®more rapidly for small amplitudes, reaching true zero at right (whereas the exponential curve only goes down to 1=100).

We can think of the three curves as showing transfer functions, from an abstract control (ranging from 0 to 1) to a linear amplitude. After we choose a suitable transfer function f , we can compute a corresponding amplitude control signal; if we wish to ramp over N samples from silence to unity gain, the control signal would be:

y[n] = f (n=N):

2. LINEAR AND CURVED AMPLITUDE SHAPES 93

1   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.173.png)

linear![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.174.png)

ampli- tude

decibels

quartic

0  

0   1  

units ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.175.png)

Figure 4.3: Three amplitude transfer functions. The horizontal axis is in linear, logarithmic, or fourth-root units depending on the curve.

3. CONTINUOUS AND DISCONTINUOUS CONTROL CHANGES 97

FREQUENCY

1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.176.png)

-1 

f()

OUT

Figure 4.4: Using a transfer function to alter the shape of amplitude curves.

A block diagram for this is shown in Figure 4.4. Here we are introducing a new type of block to represent the application of a transfer function. For now we won't worry about its implementation; depending on the function desired, this might be best done arithmetically or using table lookup.

3. Continuous and discontinuous control changes

Synthesis algorithms vary widely in their ability to deal with discontinuously changing controls. Until now in this chapter we have assumed that controls must change continuously, and the ADSR envelope generator turns out to be ideally suited for such controls. It may even happen that the maximum amplitude of a note is less than the current value of the amplitude of its predecessor (using the same generator) and the ADSR envelope will simply ramp down (instead of up) to the new value for an attack.

This isn't necessarily desirable, however, in situations where an envelope generator is in charge of some aspect of timbre: perhaps, for example, we don't want the sharpness of a note to decrease during the attack to a milder one, but rather to jump to a much lower value so as always to be able to rise during the attack.

This situation also can arise with pitch envelopes: it may be desirable to slide pitch from one note to the next, or it may be desirable that the pitch tra jectory of each note start anew at a point independent of the previous sound.

Two situations arise when we wish to make discontinuous changes to syn- thesis parameters: either we can simply make them without disruption (for instance, making a discontinuous change in pitch); or else we can't, such as a change in a wavetable index (which makes a discontinuous change in the out- put). There are even parameters that can't possibly be changed continuously;

(a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.177.png)

time![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.178.png)

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.179.png)

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.180.png)

Figure 4.5: Muting technique for hiding discontinuous changes: (a) the enve- lope (upper graph) is set discontinuously to zero and the muting signal (lower graph) ramps down in advance to prepare for the change, and then is restored (discontinuously) to its previous value; (b) the envelope changes discontinuously between two nonzero values; the muting signal must both ramp down before- hand and ramp back up afterward.

for example, a selection among a collection of wavetables. In general, discontin- uously changing the phase of an oscillator or the amplitude of a signal will cause an audible artifact, but phase increments (such as pitches) may jump without bad results.

In those cases where a parameter change can't be made continuously for one reason or another, there are at least two strategies for making the change cleanly: muting and switch-and-ramp.

1. Muting

The muting technique is to apply an envelope to the output amplitude, which is quickly ramped to zero before the parameter change and then restored after- ward. It may or may not be the case that the discontinuous changes will result in a signal that rises smoothly from zero afterward. In Figure 4.5 (part a), we take the example of an amplitude envelope (the output signal of an ADSR generator), and assume that the discontinuous change is to start a new note at amplitude zero.

To change the ADSR generator's output discontinuously we reset it. This is

a di®erent operation from triggering it; the result is to make it jump to a new value, after which we may either simply leave it there or trigger it anew. Figure 4.5 (part a) shows the e®ect of resetting and retriggering an ADSR generator.

Below the ADSR generator output we see the appropriate muting signal, which ramps to zero to prepare for the discontinuity. The amount of time we allow for muting should be small (so as to disrupt the previous sound as little as possible) but not so small as to cause audible artifacts in the output. A working example of this type of muting was already shown on Page 81; there we allowed 5 msec for ramping down. The muting signal is multiplied by the output of the process to be de-clicked.

Figure 4.5 (part b) shows the situation in which we suppose the discontinuous change is between two possibly nonzero values. Here the muting signal must not only ramp down as before (in advance of the discontinuity) but must also ramp back up afterward. The ramp-down time need not equal the ramp-up time; these must be chosen, as always, by listening to the output sound.

In general, muting presents the di±culty that you must start the muting operation in advance of making the desired control change. In real-time settings, this often requires that we intentionally delay the control change. This is another reason for keeping the muting time as low as possible. (Moreover, it's a bad idea to try to minimize delay by conditionally omitting the ramp-down period when it isn't needed; a constant delay is much better than one that varies, even if it is smaller on average.)

2. Switch-and-ramp

The switch-and-ramp technique also seeks to remove discontinuities resulting from discontinuous control changes, but does so in a di®erent way: by syn- thesizing an opposing discontinuity which we add to cancel the original one out. Figure 4.6 shows an example in which a synthetic percussive sound (an en- veloped sinusoid) starts a note in the middle of a previous one. The attack of the sound derives not from the amplitude envelope but from the initial phase of the sinusoid, as is often appropriate for percussive sounds. The lower graph in the ¯gure shows a compensating audio signal with an opposing discontinuity, which can be added to the upper one to remove the discontinuity. The advantages of this technique over muting are, ¯rst, that there need be no delay between the decision to make an attack and the sound of the attack; and second, that any artifacts arising from this technique are more likely to be masked by the new sound's onset.

Figure 4.7 shows how the switch-and-ramp technique can be realized in a block diagram. The box marked with ellipsis (\...") may hold any synthesis algorithm, which we wish to interrupt discontinuously so that it restarts from zero (as in, for example, part (a) of the previous ¯gure). At the same time that we trigger whatever control changes are necessary (exempli¯ed by the top ADSR generator), we also reset and trigger another ADSR generator (middle right) to cancel out the discontinuity. The discontinuity is minus the last value of the synthesis output just before it is reset to zero.

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.181.png)

time![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.182.png)

Figure 4.6: The switch-and-ramp technique for canceling out discontinuous changes. A discontinuity (upper graph) is measured and canceled out with a signal having the opposite discontinuity (lower graph), which then decays smoothly.

trigger

snapshot![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.183.png)

reset/

trigger level

...

OUT

Figure 4.7: Block diagram for the switch-and-ramp technique.

6. VOICE TAGS 101

To do this we measure the level the ADSR generator must now jump to. This is its own current level (which might not be zero) minus the discontinuity (or equivalently, plus the synthesis output's last value). The two are added (by the +~ object at bottom), and then a snapshot is taken. The cancelling envelope generator (at right) is reset discontinuously to this new value, and then triggered to ramp back to zero. The +~object's output (the sum of the synthesizer output and the discontinuity-cancelling signal) is the de-clicked signal.

4. Polyphony

In music, the term polyphony is usually used to mean \more than one separate voices singing or playing at di®erent pitches one from another". When speak- ing of electronic musical instruments we use the term to mean \maintaining several copies of some process in parallel." We usually call each copy a \voice" in keeping with the analogy, although the voices needn't be playing separately distinguishable sounds.

In this language, a piano is a polyphonic instrument, with 88 \voices". Each voice of the piano is normally capable of playing exactly one pitch. There is never a question of which voice to use to play a note of a given pitch, and no question, either, of playing several notes simultaneously at the same pitch.

Many polyphonic electronic musical instruments take a more °exible ap- proach to voice management. Most software synthesis programs (like Csound) use a dynamic voice allocation scheme, so that, in e®ect, a new voice is created for every note in the score. In systems such as Max or Pd, which are oriented toward real-time interactive use, a voice bank is allocated in advance, and the work to be done (playing notes, or whatever) is distributed among the voices in the bank.

This is diagrammed in Figure 4.8, where the several voices each produce one output signal, which are all added to make the total output of the voice bank. Frequently the individual voices will need several separate outputs; for instance, they might output several channels so that they may be panned individually; or they might have individual e®ect sends so that each may have its own send level.

5. Voice allocation

It is frequently desirable to automate the selection of voices to associate with individual tasks (such as notes to play). For example, a musician playing at a keyboard can't practically choose which voice should go with each note played. To automate voice selection we need a voice allocation algorithm, to be used as shown in Figure 4.9.

Armed with a suitable voice allocation algorithm, the control source need not concern itself with the detail of which voice is taking care of which task; algorithmic note generators and sequencers frequently rely on this. On the

control

voice 1 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.184.png)voice 2

voice 3

+ ` `OUT

Figure 4.8: A voice bank for polyphonic synthesis.

other hand, musical writing for ensembles frequently speci¯es explicitly which instrument plays which note, so that the notes will connect to each other end- to-end in a desirable way.

One simple voice allocation algorithm works as shown in Figure 4.10. Here we suppose that the voice bank has only two voices, and we try to allocate voices for the tasks a, b, c, and d. Things go smoothly until task d comes along, but then we see no free voices (they are taken up by b and c). We could now elect either to drop task d, or else to steal the voice of either task b or c. In practice the best choice is usually to steal one. In this particular example, we chose to steal the voice of the oldest task, b.

If we happen to know the length of the tasks b and c at the outset of task d, we may be able to make a better choice of which voice to steal. In this example it might have been better to steal from c, so that d and b would be playing together at the end and not d alone. In some situations this information will be available when the choice must be made, and in some (live keyboard input, for example) it will not.

6. Voice tags

Suppose now that we're using a voice bank to play notes, as in the example above, but suppose the notes a, b, c, and d all have the same pitch, and further- more that all their other parameters are identical. How can we design a control stream so that, when any one note is turned o®,we know which one it is?

"notes"![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.185.png)

voice allocation

voice 1 voice 2

voice 3

+ ` `OUT

Figure 4.9: Polyphonic voice allocation.

a  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.186.png)

b  

c  

d  

voice 1... ..  .......... voice 2....... ...

|||
| :- | :- |
time![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.187.png)

Figure 4.10: A polyphonic voice allocation algorithm, showing voice stealing.

This question doesn't come up if the control source is a clavier keyboard because it's impossible to play more than one simultaneous note on a single key. But it could easily arise algorithmically, or simply as a result of merging two keyboard streams together. Moreover, turning notes o®is only the simplest example of a more general problem, which is how, once having set a task o® in a voice bank, we can get back to the same voice to guide its evolution as a function of real-time inputs or any other unpredictable factor.

To deal with situations like this we can add one or more tags to the message starting a note (or, in general, a task). A tag is any collection of data with which we can later identify the task, which we can then use to search for the voice that is allocated for it.

Taking again the example of Figure 4.10, here is one way we might write those four tasks as a control stream:

start-time end-time pitch ...

1 3 60 ... 2 8 62

4 6 64

5 8 65

In this representation we have no need of tags because each message (each line of text) contains all the information we need in order to specify the entire task. (Here we have assumed that the tasks a, ..., d are in fact musical notes with pitches 60, 62, 64, and 65.) In e®ect we're representing each task as a single event in a control stream (Section 3.3).

On the other hand, if we suppose now that we do not know in advance the length of each note, a better representation would be this one:

time tag action parameters

1 a start 60 ... 2 b start 62 ... 3 a end

4 c start 64 ... 5 d start 65 ... 6 c end

8 b end

8 d end

Here each note has been split into two separate events to start and end it. The labels a, ..., d are used as tags; we know which start goes with which end since their tags are the same. Note that the tag is not necessarily related at all to the voice that will be used to play each note.

The MIDI standard does not supply tags; in normal use, the pitch of a note serves also as its tag (so tags are constantly being re-used.) If two notes having the same pitch must be addressed separately (to slide their pitches in di®erent


directions for example), the MIDI channel may be used (in addition to the note) as a tag.

In real-time music software it is often necessary to pass back and forth between the event-per-task representation and the tagged one above, since the ¯rst representation is better suited to storage and graphical editing, while the second is often better suited to real-time operations.

7. Encapsulation in Pd

The examples for this chapter will use Pd's encapsulation mechanism, which permits the building of patches that may be reused any number of times. One or more object boxes in a Pd patch may be subpatches, which are separate patches encapsulated inside the boxes. These come in two types: one-o® subpatches and abstractions. In either case the subpatch appears as an object box in another patch, called the parent.

If you type \pd" or \pd my-name" into an object box, this creates a one-o® subpatch. The contents of the subpatch are saved as part of the parent patch,

in one ¯le. If you make several copies of a subpatch you may change them individually. On the other hand, you can invoke an abstraction by typing into the box the name of a Pd patch saved to a ¯le (without the \.pd" extension). In this situation Pd will read that ¯le into the subpatch. In this way, changes to the ¯le propagate everywhere the abstraction is invoked.

A subpatch (either one-o® or abstraction) may have inlets and outlets that appear on the box in the parent patch. This is speci¯ed using the following objects:

inlet , inlet » : create inlets for the object box containing the subpatch. The inlet~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.188.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.189.png) version creates an inlet for audio signals, whereas inlet creates one for control streams. In either case, whatever comes to the inlet of the box in the parent patch comes out of the inlet or inlet~ object in the subpatch.

outlet , outlet » : Corresponding objects for output from subpatches.![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.190.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.191.png)

Pd provides an argument-passing mechanism so that you can parametrize di®erent invocations of an abstraction. If in an object box you type \$1", it is expanded to mean \the ¯rst creation argument in my box on the parent patch", and similarly for \$2" and so on. The text in an object box is interpreted at the time the box is created, unlike the text in a message box. In message boxes, the same \$1" means \the ¯rst argument of the message I just received" and is interpreted whenever a new message comes in.

An example of an abstraction, using inlets, outlets, and parametrization, is shown in Figure 4.11. In part (a), a patch invokes plusminus in an object box, with a creation argument equal to 5. The number 8 is fed to the plusminus object, and out comes the sum and di®erence of 8 and 5.

The plusminus object is not de¯ned by Pd, but is rather de¯ned by the patch residing in the ¯le named \plusminus.pd". This patch is shown in part

2) of the ¯gure. The one inlet and two outlet objects correspond to the


4\.8. EXAMPLES

(a)

8![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.192.png)

plusminus 5 13 3

103

(b) inlet![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.193.png)

+ $1 − $1 outlet outlet


Figure 4.11: Pd's abstraction mechanism: (a) invoking the abstraction, plusminus with 5 as a creation argument; (b) the contents of the ¯le, \plusmi- nus.pd".

inlets and outlets of the plusminus object. The two \$1" arguments (to the

+ and - objects) are replaced by 5 (the creation argument of the plusminus object).

  We have already seen one abstraction in the examples: the output~ object introduced in Figure 1.10 (Page 16). That example also shows that an abstrac- tion may display controls as part of its box on the parent patch; see the Pd documentation for a description of this feature.

8. Examples

ADSR envelope generator

Example D01.envelope.gen.pd (Figure 4.12) shows how the line~ object may be used to generate an ADSR envelope to control a synthesis patch (only the ADSR envelope is shown in the ¯gure). The \attack" button, when pressed, has two e®ects. The ¯rst (leftmost in the ¯gure) is to set the line~ object on its attack segment, with a target of 10 (the peak amplitude) over 200 msec (the attack time). Second, the attack button sets a delay 200 object, so that after the attack segment is done, the decay segment can start. The decay segment falls to a target of 1 (the sustain level) after another 2500 msec (the decay time).

The \release" button sends the same line~ object back to zero over 500 more milliseconds (the release time). Also, in case the delay 200 object happens to be set at the moment the \release" button is pressed, a \stop" message is sent to it. This prevents the ADSR generator from launching its decay segment after launching its release segment.

In Example D02.adsr.pd (Figure 4.13) we encapsulate the ADSR generator

8. EXAMPLES 106

attack release

stop 10 200![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.194.png) del 200

1 2500 0 500 (IN)|   line~

\*~ 

|  (OUT)

Figure 4.12: Using a line~ object to generate an ADSR envelope.

trigger![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.195.png)

adsr 1 100 200 50 300

osc~ 440

\*~ 

|  (OUT)

Figure 4.13: Invoking the adsr abstraction.

in a Pd abstraction (named adsr) so that it can easily be replicated. The design of the adsr abstraction makes it possible to control the ¯ve ADSR parameters either by supplying creation arguments or by connecting control streams to its inlets.

In this example the ¯ve creation arguments (1, 100, 200, 50, and 300) specify the peak level, attack time, decay time, sustain level (as a percentage of peak level), and release time. There are six control inlets: the ¯rst to trigger the ADSR generator, and the others to update the values of the ¯ve parameters. The output of the abstraction is an audio signal.

This abstraction is realized as shown in Figure 4.14. (You can open this subpatch by clicking on the adsr object in the patch.) The only signal objects are line~ and outlet~. The three pack objects correspond to the three message objects from the earlier Figure 4.12. From left to right, they take care of the attack, decay, and release segments.

The attack segment goes to a target speci¯ed as \$1" (the ¯rst creation

attack

trigger moses test for negative trigger![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.196.png)

inlet

t b b if so, zero the output release

sel 0

if zero t b ... do this anyway

cancel stop peak

decay

level attack decay sustain inlet inlet inlet inlet

ATTACK:

optionally

f $1

jump DECAY

to zero 0   pack 0 $2 del $2 release f $4 \* $1 inlet

... then \* 0.01 pack 0 $3 pack 0 $5 recall peak level RELEASE: ramp and pack with back to zero

line~

attack time

outlet~

Figure 4.14: Inside the adsr abstraction.

8. EXAMPLES 107

LINEAR

r freq line~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.197.png) r amp osc~ line~

\*~ |  (OUT)

sample messages

;

freq 1760 5000

QUARTIC

r freq r amp unpack![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.198.png) unpack sqrt sqrt sqrt sqrt

line~ line~ \*~  \*~ \*~  \*~ osc~

\*~ |  (OUT)

8. EXAMPLES 110

;

freq 55 5000

Figure 4.15: Linear and quartic transfer functions for changing amplitude and pitch.

argument of the abstraction) over \$2" milliseconds; these values may be over- written by sending numbers to the \peak level" and \attack" inlets. The release segment is similar, but simpler, since the target is always zero. The hard part is the decay segment, which again must be set o®after a delay equal to the attack time (the del $2 object). The sustain level is calculated from the peak level and the sustain percentage (multiplying the two and dividing by 100).

The trigger inlet, if sent a number other than zero, triggers an onset (the attack and decay segments), and if sent zero, triggers the release segment. Fur- thermore, the ADSR generator may be reset to zero by sending a negative trigger (which also generates an onset).

Transfer functions for amplitude control

Section 4.2 described using ADSR envelopes to control amplitude, for which exponential or quartic-curve segments often give more natural-sounding results than linear ones. Patches D03.envelope.dB.pd and D04.envelope.quartic.pd (the latter shown in Figure 4.15) demonstrate the use ofdecibel and quartic segments. In addition to amplitude, in Example D04.envelope.quartic.pd the frequency of a sound is also controlled, using linear and quartic shapes, for comparison.

Since converting decibels to linear amplitude units is a costly operation (at

least when compared to an oscillator or a ramp generator), Example D03.envelope.dB.pd uses table lookup to implement the necessary transfer function. This has the advantage of e±ciency, but the disadvantage that we must decide on the range

of admissible values in advance (here from 0 to 120 dB).

For a quartic segment as in Example D04.envelope.quartic.pd no table lookup

is required; we simply square the line~ object's output signal twice in succes-

sion. To compensate for raising the output to the fourth power, the target

values sent to the line~ object must be the fourth root of the desired ones.

Thus, messages to ramp the frequency or amplitude are ¯rst unpacked to sep-

arate the target and time interval, the target's fourth root is taken (via two

square roots in succession), and the two are then sent to the line~ object. Here

we have made use of one new Pd object:

unpack : unpack a list of numbers (and/or symbols) and distribute them to separate![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.199.png) outlets. As usual the outputs appear in right-to-left order. The number of outlets and their types are determined by the creation arguments. (See also pack, Page 50).

The next two patches, D05.envelope.pitch.pd and D06.envelope.portamento.pd, use an ADSR envelope generator to make a pitch envelope and a simple line~ object, also controlling pitch, to make portamento. In both cases exponential segments are desirable, and they are calculated using table lookup.

Additive synthesis: Risset's bell

The abstraction mechanism of Pd, which we used above to make a reusable ADSR generator, is also useful for making voice banks. Here we will use ab- stractions to organize banks of oscillators for additive synthesis. There are many possible ways of organizing oscillator banks besides those shown here.

The simplest and most direct organization of the sinusoids is to form partials to add up to a note. The result is monophonic, in the sense that the patch will play only one note at a time, which, however, will consist of several sinusoids whose individual frequencies and amplitudes might depend both on those of the note we're playing, and also on their individual placement in a harmonic (or inharmonic) overtone series.

Example D07.additive.pd (Figure 4.16) uses a bank of 11 copies of an ab- straction named partial (Figure 4.17) in an imitation of a well-known bell in- strument by Jean-Claude Risset. As described in [DJ85, p. 94], the bell sound has 11 partials, each with its own relative amplitude, frequency, and duration.

For each note, the partial abstraction computes a simple (quartic) ampli- tude envelope consisting only of an attack and a decay segment; there is no sustain or release segment. This is multiplied by a sinusoid, and the product is added into a summing bus. Two new object classes are introduced to implement the summing bus:

catch~ : de¯ne and output a summing bus. The creation argument (\sum- bus"![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.200.png) in this example) gives the summing bus a name so that throw~ objects

partial 1 1 0.56 0![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.201.png)

partial 0.67 0.9 0.56 1 0   pitch![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.202.png)

partial 1 0.65 0.92 0 mtof

partial 1.8 0.55 0.92 1.7 s frequency

partial 2.67 0.325 1.19 0

partial 1.67 0.35 1.7 0 0   duration, tenthsof a second partial 1.46 0.25 2 0 \* 100

partial 1.33 0.2 2.74 0 s duration

partial 1.33 0.15 3 0

partial 1 0.1 3.76 0 <-- click to play partial 1.33 0.075 4.07 0

s trigger

catch~ sum |  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.203.png)

(OUT)

Figure 4.16: A Pd realization of Jean-Claude Risset's bell instrument. The bell sound is made by summing 11 sinusoids, each made by a copy of the partial abstraction.

$1 amplitude;

trigger $2 relative duration; r trigger arguments: $3 relative frequency;![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.204.png)

$4 detune

relative t b b ATTACK frequency del 5 DECAY float $1

float $3r frequency float $2 relativeduration \* 0.1

sqrt

* times global r duration

frequency sqrt

+ $4 plus detune 0 $1\*  actual duration $1 5

osc~ attack time

line~

\*~  5 msec

\*~  quartic amplitude

throw~ sum \*~  curve

add to global

summing bus

Figure 4.17: The partial abstraction used by Risset's bell instrument from Figure 4.16.


below can refer to it. You may have as many summing busses (and hence catch~ objects) as you like but they must all have di®erent names.

throw~ : add to a summing bus. The creation argument selects which sum- ming![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.205.png) bus to use.

The control interface is crude: number boxes control the \fundamental" frequency of the bell and its duration. Sending a \bang" message to the s trigger object starts a note. (The note then decays over the period of time controlled by the duration parameter; there is no separate trigger to stop the note). There is no amplitude control except via the output~ object.

The four arguments to each invocation of the partial abstraction specify:

1. amplitude. The amplitude of the partial at its peak, at the end of the attack and the beginning of the decay of the note.
1. relative duration. This is multiplied by the overall note duration (con- trolled in the main patch) to determine the duration of the decay portion of the sinusoid. Individual partials may thus have di®erent decay times, so that some partials die out faster than others, under the main patch's overall control.
1. relative frequency. As with the relative duration, this controls each par- tial's frequency as a multiple of the overall frequency controlled in the main patch.
1. detune. A frequency in Hertz to be added to the product of the global frequency and the relative frequency.

Inside the partial abstraction, the amplitude is simply taken directly from the \$1" argument (multiplying by 0.1 to adjust for the high individual amplitudes); the duration is calculated from the r duration object, multiplying it by the \$2" argument. The frequency is computed as f p + d where f is the global frequency (from the r frequency object), p is the relative frequency of the partial, and d is the detune frequency.

Additive synthesis: spectral envelope control

The next patch example, D08.table.spectrum.pd (Figure 4.18), shows a very di®erent application of additive synthesis from the previous one. Here the si- nusoids are managed by the spectrum-partial abstraction shown in Figure 4.19. Each partial computes its own frequency as in the previous patch. Each partial also computes its own amplitude periodically (when triggered by the r poll-table object), using a tabread4 object. The contents of the table (which has a nominal range of 50 dB) are converted to linear units and used as an amplitude control in the usual way.

A similar example, D09.shepard.tone.pd (not pictured), makes a Shepard tone using the same technique. Here the frequencies of the sinusoids sweep over a ¯xed range, ¯nally jumping from the end back to the beginning and


4\.8. EXAMPLES

50![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.206.png)

s pitch

0

s whammybar

111

loadbang send bangs to "poll-table" metro 30![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.207.png) needed by the abstraction s poll-table

spectrum-partial 1 spectrum-partial 2 spectrum-partial 3


spectrum-tab

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.208.png)

Figure 4.18: Additive synthesis for a speci¯ed spectral envelope, drawn in a table.

repeating. The spectral envelope is arranged to have a peak at the middle of the pitch range and drop o®to inaudibility at the edges of the range so that we hear only the continuous sweeping and not the jumping. The result is a famous auditory conundrum, an inde¯nitely ascending or descending tone.

The technique of synthesizing to a speci¯ed spectral envelope can be general- ized in many ways: the envelope may be made to vary in time either as a result of a live analysis of another signal, or by calculating from a set of compositional rules, or by cross-fading between a collection of pre-designed spectral envelopes, or by frequency-warping the envelopes, to name a few possibilities.

Polyphonic synthesis: sampler

We move now to an example using dynamic voice allocation as described in Section 4.5. In the additive synthesis examples shown previously, each voice is used for a ¯xed purpose. In the present example, we allocate voices from a bank as needed to play notes in a control stream.

Example D11.sampler.poly.pd (Figure 4.20) shows the polyphonic sampler, which uses the abstraction sampvoice (whose interior is shown in Figure 4.21). The techniques for altering the pitch and other parameters in a one-shot sampler

8. EXAMPLES 119

$1: partial number![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.209.png)

r pitch

mtof pitch to frequency

* $1 then get the frequency of this specific partial ftom... and then convert back to pitch.

r poll−table calling patch bangs this every 30 msec.

f  ... at which time we get the pitch back...

- r whammybar and transpose by shifting table index. tabread4 spectrum−tab get the strength from the table

  moses 1

The vertical scale is dB from 1 to 50,

0   + 50 but we want true zero when

dbtorms the table value is 0 or less.

pack 0 30 osc~

line~

\*~ 

throw~ sum−bus

Figure 4.19: The spectrum-partial abstraction used in Figure 4.18.

are shown in Example D10.sampler.notes.pd (not shown) which in turn is de-

rived from the original one-shot sampler from the previous chapter (C05.sampler.oneshot.pd, shown in Figure 3.14).

The sampvoice objects in Figure 4.20 are arranged in a di®erent kind of

summing bus from the ones before; here, each one adds its own output to the

signal on its inlet, and puts the sum on its outlet. At the bottom of the eight

objects, the outlet therefore holds the sum of all eight. This has the advantage

of being more explicit than the throw~ / catch~ busses, and is preferable when

visual clutter is not a problem.

The main job of the patch, though, is to distribute the \note" messages to

the sampvoice objects. To do this we must introduce some new Pd objects:

mod : Integer modulus. For instance, 17 mod 10 gives 7, and -2 mod 10 gives 8.![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.210.png) There is also an integer division object named div ; dividing 17 by 10 via div gives 1, and -2 by 10 gives -1.

poly : Polyphonic voice allocator. Creation arguments give the number of voices![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.211.png) in the bank and a °ag (1 if voice stealing is needed, 0 if not). The inlets are a numeric tag at left and a °ag at right indicating whether to start or stop a voice with the given tag (nonzero numbers meaning \start" and zero, \stop"). The outputs are, at left, the voice number, the tag again at center, and the start/stop °ag at right. In MIDI applications, the tag can be pitch and the start/stop °ag can be the note's velocity.

makenote : Supply delayed note-o® messages to match note-on messages. The inlets![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.212.png) are a tag and start/stop °ag (\pitch" and \velocity" in MIDI usage) and the desired duration in milliseconds. The tag/°ag pair are repeated to the two outlets as they are received; then, after the delay, the tag is repeated with °ag zero to stop the note after the desired duration.

The \note" messages contain ¯elds for pitch, amplitude, duration, sample number, start location in the sample, rise time, and decay time. For instance, the message,

60 90 1000 2 500 10 20

(if received by the r note object) means to play a note at pitch 60 (MIDI units), amplitude 90 dB, one second long, from the wavetable named \sample2", starting at a point 500 msec into the wavetable, with rise and decay times of 10 and 20 msec.

After unpacking the message into its seven components, the patch creates a tag for the note. To do this, ¯rst the t b f object outputs a bang after the last of the seven parameters appear separately. The combination of the +, f, and modobjects acts as a counter that repeats after a million steps, essentially generating a unique number corresponding to the note.

The next step is to use the poly object to determine which voice to play which note. The poly object expects separate messages to start and stop tasks (i.e., notes). So the tag and duration are ¯rst fed to the makenote object, whose outputs include a °ag (\velocity") at right and the tag again at left. For each

r note![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.213.png)

unpack 0 0 0 0 0 0 0

t b f counter to f   + 1

generate tags

mod 1e+06 supply later makenote 64

note-off

allocate voice poly 8 1

get rid of stripnote

note-off

pack 0 0 0 0 0 0 0 0 route to a voice depending

on voice number from poly route 1 2 3 4 5 6 7 8

sampvoice one "sampvoice" sampvoice abstraction

sampvoice for each

voice, each sampvoice adding its sampvoice own output

to a sum (left sampvoice inlets and sampvoice

outlets) sampvoice |  

(OUT)

Figure 4.20: A polyphonic sampler demonstrating voice allocation and use of tags.

bang inlet store parameters first in delay for![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.214.png) floats below until muted

mute to delay 5 unpack 0 0 0 0 0 0 0

take effect t b b b

f   delay for

f  f  f   f  delay note end mtof \* 44.1 f  

/ 261.62 + 1

starting

* 4.41e+08 read

point

 

ending

read pack 0 0 0 0 0

point

mute and attack decay

unmute 0 5 1 5 $3, $4 1e+07 $5  0, $1 $2 0 $1 wavetable

indexvline~ makefilename sample%d vline~ unpack

set $1 select mute dbtorms

wavetable

sqrt

tabread4~ sample1

sqrt

\*~  amplitude

line~ envelope

\*~ \*~ 

add to inlet~ \*~ summing +~ 

bus

outlet~

Figure 4.21: The sampvoice abstraction used in the polyphonic sampler of Figure 4.20.

tag makenote receives, two pairs of numbers are output, one to start the note, and another, after a delay equal to the note duration, to stop it.

Having treated poly to this separated input, we now have to strip the mes- sages corresponding to the ends of notes, since we really only need combined \note" messages with duration ¯elds. The stripnote object does this job. Fi- nally, the voice number we have calculated is prepended to the seven parameters we started with (the pack object), so that the output of the pack object looks like this:

4 60 90 1000 2 500 10 20

where the \4" is the voice number output by the poly object. The voice number is used to route the message to the desired voice using the route object. The appropriate sampvoice object then gets the original list starting with \60".

Inside the sampvoice object (Figure 4.21), the message is used to control the tabread4~ and surrounding line~ and vline~ objects. The control takes place with a delay of 5 msec as in the earlier sampler example. Here, however, we must store the seven parameters of the note (earlier there were no parameters). This is done using the six f objects, plus the right inlet of the rightmost delay object. These values are used after the delay of 5 msec. This is done in tandem with the muting mechanism described on Page 95, using another vline~ object.

When the 5 msec have elapsed, the vline~ object in charge of generating the wavetable index gets its marching orders (and, simultaneously, the wavetable number is set for the tabread4~ object and the amplitude envelope generator starts its attack.) The wavetable index must be set discontinuously to the start- ing index, then ramped to an ending index over an appropriate time duration to obtain the needed transposition. The starting index in samples is just 44.1 times the starting location in milliseconds, plus one to allow for four-point table interpolation. This becomes the third number in a packed list generated by the pack object at the center of the voice patch.

We arbitrarily decide that the ramp will last ten thousand seconds (this is the \1e+07" appearing in the message box sent to the wavetable index genera- tor), hoping that this is at least as long as any note we will play. The ending index is the starting index plus the number of samples to ramp through. At a transposition factor of one, we should move by 441,000,000 samples during those 10,000,000 milliseconds, or proportionally more or less depending on the transposition factor. This transposition factor is computed by the mtof object, dividing by 261.62 (the frequency corresponding to MIDI note 60) so that a speci¯ed \pitch" of 60 results in a transposition factor of one.

These and other parameters are combined in one message via the pack object so that the following message boxes can generate the needed control messages. The only novelty is the makefilename object, which converts numbers such as \2" to symbols such as \sample2" so that the tabread4~ object's wavetable

may be set.

At the bottom of the voice patch we see how a summing bus is implemented inside a subpatch; an inlet~ object picks up the sum of all the preceding voices,

the output of the current voice is added in, and the result is sent on to the next voice via the outlet~ object.

Exercises

1. What input to a fourth-power transfer function gives an output of -12 dB, if an input of 1 outputs 0 dB?
1. An envelope generator rises from zero to a peak value during its attack segment. How many decibels less than the peak has the output reached halfway into the attack, assuming linear output? Fourth-power output?
1. What power-law transfer function (i.e. what choice of n for the function f (x) = xn ) would you use if you wish the halfway-point value to be -12 decibels?
1. Suppose you wish to cross-fade two signals, i.e., to ramp one signal in and simultaneously another one out. If they have equal power and are uncor- related, a linear cross-fade would result in a drop of 3 decibels halfway though the cross-fade. What power law would you use to maintain con- stant power throughout the cross-fade?
1. A three-note chord, lasting 1.5 seconds, is played starting once every sec- ond. How many voices would be needed to synthesize this without cutting o®any notes?
1. Suppose a synthesis patch gives output between ¡1 and 1. While a note is playing, a new note is started using the \rampdown" voice-stealing technique. What is the maximum output?

120 CHAPTER 4. AUTOMATION AND VOICE MANAGEMENT


Chapter 5

Modulation

Having taken a two-chapter detour into aspects of control and organization in electronic music, we return to describing audio synthesis and processing tech- niques. So far we have seen additive and wavetable-based methods. In this chapter we will introduce three so-called modulation techniques: amplitude mod- ulation, frequency modulation, and waveshaping. The term \modulation" refers loosely to any technique that systematically alters the shape of a waveform by bending its graph vertically or horizontally. Modulation is widely used for build- ing synthetic sounds with various families of spectra, for which we must develop some terminology before getting into the techniques.

1. Taxonomy of spectra

Figure 5.1 introduces a way of visualizing the spectrum of an audio signal. The spectrum describes, roughly speaking, how the signal's power is distributed into frequencies. (Much more precise de¯nitions can be given than those that we'll develop here, but they would require more mathematical background.)

Part (a) of the ¯gure shows the spectrum of a harmonic signal, which is a periodic signal whose fundamental frequency is in the range of perceptible pitches, roughly between 50 and 4000 Hertz. The Fourier series (Page 12) gives a description of a periodic signal as a sum of sinusoids. The frequencies of the sinusoids are in the ratio 0 : 1 : 2 : ¢¢¢. (The constant term in the Fourier series may be thought of as a sinusoid,

a0 = a0 cos(0 ¢!n);

whose frequency is zero.)

In a harmonic signal, the power shown in the spectrum is concentrated on a discrete subset of the frequency axis (a discrete set consists of isolated points, only ¯nitely many in any bounded interval). We call this a discrete spectrum. Furthermore, the frequencies where the signal's power lies are in the 0 : 1 : 2¢¢¢ ratio that arises from a periodic signal. (It's not necessary for all ofthe harmonic

119

1) harmonic![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.215.png)

amplitude spectral envelope

frequency

2) inharmonic![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.216.png)
100) continuous![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.217.png)

Figure 5.1: A taxonomy of timbres. The spectral envelope describes the shape of the spectrum. The sound may be discretely or continuously distributed in frequency; if discretely, it may be harmonic or inharmonic.

5\.1. TAXONOMY OF SPECTRA 121

frequencies to be present; some harmonics may have zero amplitude.) For a harmonic signal, the graph of the spectrum shows the amplitudes of the partials of the signals. Knowing the amplitudes and phases of all the partials fully determines the original signal.

Part (b) of the ¯gure shows a spectrum which is also discrete, so that the signal can again be considered as a sum of a series of partials. In this case, however, there is no fundamental frequency, i.e., no audible common submultiple of all the partials. This is called an inharmonic signal. (The terms harmonic and inharmonic may be used to describe both the signals and their spectra.)

When dealing with discrete spectra, we report a partial's amplitude in a slightly non-intuitive way. Each component sinusoid,

a cos(!n + Á)

only counts as having amplitude a=2 as long as the angular frequency ! is nonzero. But for a component of zero frequency, for which ! = Á= 0, the am- plitude is given as a|without dividing by two. (Components of zero frequency are often called DC components; \DC" is historically an acronym for \direct current"). These conventions for amplitudes in spectra will simplify the math- ematics later in this chapter; a deeper reason for them will become apparent in Chapter 7.

Part (c) of the ¯gure shows a third possibility: the spectrum might not be concentrated into a discrete set of frequencies, but instead might be spread out among all possible frequencies. This can be called a continuous, or noisy spectrum. Spectra don't necessarily fall into either the discrete or continuous categories; real sounds, in particular, are usually somewhere in between.

Each of the three parts of the ¯gure shows a continuous curve called the spectral envelope. In general, sounds don't have a single, well-de¯ned spectral envelope; there may be many ways to draw a smooth-looking curve through a spectrum. On the other hand, a spectral envelope may be speci¯ed intentionally; in that case, it is usually clear how to make a spectrum conform to it. For a discrete spectrum, for example, we could simply read o®, from the spectral envelope, the desired amplitude of each partial and make it so.

A sound's pitch can sometimes be inferred from its spectrum. For discrete spectra, the pitch is primarily encoded in the frequencies of the partials. Har- monic signals have a pitch determined by their fundamental frequency; for inhar- monic ones, the pitch may be clear, ambiguous, or absent altogether, according to complex and incompletely understood rules. A noisy spectrum may also have a perceptible pitch if the spectral envelope contains one or more narrow peaks. In general, a sound's loudness and timbre depend more on its spectral enve- lope than on the frequencies in the spectrum, although the distinction between continuous and discrete spectra may also be heard as a di®erence in timbre.

Timbre, as well as pitch, may evolve over the life of a sound. We have been speaking of spectra here as static entities, not considering whether they change in time or not. If a signal's pitch and timbre are changing over time, we can think of the spectrum as a time-varying description of the signal's momentary behavior.

2. MULTIPLYING AUDIO SIGNALS 127

This way of viewing sounds is greatly oversimpli¯ed. The true behavior of audible pitch and timbre has many aspects which can't be explained in terms of this model. For instance, the timbral quality called \roughness" is sometimes thought of as being re°ected in rapid changes in the spectral envelope over time. The simpli¯ed description developed here is useful nonetheless in discussions about how to construct discrete or continuous spectra for a wide variety of musical purposes, as we will begin to show in the rest of this chapter.

2. Multiplying audio signals

We have been routinely adding audio signals together, and multiplying them by slowly-varying signals (used, for example, as amplitude envelopes) since Chapter 1. For a full understanding of the algebra of audio signals we must also consider the situation where two audio signals, neither of which may be assumed to change slowly, are multiplied. The key to understanding what happens is the Cosine Product Formula:

1h i cos(a) cos(b) = cos(a + b) + cos(a ¡ b)

2

To see why this formula holds, we can use the formula for the cosine of a sum of two angles:

cos(a + b) = cos(a) cos(b) ¡ sin(a) sin(b)

to evaluate the right hand side of the cosine product formula; it then simpli¯es to the left hand side.

We can use this formula to see what happens when we multiply two sinusoids (Page 1):

cos(®n + Á) cos(¯n + ») =

1h i

- cos((®+ ¯)n + (Á+ »)) + cos((®¡ ¯)n + (Á¡ »)) 2

In words, multiply two sinusoids and you get a result with two partials, one at the sum of the two original frequencies, and one at their di®erence. (If the di®erence ®¡¯ happens to be negative, simply switch the original two sinusoids and the di®erence will then be positive.) These two new components are called sidebands.

This gives us a technique for shifting the component frequencies of a sound, called ring modulation, which is shown in its simplest form in Figure 5.2. An os- cillator provides a carrier signal, which is simply multiplied by the input. In this context the input is called the modulating signal. The term \ring modulation" is often used more generally to mean multiplying any two signals together, but here we'll just consider using a sinusoidal carrier signal. (The technique of ring modulation dates from the analog era [Str95]; digital multipliers now replace both the VCA (Section 1.5) and the ring modulator.)

Figure 5.3 shows a variety of results that may be obtained by multiplying a (modulating) sinusoid of angular frequency ® and peak amplitude 2a, by a

IN 

1  -1 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.218.png)

OUT

Figure 5.2: Block diagram for ring modulating an input signal with a sinusoid.

(carrier) sinusoid of angular frequency ¯ and peak amplitude 1:

[2a cos(®n)] ¢[cos(¯n)]

(For simplicity the phase terms are omitted.) Each part of the ¯gure shows both the modulation signal and the result in the same spectrum. The modulating signal appears as a single frequency, ®, at amplitude a. The product in general has two component frequencies, each at an amplitude of a=2.

Parts (a) and (b) of the ¯gure show \general" cases where ® and ¯ are nonzero and di®erent from each other. The component frequencies of the output are ®+ ¯ and ®¡ ¯. In part (b), since ®¡ ¯ < 0, we get a negative frequency component. Since cosine is an even function, we have

cos((®¡ ¯)n) = cos((¯ ¡ ®)n)

so the negative component is exactly equivalent to one at the positive frequency

- ¡ ®, at the same amplitude.

In the special case where ® = ¯, the second (di®erence) sideband has zero frequency. In this case phase will be signi¯cant so we rewrite the product with explicit phases, replacing ¯ by ®, to get:

2a cos(®n + Á) cos(®n + ») =

- a cos(2®n + (Á+ »)) + a cos(Á¡ »):

The second term has zero frequency; its amplitude depends on the relative phase of the two sinusoids and ranges from +a to ¡a as the phase di®erence Á¡ » varies from 0 to ¼radians. This situation is shown in part (c) of Figure 5.3.

Finally, part (d) shows a carrier signal whose frequency is zero. Its value is the constant a (not 2a; zero frequency is a special case). Here we get only one sideband, of amplitude a=2 as usual.

We can use the distributive rule for multiplication to ¯nd out what happens when we multiply signals together which consist of more than one partial each.

amplitude

a  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.219.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.220.png)

(a)

a/2 a/2

OUT IN  OUT ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.221.png)

frequency 

- +  

a  (b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.222.png)

a/2 a/2 −  

a  (c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.223.png)

a/2 z  

- ` `a  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.224.png)

(d)

a/2

- 0  

Figure 5.3: Sidebands arising from multiplying two sinusoids of frequency ® and ¯: (a) with ® > ¯ > 0; (b) with ¯ > ® so that the lower sideband is re°ected about the f = 0 axis; (c) with ®= ¯, for which the amplitude of the zero-frequency sideband depends on the phases of the two sinusoids; (d) with ®= 0.

amplitude![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.225.png)

(a)

frequency

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.226.png)

(c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.227.png)

Figure 5.4: Result of ring modulation of a complex signal by a pure sinusoid: (a) the original signal's spectrum and spectral envelope; (b) modulated by a relatively low modulating frequency (1/3 of the fundamental); (c) modulated by a higher frequency, 10/3 of the fundamental.

For example, in the situation above we can replace the signal of frequency ® with a sum of several sinusoids, such as:

a1 cos(®1n) + ¢¢¢+ ak cos(®kn)

Multiplying by the signal of frequency ¯ gives partials at frequencies equal to: ®1 + ¯;®1 ¡ ¯;:::;®k + ¯;®k ¡ ¯

As before if any frequency is negative we take its absolute value.

Figure 5.4 shows the result of multiplying a complex periodic signal (with several components tuned in the ratio 0:1:2:¢¢¢) by a sinusoid. Both the spectral envelope and the component frequencies of the result are changed according to relatively simple rules.

The resulting spectrum is essentially the original spectrum combined with its re°ection about the vertical axis. This combined spectrum is then shifted

3. WAVESHAPING 133

to the right by the carrier frequency. Finally, if any components of the shifted spectrum are still left of the vertical axis, they are re°ected about it to make positive frequencies again.

In part (b) of the ¯gure, the carrier frequency (the frequency of the sinusoid) is below the fundamental frequency of the complex signal. In this case the shifting is by a relatively small distance, so that re-folding the spectrum at the end almost places the two halves on top of each other. The result is a spectral envelope roughly the same as the original (although half as high) and a spectrum twice as dense.

A special case, not shown, is to use a carrier frequency half the fundamental. In this case, pairs of partials will fall on top of each other, and will have the ratios 1/2 : 3/2 : 5/2 :¢¢¢to give an odd-partial-only signal an octave below the original. This is a very simple and e®ective octave divider for a harmonic signal, assuming you know or can ¯nd its fundamental frequency. If you want even partials as well as odd ones (for the octave-down signal), simply mix the original signal with the modulated one.

Part (c) of the ¯gure shows the e®ect of using a modulating frequency much higher than the fundamental frequency ofthe complex signal. Here the unfolding e®ect is much more clearly visible (only one partial, the leftmost one, had to be re°ected to make its frequency positive). The spectral envelope is now widely displaced from the original; this displacement is often a more strongly audible e®ect than the relocation of partials.

As another special case, the carrier frequency may be a multiple of the fundamental of the complex periodic signal; then the partials all land back on other partials of the same fundamental, and the only e®ectis the shift in spectral envelope.

3. Waveshaping

Another approach to modulating a signal, called waveshaping, is simply to pass it through a suitably chosen nonlinear function. A block diagram for doing this is shown in Figure 5.5. The function f () (called the transfer function ) distorts the incoming waveform into a di®erent shape. The new shape depends on the shape of the incoming wave, on the transfer function, and also|crucially|on

the amplitude of the incoming signal. Since the amplitude of the input waveform a®ects the shape of the output waveform (and hence the timbre), this gives us an easy way to make a continuously varying family of timbres, simply by varying the input level of the transformation. For this reason, it is customary to include a leading amplitude control as part of the waveshaping operation, as shown in the block diagram.

The amplitude of the incoming waveform is called the waveshaping index. In many situations a small index leads to relatively little distortion (so that the output closely resembles the input) and a larger one gives a more distorted, richer timbre.

Figure 5.6 shows a familiar example of waveshaping, in which f () amounts

IN 

f()![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.228.png)

OUT

Figure 5.5: Block diagram for waveshaping an input signal using a nonlinear function f (). An amplitude adjustment step precedes the function lookup, to take advantage of the di®erent e®ect of the wavetable lookup at di®erent am- plitudes.

to a clipping function. This example shows clearly how the input amplitude| the index|can a®ect the output waveform. The clipping function passes its input to the output unchanged as long as it stays in the interval between - 0.3 and +0.3. So when the input does not exceed 0.3 in absolute value, the output is the same as the input. But when the input grows past the limits, the output stays within; and as the amplitude of the signal increases the e®ect of this clipping action is progressively more severe. In the ¯gure, the input is a decaying sinusoid. The output evolves from a nearly square waveform at the beginning to a pure sinusoid at the end. This e®ectwill be well known to anyone who has played an instrument through an overdriven ampli¯er. The louder the input, the more distorted will be the output. For this reason, waveshaping is also sometimes called distortion.

Figure 5.7 shows a much simpler and easier to analyse situation, in which the transfer function simply squares the input:

f (x) = x2

For a sinusoidal input,

x[n] = a cos(!n + Á)

we get

a2

f (x[n]) = (1 + cos(2!n + 2Á))

2

If the amplitude a equals one, this just amounts to ring modulating the sinusoid by a sinusoid of the same frequency, whose result we described in the previ- ous section: the output is a DC (zero-frequency) sinusoid plus a sinusoid at

1   (a) -1 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.229.png)

0\.3![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.230.png)

(b)

-0.3

(c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.231.png)

0\.3 -0.3

Figure 5.6: Clipping as an example of waveshaping: (a) the input, a decaying sinusoid; (b) the waveshaping function, which clips its input to the interval between -0.3 and +0.3; (c) the result.

1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.232.png)

(a)

-1 

1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.233.png)

(b) -1  1  

1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.234.png)

(c)

Figure 5.7: Waveshaping using a quadratic transfer function f (x) = x2: (a) the input; (b) the transfer function; (c) the result, sounding at twice the original frequency.

twice the original frequency. However, in this waveshaping example, unlike ring modulation, the amplitude of the output grows as the square of the input.

Keeping the same transfer function, we now consider the e®ect of sending in a combination of two sinusoids with amplitudes a and b, and angular frequencies ® and ¯. For simplicity, we'll omit the initial phase terms. We set:

x[n] = a cos(®n) + bcos(¯n) and plugging this into f () gives

a2

f (x[n]) = (1 + cos(2®n)) +

2

b2

+ (1 + cos(2¯n))

  2

+ab[cos((®+ ¯)n) + cos((®¡ ¯)n)]

The ¯rst two terms are just what we would get by sending the two sinusoids through separately. The third term is twice the product of the two input terms,

which comes from the middle, cross term in the expansion,

f (x + y) = x2 + 2xy + y2

This e®ect, called intermodulation, becomes more and more dominant as the number of terms in the input increases; if there are k sinusoids in the input there are only k \straight" terms in the product, but there are (k2 ¡ k)=2 intermodulation terms.

In contrast with ring modulation, which is a linear function of its input signal, waveshaping is nonlinear. While we were able to analyze linear processes by considering their action separately on all the components of the input, in this nonlinear case we also have to consider the interactions between components. The results are far more complex|sometimes sonically much richer, but, on the other hand, harder to understand or predict.

In general, we can show that a periodic input, no matter how complex, will repeat at the same period after waveshaping: if the period is ¿ so that

x[n + ¿] = x[n] and temporarily setting the index a = 1,

f (x[n + ¿]) = f (x[n])

(In some special cases the output can repeat at a submultiple of ¿, so that we get a harmonic of the input as a result; this happened for example in Figure 5.4.)

Combinations of periodic tones at consonant intervals can give rise to dis- tortion products at subharmonics. For instance, if two periodic signals x and y are a musical fourth apart (periods in the ratio 4:3), then the sum of the two repeats at the lower rate given by the common subharmonic. In equations we would have:

x[t + ¿=3] = x[t] y[t + ¿=4] = y[t]

which implies

x[t + ¿]+ y[t + ¿] = x[t]+ y[t]

and so the distorted sum f (x + y) would repeat after a period of ¿:

f (x + y)[n + ¿] = f (x + y)[n]:

This has been experienced by every electric guitarist who has set the ampli¯er to \overdrive" and played the open B and high E strings together: the distortion product sometimes sounds at the pitch of the low E string, two octaves below the high one.

To get a somewhat more explicit analysis of the e®ect of waveshaping on an incoming signal, it is sometimes useful to write the function f as a ¯nite or in¯nite power series :

f (x) = f0 + f1x + f2x2 + f3x3 + ¢¢¢

If the input signal x[n] is a unit-amplitude sinusoid, cos(!n), we can consider the action of the above terms separately:

f (a ¢x[n]) = f0 + af1 cos(!n) + a2f2cos2(!n) + a3f3cos3(!n) + ¢¢¢

Since the terms of the series are successively multiplied by higher powers of the index a, a lower value of a will emphasize the earlier terms more heavily, and a higher value will emphasize the later ones.

The individual terms' spectra can be found by applying the cosine product formula repeatedly:

1 = cos(0)

x[n] = cos(!n)

1  1

x2[n] = + cos(2!n)

2  2

3 1 2 1

x [n] = cos(¡!n) + cos(!n) + cos(3!n)

4 4 4

4 1 3 3 1

x [n] = cos(¡2!n) + cos(0) + cos(2!n) + cos(4!n)

8 8 8 8

1 4 6 4 1
x5[n] = cos(¡3!n)+ cos(¡!n)+ cos(!n)+ cos(3!n)+ cos(5!n)

16 16 16 16 16

and so on. The numerators of the fractions will be recognized as Pascal's trian- gle. The Central Limit Theorem of probability implies that each kth row can be approximated by a Gaussian curve whose standard deviation (a measure of width) is proportional to the square root of k.

The negative-frequency terms (which have been shown separately here for clarity) are to be combined with the positive ones; the spectral envelope is folded into itself in the same way as in the ring modulation example of Figure 5.4.

As long as the coe±cients fk are all positive numbers or zero, then so are all the amplitudes of the sinusoids in the expansions above. In this case all the phases stay coherent as a varies and so we get a widening of the spectrum (and possibly a drastically increasing amplitude) with increasing values of a. On the other hand, if some of the fk are positive and others negative, the di®erent ex- pansions will interfere destructively; this will give a more complicated-sounding spectral evolution.

Note also that the successive expansions all contain only even or only odd partials. If the transfer function (in series form) happens to contain only even powers:

f (x) = f0 + f2x2 + f4x4 + ¢¢¢

then the result, having only even partials, will sound an octave higher than the incoming sinusoid. If only odd powers show up in the expansion of f (x), then the output will contain only odd partials. Even if f can't be expressed exactly as a power series (for example, the clipping function of Figure 5.3), it is still true that if f is an even function, i.e., if

f (¡x) = f (x)


you will get only even harmonics and if f is an odd function,

f (¡x) = ¡f (x)

you will get odd harmonics.

Many mathematical tricks have been proposed to use waveshaping to gener- ate speci¯ed spectra. It turns out that you can generate pure sinusoids at any harmonic of the fundamental by using a Chebychev polynomial as a transfer function [Leb79] [DJ85], and from there you can go on to build any desired static spectrum (Example E05.chebychev.pd demonstrates this.) Generating families of spectra by waveshaping a sinusoid of variable amplitude turns out to be trickier, although several interesting special cases have been found, some of which are developed in detail in Chapter 6.

4. Frequency and phase modulation

If a sinusoid is given a frequency which varies slowly in time we hear it as having a varying pitch. But if the pitch changes so quickly that our ears can't track the change|for instance, if the change itself occurs at or above the fundamental frequency of the sinusoid|we hear a timbral change. The timbres so generated are rich and widely varying. The discovery by John Chowning of this possibility [Cho73] revolutionized the ¯eld of computer music. Here we develop frequency modulation, usually called FM, as a special case of waveshaping [Leb79] [DJ85, pp.155-158]; the analysis given here is somewhat di®erent [Puc01].

The FM technique, in its simplest form, is shown in Figure 5.8 (part a). A frequency-modulated sinusoid is one whose frequency varies sinusoidally, at some angular frequency !m, about a central frequency !c, so that the instan- taneous frequencies vary between (1 ¡ r)!c and (1 + r)!c, with parameters !m controlling the frequency of variation, and r controlling the depth of variation. The parameters !c, !m, and r are called the carrier frequency, the modulation frequency, and the index of modulation, respectively.

It is customary to use a simpler, essentially equivalent formulation in which the phase, instead of the frequency, of the carrier sinusoid is modulated sinu- soidally. (This gives an equivalent result since the instantaneous frequency is the rate of change of phase, and since the rate of change of a sinusoid is just another sinusoid.) The phase modulation formulation is shown in part (b) of the ¯gure.

We can analyze the result of phase modulation as follows, assuming that the modulating oscillator and the wavetable are both sinusoidal, and that the carrier and modulation frequencies don't themselves vary in time. The resulting signal can then be written as

x[n] = cos(a cos(!mn) + !cn)

The parameter a, which takes the place of the earlier parameter r, is likewise called the index of modulation; it too controls the extent of frequency variation

4. FREQUENCY AND PHASE MODULATION 133
1) (b)


modulation frequency

1  -1 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.235.png)

index of modulation

1  

carrier frequency

1  -1 

OUT

modulation frequency

1  -1 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.236.png)

index of modulation

carrier frequency

N  0  


OUT

Figure 5.8: Block diagram for frequency modulation (FM) synthesis: (a) the classic form; (b) realized as phase modulation.

relative to the carrier frequency !c. If a = 0, there is no frequency variation and the expression reduces to the unmodi¯ed, carrier sinusoid; as a increases the waveform becomes more complex.

To analyse the resulting spectrum we can rewrite the signal as,

x[n] = cos(!cn) ¤ cos(a cos(!m n))

- sin(!cn) ¤ sin(a cos(!mn))

We can consider the result as a sum of two waveshaping generators, each oper- ating on a sinusoid of frequency !m and with a waveshaping index a, and each ring modulated with a sinusoid of frequency !c. The waveshaping function f is given by f (x) = cos(x) for the ¯rst term and by f (x) = sin(x) for the second.

Returning to Figure 5.4, we can predict what the spectrum will look like.

5. EXAMPLES 139

The two harmonic spectra, of the waveshaping outputs

cos(a cos(!m n))

and

sin(a cos(!mn))

have, respectively, harmonics tuned to

0;2!m ;4!m ;:::

and

!m;3!m ;5!m ;:::

and each is multiplied by a sinusoid at the carrier frequency. So there will be a spectrum centered at the carrier frequency !c, with sidebands at both even and odd multiples of the modulation frequency !m, contributed respectively by the sine and cosine waveshaping terms above. The index of modulation a, as it changes, controls the relative strength of the various partials. The partials themselves are situated at the frequencies

!c + m!m

where

m = ::: ¡ 2;¡1;0;1;2;:::

As with any situation where two periodic signals are multiplied, if there is some common supermultiple of the two periods, the resulting product will repeat at that longer period. So if the two periods are k¿ and m¿, where k and m are relatively prime, they both repeat after a time interval of km¿. In other words, if the two have frequencies which are both multiples of some common frequency, so that !m = k! and !c = m!, again with k and m relatively prime, the result will repeat at a frequency of the common submultiple !. On the other hand, if no common submultiple ! can be found, or if the only submultiples are lower than any discernible pitch, then the result will be inharmonic.

Much more about FM can be found in textbooks [Moo90, p. 316] [DJ85, pp.115-139] [Bou00] and the research literature. Some of the possibilities are shown in the following examples.

5. Examples

Ring modulation and spectra

Example E01.spectrum.pd serves to introduce a spectrum measurement tool we'll be using; here we'll skip to the second example, E02.ring.modulation.pd, which shows the e®ect of ring modulating a harmonic spectrum (which was worked out theoretically in Section 5.2 and shown in Figure 5.4). In the example we consider a signal whose harmonics (from 0 through 5) all have unit amplitude.

The harmonics may be turned on and o®separately using toggle switches. When they are all on, the spectral envelope peaks at DC (because the constant signal counts twice as strongly as the other sinusoids), has a °at region from harmonics 1 through 5, and then descends to zero.

In the signal generation portion of the patch (part (a) of the ¯gure), we sum the six partials and multiply the sum by the single, carrier oscillator. (The six signals are summed implicitly by connecting them all to the same inlet of the \*~ object.) The value of \fundamental" at the top is computed to line up well with the spectral analysis, whose result is shown in part (b) of the ¯gure.

The spectral analysis (which uses techniques that won't be described until Chapter 9) shows the location of the sinusoids (assuming a discrete spectrum) on the horizontal axis and their magnitudes on the vertical one. So the presence of a peak at DC of magnitude one in the spectrum of the input signal predicts, µa la Figure 5.3, that there should be a peak in the output spectrum, at the carrier frequency, of height 1/2. Similarly, the two other sinusoids in the input signal, which have height 1/2 in the spectrum, give rise to two peaks each, of height 1/4, in the output. One of these four has been re°ected about the left edge of the ¯gure (taking the absolute value of its negative frequency).

Octave divider and formant adder

As suggested in Section 5.2, when considering the result of modulating a com- plex harmonic (i.e., periodic) signal by a sinusoid, an interesting special case is to set the carrier oscillator to 1=2 the fundamental frequency, which drops the resulting sound an octave with only a relatively small deformation of the spectral envelope. Another is to modulate by a sinusoid at several times the fundamental frequency, which in e®ect displaces the spectral envelope without changing the fundamental frequency of the result. This is demonstrated in Example E03.octave.divider.pd (Figure 5.10). The signal we process here is a recorded, spoken voice.

The subpatches pd looper and pd delay hide details. The ¯rst is a looping sampler as introduced in Chapter 2. The second is a delay of 1024 samples, which uses objects that are introduced later in Chapter 7. We will introduce one object class here:

fiddle~ : pitch tracker. The inlet takes a signal to analyze, and messages to![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.237.png) change settings. Depending on its creation arguments fiddle~may have a variable number of outlets o®ering various information about the input signal. As shown here, with only one creation argument to specify window size, the third outlet attempts to report the pitch of the input, and the amplitude of that portion of the input which repeats (at least approximately) at the reported pitch. These are output as a list of two numbers. The pitch, which is in MIDI units, is reported as zero if none could be identi¯ed.

In this patch the third outlet is unpacked into its pitch and amplitude com- ponents, and the pitch component is ¯ltered by the moses object so that only successful pitch estimates (nonzero ones) are used. These are converted to units

r fundamental![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.238.png)

* 0 \* 1 \* 2 \* 3 \* 4 \* 5

osc~ osc~ osc~ osc~ osc~ osc~

partials <-- On/Off

\*~  \*~  \*~  \*~  \*~  \*~ 

0 carrier

\*~  osc~ frequency

|  

(OUT) (a)

- SPECTRUM

1  0.5 0  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.239.png)

0   1   2   3   4   5   6   7  

-- partial number --

(b)

Figure 5.9: Ring modulation of a complex tone by a sinusoid: (a) its realization;

2) a measured spectrum.

pd looper![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.240.png)

fiddle~ 2048 pd delay

unpack

loadbang

moses 1

0\.5 15 

mtof

0\.5<-- multiplier \*  

\*~  osc~ ring modulation \*~ 2 extra gain

on/off for original pd  pd  <--and processed sounds

+~ |  (OUT)

Figure 5.10: Lowering the pitch of a sound by an octave by determining its pitch and modulating at half the fundamental.


osc~ 300![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.241.png)

loadbang

225

225 <-- frequency of second tone osc~

loadbang

+~ 

50 

\*~  amplitude of sum

50 <-- before clipping

clip~ -1 1 / 100

|  

(OUT)

Figure 5.11: Nonlinear distortion of a sum of two sinusoids to create a di®erence tone.

of frequency by the mtof object. Finally, the frequency estimates are either reduced by 1=2 or else multiplied by 15, depending on the selected multiplier, to provide the modulation frequency. In the ¯rst case we get an octave divider, and in the second, additional high harmonics that deform the vowels.

Waveshaping and di®erence tones

Example E04.di®erence.tone.pd (Figure 5.11) introduces waveshaping, demon- strating the nonlinearity of the process. Two sinusoids (300 and 225 Hertz, or a ratio of 4 to 3) are summed and then clipped, using a new object class:

clip~ : signal clipper. When the signal lies between the limits speci¯ed by ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.242.png)the arguments to the clip~ object, it is passed through unchanged; but when it falls below the lower limit or rises above the upper limit, it is replaced by the limit. The e®ect of clipping a sinusoidal signal was shown graphically in Figure 5.6.

As long as the amplitude of the sum of sinusoids is less than 50 percent, the sum can't exceed one in absolute value and the clip~ object passes the pair of sinusoids through unchanged to the output. As soon as the amplitude exceeds 50 percent, however, the nonlinearity of the clip~ object brings forth distor- tion products (at frequencies 300m + 225n for integers m and n), all of which happening to be multiples of 75, which is thus the fundamental of the resulting tone. Seen another way, the shortest common period of the two sinusoids is 1/75 second (which is four periods of the 300 Hertz, tone and three periods of the 225 Hertz tone), so the result repeats 75 times per second.

The frequency of the 225 Hertz tone in the patch may be varied. If it is


5. EXAMPLES osc~ 220![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.243.png)

0 <- index / 100

pack 0 50

line~ \*~ 

\*~ 128 +~ 129

tabread4~ E05-tab

hip~ 5

|  (OUT)

139

E05-tab![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.244.png)


Figure 5.12: Using Chebychev polynomials as waveshaping transfer functions.

moved slightly away from 225, a beating sound results. Other values ¯nd other common subharmonics, and still others give rise to rich, inharmonic tones.

Waveshaping using Chebychev polynomials

Example E05.chebychev.pd (Figure 5.12) demonstrates how you can use wave- shaping to generate pure harmonics. We'll limit ourselves to a speci¯c example here in which we would like to generate the pure ¯fth harmonic,

cos(5!n) by waveshaping a sinusoid

x[n] = cos(!n)

We need to ¯nd a suitable transfer function f (x). First we recall the formula for the waveshaping function f (x) = x5 (Page 131), which gives ¯rst, third and

¯fth harmonics:

16x5 = cos(5!n) + 5cos(3!n) + 10cos(!n)

Next we add a suitable multiple of x3 to cancel the third harmonic:

16x5 ¡ 20x3 = cos(5!n) ¡ 5cos(!n)

and then a multiple of x to cancel the ¯rst harmonic:

16x5 ¡ 20x3 + 5x = cos(5!n)

5. EXAMPLES 146

So for our waveshaping function we choose

f (x) = 16x5 ¡ 20x3 + 5x

This procedure allows us to isolate any desired harmonic; the resulting functions f are known as Chebychev polynomials [Leb79].

To incorporate this in a waveshaping instrument, we simply build a patch that works as in Figure 5.5, computing the expression

x[n] = f (a[n]cos(!n))

where a[n]is a suitable index which may vary as a function ofthe sample number n. When a happens to be one in value, out comes the pure ¯fth harmonic. Other values of a give varying spectra which, in general, have ¯rst and third harmonics as well as the ¯fth.

By suitably combining Chebychev polynomials we can ¯x any desired su- perposition of components in the output waveform (again, as long as the wave- shaping index is one). But the real promise of waveshaping|that by simply changing the index we can manufacture spectra that evolve in interesting but controllable ways|is not addressed, at least directly, in the Chebychev picture.

Waveshaping using an exponential function

We return again to the spectra computed on Page 131, corresponding to wave- shaping functions of the form f (x) = xk. We note with pleasure that not only

are they all in phase (so that they can be superposed with easily predictable results) but also that the spectra spread out as k increases. Also, in a series of the form,

f (x) = f0 + f1x + f2x2 + ¢¢¢;

a higher index of modulation will lend more relative weight to the higher power terms in the expansion; as we saw seen earlier, if the index of modulation is a, the various xk terms are multiplied by f , af , a2f , and so on.

0  1 2

Now suppose we wish to arrange for di®erent terms in the above expansion to dominate the result in a predictable way as a function of the index a. To choose the simplest possible example, suppose we wish f0 to be the largest term for 0 < a < 1, then for it to be overtaken by the more quickly growing af1 term for 1 < a < 2, which is then overtaken by the a2f2 term for 2 < a < 3 and so on, so that each nth term takes over at index n. To make this happen we just require that

f1 = f0;2f2 = f1;3f3 = f2;:::

and so choosing f0 = 0, we get f1 = 1, f2 = 1=2, f3 = 1=6, and in general,

1

f k = 1 ¢2 ¢3 ¢::: ¢k

These happen to be the coe±cients of the power series for the function

f (x) = ex

where e ¼ 2:7 is Euler's constant.

Before plugging in e[^1] as a transfer function it's wise to plan how we will deal with signal amplitude, since ex grows quickly as x increases. If we're going to plug in a sinusoid of amplitude a, the maximum output will be ea , occurring whenever the phase is zero. A simple and natural choice is simply to divide by ea to reduce the peak to one, giving:

f (a cos(!n)) = ea cos(!n) = ea(cos(!n)¡1)

ea

This is realized in Example E06.exponential.pd. Resulting spectra for a = 0, 4, and 16 are shown in Figure 5.13. As the waveshaping index rises, progressively less energy is present in the fundamental; the energy is increasingly spread over the partials.

Sinusoidal waveshaping: evenness and oddness

Another interesting class of waveshaping transfer functions is the sinusoids:

f (x) = cos(x + Á)

which include the cosine and sine functions (got by choosing Á = 0 and Á = ¡¼=2, respectively). These functions, one being even and the other odd, give rise to even and odd harmonic spectra, which turn out to be:

cos(a cos(!n)) = J0(a)¡2J2(a) cos(2!n)+2J4(a) cos(4!n)¡2J6(a) cos(6!n)§¢ ¢¢ sin(a cos(!n)) = 2J1(a) cos(!n) ¡ 2J3(a) cos(3!n) + 2J5(a) cos(5!n) ¨ ¢¢¢

The functions Jk(a) are the Bessel functions of the ¯rst kind, which engineers sometimes use to solve problems about vibrations or heat °ow on discs. For other values of Á, we can expand the expression for f :

f (x) = cos(x) cos(Á) ¡ sin(x) sin(Á)

so the result is a mix between the even and the odd harmonics, with Á con- trolling the relative amplitudes of the two. This is demonstrated in Patch E07.evenodd.pd, shown in Figure 5.14.

Phase modulation and FM

Example E08.phase.mod.pd, shown in Figure 5.15, shows how to use Pd to re- alize true frequency modulation (part a) and phase modulation (part b). These correspond to the block diagrams of Figure 5.8. To accomplish phase modula- tion, the carrier oscillator is split into its phase and cosine lookup components. The signal is of the form

1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.245.png)

a=0 0  

0\.25![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.246.png)

a=4 0  

0\.25![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.247.png)

a=16 0  

0   1   2   3   4   5   6   7  

−− partial number −−

Figure 5.13: Spectra of waveshaping output using an exponential transfer func- tion. Indices of modulation of 0, 4, and 16 are shown; note the di®erent vertical scales.

(frequency)

|  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.248.png)

(index)|   osc~

\*~ 

symmetry +~ 0.1 0.1 mixed

cos~ 0   even |   0.25 odd

(OUT)

Figure 5.14: Using an additive o®set to a cosine transfer function to alter the symmetry between even and odd. With no o®setthe symmetry is even. For odd symmetry, a quarter cycle is added to the phase. Smaller o®sets give a mixture of even and odd.

5. EXAMPLES 

modulation frequency |  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.249.png)

osc~

modulation carrier index

frequency |  

|   \*~ 

+~ 

osc~

|  (OUT)

modulation frequency |  

osc~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.250.png)

carrier

frequency modulation

|   index phasor~ |  

\*~ 

+~ 

cos~

|  (OUT)

5. EXAMPLES 148
1) (b)

Figure 5.15: Pd patches for: (a) frequency modulation; (b) phase modulation.

where !c is the carrier frequency, !m is the modulation frequency, and a is the index of modulation|all in angular units.

We can predict the spectrum by expanding the outer cosine:

x[t] = cos(!cn) cos(a cos(!m n)) ¡ sin(!cn) sin(a cos(!m n)) Plugging in the expansions from Page 141 and simplifying yields: x[t] = J (a) cos(! n)

+ !m)n + ¼20 ) + J c ¼

+J1(a) cos((!c 1(a) cos((!c ¡ !m)n + 2) +J2(a) cos((!c + 2!m)n + ¼) + J2(a) cos((!c ¡ 2!m)n + ¼)

+J3(a) cos((!c + 3!m )n + 32¼) + J3(a) cos((!c ¡ 3!m)n + 32¼) + ¢¢¢

So the components are centered about the carrier frequency !c with sidebands extending in either direction, each spaced !m from the next. The amplitudes are functions of the index of modulation, and don't depend on the frequencies. Figure 5.16 shows some two-operator phase modulation spectra, measured using Example E09.FM.spectrum.pd.

Phase modulation can thus be seen simply as a form of ring modulated waveshaping. So we can use the strategies described in Section 5.2 to generate particular combinations of frequencies. For example, if the carrier frequency is half the modulation frequency, you get a sound with odd harmonics exactly as in the octave dividing example (Figure 5.10).

Frequency modulation need not be restricted to purely sinusoidal carrier or modulation oscillators. One well-trodden path is to e®ect phase modulation on the phase modulation spectrum itself. There are then two indices of modulation (call them a and b) and two frequencies of modulation (!m and !p) and the waveform is:

x[n] = cos(!cn + a cos(!mn) + bcos(!pn))

To analyze the result, just rewrite the original FM series above, replacing !cn instance: J3n(a+) cosbcos(((!!c + 3!m )n + 32¼+ bcos(!pn))

everywhere with !c pn). The third positive sideband becomes for This is itself just another FM spectrum, with its own sidebands of frequency

!c + 3!m + k!p;k = 0;§1;§2;:::

having amplitude J3(a)Jk(b) and phase (3+k)¼=2 [Leb77]. Example E10.complex.FM.pd (not shown here) illustrates this by graphing spectra from a two-modulator FM instrument.

Since early times [Sch77] researchers have sought combinations of phases, frequencies, and modulation indices, for simple and compact phase modulation instruments, that manage to imitate familiar instrumental sounds. This became

a major industry with the introduction of commercial FM synthesizers.

0\.5![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.251.png)

a=0.15 0  

0   2   4   6   8   10  12  14 

0\.25![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.252.png)

a=0.38 0  

0   2   4   6   8   10  12  14 

0\.25![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.253.png)

a=0.84 0  

0   2   4   6   8   10  12  14 

−− partial number −−

Figure 5.16: Spectra from phase modulation at three di®erent indices. The indices are given as multiples of 2¼radians.

149 CHAPTER 5. MODULATION

Exercises

1. A sound has fundamental 440. How could it be ring modulated to give a tone at 110 Hertz with only odd partials? How could you then ¯ll in the even ones if you wanted to?
1. A sinusoid with frequency 400 and unit peak amplitude is squared. What are the amplitudes and frequencies of the new signal's components?
1. What carrier and modulation frequencies would you give a two-operator FM instrument to give frequencies of 618, 1000, and 2618 Hertz? (This is a prominent feature of Chowning's Stria [DJ85].)
1. Two sinusoids with frequency 300 and 400 Hertz and peak amplitude one (so RMS amplitude ¼0.707) are multiplied. What is the RMS amplitude of the product?
1. Suppose you wanted to make FM yet more complicated by modulating the modulating oscillator, as in:

cos(!cn + a cos(!m n + bcos(!pn)))

How, qualitatively speaking, would the spectrum di®er from that of the simple two-modulator example (Section 5.5)?

6. A sinusoid at a frequency ! is ring modulated by another sinusoid at exactly the same frequency. At what phase di®erences will the DC com- ponent of the result disappear?


Chapter 6

Designer spectra

As suggested at the beginning of the previous chapter, a powerful way to synthe- size musical sounds is to specify|and then realize|speci¯c tra jectories of pitch (or more generally, frequencies of partials), along with tra jectories of spectral envelope [Puc01]. The spectral envelope is used to determine the amplitude of the individual partials, as a function of their frequencies, and is thought of as controlling the sound's (possibly time-varying) timbre.

A simple example ofthis would be to imitate a plucked string by constructing a sound with harmonically spaced partials in which the spectral envelope starts out rich but then dies away exponentially with higher frequencies decaying faster than lower ones, so that the timbre mellows over time. Spectral-evolution models for various acoustic instruments have been proposed [GM77] [RM69] . A more complicated example is the spoken or sung voice, in which vowels appear as spectral envelopes, dipthongs and many consonants appear as time variations in the spectral envelopes, and other consonants appear as spectrally shaped noise.

Spectral envelopes may be obtained from analysis of recorded sounds (de- veloped in Chapter 9) or from purely synthetic criteria. To specify a spectral envelope from scratch for every possible frequency would be tedious, and in most cases you would want to describe them in terms of their salient features. The most popular way of doing this is to specify the size and shape of the spectral envelope's peaks, which are called formants. Figure 6.1 shows a spectral enve- lope with two formants. Although the shapes of the two peaks in the spectral envelope are di®erent, they can both be roughly described by giving the coordi- nates of each apex (which give the formant's center frequency and amplitude) and each formant's bandwidth. A typical measure of bandwidth would be the width of the peak at a level 3 decibels below its apex. Note that if the peak is at (or near) the f = 0 axis, we pretend it falls o®to the left at the same rate as (in reality) it falls o®to the right.

Suppose we wish to generate a harmonic sound with a speci¯ed collection of formants. Independently of the fundamental frequency desired, we wish the spectrum to have peaks with prescribed center frequencies, amplitudes, and

147

, a ) (f 1   1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.254.png)

b  1  

(f 2  , a )2  

ampli- b  2  tude

frequency

Figure 6.1: A spectral envelope showing the frequencies, amplitudes, and band- widths of two formants.

bandwidths. Returning to the phase modulation spectra shown in Figure 5.16, we see that, at small indices of modulation at least, the result has a single, well-de¯ned spectral peak. We can imagine adding several of these, all shar- ing a fundamental (modulating) frequency but with carriers tuned to di®erent harmonics to select the various desired center frequencies, and with indices of modulation chosen to give the desired bandwidths. This was ¯rst explored by Chowning [Cho89] who arranged formants generated by phase modulation to synthesize singing voices. In this chapter we'll establish a general framework for building harmonic spectra with desired, possibly time-varying, formants.

1. Carrier/modulator model

Earlier we saw how to use ring modulation to modify the spectrum of a peri- odic signal, placing spectral peaks in speci¯ed locations (see Figure 5.4, Page 125). To do so we need to be able to generate periodic signals whose spectra have maxima at DC and fall o®monotonically with increasing frequency. If we can make a signal with a formant at frequency zero|and no other formants besides that one|we can use ring modulation to displace the formant to any desired harmonic. If we use waveshaping to generate the initial formant, the ring modulation product will be of the form

x[n] = cos(!cn)f (a cos(!mn))

where !c (the carrier frequency) is set to the formant center frequency and f (a¢ cos(!mn)) is a signal with fundamental frequency determined by !m, produced

6\.1. CARRIER/MODULATOR MODEL 149

modulation frequency

1  -1 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.255.png)

index of modulation

1  

carrier

frequency

-1  1  

-1 

OUT

Figure 6.2: Ring modulated waveshaping for formant generation

using a waveshaping function f and index a. This second term is the signal we wish to give a formant at DC with a controllable bandwidth. A block diagram for synthesizing this signal is shown in Figure 6.2.

Much earlier in Section 2.4 we introduced the technique of timbre stretching, as part of the discussion of wavetable synthesis. This technique, which is capable ofgenerating complex, variable timbres, can be ¯t into the same framework. The enveloped wavetable output for one cycle is:

x(Á) = T(cÁ) ¤ W(aÁ);

where Á, the phase, satis¯es ¡¼ · Á · ¼. Here T is a function stored in a wavetable, W is a windowing function, and c and a are the wavetable stretching and a modulation index for the windowing function. Figure 6.3 shows how to realize this in block diagram form. Comparing this to Figure 2.7, we see that the only signi¯cant new feature is the addition of the index a.

In this setup, as in the previous one, the ¯rst term speci¯es the placement of energy in the spectrum|in this case, with the parameter c acting to stretch out the wavetable spectrum. This is the role that was previously carried out by the choice of ring modulation carrier frequency !c.

Both of these (ring modulated waveshaping and stretched wavetable synthe-

2. PULSE TRAINS 158

frequency 1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.256.png)

-1 

stretch index 1   1  

0  

-1 

-M  M   -N  N  

OUT

Figure 6.3: Wavetable synthesis generalized as a variable spectrum generator.

sis) can be considered as particular cases of a more general approach which is to compute functions of the form,

x[n] = c(!n)ma (!n)

where c is a periodic function describing the carrier signal, and ma is a periodic modulator function which depends on an index a. The modulation functions we're interested in will usually take the form of pulse trains, and the index a will control the width of the pulse; higher values of a will give narrower pulses. In the wavetable case, the modulation function must reach zero at phase wraparound points to suppress any discontinuities in the carrier function when the phase wraps around. The carrier signal will give rise to a single spectral peak (a formant) in the ring modulated waveshaping case; for wavetables, it may have a more complicated spectrum.

In the next section we will further develop the two forms of modulating signal we've introduced here, and in the following one we'll look more closely at the carrier signal.

2. Pulse trains

Pulse trains may be generated either using the waveshaping formulation or the stretched wavetable one. The waveshaping formulation is easier to analyze and control, and we'll consider it ¯rst.

1. Pulse trains via waveshaping

When we use waveshaping the shape of the formant is determined by a modu- lation term

ma[n] = f (a cos(!n))

For small values of the index a, the modulation term varies only slightly from the constant value f (0), so most of the energy is concentrated at DC. As a increases, the energy spreads out among progressively higher harmonics ofthe fundamental !. Depending on the function f , this spread may be orderly or disorderly. An orderly spread may be desirable and then again may not, depending on whether our goal is a predictable spectrum or a wide range of di®erent (and perhaps hard-to-predict) spectra.

The waveshaping function f (x) = ex , analyzed on Page 140, gives well- behaved, simple and predictable results. After normalizing suitably, we got the spectra shown in Figure 5.13. A slight rewriting of the waveshaping modulator for this choice of f (and taking the renormalization into account) gives:

ma[n] = ea¢(cos(!n)¡1))

- e¡[b sin !2 ]2![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.257.png)

where b2 = 2a so that bis proportional to the bandwidth. This can be rewritten as

ma [n] = g(bsin !2 n)

with

g(x) = e¡x2

Except for a missing normalization factor, this is a Gaussian distribution, some- times called a \bell curve". The amplitudes of the harmonics are given by Bessel \I" type functions.

Another ¯ne choice is the (again unnormalized) Cauchy distribution:

1 h(x) =

1 + x2

which gives rise to a spectrum of exponentially falling harmonics:

µ ¶ h(bsin(! n)) = G ¢ 1 + H cos(!n) + H 2 cos(2!n) + ¢¢¢

2 2

where G and H are functions of the index b (explicit formulas are given in [Puc95a]).

In both this and the Gaussian case above, the bandwidth (counted in peaks, i.e., units of !) is roughly proportional to the index b, and the amplitude of the DC term (the apex of the spectrum) is roughly proportional to 1=(1 + b) . For either waveshaping function (g or h), if bis larger than about 2, the waveshape of ma(!n) is approximately a (forward or backward) scan of the transfer function, so the resulting waveform looks like pulses whose widths decrease as the speci¯ed bandwidth increases.

2. Pulse trains via wavetable stretching

In the wavetable formulation, a pulse train can be made by a stretched wavetable: Ma(Á) = W(aÁ);

where ¡¼· Á· ¼ is the phase, i.e., the value !n wrapped to lie between ¡¼ and ¼. The function W should be zero at and beyond the points ¡¼and ¼, and rise to a maximum at 0. A possible choice for the function W is

1

W(Á) = (cos(Á) + 1)

2

which is graphed in part (a) of Figure 6.4. This is known as the Hann window function ; it will come up again in Chapter 9.

Realizing this as a repeating waveform, we get a succession of (appropriately sampled) copies of the function W, whose duty cycle is 1=a (parts b and c of the ¯gure). If you don't wish the copies to overlap the index a must be at least 1. If you want to allow overlap the simplest strategy is to duplicate the block diagram (Figure 6.3) out of phase, as described in Section 2.4 and realized in Section 2.6.

(a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.258.png)

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.259.png)

(c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.260.png)

Figure 6.4: Pulse width modulation using the von Hann window function: (a) the function W(Á) = (1 + cos(Á))=2; (b) the function as a waveform, repeated at a duty cycle of 100% (modulation index a = 1); (c) the waveform at a 50% duty cycle (a = 2).

(a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.261.png)

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.262.png)

Figure 6.5: Audio signals resulting from multiplying a cosine (partial number 6) by pulse trains: (a) windowing function from the wavetable formulation; (b) waveshaping output using the Cauchy lookup function.

3. Resulting spectra

Before considering more complicated carrier signals to go with the modulators we've seen so far, it is instructive to see what multiplication by a pure sinusoid gives us as waveforms and spectra. Figure 6.5 shows the result of multiplying two di®erent pulse trains by a sinusoid at the sixth partial:

cos(6!n)Ma (!n)

where the index of modulation a is two in both cases. In part (a) Ma is the stretched Hann windowing function; part (b) shows waveshaping via the unnor- malized Cauchy distribution. One period of each waveform is shown.

In both situations we see, in e®ect, the sixth harmonic (the carrier signal) enveloped into a wave packet centered at the middle ofthe cycle, where the phase ofthe sinusoid is zero. Changing the frequency ofthe sinusoid changes the center frequency of the formant; changing the width of the packet (the proportion of the waveform during which the sinusoid is strong) changes the bandwidth. Note that the stretched Hann window function is zero at the beginning and end of the period, unlike the waveshaping packet.

Figure 6.6 shows how the shape of the formant depends on the method of production. The stretched wavetable form (part (a) of the ¯gure) behaves well in the neighborhood of the peak, but somewhat oddly starting at four partials' distance from the peak, past which we see what are called sidelobes: spurious extra peaks at lower amplitude than the central peak. As the analysis of Section 2.4 predicts, the entire formant, sidelobes and all, stretches or contracts inversely as the pulse train is contracted or stretched in time.

Hann ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.263.png)100

80

60

40

20

Gaussian ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.264.png)100

80

60

40

20

2. PULSE TRAINS 

100 80 60 40

amplitude

20 (dB)

Cauchy

0  2  4  6  ...![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.265.png)

2. PULSE TRAINS 

partial number

Figure 6.6: Spectra of three ring-modulated pulse trains: (a) the von Hann window function, 50% duty cycle (corresponding to an index of 2); (b) a wave- shaping pulse train using a Gaussian transfer function; (c) the same, with a Cauchy transfer function. Amplitudes are in decibels.


The ¯rst, strongest sidelobes on either side are about 32 dB lower in ampli- tude than the main peak. Further sidelobes drop o®slowly when expressed in decibels; the amplitudes decrease as the square of the distance from the center peak so that the sixth sidelobe to the right, three times further than the ¯rst one from the center frequency, is about twenty decibels further down. The e®ect of these sidelobes is often audible as a slight buzziness in the sound.

This formant shape may be made arbitrarily fat (i.e., high bandwidth), but there is a limit on how thin it can be made, since the duty cycle of the waveform cannot exceed 100%. At this maximum duty cycle the formant strength drops to zero at two harmonics' distance from the center peak. If a still lower bandwidth is needed, waveforms may be made to overlap as described in Section 2.6.

Parts (b) and (c) of the ¯gure show formants generated using ring modu- lated waveshaping, with Gaussian and Cauchy transfer functions. The index of modulation is two in both cases (the same as for the Hann window of part a), and the bandwidth is comparable to that of the Hann example. In these examples there are no sidelobes, and moreover, the index of modulation may be dropped all the way to zero, giving a pure sinusoid; there is no lower limit on bandwidth. On the other hand, since the waveform does not reach zero at the ends of a cycle, this type of pulse train cannot be used to window an arbitrary wavetable, as the Hann pulse train could.

The Cauchy example is particularly handy for designing spectra, since the shape of the formant is a perfect isosceles triangle, when graphed in decibels. On the other hand, the Gaussian example gathers more energy toward the formant, and drops o® faster at the tails, and so has a cleaner sound and o®ers better protection against foldover.

3. Movable ring modulation

We turn now to the carrier signal, seeking ways to make it more controllable. We would particularly like to be able to slide the spectral energy continuously up and down in frequency. Simply ramping the frequency of the carrier oscillator will not accomplish this, since the spectra won't be harmonic except when the carrier is an integer multiple of the fundamental frequency.

In the stretched wavetable approach we can accomplish this simply by sam- pling a sinusoid and transposing it to the desired \pitch". The transposed pitch isn't heard as a periodicity since the wavetable itself is read periodically at the fundamental frequency. Instead, the sinusoid is transposed as a spectral envelope.

Figure 6.7 shows a carrier signal produced in this way, tuned to produce a formant centered at 1.5 times the fundamental frequency. The signal has no outright discontinuity at the phase wraparound frequency, but it does have a discontinuity in slope, which, if not removed by applying a suitable modulation signal, would have very audible high-frequency components.

Using this idea we can make a complete description of how to use the block diagram of Figure 6.3 to produce a desired formant. The wavetable lookup on

6\.3. MOVABLE RING MODULATION 157

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.266.png)

Figure 6.7: Waveform for a wavetable-based carrier signal tuned to 1.5 times the fundamental. Two periods are shown.

the left hand side would hold a sinusoid (placed symmetrically so that the phase is zero at the center of the wavetable). The right-hand-side wavetable would hold a Hann or other appropriate window function. If we desire the fundamental frequency to be !, the formant center frequency to be !c, and the bandwidth to be !b, we set the \stretch" parameter to the center frequency quotient de¯ned as !c=!, and the index of modulation to the bandwidth quotient, !b=!.

The output signal is simply a sample of a cosine wave at the desired center frequency, repeated at the (unrelated in general) desired period, and windowed to take out the discontinuities at period boundaries.

Although we aren't able to derive this result yet (we will need Fourier anal- ysis), it will turn out that, in the main lobe of the formant, the phases are all zero at the center of the waveform (i.e., the components are all cosines if we con- sider the phase to be zero at the center of the waveform). This means we may superpose any number of these formants to build a more complex spectrum and the amplitudes of the partials will combine by addition. (The sidelobes don't behave so well: they are alternately of opposite sign and will produce cancella- tion patterns; but we can often just shrug them o®as a small, uncontrollable, residual signal.)

This method leads to an interesting generalization, which is to take a se- quence of recorded wavetables, align all their component phases to those of cosines, and use them in place of the cosine function as the carrier signal. The phase alignment is necessary to allow coherent cross-fading between samples so that the spectral envelope can change smoothly. If, for example, we use succes- sive snippets of a vocal sample as input, we get a strikingly e®ective vocoder; see Section 9.6.

Another technique for making carrier signals that can be slid continuously up and down in frequency while maintaining a fundamental frequency is simply to cross-fade between harmonics. The carrier signal is then:

c(Á) = c(!n) = pcos(k!n) + qcos((k + 1)!n) where p + q = 1 and k is an integer, all three chosen so that (k + q) ¤ ! = !c

4. PHASE-ALIGNED FORMANT (PAF) GENERATOR 164

so that the spectral center of mass of the two cosines is placed at !c. (Note that we make the amplitudes of the two cosines add to one instead of setting the total power to one; we do this because the modulator will operate phase- coherently on them.) To accomplish this we simply set k and q to be the integer and fractional part, respectively, of the center frequency quotient !c=!.

The simplest way of making a control interface for this synthesis technique would be to use ramps to update ! and !c, and then to compute q and k as audio signals from the ramped, smoothly varying ! and !c. Oddly enough, despite the fact that k, p, and q are discontinuous functions of !c=!, the carrier c(Á) turns out to vary continuously with !c=!, and so if the desired center frequency !c is ramped from value to value the result is a continuous sweep in center frequency. However, more work is needed if discontinuous changes in center frequency are needed. This is not an unreasonable thing to wish for, being analogous to changing the frequency of an oscillator discontinuously.

There turns out to be a good way to accomodate this. The trick to updating k and q is to note that c(Á) = 1 whenever Áis a multiple of 2¼, regardless of the choice of k, p, and q as long as p + q = 1. Hence, we may make discontinuous changes in k, p, and q once per period (right when the phase is a multiple of 2¼), without making discontinuities in the carrier signal.

In the speci¯c case of FM, if we wish we can now go back and modify the original formulation to:

pcos(n!2t + r cos(!1t))+ +qcos((n + 1)!2t + r cos(!1t))

This allows us to add glissandi (which are heard as dipthongs) to Chowning's original phase-modulation-based vocal synthesis technique.

4. Phase-aligned formant (PAF) generator

Combining the two-cosine carrier signal with the waveshaping pulse generator gives the phase-aligned formant generator, usually called by its acronym, PAF. (The PAF is the subject of a 1994 patent owned by IRCAM.) The combined formula is,

x[n] = g(a sin(!n=2)) [pcos(k!n) + qcos((k + 1)!n)]

| {z } | {z }![ref1]![ref1]![ref2]![ref2]

modulator carrier

Here the function g may be either the Gaussian or Cauchy waveshaping function,

- is the fundamental frequency, a is a modulation index controlling bandwidth, and k, p, and q control the formant center frequency.

  Figure 6.8 shows the PAF as a block diagram, separated into a phase gen- eration step, a carrier, and a modulator. The phase generation step outputs a sawtooth signal at the fundamental frequency. The modulator is done by stan- dard waveshaping, with a slight twist added. The formula for the modulator

phase generator

fundamental frequency![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.269.png)

phase

trigger

S/H

1  0  

modulator carrier

k   k+1

WRAP WRAP

0   1  

b  

0   1  0   1  p   q  

-10 10 

OUT

Figure 6.8: The PAF generator as a block diagram.

signals in the PAF call for an incoming sinusoid at half the fundamental fre- quency, i.e., sin( ! ), and this nominally would require us to use a phasor tuned

2

to half the fundamental frequency. However, since the waveshaping function is even, we may substitute the absolute value of the sinusoid:

¯¯¯sin( ! )¯¯ ¯

2

which repeats at the frequency ! (the ¯rst half cycle is the same as the second one.) We can compute this simply by using a half-cycle sinusoid as a wavetable lookup function (with phase running from ¡¼=2 to ¼=2), and it is this recti¯ed sinusoid that we pass to the waveshaping function.

Although the wavetable function is pictured over both negative and positive values (reaching from -10 to 10), in fact we're only using the positive side for lookup, ranging from 0 to b, the index of modulation. If the index of modulation exceeds the input range of the table (here set to stop at 10 as an example), the table lookup address should be clipped. The table should extend far enough into the tail of the waveshaping function so that the e®ect of clipping is inaudible.

The carrier signal is a weighted sum of two cosines, whose frequencies are increased by multiplication (by k and k+ 1, respectively) and wrapping. In this way all the lookup phases are controlled by the same sawtooth oscillator.

The quantities k, q, and the wavetable index b are calculated as shown in Figure 6.9. They are functions of the speci¯ed fundamental frequency, the formant center frequency, and the bandwidth, which are the original parameters of the algorithm. The quantity p, not shown in the ¯gure, is just 1 ¡ q.

As described in the previous section, the quantities k, p, and q should only change at phase wraparound points, that is to say, at periods of 2¼=!. Since the calculation of k, etc., depends on the value of the parameter !, it follows that

- itself should only be updated when the phase is a multiple of 2¼; otherwise, a change in ! could send the center frequency (k + q)! to an incorrect value for a (very audible) fraction of a period. In e®ect, all the parameter calculations should be synchronized to the phase of the original oscillator.

  Having the oscillator's phase control the updating of its own frequency is an example of feedback, which in general means using any process's output as one of its inputs. When processing digital audio signals at a ¯xed sample rate (as we're doing), it is never possible to have the process's current output as an input, since at the time we would need it we haven't yet calculated it. The best we can hope for is to use the previous sample of output|in e®ect, adding one sample of delay. In block environments (such as Max, Pd, and Csound) the situation becomes more complicated, but we will delay discussing that until the next chapter (and simply wish away the problem in the examples at the end of this one).

  The amplitude of the central peak in the spectrum of the PAF generator is roughly 1=(1 + b); in other words, close to unity when the index b is smaller than one, and falling o® inversely with larger values of b. For values of b less than about ten, the loudness of the output does not vary greatly, since the introduction of other partials, even at lower amplitudes, o®sets the decrease of

center

frequencyfrequencyfundamental bandwidthfundamental![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.270.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.271.png)

frequency

phase

phase trigger

trigger S/H

S/H

WRAP b  

q  

k  

Figure 6.9: Calculation of the time-varying parameters a (the waveshaping in- dex), k, and q for use in the block diagram of Figure 6.8.

the center partial's amplitude. However, if using the PAF to generate formants with speci¯ed peak amplitudes, the output should be multiplied by 1 + b (or even, if necessary, a better approximation of the correction factor, whose exact value depends on the waveshaping function). This amplitude correction should be ramped, not sampled-and-held.

Since the expansion of the waveshaping (modulator) signal consists of all co- sine terms (i.e., since they all have initial phase zero), as do the two components of the carrier, it follows from the cosine product formula that the components of the result are all cosines as well. This means that any number of PAF gen- erators, if they are made to share the same oscillator for phase generation, will all be in phase and combining them gives the sum of the individual spectra. So we can make a multiple-formant version as shown in Figure 6.10.

Figure 6.12 shows a possible output of a pair of formants generated this way; the ¯rst formant is centered halfway between partials 3 and 4, and the second at partial 12, with lower amplitude and bandwidth. The Cauchy waveshaping function was used, which makes linearly sloped spectra (viewed in dB). The two superpose additively, so that the spectral envelope curves smoothly from one formant to the other. The lower formant also adds to its own re°ection about the vertical axis, so that it appears slightly curved upward there.

The PAF generator can be altered if desired to make inharmonic spectra by sliding the partials upward or downward in frequency. To do this, add a second oscillator to the phase ofboth carrier cosines, but not to the phase ofthe modula-

5. EXAMPLES 172

fundamental frequency

phase generation![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.272.png)

k1, k2, b1  p1, q1 b2  p2, q2

modulator 1 carrier 1 modulator 2 carrier 2

OUT

Figure 6.10: Block diagram for making a spectrum with two formants using the PAF generator.

. 100 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.273.png)

80 

ampli- tude 60 (dB) 

40 20 

0  2  4  6  ...

partial number

Figure 6.11: Spectrum from a two-formant PAF generator.

tion portion of the diagram, nor to the controlling phase of the sample-and-hold units. It turns out that the sample-and-hold strategy for smooth parameter up- dates still works; and furthermore, multiple PAF generators sharing the same phase generation portion will still be in phase with each other.

This technique for superposing spectra does not work as predictably for phase modulation as it does for the PAF generator; the partials of the phase modulation output have complicated phase relationships and they seem di±cult to combine coherently. In general, phase modulation will give more complicated patterns of spectral evolution, whereas the PAF is easier to predict and turn to speci¯c desired e®ects.

5. Examples

Wavetable pulse train

Example F01.pulse.pd (Figure 6.13) generates a variable-width pulse train using stretched wavetable lookup. Figure 6.14 shows two intermediate products of the patch and its output. The patch carries out the job in the simplest possible way, placing the pulse at phase ¼ instead of phase zero; in later examples this will be ¯xed by adding 0.5 to the phase and wrapping.

The initial phase is adjusted to run from -0.5 to 0.5 and then scaled by a multiplier of at least one, resulting in the signal of Figure 6.14 (part a); this corresponds to the output of the \*~ object, ¯fth from bottom in the patch shown. The graph in part (b) shows the result of clipping the sawtooth wave back to the interval between ¡0:5 and 0:5, using the clip~ object. If the scaling multiplier were at its minimum (one), the sawtooth would only range from -0.5

. 100 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.274.png)

80 

ampli- tude 60 (dB) 

40 20 

0  2  4  6  ...

partial number

Figure 6.12: Spectrum from a two-formant PAF generator.

to 0.5 anyway and the clipping would have no e®ect. For any value of the scaling multiplier greater than one, the clipping output sits at the value -0.5, then ramps to 0.5, then sits at 0.5. The higher the multiplier, the faster the waveform ramps and the more time it spends clipped at the bottom and top.

The cos~ object then converts this waveform into a pulse. Inputs of both -0.5 and 0.5 go to -1 (they are one cycle apart); at the midpoint of the waveform, the input is 0 and the output is thus 1. The output therefore sits at -1, traces a full cycle of the cosine function, then comes back to rest at -1. The proportion of time the waveform spends tracing the cosine function is one divided by the multiplier; so it's 100% for a multiplier of 1, 50% for 2, and so on. Finally, the pulse output is adjusted to range from 0 to 1 in value; this is graphed in part (c) of the ¯gure.

Simple formant generator

The next three examples demonstrate the sound of the varying pulse width, graph its spectrum, and contrast the waveshaping pulse generator. Skipping to Example F05.ring.modulation.pd (Figure 6.15), we show the simplest way of combining the pulse generator with a ring modulating oscillator to make a formant. The pulse train from the previous example is contained in the pd pulse-train subpatch. It is multiplied by an oscillator whose frequency is controlled as a multiple of the fundamental frequency. If the multiple is an integer, a harmonic sound results. No attempt is made to control the relative phases of the components of the pulse train and of the carrier sinusoid.

The next example, F06.packets.pd (Figure 6.16), shows how to combine the stretched wavetable pulse train with a sampled sinusoid to realize movable formants, as described in Section 6.3. The pulse generator is as before, but now

0   <-frequency![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.275.png)

phasor~

-~ 0.5 0-centered sawtooth

0  <-index

/ 10 ...in tenths pack 0 50

line~ smooth it +~ 1 add 1

\*~ increase amplitude of sawtooth

clip~ -0.5 0.5 clip to range -1/2 to 1/2 cos~ cosine wave lookup (-1/2 and 1/2 give -1) +~ 1 add one (range now from 0 to 2)

\*~ 0.5 ...and now from 0 to 1

|  

(OUT)

Figure 6.13: Example patch F01.pulse.pd, which synthesizes a pulse train using stretched wavetable lookup.

phase![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.276.png)

(a)

0\.5 -0.5

clipped

2) 0.5![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.277.png)

-0.5 output

1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.278.png)

(c)

0  

Figure 6.14: Intermediate audio signals from Figure 6.13: (a) the result of multiplying the phasor by the \index"; (b) the same, clipped to lie between -0.5 and 0.5; (c) the output.

RING MODULATED PULSE TRAINS

0  <-- bandwidth![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.279.png)

pd pulse-train pulse train

generator from before

0   <-- carrier frequency as

multiple of fundamental

* r freq

osc~ carrier oscillator

\*~ |  (OUT)

Figure 6.15: Excerpt from example F05.ring.modulation.pd combining ring modulation with a stretched wavetable pulse generator

the carrier signal is a broken sinusoid. Since its phase is the fundamental phase times the center frequency quotient, the sample-to-sample phase increment is the same as for a sinusoid at the center frequency. However, when the phase wraps around, the carrier phase jumps to a di®erent place in the cycle, as was illustrated in Figure 6.7. Although the bandwidth quotient !b=! must be at least one, the center frequency quotient !c=! may be as low as zero if desired.

Two-cosine carrier signal

Example F08.two.cosines.pd (Figure 6.17) shows how to make a carrier sig- nal that cross-fades between harmonics to make continuously variable center frequencies. The center frequency quotient appears as the output of a line~ object. This is separated into its fractional part (using the wrap~ object) and its integer part (by subtracting the fractional part from the original). These are labeled as q and k to agree with the treatment in Section 6.3.

The phase|a sawtooth wave at the fundamental frequency|is multiplied by both k and k+ 1 (the latter by adding the original sawtooth into the former), and the cosines of both are taken; they are therefore at k and k + 1 times the fundamental frequency and have no discontinuities at phase wrapping points. The next several objects in the patch compute the weighted sum pc1 + qc2, where c1, c2 are the two sinusoids and p = 1 ¡ q, by evaluating an equivalent expression, c1 + q(c2 ¡ c1). This gives us the desired movable-frequency carrier signal.

Example F09.declickit.pd (not shown here) shows how, by adding a samphold~

center (frequency) frequency

|  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.280.png)

(as multiple of phasor~ 100

fundamental) -~ 0.5 |  

\*~ 

bandwidth

(as multiple of magnified fundamental) phase signal

|  

\*~ 

clip~ -0.5 0.5

cos~ raised

+~ 1 cosine

pulse

\*~ 0.5

cos~

\*~  carrier

|  

(OUT)

Figure 6.16: Using stretched wavetable synthesis to make a formant with mov- able center frequency.

center frequency

(relative to fundamental)

fundamental |  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.281.png)

frequency line~

|  

phasor~ wrap~ the fractional part "q"

-~  subtract to get the integer part "k" \*~  +~  multiply phase by k and k+1

cos~ cos~ synthesize two partials "c1" and "c2"

-~  c2 - c1

\*~  q \* (c2 - c1) +~  q \* c2 + (1-q) \* c1

|  

(OUT)

Figure 6.17: Cross-fading between sinusoids to make movable center frequencies.

object after the line~ object controlling center frequency, you can avoid dis- continuities in the output signal even if the desired center frequency changes discontinuously. In the example the center frequency quotient alternates be- tween 4 and 13.5. At ramp times below about 20 msec there are audible arti- facts when using the line~ object alone which disappear when the samphold~ object is added. (A disadvantage of sample-and-holding the frequency quotient is that, for very low fundamental frequencies, the changes can be heard as dis- crete steps. So in situations where the fundamental frequency is low and the center frequency need not change very quickly, it may be better to omit the sample-and-hold step.)

The next two examples demonstrate using the crossfading-oscillators car- rier as part of the classic two-operator phase modulation technique. The same modulating oscillator is added separately to the phases of the two cosines. The resulting spectra can be made to travel up and down in frequency, but because of the complicated phase relationships between neighboring peaks in the phase modulation spectrum, no matter how you align two such spectra you can never avoid getting phase cancellations where they overlap.

The PAF generator

Example F12.paf.pd (Figure 6.18) is a realization of the PAF generator, de- scribed in Section 6.4. The control inputs specify the fundamental frequency, the center frequency, and the bandwidth, all in \MIDI" units. The ¯rst steps taken in the realization are to divide center frequency by fundamental (to get the center frequency quotient) and bandwidth by fundamental to get the index of modulation for the waveshaper. The center frequency quotient is sampled- and-held so that it is only updated at periods of the fundamental.

The one oscillator (the phasor~ object) runs at the fundamental frequency. This is used both to control a samphold~ object which synchronizes updates to the center frequency quotient (labeled \C.F. relative to fundamental" in the ¯gure), and to compute phases for both cos~ objects which operate as shown earlier in Figure 6.17.

The waveshaping portion of the patch uses a half period of a sinusoid as a lookup function (to compensate for the frequency doubling because of the symmetry of the lookup function). To get a half-cycle of the sine function we multiply the phase by 0.5 and subtract 0.25, so that the adjusted phase runs from -0.25 to +0.25, once each period. This scans the positive half of the cycle de¯ned by the cos~ object.

The amplitude ofthe half-sinusoid is then adjusted by an index ofmodulation (which is just the bandwidth quotient !b=!). The table (\bell-curve") holds an unnormalized Gaussian curve sampled from -4 to 4 over 200 points (25 points per unit), so the center of the table, at point 100, corresponds to the central peak of the bell curve. Outside the interval from -4 to 4 the Gaussian curve is negligibly small.

Figure 6.19 shows how the Gaussian wavetable is prepared. One new control object is needed:


center frequency

0 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.282.png)fundamental

(MIDI units) mtof

0 pack 0 50 bandwidth mtof line~ 0

expr 1/$f1 mtof

\*~  pack 0 50 phasor~ C.F. relative line~

to fundamental divide by \*~ 0.5 \*~  fundamental

samphold~

-~ 0.25

-~  wrap~ cos~ \*~ 25

\*~  +~  \*~  range for table cos~ cos~

offset to middle +~ 100

-~  of table

tabread4~ bell-curve

+~  \*~ 

waveshaper

\*~  ring mod

|  

(OUT)

Figure 6.18: The phase-aligned formant (PAF) synthesis algorithm.


6\.5. EXAMPLES

t b b![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.283.png)

until 0  

f   + 1 sel 199 t f f

expr ($f1-100)/25 expr exp(-$f1\*$f1) tabwrite bell-curve

171

bell-curve

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.284.png)


Figure 6.19: Filling in the wavetable for Figure 6.18.

until : When the left, \start" inlet is banged, output sequential bangs (with no![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.285.png) elapsed time between them) iteratively, until the right, \stop" inlet is banged. The stopping \bang" message must originate somehow from the until object's outlet; otherwise, the outlet will send \bang" messages forever, freezing out any other object which could break the loop.

As used here, a loop driven by an until object counts from 0 to 199, inclu- sive. The loop count is maintained by the \f" and \+ 1" objects, each of which feeds the other. But since the \+ 1" object's output goes to the right inlet of the \f", its result (one greater) will only emerge from the \f" the next time it is banged by \until". So each bang from \until" increments the value by one.

The order in which the loop is started matters: the upper \t b b" object (short for \trigger bang bang") must ¯rst send zero to the \f", thus initializing it, and then set the until object sending bangs, incrementing the value, until stopped. To stop it when the value reaches 199, a select object checks the value and, when it sees the match, bangs the \stop" inlet of the until object.

Meanwhile, for every number from 0 to 199 that comes out of the \f" object, we create an ordered pair of messages to the tabwrite object. First, at right, goes the index itself, from 0 to 199. Then for the left inlet, the ¯rst expr object adjusts the index to range from -4 to 4 (it previously ranged from 0 to 199) and the second one evaluates the Gaussian function.

In this patch we have not fully addressed the issue of updating the center frequency quotient at the appropriate times. Whenever the carrier frequency is changed the sample-and-hold step properly delays the update of the quotient. But if, instead or in addition, the fundamental itself changes abruptly, then for a fraction of a period the phasor~ object's frequency and the quotient are out of sync. Pd does not allow the samphold~ output to be connected back into the

phasor~ input without the inclusion of an explicit delay (see the next chapter) and there is no simple way to modify the patch to solve this problem.

Assuming that we did somehow clock the phasor~ object's input synchronously with its own wraparound points, we would then have to do the same for the bandwidth/fundamental quotient on the right side of the patch as well. In the current scenario, however, there is no problem updating that value continuously.

A practical solution to this updating problem could be simply to rewrite the entire patch in C as a Pd class; this also turns out to use much less CPU time than the pictured patch, and is the more practical solution overall|as long as you don't want to experiment with making embellishments or other changes

to the algorithm. Such embellishments might include: adding an inharmonic upward or downward shift in the partials; allowing to switch between smooth and sampled-and-held center frequency updates; adding separate gain controls for even and odd partials; introducing gravel by irregularly modulating the phase; allowing mixtures of two or more waveshaping functions; or making sharper percussive attacks by aligning the phase of the oscillator with the timing

of an amplitude envelope generator.

One ¯nal detail about amplitude is in order: since the amplitude of the strongest partial decreases roughly as 1=(1 + b) where b is the index of modu- lation, it is sometimes (but not always) desirable to correct the amplitude of the output by multiplying by 1 + b. This is only an option if b is smoothly up- dated (as in this example), not if it is sampled-and-held. One situation in which this is appropriate is in simulating plucked strings (by setting center frequency to the fundamental, starting with a high index of modulation and dropping it exponentially); it would be appropriate to hear the fundamental dropping, not rising, in amplitude as the string decays.

Stretched wavetables

Instead of using waveshaping, fomant synthesis is also possible using stretched wavetables, as demonstrated Example F14.wave.packet.pd (not shown here). The technique is essentially that of Example B10.sampler.overlap.pd (described in Section 2.6), with a cosine lookup instead of the more general wavetable, but with the addition of a control to set the duty cycle of the amplitude envelopes. The units are adjusted to be compatible with those of the previous example.

Exercises

1. A pulse train consists of Hann windows (raised cosines), end to end, with- out any gaps between them. What is the resulting spectrum?
1. To synthesize a formant at 2000 Hertz center frequency and fundamental 300 Hertz, what should the values of k and q be (in the terminology of Figure 6.8)?

6\.5. EXAMPLES 173

3. How would you modify the block diagram of Figure 6.8 to produce only odd harmonics?




Chapter 7

Time shifts and delays

At 5:00 some afternoon, put on your favorite recording of the Ramones string quarter number 5. The next Saturday, play the same recording at 5:00:01, one second later in the day. The two playings ideally should sound the same. Shifting the whole thing one second (or, if you like, a few days and a second) has no physical e®ect on the sound.

But now suppose you played it at 5:00 and 5:00:01 on the same day (on two di®erent playback systems, since the music lasts much longer than one second). Now the sound is much di®erent. The di®erence, whatever it is, clearly resides in neither of the two individual sounds, but rather in the interference between the two. This interference can be perceived in at least four di®erent ways:

Canons: Combining two copies of a signal with a time shift su±cient for the

signal to change appreciably, we might hear the two as separate musical streams, in e®ect comparing the signal to its earlier self. If the signal is a melody, the time shift might be comparable to the length of one or several notes.

Echos: At time shifts between about 30 milliseconds and about a second, the

later copy of the signal can sound like an echo of the earlier one. An echo may reduce the intelligibility of the signal (especially if it consists of speech), but usually won't change the overall \shape" of melodies or phrases.

Filtering: At time shifts below about 30 milliseconds, the copies are too close

together in time to be perceived separately, and the dominant e®ect is that some frequencies are enhanced and others suppressed. This changes the spectral envelope of the sound.

Altered room quality: If the second copy is played more quietly than the ¯rst,

and especially if we add many more delayed copies at reduced amplitudes, the result can mimic the echos that arise in a room or other acoustic space.

175

b  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.286.png)

Z=a+bi |Z|

arg(Z)

a  

Figure 7.1: A number, Z, in the complex plane. The axes are for the real part a and the imaginary part b.

The sound of a given arrangement of delayed copies of a signal may combine two or more of these a®ects.

Mathematically, the e®ect of a time shift on a signal can be described as a phase change of each of the signal's sinusoidal components. The phase shift of each component is di®erent depending on its frequency (as well as on the amount of time shift). In the rest of this chapter we will often consider superpositions of sinusoids at di®erent phases. Heretofore we have been content to use real- valued sinusoids in our analyses, but in this and later chapters the formulas will become more complicated and we will need more powerful mathematical tools to manage them. In a preliminary section of this chapter we will develop the additional background needed.

1. Complex numbers

Complex numbers are written as:

Z = a + bi

p ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.287.png)

where a and b are real numbers and i = ¡1. (In this book we'll use the upper case Roman letters such as Z to denote complex numbers. Real numbers appear as lower case Roman or Greek letters, except for integer bounds, usually written as M or N.) Since a complex number has two real components, we use a Cartesian plane (in place of a number line) to graph it, as shown in Figure 7.1. The quantities a and b are called the real and imaginary parts of Z, written as:

a = re(Z) b= im(Z)

1. COMPLEX NUMBERS 177

If Z is a complex number, its magnitude (or absolute value), written as jZj, is just the distance in the plane from the origin to the point (a; b):

p ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.288.png)

jZj = (a2 + b2)

and its argument, written as 6 (Z), is the angle from the positive a axis to the ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.289.png)point (a; b): µ ¶

b

6 (Z) = arctan![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.290.png)

a

If we know the magnitude and argument of a complex number (call them r and µ) we can reconstruct the real and imaginary parts:

a = r cos(µ) b= r sin(µ)

A complex number may be written in terms of its real and imaginary parts a and b, as Z = a + bi (this is called rectangular form), or alternatively in polar form, in terms of r and µ:

Z = r ¢[cos(µ) + i sin(µ)]

The rectangular and polar formulations are interchangeable; the equations above show how to compute a and b from r and µ and vice versa.

The main reason we use complex numbers in electronic music is because they magically automate trigonometric calculations. We frequently have to add angles together in order to talk about the changing phase of an audio signal as time progresses (or as it is shifted in time, as in this chapter). It turns out that, if you multiply two complex numbers, the argument of the product is the sum of the arguments of the two factors. To see how this happens, we'll multiply two numbers Z1 and Z2, written in polar form:

Z1 = r1 ¢[cos(µ1) + i sin(µ1)] Z2 = r2 ¢[cos(µ2) + i sin(µ2)]

giving:

Z1Z2 = r1r2 ¢[cos(µ1) cos(µ2) ¡ sin(µ1) sin(µ2) +

+i (sin(µ1) cos(µ2) + cos(µ1) sin(µ2))]

Here the minus sign in front of the sin(µ1) sin(µ2) term comes from multiplying i

by itself, which gives ¡1. We can spot the cosine and sine summation formulas in the above expression, and so it simpli¯es to:

Z1Z2 = r1r2 ¢[cos(µ1 + µ2) + i sin(µ1 + µ2)]

By inspection, it follows that the product Z1Z2 has magnitude r1r2 and argu- ment µ1 + µ2.

We can use this property of complex numbers to add and subtract angles (by multiplying and dividing complex numbers with the appropriate arguments) and then to take the cosine and sine of the result by extracting the real and imaginary parts.

A  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.291.png)

AZ 

AZ 2   Z  2  Z  

1  

Z  −1 

Figure 7.2: The powers of a complex number Z with jZj = 1, and the same sequence multiplied by a constant A.

7\.1.1 Complex sinusoids

Recall the formula for a (real-valued) sinusoid from Page 1:

x[n] = a cos(!n + Á)

This is a sequence of cosines of angles (called phases) which increase arithmeti- cally with the sample number n. The cosines are all adjusted by the factor a. We can now rewrite this as the real part of a much simpler and easier to manip- ulate sequence of complex numbers, by using the properties of their arguments and magnitudes.

Suppose that a complex number Z happens to have magnitude one and argument !, so that it can be written as:

Z = cos(!) + i sin(!)

Then for any integer n, the number Z n must have magnitude one as well (be- cause magnitudes multiply) and argument n! (because arguments add). So,

Zn = cos(n!) + i sin(n!)

This is also true for negative values of n, so for example,

1  ¡1
- Z = cos(!) ¡ i sin(!)

Z

Figure 7.2 shows graphically how the powers of Z wrap around the unit circle, which is the set ofall complex numbers ofmagnitude one. They form a geometric sequence:

:::;Z0;Z1;Z2;:::

2. TIME SHIFTS AND PHASE CHANGES 179

and taking the real part of each term we get a real sinusoid with initial phase zero and amplitude one:

:::;cos(0);cos(!);cos(2!);:::

Furthermore, suppose we multiply the elements of the sequence by some (com- plex) constant A with magnitude a and argument Á. This gives

:::;A;AZ;AZ 2;:::

The magnitudes are all a and the argument of the nth term is n! + Á, so the sequence is equal to

AZ n = a ¢[cos(n! + Á) + i sin(n! + Á)] and the real part is just the real-valued sinusoid:

re(AZ n ) = a ¢cos(n! + Á)

The complex number A encodes both the real amplitude a and the initial phase Á; the unit-magnitude complex number Z controls the frequency which is just its argument !.

Figure 7.2 also shows the sequence A;AZ;AZ 2;:::; in e®ect this is the same sequence as 1;Z;Z 2;:::, but ampli¯ed and rotated according to the amplitude and initial phase. In a complex sinusoid of this form, A is called the complex amplitude.

Using complex numbers to represent the amplitudes and phases of sinusoids can clarify manipulations that otherwise might seem unmotivated. For instance, suppose we want to know the amplitude and phase of the sum of two sinusoids with the same frequency. In the language ofthis chapter, we let the two sinusoids be written as:

X[n] = AZ n ; Y[n] = BZ n

where A and B encode the phases and amplitudes of the two signals. The sum is then equal to:

X[n]+ Y[n] = (A + B)Z n

which is a sinusoid whose amplitude equals jA + Bj and whose phase equals 6 (A + B). This is clearly a much easier way to manipulate amplitudes and phases![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.289.png) than using properties of sines and cosines. Eventually, of course, we will take the real part of the result; this can usually be left to the end of whatever we're doing.

2. Time shifts and phase changes

Starting from any (real or complex) signal X[n], we can make other signals by time shifting the signal X by a (positive or negative) integer d:

Y[n] = X[n ¡ d]

3. DELAY NETWORKS 186

so that the dth sample of Y is the 0th sample of X and so on. If the integer d is positive, then Y is a delayed copy of X. If d is negative, then Y anticipates X; this can be done to a recorded sound but isn't practical as a real-time operation.

Time shifting is a linear operation (considered as a function of the input signal X); if you time shift a sum X1 + X2 you get the same result as if you time shift them separately and add afterward.

Time shifting has the further property that, if you time shift a sinusoid of frequency !, the result is another sinusoid of the same frequency; time shifting never introduces frequencies that weren't present in the signal before it was shifted. This property, called time invariance, makes it easy to analyze the ef- fects of time shifts|and linear combinations of them|by considering separately what the operations do on individual sinusoids.

Furthermore, the e®ectof a time shift on a sinusoid is simple: it just changes the phase. If we use a complex sinusoid, the e®ectis even simpler. If for instance

X[n] = AZ n

then

Y[n] = X[n ¡ d] = AZ (n¡d) = Z¡dAZ n = Z¡dX[n]

so time shifting a complex sinusoid by d samples is the same thing as scaling it by Z¡d|it's just an amplitude change by a particular complex number. Since

jZj = 1 for a sinusoid, the amplitude change does not change the magnitude of the sinusoid, only its phase.

The phase change is equal to ¡d!, where ! = 6 (Z) is the angular frequency of![ref3] the sinusoid. This is exactly what we should expect since the sinusoid ad- vances ! radians per sample and it is o®set (i.e., delayed) by d samples.

3. Delay networks

If we consider our digital audio samples X[n] to correspond to successive mo- ments in time, then time shifting the signal by d samples corresponds to a delay of d=R time units, where R is the sample rate. Figure 7.3 shows one example of a linear delay network : an assembly of delay units, possibly with amplitude scaling operations, combined using addition and subtraction. The output is a linear function of the input, in the sense that adding two signals at the input is the same as processing each one separately and adding the results. More- over, linear delay networks create no new frequencies in the output that weren't present in the input, as long as the network remains time invariant, so that the gains and delay times do not change with time.

In general there are two ways of thinking about delay networks. We can think in the time domain, in which we draw waveforms as functions of time (or of the index n), and consider delays as time shifts. Alternatively we may think in the frequency domain, in which we dose the input with a complex sinusoid (so that its output is a sinusoid at the same frequency) and report the amplitude and/or phase change wrought by the network, as a function of the frequency.

IN 

d  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.293.png)

OUT

Figure 7.3: A delay network. Here we add the incoming signal to a delayed copy of itself.

We'll now look at the delay network of Figure 7.3 in each of the two ways in turn.

Figure 7.4 shows the network's behavior in the time domain. We invent some sort of suitable test function as input (it's a rectangular pulse eight samples wide in this example) and graph the input and output as functions of the sample number n. This particular delay network adds the input to a delayed copy of itself.

A frequently used test function is an impulse, which is a pulse lasting only one sample. The utility of this is that, if we know the output of the network for an impulse, we can ¯nd the output for any other digital audio signal|because any signal x[n] is a sum of impulses, one of height x[0], the next one occurring one sample later and having height x[1], and so on. Later, when the networks get more complicated, we will move to using impulses as input signals to show their time-domain behavior.

On the other hand, we can analyze the same network in the frequency domain by considering a (complex-valued) test signal,

X[n] = Zn

where Z has unit magnitude and argument !. We already know that the output is another complex sinusoid with the same frequency, that is,

HZN

for some complex number H (which we want to ¯nd). So we write the output directly as the sum of the input and its delayed copy:

Zn + Z¡dZn = (1 + Z¡d)Zn

input![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.294.png)

n  

output![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.295.png)

d  

Figure 7.4: The time domain view of the delay network of Figure 7.3. The output is the sum of the input and its time shifted copy.

and ¯nd by inspection that:

H = 1 + Z¡d

We can understand the frequency-domain behavior of this delay network by studying how the complex number H varies as a function of the angluar fre- quency !. We are especially interested in its argument and magnitude|which

tell us the relative phase and amplitude of the sinusoid that comes out. We will work this example out in detail to show how the arithmetic of complex numbers can predict what happens when sinusoids are combined additively.

Figure 7.5 shows the result, in the complex plane, when the quantities 1 and Z¡d are combined additively. To add complex numbers we add their real and

complex parts separately. So the complex number 1 (real part 1, imaginary part 0) is added coordinate-wise to the complex number Z ¡d (real part cos(¡d!), imaginary part sin(¡d!)). This is shown graphically by making a parallelogram, with corners at the origin and at the two points to be added, and whose fourth corner is the sum H.

As the ¯gure shows, the result can be understood by symmetrizing it about the real axis: instead of 1 and Z ¡d, it's easier to sum the quantities Z d=2 and Z¡d=2, because they are symmetric about the real (horizontal) axis. (Strictly speaking, we haven't properly de¯ned the quantities Z d=2 and Z¡d=2; we are

using those expressions to denote unit complex numbers whose arguments are half those of Z d and Z¡d, so that squaring them would give Z d and Z¡d.) We

rewrite the gain as:

H = Z¡d=2(Zd=2 + Z¡d=2)

The ¯rst term is a phase shift of ¡d!=2. The second term is best understood

Z  d/2![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.296.png)

d/2 HZ  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.297.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.298.png)

real 1   

Z  -d/2

H  -d 

imaginary Z  

Figure 7.5: Analysis, in the complex plane, of the frequency-domain behavior of the delay network of Figure 7.3. The complex number Z encodes the frequency of the input. The delay line output is the input times Z ¡d. The total (complex) gain is H. We ¯nd the magnitude and argument of H by symmetrizing the sum, rotating it by d=2 times the angular frequency of the input.

in rectangular form:

Zd=2 + Z¡d=2

- (cos(!d=2) + i sin(!d=2)) + (cos(!d=2) ¡ i sin(!d=2))
  - 2cos(!d=2)

This real-valued quantity may be either positive or negative; its absolute value gives the magnitude of the output:

jHj = 2jcos(!d=2)j

The quantity jHj is called the gain of the delay network at the angular frequency !, and is graphed in Figure 7.6. The frequency-dependent gain of a delay network (that is, the gain as a function of frequency) is called the network's frequency response.

Since the network has greater gain at some frequencies than at others, it may be considered as a ¯lter that can be used to separate certain components of a sound from others. Because of the shape of this particular gain expression as a function of !, this kind of delay network is called a (non-recirculating) comb ¯lter.

The output of the network is a sum of two sinusoids of equal amplitude, and whose phases di®er by !d. The resulting frequency response agrees with common sense: if the angular frequency ! is set so that an integer number of periods ¯t into d samples, i.e., if ! is a multiple of 2¼=d, the output of the delay is exactly the same as the original signal, and so the two combine to make an output with twice the original amplitude. On the other hand, if for example we

4. RECIRCULATING DELAY NETWORKS 190

gain![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.299.png)

2  

2   4  

d   d  

Figure 7.6: Gain of the delay network of Figure 7.3, shown as a function of angular frequency !.

take ! = ¼=d so that the delay is half the period, then the delay output is out of phase and cancels the input exactly.

This particular delay network has an interesting application: if we have a periodic (or nearly periodic) incoming signal, whose fundamental frequency is

- radians per sample, we can tune the comb ¯lter so that the peaks in the gain are aligned at even harmonics and the odd ones fall where the gain is zero. To do this we choose d = ¼=!, i.e., set the delay time to exactly one half period of the incoming signal. In this way we get a new signal whose harmonics are 2!;4!;6!;:::, and so it now has a new fundamental frequency at twice the original one. Except for a factor of two, the amplitudes of the remaining harmonics still follow the spectral envelope of the original sound. So we have a tool now for raising the pitch of an incoming sound by an octave without changing its spectral envelope. This octave doubler is the reverse of the octave divider introduced back in Chapter 5.

  The time and frequency domains o®ercomplementary ways of looking at the same delay network. When the delays inside the network are smaller than the ear's ability to resolve events in time|less than about 20 milliseconds|the time domain picture becomes less relevant to our understanding of the delay network, and we turn mostly to the frequency-domain picture. On the other hand, when delays are greater than about 50 msec, the peaks and valleys of plots showing gain versus frequency (such as that of Figure 7.6) crowd so closely together that the frequency-domain view becomes less important. Both are nonetheless valid over the entire range of possible delay times.

4. Recirculating delay networks

It is sometimes desirable to connect the outputs of one or more delays in a network back into their own or each others' inputs. Instead of getting one or several echos of the original sound as in the example above, we can potentially get an in¯nite number of echos, each one feeding back into the network to engender yet others.

IN 

OUT![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.300.png)

d  

g  

Figure 7.7: Block diagram for a recirculating comb ¯lter. Here d is the delay time in samples and g is the feedback coe±cient.

The simplest example of a recirculating network is the recirculating comb ¯lter whose block diagram is shown in Figure 7.7. As with the earlier, simple comb ¯lter, the input signal is sent down a delay line whose length is d samples. But now the delay line's output is also fed back to its input; the delay's input is the sum of the original input and the delay's output. The output is multiplied by a number g before feeding it back into its input.

The time domain behavior of the recirculating comb ¯lter is shown in Figure 7.8. Here we consider the e®ect of sending an impulse into the network. We get back the original impulse, plus a series of echos, each in turn d samples after the previous one, and multiplied each time by the gain g. In general, a delay network's output given an impulse as input is called the network's impulse response.

Note that we have chosen a gain g that is less than one in absolute value. If we chose a gain greater than one (or less than -1), each echo would have a larger magnitude than the previous one. Instead of falling exponentially as they do in the ¯gure, they would grow exponentially. A recirculating network whose output eventually falls toward zero after its input terminates is called stable; one whose output grows without bound is called unstable.

We can also analyse the recirculating comb ¯lter in the frequency domain. The situation is now quite hard to analyze using real sinusoids, and so we get the ¯rst big payo®for having introduced complex numbers, which greatly simplify the analysis.

If, as before, we feed the input with the signal,

X[n] = Zn

with jZj = 1, we can write the output as

Y[n] = (1 + gZ ¡d + g2Z¡2d + ¢¢¢)X[n]

input![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.301.png)

n  

output![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.302.png)

d  

Figure 7.8: Time-domain analysis of the recirculating comb ¯lter, using an impulse as input.

Here the terms in the sum come from the series of discrete echos. It follows that the amplitude of the output is:

H = 1 + gZ¡d + (gZ¡d)2 + ¢¢¢

This is a geometric series; we can sum it using the standard technique. First multiply both sides by gZ ¡d to give:

gZ¡dH = gZ¡d + (gZ¡d)2 + (gZ¡d)3 + ¢¢¢ and subtract from the original equation to give:

H ¡ gZ¡dH = 1

Then solve for H:

1

H =

1 ¡ gZ¡d

A faster (but slightly less intuitive) method to get the same result is to examine the recirculating network itself to yield an equation for H, as follows. We named the input X[n] and the output Y[n]. The signal going into the delay line is the output Y[n], and passing this through the delay line and multiplier gives

Y[n]¢gZ ¡d

This plus the input is just the output signal again, so:

Y[n] = X[n]+ Y[n]¢gZ ¡d

and dividing by X[n] and using H = Y[n]=X[n] gives:

H = 1 + HgZ¡d

This is equivalent to the earlier equation for H.

Now we would like to make a graph of the frequency response (the gain as a function of frequency) as we did for non-recirculating comb ¯lters in Figure 7.6. This again requires that we make a preliminary picture in the complex plane. We would like to estimate the magnitude of H equal to:

1 jHj =

j1 ¡ gZ¡dj

where we used the multiplicative property of magnitudes to conclude that the magnitude of a (complex) reciprocal is the reciprocal of a (real) magnitude. Figure 7.9 shows the situation graphically. The gain jHj is the reciprocal of the length of the segment reaching from the point 1 to the point gZ ¡d. Figure 7.10 shows a graph of the frequency response jHj as a function of the angular frequency ! = 6 (Z).![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.303.png)

Figure 7.9 can be used to analyze how the frequency response jH(!)j should behave qualitatively as a function of g. The height and bandwidth of the peaks both depend on g. The maximum value that jHj can attain is when

Z¡d = 1

This occurs at the frequencies ! = 0;2¼=d;4¼=d;::: as in the simple comb ¯lter above. At these frequencies the gain reaches

1 jHj =

1 ¡ g

The next important question is the bandwidth of the peaks in the frequency response. So we would like to ¯nd sinusoids W n , with frequency 6 (W), giving![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.304.png)

rise to a value of jHj that is, say, 3 decibels below the maximum. To do this, we return to Figure 7.9, and tryp to place W so that the distance from theppoint 1 to the point gW¡d is about 2 times the distance from 1 to g (since 2:1 is a ratio of approximately 3 decibels).

We do this by arranging for the imaginary part of gW ¡d to be roughly 1¡ g or its negative, making a nearly isosceles right triangle between the points 1, 1 ¡ g, and gW¡d. (Here we're supposing that g is at least 2/3 or so; otherwise this appropximation isn't very good). The hypotenuse of a right isosceles triangle is![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.305.png) always 2 times the leg, and so the gain drops by that factor compared to its maximum.

We now make another approximation, that the imaginary part of gW ¡d is approximately the angle in radians it cuts from the real axis:

§(1 ¡ g) ¼ im(gW¡d) ¼ 6 (W¡d)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.306.png)

5. POWER CONSERVATION AND COMPLEX DELAY NETWORKS 192

imaginary![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.307.png)

1−g

real 1  

gW −d 

−d 1−gW

gZ −d 

Figure 7.9: Diagram in the complex plane for approximating the output gain jHj of the recirculating comb ¯lters at three di®erent frequencies: 0, and the arguments of two unit complex numbers W and Z; W is chosen to give a gain about 3 dB below the peak.

gain![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.308.png)

5  

2   4  

d   d  

Figure 7.10: Frequency response of the recirculating comb ¯lter with g = 0:8. The peak gain is 1=(1 ¡ g) = 5. Peaks are much narrower than for the non- recirculating comb ¯lter.

So the region of each peak reaching within 3 decibels of the maximum value is about

(1 ¡ g)=d

(in radians) to either side of the peak. The bandwidth narrows (and the ¯lter peaks become sharper) as g approaches its maximum value of 1.

As with the non-recirculating comb ¯lter of Section 7.3, the teeth of the comb are closer together for larger values of the delay d. On the other hand, a delay of d = 1 (the shortest possible) gets only one tooth (at zero frequency) below the Nyquist frequency ¼ (the next tooth, at 2¼, corresponds again to a frequency of zero by foldover). So the recirculating comb ¯lter with d = 1 is just a low-pass ¯lter. Delay networks with one-sample delays will be the basis for designing many other kinds of digital ¯lters in Chapter 8.

7\.5 Power conservation and complex delay net-

works

The same techniques will work to analyze any delay network, although for more complicated networks it becomes harder to characterize the results, or to design the network to have speci¯c, desired properties. Another point of view can sometimes be usefully brought to the situation, particularly when °at frequency responses are needed, either in their own right or else to ensure that a complex, recirculating network remains stable at feedback gains close to one.

The central fact we will use is that if any delay network, with either one or many inputs and outputs, is constructed so that its output power (averaged over time) always equals its input power, that network has to have a °at frequency response. This is almost a tautology; if you put in a sinusoid at any frequency on one of the inputs, you will get sinusoids of the same frequency at the outputs, and the sum of the power on all the outputs will equal the power of the input, so the gain, suitably de¯ned, is exactly one.

In order to work with power-conserving delay networks we will need an explicit de¯nition of \total average power". If there is only one signal (call it x[n]), the average power is given by:

h i

P (x[n]) = jx[0]j2 + jx[1]j2 + ¢¢¢+ jx[N ¡ 1]j2 =N

where N is a large enough number so that any °uctuations in amplitude get averaged out. This de¯nition works as well for complex-valued signals as for real-valued ones. The average total power for several digital audio signals is just the sum of the individual signal's powers:

P (x1[n];:::;xr [n]) = P (x1[n]) + ¢¢¢+ P (xr [n])

where r is the number of signals to be combined.

It turns out that a wide range of interesting delay networks has the property that the total power output equals the total power input; they are called unitary.

193 CHAPTER 7. TIME SHIFTS AND DELAYS

IN 

d  1  d  2  d  3  d  4  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.309.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.310.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.311.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.312.png)

OUT

Figure 7.11: First fundamental building block for unitary delay networks: delay lines in parallel.

To start with, we can put any number of delays in parallel, as shown in Figure 7.11. Whatever the total power of the inputs, the total power of the outputs has to equal it.

A second family of power-preserving transformations is composed of rota- tions and re°ections of the signals x1[n], ... , xr [n], considering them, at each ¯xed time point n, as the r coordinates of a point in r-dimensional space. The rotation or re°ection must be one that leaves the origin (0;:::;0) ¯xed.

For each sample number n, the total contribution to the average signal power is proportional to

jx1j2 + ¢¢¢+ jxr j2

This is just the Pythagorean distance from the origin to the point (x1;:::;xr ). Since rotations and re°ections are distance-preserving transformations, the dis- tance from the origin before transforming must equal the distance from the origin afterward. So the total power of a collection of signals must must be preserved by rotation.

Figure 7.12 shows a rotation matrix operating on two signals. In part (a) the transformation is shown explicitly. If the input signals are x1[n] and x2[n], the outputs are:

y1[n] = cx1[n]¡ sx2[n] y2[n] = sx1[n]+ cx2[n]

where c;s are given by

c = cos(µ) s = sin(µ)

for an angle of rotation µ. Considered as points on the Cartesian plane, the point (y1;y2) is just the point (x1;x2) rotated counter-clockwise by the angle µ. The two points are thus at the same distance from the origin:

jy1j2 + jy2j2 = jx1j2 + jx2j2


1) (b)

IN 

IN ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.313.png)

c  -s  s  c   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.314.png)

c  -s 

s   c  

OUT

OUT

Figure 7.12: Second fundamental building block for unitary delay networks: rotating two digital audio signals. Part (a) shows the transformation explicitly;

2) shows it as a matrix operation.

and so the two output signals have the same total power as the two input signals.

For an alternative description of rotation in two dimensions, consider com- plex numbers X = x1 + x2i and Y = y1 + y2i. The above transformation amounts to setting

Y = XZ

where Z is a complex number with unit magnitude and argument µ. Since jZj = 1, it follows that jXj = jYj.

If we perform a rotation on a pair of signals and then invert one (but not the other) of them, the result is a re°ection. This also preserves total signal power, since we can invert any or all of a collection of signals without changing the total power. In two dimensions, a re°ection appears as a transformation of the form

y1[n] = cx1[n]+ sx2[n] y2[n] = sx1[n]¡ cx2[n]

A specialp and useful rotation matrix is obtained by setting µ= ¼=4, so that s = c = 1=2. This allows us to simplify the computation as shown in Figure

7\.13 (part a) because each signal need only be multiplied by the one quantity c = s.

More complicated rotations or re°ections of more than two input signals may be made by repeatedly rotating and/or re°ecting them in pairs. For example, in Figure 7.13 (part b), four signals are combined in pairs, in two successive


192

(a)

IN 

a  a  OUT![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.315.png)

CHAPTER 7. TIME SHIFTS AND DELAYS (b)

IN 

R  1   R  2  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.316.png)

R  3  

R  4  

OUT


Figure 7.13: Details about rotation (and re°ection) matrixpoperations: (a) ro- tation![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.317.png) by the angle µ = ¼=4, so that a = cos(µ) = sin(µ) = 1=2 ¼ 0:7071; (b) combining two-dimensional rotations to make higher-dimensional ones.

stages, so that in the end every signal input feeds into all the outputs. We could do the same with eight signals (using three stages) and so on. Furthermore, if we use the special angle ¼=4, all the input signals will contribute equally to each of the outputs.

Any combination of delays and rotation matrices, applied in succession to a collection of audio signals, will result in a °at frequency response, since each individual operation does. This already allows us to generate an in¯nitude of °at-response delay networks, but so far, none of them are recirculating. A third operation, shown in Figure 7.14, allows us to make recirculating networks that still enjoy °at frequency responses.

Part (a) of the ¯gure shows the general layout. The transformation R is assumed to be any combination of delays and mixing matrices that preserves total power. The signals x1;:::xk go into a unitary delay network, and the output signals y1;:::yk emerge. Some other signals w1;:::wj (where j is not necessarily equal to k) appear at the output of the transformation R and are fed back to its input.

If R is indeed power preserving, the total input power (the power of the signals x1;:::xk plus that of the signals w1;:::wj ) must equal the output power (the power ofthe signals y1;:::yk plus w1;:::wj ), and subtracting all the w from the equality, we ¯nd that the total input and output power are equal.

If we let j = k = 1 so that there is one x, y, and w, and let the transformation R be a rotation by µfollowed by a delay of d samples on the W output, the result

6. ARTIFICIAL REVERBERATION 199

(a) (b)

IN 

x  1  x  k   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.318.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.319.png)

... 

... 

R   

w  j  w   d   c  ... 1  

d  1  ...d  j  

c  

y  1  y  k  

OUT

Figure 7.14: Flat frequency response in recirculating networks: (a) in general, using a rotation matrix R; (b) the \all-pass" con¯guration.

is the well-known all-pass ¯lter. With some juggling, and letting c = cos(µ), we can show it is equivalent to the network shown in part (b) of the ¯gure. All-pass ¯lters have many applications, some of which we will visit later in this book.

6. Arti¯cial reverberation

Arti¯cial reverberation is widely used to improve the sound of recordings, but has a wide range of other musical applications [DJ85, pp.289-340]. Reverbera- tion in real, natural spaces arises from a complicated pattern of sound re°ections o® the walls and other objects that de¯ne the space. It is a great oversim- pli¯cation to imitate this process using recirculating, discrete delay networks. Nonetheless, modeling reverberation using recirculating delay lines can, with much work, be made to yield good results.

The central idea is to idealize any room (or other reverberant space) as a collection of parallel delay lines that models the memory of the air inside the room. At each point on the walls of the room, many straight-line paths terminate, each carrying sound to that point; the sound then re°ects into many other paths, each one originating at that point, and leading eventually to some other point on a wall.

Although the wall (and the air we passed through to get to the wall) absorbs some of the sound, some portion of the incident power is re°ected and makes it to another wall. If most of the energy recirculates, the room reverberates for a long time; if all of it does, the reverberation lasts forever. If at any frequency the walls re°ect more energy overall than they receive, the sound will feed back

unstably; this never happens in real rooms (conservation of energy prevents it), but it can happen in an arti¯cial reverberator if it is not designed correctly.

To make an arti¯cial reverberator using a delay network, we must ¯ll two competing demands simultaneously. First, the delay lines must be long enough to prevent coloration in the output as a result of comb ¯ltering. (Even if we move beyond the simple comb ¯lter of Section 7.4, the frequency response will tend to have peaks and valleys whose spacing varies inversely with total delay time.) On the other hand, we should not hear individual echoes; the echo density should ideally be at least one thousand per second.

In pursuit of these aims, we assemble some number of delay lines and connect their outputs back to their inputs. The feedback path|the connection from the outputs back to the inputs of the delays|should have an aggregate gain that varies gently as a function of frequency, and never exceeds one for any frequency. A good starting point is to give the feedback path a °at frequency response and a gain slightly less than one; this is done using rotation matrices.

Ideally this is all we should need to do, but in reality we will not always want to use the thousands of delay lines it would take to model the paths between every possible pair of points on the walls. In practice we usually use between four and sixteen delay lines to model the room. This simpli¯cation sometimes reduces the echo density below what we would wish, so we might use more delay lines at the input of the recirculating network to increase the density.

Figure 7.15 shows a simple reverberator design that uses this principle. The incoming sound, shown as two separate signals in this example, is ¯rst thickened by progressively delaying one of the two signals and then intermixing them using a rotation matrix. At each stage the number of echoes of the original signal is doubled; typically we would use between 6 and 8 stages to make between 64 and 256 echos, all with a total delay of between 30 and 80 milliseconds. The ¯gure shows three such stages.

Next comes the recirculating part of the reverberator. After the initial thick- ening, the input signal is fed into a bank of parallel delay lines, and their outputs are again mixed using a rotation matrix. The mixed outputs are attenuated by a gain g · 1, and fed back into the delay lines to make a recirculating network.

The value g controls the reverberation time. If the average length of the recirculating delay lines is d, then any incoming sound is attenuated by a factor of g after a time delay of d. After time t the signal has recirculated t=d times, losing 20log10 (g) decibels each time around, so the total gain, in decibels, is:

t

20 log (g) d 10

The usual measure of reverberation time (RT) is the time at which the gain drops by sixty decibels:

RT

20~~ log (g) = ¡60

d 10

¡3d

RT =

log10 (g)

IN 

R  1  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.320.png)

d  1  

R  2  

d  2  

R  3   R  9  

d  3   g  

d  7  d  8  d  9  

OUT

Figure 7.15: Reverberator design using power-preserving transformations and recirculating delays.

7. VARIABLE AND FRACTIONAL SHIFTS 203

If g is one, this formula gives 1, since the logarithm of one is zero.

The framework shown above is the basis for many modern reverberator de- signs. Many extensions of this underlying design have been proposed. The most important next step would be to introduce ¯lters in the recirculation path so that high frequencies can be made to decay more rapidly than low ones; this is readily accomplished with a very simple low-pass ¯lter, but we will not work this out here, having not yet developed the needed ¯lter theory.

In general, to use this framework to design a reverberator involves making many complicated choices of delay times, gains, and ¯lter coe±cients. Moun- tains of literature have been published on this topic; Barry Blesser has published a good overview [Ble01]. Much more is known about reverberator design and tuning that has not been published; precise designs are often kept secret for commercial reasons. In general, the design process involves painstaking and lengthy tuning by trial, error, and critical listening.

7\.6.1 Controlling reverberators

Arti¯cial reverberation is used almost universally in recording or sound rein- forcement to sweeten the overall sound. However, and more interestingly, re- verberation may be used as a sound source in its own right. The special case of in¯nite reverberation is useful for grabbing live sounds and extending them in time.

To make this work in practice it is necessary to open the input of the re- verberator only for a short period of time, during which the input sound is not varying too rapidly. If an in¯nite reverberator's input is left open for too long, the sound will collect and quickly become an indecipherable mass. To \in¯nitely reverberate" a note of a live instrument, it is best to wait until after the attack portion of the note and then allow perhaps 1/2 second of the note's steady state to enter the reverberator. It is possible to build chords from a monophonic instrument by repeatedly opening the input at di®erent moments of stable pitch.

Figure 7.16 shows how this can be done in practice. The two most important controls are the reverberator's input and feedback gains. To capture a sound, we set the feedback gain to one (in¯nite reverberation time) and momentarily open the input at time t1. To add other sounds to an already held one, we simply reopen the input gain at the appropriate moments (at time t2 in the ¯gure, for example). Finally, we can erase the recirculating sound, thus both fading the output and emptying the reverberator, by setting the feedback gain to a value less than one (as at time t3). The further we reduce the feedback gain, the faster the output will decay.

7. Variable and fractional shifts

Like any audio synthesis or processing technique, delay networks become much more powerful and interesting if their characteristics can be made to change over

IN  (a)

reverb![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.321.png)

feedback OUT

(b) input![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.322.png)

1  gain

t  1   t  2   time

feedback![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.323.png)

1  

t  3  

Figure 7.16: Controlling a reverberator to capture sounds selectively: (a) the network; (b) examples of how to control the input gain and feedback to capture two sounds at times t1 and t2, and to hold them until a later time t3.

time. The gain parameters (such as g in the recirculating comb ¯lter) may be controlled by envelope generators, varying them while avoiding clicks or other artifacts. The delay times (such as d before) are not so easy to vary smoothly for two reasons.

First, we have only de¯ned time shifts for integer values of d, since for fractional values of d an expression such as x[n ¡ d] is not determined if x[n] is only de¯ned for integer values of n. To make fractional delays we will have to introduce some suitable interpolation scheme. And if we wish to vary d smoothly over time, it will not give good results simply to hop from one integer to the next.

Second, even once we have achieved perfectly smoothly changing delay times, the artifacts caused by varying delay time become noticeable even at very small relative rates of change; while in most cases you may ramp an amplitude control between any two values over 30 milliseconds without trouble, changing a delay by only one sample out of every hundred makes a very noticeable shift in pitch| indeed, one frequently will vary a delay deliberately in order to hear the artifacts, only incidentally passing from one speci¯c delay time value to another one.

The ¯rst matter (fractional delays) can be dealt with using an interpolation scheme, in exactly the same way as for wavetable lookup (Section 2.5). For example, suppose we want a delay of d = 1:5 samples. For each n we must estimate a value for x[n ¡ 1:5]. We could do this using standard four-point interpolation, putting a cubic polynomial through the four \known" points (0, x[n]), (1, x[n-1]), (2, x[n-2]), (3, x[n-3]), and then evaluating the polynomial at the point 1.5. Doing this repeatedly for each value of n gives the delayed signal.

This four-point interpolation scheme can be used for any delay of at least one sample. Delays of less than one sample can't be calculated this way because we need two input points at least as recent as the desired delay. They were available in the above example, but for a delay time of 0.5 samples, for instance, we would need the value of x[n + 1], which is in the future.

The accuracy of the estimate could be further improved by using higher- order interpolation schemes. However, there is a trade-o® between quality and computational e±ciency. Furthermore, if we move to higher-order interpolation schemes, the minimum possible delay time will increase, causing trouble in some situations.

The second matter to consider is the artifacts|whether wanted or unwanted| that arise from changing delay lines. In general, a discontinuous change in delay time will give rise to a discontinuous change in the output signal, since it is in e®ect interrupted at one point and made to jump to another. If the input is a sinusoid, the result is a discontinuous phase change.

If it is desired to change the delay line occasionally between ¯xed delay times (for instance, at the beginnings of musical notes), then we can use the techniques for managing sporadic discontinuities that were introduced in Section 4.3. In e®ectthese techniques all work by muting the output in one way or another. On the other hand, if it is desired that the delay time change continuously|while we are listening to the output|then we must take into account the artifacts that result from the changes.

input time![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.324.png)

D   output time

Figure 7.17: A variable length delay line, whose output is the input from some previous time. The output samples can't be newer than the input samples, nor older than the length D of the delay line. The slope of the input/output curve controls the momentary transposition of the output.


Figure 7.17 shows the relationship between input and output time in a vari- able delay line. The delay line is assumed to have a ¯xed maximum length D. At each sample of output (corresponding to a point on the horizontal axis), we output one (possibly interpolated) sample of the delay line's input. The vertical axis shows which sample (integer or fractional) to use from the input signal. Letting n denote the output sample number, the vertical axis shows the quan- tity n ¡ d[n], where d[n] is the (time-varying) delay in samples. If we denote the input sample location by:

y[n] = n ¡ d[n] then the output of the delay line is:

z[n] = x[y[n]]

where the signal x is evaluated at the point y[n], interpolating appropriately in case y[n] is not an integer. This is exactly the formula for wavetable lookup (Page 27). We can use all the properties of wavetable lookup of recorded sounds to predict the behavior of variable delay lines.

There remains one di®erence between delay lines and wavetables: the ma- terial in the delay line is constantly being refreshed. Not only can we not read into the future, but, if the the delay line is D samples in length, we can't read further than D samples into the past either:

0 < d[n] < D or, negating this and adding n to each side,

n > y[n] > n ¡ D:

This last relationship appears as the region between the two diagonal lines in Figure 7.17; the function y[n] must stay within this strip.

Returning to Section 2.2, we can use the Momentary Transposition Formulas for wavetables to calculate the transposition t[n] of the output. This gives the Momentary Transposition Formula for delay lines:

t[n] = y[n]¡ y[n ¡ 1] = 1 ¡ (d[n]¡ d[n ¡ 1])

If d[n] does not change with n, the transposition factor is 1 and the sound emerges from the delay line at the same speed as it went in. But if the delay time is increasing as a function ofn, the resulting sound is transposed downward, and if d[n] decreases, upward.

This is called the Doppler e®ect, and it occurs in nature as well. The air that sound travels through can sometimes be thought of as a delay line. Changing the length of the delay line corresponds to moving the listener toward or away from a stationary sound source; the Doppler e®ect from the changing path length works precisely the same in the delay line as it would be in the physical air.

Returning to Figure 7.17, we can predict that there is no pitch shift at the beginning, but then when the slope of the path decreases the pitch will drop for

7\.8. FIDELITY OF INTERPOLATING DELAY LINES 201

an interval oftime before going back to the original pitch (when the slope returns to one). The delay time can be manipulated to give any desired transposition, but the greater the transposition, the less long we can maintain it before we run o®the bottom or the top of the diagonal region.

8. Fidelity of interpolating delay lines

Since they are in e®ect doing wavetable lookup, variable delay lines introduce distortion to the signals they operate on. Moreover, a subtler problem can come up even when the delay line is not changing in length: the frequency response, in real situations, is never perfectly °at for a delay line whose length is not an integer.

If the delay time is changing from sample to sample, the distortion results of Section 2.5 apply. To use them, we suppose that the delay line input can be broken down into sinusoids and consider separately what happens to each individual sinusoid. We can use Table 2.1 (Page 46) to predict the RMS level of the combined distortion products for an interpolated variable delay line.

We'll assume here that we want to use four-point interpolation. For sinu- soids with periods longer than 32 samples (that is, for frequencies below 1/16 of the Nyquist frequency) the distortion is 96 dB or better|unlikely ever to be noticeable. At a 44 kHz. sample rate, these periods would correspond to frequencies up to about 1400 Hertz. At higher frequencies the quality degrades, and above 1/4 the Nyquist frequency the distortion products, which are only down about 50 dB, will probably be audible.

The situation for a complex tone depends primarily on the amplitudes and frequencies of its higher partials. Suppose, for instance, that a tone's partials above 5000 Hertz are at least 20 dB less than its strongest partial, and that above 10000 Hertz they are down 60 dB. Then as a rough estimate, the distortion products from the range 5000-10000 will each be limited to about -68 dB and those from above 10000 Hertz will be limited to about -75 dB (because the worst ¯gure in the table is about -15 dB and this must be added to the strength of the partial involved.)

If the high-frequency content of the input signal does turn out to give un- acceptable distortion products, in general it is more e®ective to increase the sample rate than the number of points of interpolation. For periods greater than 4 samples, doubling the period (by doubling the sample rate, for example) decreases distortion by about 24 dB.

The 4-point interpolating delay line's frequency response is nearly °at up to half the Nyquist frequency, but thereafter it dives quickly. Suppose (to pick the worst case) that the delay is set halfway between two integers, say 1.5. Cubic interpolation gives:

¡x[0]+ 9x[1]+ 9x[2]¡ x[3]

x[1:5] =

8

Now let x[n] be a (real-valued) unit-amplitude sinusoid with angular frequency

9. PITCH SHIFTING 211

gain![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.325.png)

1  

2  

Figure 7.18: Gain of a four-point interpolating delay line with a delay halfway between two integers. The DC gain is one.

!, whose phase is zero at 1:5:

x[n] = cos(! ¢(n ¡ 1:5)) and compute x[1:5] using the above formula:

9cos(!=2) ¡ cos(3!=2) x[1:5] =

4

This is the peak value of the sinusoid that comes back out of the delay line, and since the peak amplitude going in was one, this shows the frequency re- sponse of the delay line. This is graphed in Figure 7.18. At half the Nyquist frequency (! = ¼=2) the gain is about -1 dB, which is a barely perceptible drop in amplitude. At the Nyquist frequency itself, however, the gain is zero.

As with the results for distortion, the frequency response improves radically with a doubling of sample rate. If we run our delay at a sample rate of 88200 Hertz instead of the standard 44100, we will get only about 1 dB of roll-o® all the way up to 20000 Hertz.

9. Pitch shifting

A favorite use of variable delay lines is to alter the pitch of an incoming sound using the Doppler e®ect. It may be desirable to alter the pitch variably (ran- domly or periodically, for example), or else to maintain a ¯xed musical interval of transposition over a length of time.

Returning to Figure 7.17, we see that with a single variable delay line we can maintain any desired pitch shift for a limited interval of time, but if we wish to sustain a ¯xed transposition we will always eventually land outside the diagonal strip of admissible delay times. In the simplest scenario, we simply vary the transposition up and down so as to remain in the strip.

input time![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.326.png)

output time

Figure 7.19: Vibrato using a variable delay line. Since the pitch shift alternates between upward and downward, it is possible to maintain it without drifting outside the strip of admissible delay.

input time![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.327.png)

output time

Figure 7.20: Piecewise linear delay functions to maintain a constant transpo- sition (except at the points of discontinuity). The outputs are enveloped as suggested by the bars above each point, to smooth the output at the points of discontinuity in delay time.

This works, for example, if we wish to apply vibrato to a sound as shown in Figure 7.19. Here the delay function is

d[n] = d0 + a cos(!n)

where d0 is the average delay, a is the amplitude of variation about the average delay, and ! is an angular frequency. The Momentary Transposition (Page 200), is approximately

t = 1 + a! cos(!n ¡ ¼=2)

This ranges in value between 1 ¡ a! and 1 + a!.

Suppose, on the other hand, that we wish to maintain a constant trans- position over a longer interval of time. In this case we can't maintain the transposition forever, but it is still possible to maintain it over ¯xed intervals of time broken by discontinuous changes, as shown in Figure 7.20. The delay time is the output of a suitably normalized sawtooth function, and the output of the variable delay line is enveloped as shown in the ¯gure to avoid discontinuities.

This is accomplished as shown in Figure 7.21. The output of the sawtooth generator is used in two ways. First it is adjusted to run between the bounds d0

f  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.328.png)

1  IN 

0  

s  

N  

d  

delay 0  

time

1  

0  

0   N  

OUT

Figure 7.21: Using a variable delay line as a pitch shifter. The sawtooth wave creates a smoothly increasing or decreasing delay time. The output of the delay line is enveloped to avoid discontinuities. Another copy of the same diagram should run 180 degrees (¼radians) out of phase with this one.

and d0 + s, and this adjusted sawtooth controls the delay time, in samples. The initial delay d0 should be at least enough to make the variable delay feasible; for four-point interpolation it must be at least one sample. Larger values of d0 add a constant, additional delay to the output; this is usually o®ered as a control in a pitch shifter since it is essentially free. The quantity s is sometimes called the window size. It corresponds roughly to the sample length in a looping sampler (Section 2.2).

The sawtooth output is also used to envelope the output in exactly the same way as in the enveloped wavetable sampler ofFigure 2.7 (Page 38). The envelope is zero at the points where the sawtooth wraps around, and in between, rises smoothly to a maximum value of 1 (for unit gain).

If the frequency of the sawtooth wave is f (in cycles per second), then its value sweeps from 0 to 1 every R=f samples (where R is the sample rate). The di®erence between successive values is thus f =R. If we let x[n]denote the output of the sawtooth oscillator, then

f x[n + 1]¡ x[n] =

R

(except at the wraparound points). If we adjust the output range of the wavetable oscillator to the value s (as is done in the ¯gure) we get a new slope:

sf

s ¢x[n + 1]¡ s ¢x[n] =

R

Adding the constant d0 has no e®ect on this slope. The Momentary Transposi- tion (Page 200) is then:

sf

t = 1 ¡

R

To complete the design of the pitch shifter we must add the other copy halfway out of phase. This gives rise to a delay reading pattern as shown in Figure 7.22.

The pitch shifter can transpose either upward (using negative sawtooth fre- quencies, as in the ¯gure) or downward, using positive ones. Pitch shift is usually controlled by changing f with s ¯xed. To get a desired transposition interval t, set

(t ¡ 1)R

f =

s

The window size s should be chosen small enough, if possible, so that the two delayed copies (s=2 samples apart) do not sound as distinct echoes. However, very small values of s will force f upward; values of f greater than about 5 Hertz result in very audible modulation. So if very large transpositions are required, the value of s may need to be increased. Typical values range from 30 to 100 milliseconds (about R=30 to R=10 samples).

Although the frequency may be changed at will, even discontinuously, s must be changed more carefully. A possible solution is to mute the output while changing s discontinuously; alternatively, s may be ramped continuously but this causes hard-to-control Doppler shifts.

input time![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.329.png)

output time

Figure 7.22: The pitch shifter's delay reading pattern using two delay lines, so that one is at maximum amplitude exactly when the other is switching.

10. EXAMPLES 214

loadbang metro 1000![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.330.png)

tabplay~ G01-tab

input signal

write to delay line delwrite~ delay1 1000

0 <-- delay time

(msec)

delread~ delay1

+~  read from delay line |  

(OUT)

Figure 7.23: Example patch G01.delay.pd, showing a noninterpolating delay with a delay time controlled in milliseconds.

A good choice of envelope is one half cycle of a sinusoid. If we assume on average that the two delay outputs are uncorrelated (Page 11), the signal power from the two delay lines, after enveloping, will add to a constant (since the sum of squares of the two envelopes is one).

Many variations exist on this pitch shifting algorithm. One classic variant uses a single delay line, with no enveloping at all. In this situation it is necessary to choose the point at which the delay time jumps, and the point it jumps to, so that the output stays continuous. For example, one could ¯nd a point where the output signal passes through zero (a \zero crossing") and jump discontinuously to another one. Using only one delay line has the advantage that the signal output sounds more \present". A disadvantage is that, since the delay time is a function of input signal value, the output is no longer a linear function of the input, so non-periodic inputs can give rise to artifacts such as di®erence tones.

10. Examples

Fixed, noninterpolating delay line

Example G01.delay.pd (Figure 7.23) applies a simple delay line to an input signal. Two new objects are needed:

delwrite~ : de¯ne and write to a delay line. The ¯rst creation argument gives the![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.331.png) name of the delay line (and two delay lines may not share the same name).

The second creation argument is the length of the delay line in milliseconds. The inlet takes an audio signal and writes it continuously into the delay line.

delread~ : read from (or \tap") a delay line. The ¯rst creation argument gives![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.332.png) the name of the delay line (which should agree with the name of the corre- sponding delwrite~ object; this is how Pd knows which delwrite~ to associate with the delread~ object). The second (optional) creation argument gives the delay time in milliseconds. This may not be negative and also may not exceed the length of the delay line as speci¯ed to the delwrite~ object. Incoming num- bers (messages) may be used to change the delay time dynamically. However, this will make a discontinuous change in the output, which should therefore be muted if the delay time changes.

The example simply pairs one delwrite~ and one delread~ object to make a simple, noninterpolating delay. The input signal is a looped recording. The delayed and the non-delayed signal are added to make a non-recirculating comb ¯lter. At delay times below about 10 milliseconds, the ¯ltering e®ect is most prominent, and above that, a discrete echo becomes audible. There is no mut- ing protection on the delay output, so clicks are possible when the delay time changes.

Recirculating comb ¯lter

Example G02.delay.loop.pd (Figure 7.24) shows how to make a recirculating delay network. The delay is again accomplished with a delwrite~/delread~ pair. The output of the delread~ object is multiplied by a feedback gain of 0.7 and fed into the delwrite~ object. An input (supplied by the phasor~ and associated objects) is added into the delwrite~ input; this sum becomes the output of the network. This is the recirculating comb ¯lter of Section 7.4.

The network of tilde objects does not have any cycles, in the sense of ob- jects feeding either directly or indirectly (via connections through other ob- jects) to themselves. The feedback in the network occurs implicitly between the delwrite~and delread~ objects.

Variable delay line

The next example, G03.delay.variable.pd (Figure 7.25), is another recirculating comb ¯lter, this time using a variable-length delay line. One new object is introduced here:

vd~ : Read from a delay line, with a time-varying delay time. As with the delread~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.333.png) object, this reads from a delay line whose name is speci¯ed as a creation argument. Instead of using a second argument and/or control messages to specify the delay time, for the vd~ object the delay in milliseconds is speci¯ed by an incoming audio signal. The delay line is read using four-point (cubic) interpolation; the minimum achievable delay is one sample.

Here the objects on the left side, from the top down to the clip~ -0.2 0.2 object, form a waveshaping network; the index is set by the \timbre" control,

0 <-- pitch mtof![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.334.png) 1  

phasor~ adsr 1 100 1000 0 1000 \*~  \*~ 

input

signal 0  <-- delay time

delread~ G02-del 160 read from delay line \*~ 0.7 feedback gain

+~  add the original and the delayed signal

|  

(OUT) delwrite~ G02-del 2000 write to delay line

Figure 7.24: Recirculating delay (still noninterpolating).

0  <-- pitch![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.335.png)

mtof

0  <-- timbre

* 0.5 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.336.png)
  * 0.01 0  <-- cycle frequency (hundredths)

osc~

pack 0 100 / 100 0  

<-- cycle depth (msec) line~ osc~ 0 pack 0 100

\*~  +~ 1 line~

cos~ \*~ 

0   <-- feedback hip~ 10 +~ 1.46 \* 0.01 (hundredths)

clip~ -0.2 0.2 vd~ G03-del

pack 0 100

+~ 

line~

hip~ 5

|   \*~ 

(OUT)

clip~ -1 1

delwrite~ G03-del 1000

Figure 7.25: The °anger: an interpolating, variable delay line.

10. EXAMPLES 215

and the waveshaping output varies between a near sinusoid and a bright, buzzy sound. The output is added to the output of the vd~ object. The sum is then high pass ¯ltered (the hip~ object at lower left), multiplied by a feedback gain, clipped, and written into the delay line at bottom right. There is a control at right to set the feedback gain; here, in contrast with the previous example, it is possible to specify a gain greater than one in order to get unstable feedback. For this reason the second clip~ object is inserted within the delay loop (just above the delwrite~ object) so that the signal cannot exceed 1 in absolute value.

The length ofthe delay is controlled by the signal input to the vd~ object. An oscillator with variable frequency and gain, in the center of the ¯gure, provides the delay time. The oscillator is added to one to make it nonnegative before multiplying it by the \cycle depth" control, which e®ectively sets the range of delay times. The minimum possible delay time of 1.46 milliseconds is added so that the true range of delay times is between the minimum and the same plus twice the \depth". The reason for this minimum delay time is taken up in the discussion of the next example.

Comb ¯lters with variable delay times are sometimes called °angers. As the delay time changes the peaks in the frequency response move up and down in frequency, so that the timbre of the output changes constantly in a characteristic way.

Order of execution and lower limits on delay times

When using delays (as well as other state-sharing tilde objects in Pd), the order in which the writing and and reading operations are done can a®ect the outcome of the computation. Although the tilde objects in a patch may have a complicated topology of audio connections, in reality Pd executes them all in a sequential order, one after the other, to compute each block of audio output. This linear order is guaranteed to be compatible with the audio interconnections, in the sense that no tilde object's computation is done until all its inputs, for that same block, have been computed.

Figure 7.26 shows two examples of tilde object topologies and their transla- tion into a sequence of computation. In part (a) there are four tilde objects, and because of the connections, the object a~ must produce its output before either of b~ or c~ can run; and both of those in turn are used in the computation of d~. So the possible orderings of these four objects are \a-b-c-d" and \a-c-b-d". These two orderings will have exactly the same result unless the computation of b~ and c~ somehow a®ect each other's output (as delay operations might, for example).

Part (b) of the ¯gure shows a cycle of tilde objects. This network cannot be sorted into a compatible sequential order, since each of a~ and b~ requires the other's output to be computed ¯rst. In general, a sequential ordering of the tilde objects is possible if and only if there are no cycles anywhere in the network of tilde objects and their audio signal interconnections. Pd reports an error when such a cycle appears. (Note that the situation for control interconnections between objects is more complicated and °exible; see the Pd documentation for


212

(a) a~ ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.337.png)

b~  c~ d~ 

CHAPTER 7. TIME SHIFTS AND DELAYS

(b)

a~  b~ ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.338.png)


Figure 7.26: Order of execution of tilde objects in Pd: (a), an acyclic network. The objects may be executed in either the order \a-b-c-d" or \a-c-b-d". In part (b), there is a cycle, and there is thus no compatible linear ordering of the objects because each one would need to be run before the other.

details.)

To see the e®ectof the order of computation on a delwrite~/delread~ pair, we can write explicitly the input and output signals in the two possible orders, with the minimum possible delay. If the write operation comes ¯rst, at a block starting at sample number N, the operation can be written as:

x[N];:::;x[N + B ¡ 1] ¡! delwrite~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.339.png)

where B is the block size (as in Section 3.2). Having put those particular samples into the delay line, a following delread~ is able to read the same values out:

delread~ ¡! x[N];:::;x[N + B ¡ 1]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.340.png)

On the other hand, suppose the delread~ object comes before the delwrite~. Then the samples x[N];:::;x[N + B ¡ 1] have not yet been stored in the delay line, so the most recent samples that may be read belong to the previous block:

delread~ ¡! x[N ¡ B];:::;x[N ¡ 1] ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.341.png)x[N];:::;x[N + B ¡ 1] ¡! delwrite~ ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.342.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.343.png)

Here the minimum delay we can possibly obtain is the block size B. So the minimum delay is either 0 or B, depending on the order in which the delread~ and delwrite~objects are sorted into a sequence of execution.

Looking back at the patches of Figures 7.24 and 7.25, which both feature recirculating delays, the delread~ or vd~ object must be placed earlier in the sequence than the delwrite~ object. This is true ofany design in which a delay's output is fed back into its input. The minimum possible delay is B samples. For a (typical) sample rate of 44100 Hertz and block size of 64 samples, this comes to 1.45 milliseconds. This might not sound at ¯rst like a very important restriction. But if you are trying to tune a recirculating comb ¯lter to a speci¯c

7\.10. EXAMPLES

(a) loadbang metro 500![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.344.png)

random 60 del 1

+ 30

1   0  

mtof

vline~ expr 1000/$f1

pd delay-writer |  

(OUT)

213

(b)

incoming delay pulses time

inlet~ inlet![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.345.png)

delread~ G04-del +~  \*~ 0.99

delwrite~ G04-del 1000 outlet~ block~ 1

set block size

Figure 7.27: A patch using block size control to lower the loop delay below the normal 64 samples: (a) the main patch; (b) the \delay-writer" subpatch with a block~ object and a recirculating delay network.

pitch, the highest you can get only comes to about 690 Hertz. To get shorter recirculating delays you must increase the sample rate or decrease the block size.

Example G04.control.blocksize.pd (Figure 7.27) shows how the block size can be controlled in Pd using a new object:

block~ , switch~ : Set the local block size of the patch window the object![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.346.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.347.png)

sits in. Block sizes are normally powers of two. The switch~ object, in addition, can be used to turn audio computation within the window on and o®, using control messages. Additional creation arguments can set the local sample rate and specify overlapping computations (demonstrated in Chapter 9).

In part (a) of the ¯gure (the main patch), a rectangular pulse is sent to the pd delay-writer subpatch, whose output is then returned to the main patch. Part (b) shows the contents of the subpatch, which sends the pulses into a recirculating delay. The block~ object speci¯es that, in this subpatch, signal computation uses a block size (B) of only one. So the minimum achievable delay is one sample instead of the default 64.

Putting a pulse (or other excitation signal) into a recirculating comb ¯lter to make a pitch is sometimes called Karplus-Strong synthesis, having been de- scribed in a paper by them [KS83], although the idea seems to be older. It shows up for example in Paul Lansky's 1979 piece, Six Fantasies on a Poem by Thomas Campion.

10. EXAMPLES 221

delay in![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.348.png)

(a) (b) 45  samples

/ 44.1

pd pulse

pack 0 30 delwrite~ G05−d1 1000

line~

vd~ G05−d1

pd pulse

+~ 

pd delay−writer

(BAD)

pd delay−reader

(GOOD)

Figure 7.28: Using subpatches to ensure that delay lines are written before they are read in non-recirculating networks: (a) the delwrite~ and vd~ objects might be executed in either the \right" or the \wrong" order; (b) the delwrite~ object is inside the pd delay-writer subpatch and the vd~ object is inside the pd delay-reader one. Because of the audio connection between the two subpatches, the order of execution of the read/write pair is forced to be the correct one.

Order of execution in non-recirculating delay lines

In non-recirculating delay networks, it should be possible to place the operation of writing into the delay line earlier in the sequence than that of reading it. There should thus be no lower limit on the length of the delay line (except whatever is imposed by the interpolation scheme; see Section 7.7). In languages such as Csound, the sequence of unit generator computation is (mostly) explicit, so this is easy to specify. In graphical patching environments, however, the order is implicit and another approach must be taken to ensuring that, for example, a delwrite~ object is computed before the corresponding delread~ object. One way of accomplishing this is shown in example G05.execution.order.pd (Figure 7.28).

In part (a) of the ¯gure, the connections in the patch do not determine which order the two delay operations appear in the sorted sequence of tilde object computation; the delwrite~ object could be computed either before or after the vd~ object. If we wish to make sure the writing operation happens before the reading operation, we can proceed as in part (b) of the ¯gure and put the two operations in subpatches, connecting the two via audio signals so that the ¯rst subpatch must be computed before the second one. (Audio computation in subpatches is done atomically, in the sense that the entire subpatch contents are considered as the audio computation for the subpatch as a whole. So everything in the one subpatch happens before anything in the second one.)

pd looper![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.349.png)

delwrite~ G06-del 100

fiddle~ 2048

unpack mtof fundamental frequency moses 1 expr 500/$f1 1/2 period, in msec

t f b samplerate~

expr 2048000/$f1

estimate fiddle~ delay

+ as one window (in msec)

delread~ G06-del pack 0 20

line~

vd~ G06-del

+~ |  

(OUT)

Figure 7.29: An \octave doubler" uses pitch information (obtained using a fiddle~ object) to tune a comb ¯lter to remove the odd harmonics in an in- coming sound.

In this example, the \right" and the \wrong" way to make the comb ¯lter have audibly di®erent results. For delays less than 64 samples, the right hand side of the patch (using subpatches) gives the correct result, but the left hand side can't produce delays below the 64 sample block size.

Non-recirculating comb ¯lter as octave doubler

In example G06.octave.doubler.pd (Figure 7.29) we revisit the idea of pitch- based octave shifting introduced earlier in E03.octave.divider.pd. There, know- ing the periodicity of an incoming sound allowed us to tune a ring modulator to introduce subharmonics. Here we realize the octave doubler described in Section 7.3. Using a variable, non-recirculating comb ¯lter we take out odd har- monics, leaving only the even ones, which sound an octave higher. As before, the spectral envelope of the sound is roughly preserved by the operation, so we can avoid the \chipmunk" e®ect we would have got by using speed change to do the transposition.

The comb ¯ltering is done by combining two delayed copies of the incoming signal (from the pd looper subpatch at top). The ¯xed one (delread~) is set to the window size of the pitch following algorithm. Whereas in the earlier example

this was hidden in another subpatch, we can now show this explicitly. The delay in milliseconds is estimated as equal to the 2048-sample analysis window used by the fiddle~ object; in milliseconds this comes to 1000 ¢2048=R where R is the sample rate.

The variable delay is the same, plus 1/2 of the measured period of the incoming sound, or 1000=(2f ) milliseconds where f is the frequency in cycles per second. The sum of this and the ¯xed delay time is then smoothed using a line~ object to make the input signal for the variable delay line.

Since the di®erence between the two delays is 1=(2f ), the resonant frequen- cies of the resulting comb ¯lter are 2f;4f;6f ¢¢¢; the frequency response (Section 7.3) is zero at the frequencies f;3f;:::, so the resulting sound contains only the partials at multiples of 2f |an octave above the original. Seen another way, the incoming sound is output twice, a half-cycle apart; odd harmonics are thereby shifted 180 degrees (¼ radians) and cancel; even harmonics are in phase with their delayed copies and remain in the sum.

Both this and the octave divider may be altered to make shifts of 3 or 4 to one in frequency, and they may also be combined to make compound shifts such as a musical ¯fth (a ratio of 3:2) by shifting down an octave and then back up a factor of three. (You should do the down-shifting before the up-shifting for best results.)

Time-varying complex comb ¯lter: shakers

Example G07.shaker.pd (Figure 7.30) shows a di®erent way of extending the idea of a comb ¯lter. Here we combine the input signal at four di®erent time shifts (instead of two, as in the original non-recirculating comb ¯lter), each at a di®erent positive or negative gain. To do this, we insert the input signal into a delay line and tap it at three di®erent points; the fourth \tap" is the original, un-delayed signal.

As a way of thinking about the frequency response of a four-tap comb ¯lter, we consider ¯rst what happens when two of the four gains are close to zero. Then we end up with a simple non-recirculating comb ¯lter, with the slight complication that the gains of the two delayed copies may be di®erent. If they are both of the same sign, we get the same peaks and valleys as predicted in Section 7.3, only with the valleys between peaks possibly more shallow. If they are opposite in sign, the valleys become peaks and the peaks become valleys.

Depending on which two taps we supposed were nonzero, the peaks and valleys are spaced by di®erent amounts; the delay times are chosen so that 6 di®erent delay times can arise in this way, ranging between 6 and 30 millisec- onds. In the general case in which all the gains are non-zero, we can imagine the frequency response function varying continuously between these extremes, giving a succession of complicated patterns. This has the e®ect of raising and lowering the amplitudes of the partials of the incoming signal, all independently of the others, in a complicated pattern, to give a steadily time-varying timbre.

The right-hand side of the patch takes care of changing the gains of the input signal and its three time-shifted copies. Each time the metro object ¯res,

frequency time constant

on/off (msec)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.350.png)

0 0 phasor~ 80 metro \* 4

delwrite~ G07-del 30 f   + 1

\*~  line~ mod 4

t f b

delread~ G07-del 30

random 1000

\*~  line~

expr 2 \* $f1/1000 - 0.7 delread~ G07-del 17

pack 0 0 200

\*~  line~

route 0 1 2 3

delread~ G07-del 11 \*~  line~

+~ 

|  (OUT)

Figure 7.30: A \shaker", a four-tap comb ¯lter with randomly varying gains on the taps.


a counter is incremented (the f, + 1, and mod 4 objects). This controls which of the amplitudes will be changed. The amplitude itself is computed by making a random number and normalizing it to lie between -0.7 and 1.3 in value. The random value and the index are packed (along with a third value, a time interval) and this triple goes to the route object. The ¯rst element of the triple (the counter) selects which output to send the other two values to; as a result, one of the four possible line~ objects gets a message to ramp to a new value.

If the time variation is done quickly enough, there is also a modulation e®ect on the original signal; in this situation the straight line segments used in this example should be replaced by modulating signals with more controllable frequency content, for instance using ¯lters (the subject of Chapter 8).

Reverberator

Example G08.reverb.pd (Figure 7.31) shows a simple arti¯cial reverberator, es- sentially a realization of the design shown in Figure 7.15. Four delay lines are fed by the input and by their own recirculated output. The delay outputs are intermixed using rotation matrices, built up from elementary rotations of ¼=4 as in Figure 7.13 (part a). p ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.351.png)

The normalizing multiplication (by 1=2 at each stage) is absorbed into the feedback gain, which therefore cannot exceed 1=2. At a feedback gain of exactly 1=2, all the energy leaving the delay lines is reinserted into them, so the reverberation lasts perpetually.

Figure 7.32 shows the interior of the reverb-echo abstraction used in the reverberator. The two inputs are mixed (using the same rotation matrix and again leaving the renormalization for later). One channel is then delayed. The delay times are selected to grow roughly exponentially; this ensures a smooth and spread-out pattern of echos.

Many extensions of this idea are possible of which we'll only name a few. It is natural, ¯rst, to put low-pass ¯lters at the end of the delay lines, to mimic the typically faster decay of high frequencies than low ones. It is also common to use more than four recirculating delays; one reverberator in the Pd distribution uses sixteen. Finally, it is common to allow separate control of the amplitudes of the early echos (heard directly) and that of the recirculating signal; parameters such as these are thought to control sonic qualities described as \presence", \warmth", \clarity", and so on.

Pitch shifter

Example G09.pitchshift.pd (Figure 7.33) shows a realization of the pitch shifter described in Section 7.9. A delay line (de¯ned and written elsewhere in the patch) is read using two vd~ objects. The delay times vary between a minimum delay (provided as the \delay" control) and the minimum plus a window size (the \window" control.)

The desired pitch shift in half-tones (h) is ¯rst converted into a transposition


7\.10. EXAMPLES

inlet~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.352.png)

reverb-echo echo-del1 5.43216 reverb-echo echo-del2 8.45346 reverb-echo echo-del3 13.4367 reverb-echo echo-del4 21.5463 reverb-echo echo-del5 34.3876 reverb-echo echo-del6 55.5437

219

"early echo" generators,

which also increase echo density.


Get the outputs of the recirculating delays. Add the inputs to two of them.

delread~ loop-del1 60

delread~ loop-del2 71.9345

delread~ loop-del3 86.7545 +~  +~ 

delread~ loop-del4 95.945

outlet~ outlet~

Do a power-conserving Tap outputs here. +~  -~  +~  -~  mix of them in pairs.

First combine (1, 2) and

(3, 4)...

+~  +~  -~  -~  then (1, 3) and (2, 4)

feedback gain on a scale of 0-100 controls reverb

time. / 200 inlet

\*~  \*~  \*~  \*~  min 100

max 0

delwrite~ loop-del4 95.945 delwrite~ loop-del3 86.7545

delwrite~ loop-del2 71.9345 delwrite~ loop-del1 60

Put the signals back into

the recirculating delays.

Figure 7.31: An arti¯cial reverberator.

inlet~ inlet~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.353.png)

+~  -~ 

delwrite~ $1 $2

delread~ $1 $2

outlet~ outlet~

Figure 7.32: The echo generator used in the reverberator.

r transpose![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.354.png)

7   <-- transposition r window

(halftones)

80  <--window

* 0.05776 (msec)

max 1

exp

speed

1\.4982 change

\- 1 \* 0.001

* -1 t b f delay (msec)

tape head

/   rotation freq r delay -6.228 +~ 0.5 pack 0 200 0  

line~

phasor~ wrap~ max 1.5

pack 0 200 -~ 0.5 \*~  -~ 0.5 \*~  line~

\*~ 0.5 +~  \*~ 0.5 +~ 

cos~ vd~ G09-del

cos~ vd~ G09-del

\*~ 

\*~ 

+~ |  (OUT)

Figure 7.33: A pitch shifter using two variable taps into a delay line.

7\.10. EXAMPLES 221 factor

t = 2h=12 = elog(2)=12¢h ¼ e0:05776h

(called \speed change" in the patch). The computation labeled \tape head rotation speed" is the same as the formula for f given on Page 206. Here the positive interval (seven half-steps) gives rise to a transposition factor greater than one, and therefore to a negative value for f .

Once f is calculated, the production of the two phased sawtooth signals and the corresponding envelopes parallels exactly that of the overlapping sam- ple looper (example B10.sampler.overlap.pd, Page 54). The minimum delay is added to each of the two sawtooth signals to make delay inputs for the vd~ ob- jects, whose outputs are multiplied by the corresponding envelopes and summed.

Exercises

1. A complex number has magnitude one and argument ¼=4. What are its real and imaginary parts?
1. A complex number has magnitude one and real part 1=2. What is its imaginary part? (There are two possible values.)
1. What delay time would you give a comb ¯lter so that its ¯rst frequency response peak is at 440 Hertz? If the sample rate is 44100, what frequency would correspond to the nearest integer delay?
1. Suppose you made a variation on the non-recirculating comb ¯lter so that the delayed signal was subtracted from the original instead of adding. What would the new frequency response be?
1. If you want to make a 6-Hertz vibrato with a sinusoidally varying delay line, and if you want the vibrato to change the frequency by 5%, how big a delay variation would you need? How would this change if the same depth of vibrato was desired at 12 Hertz?
1. A complex sinusoid X[n] has frequency 11025 Hertz, amplitude 50 and initial phase 135 degrees. Another one, Y[n], has the same frequency, but amplitude 20 and initial phase 45 degrees. What are the amplitude and initial phase of the sum of X and Y?
1. What are the frequency, initial phase, and amplitude ofthe signal obtained when X[n] (above) is delayed 4 samples?
1. Show that the frequency response of a recirculating comb ¯lter with delay time d and feedback gain g, as a function of angular frequency !, is equal to:

[(1 ¡ gcos(!d))2 + (gsin(!d))2]¡1=2


Chapter 8

Filters

In the previous chapter we saw that a delay network can have a non-uniform frequency response|a gain that varies as a function of frequency. Delay net- works also typically change the phase of incoming signals variably depending on frequency. When the delay times used are very short, the most important properties of a delay network become its frequency and phase response. A delay network that is designed speci¯cally for its frequency or phase response is called a ¯lter.

In block diagrams, ¯lters are shown as in Figure 8.1 (part a). The curve shown within the block gives a qualitative representation of the ¯lter's frequency response. The frequency response may vary with time, and depending on the design of the ¯lter, one or more controls (or additional audio inputs) might be used to change it.

Suppose, following the procedure of Section 7.3, we put a unit-amplitude, complex-valued sinusoid with angular frequency ! into a ¯lter. We expect to get out a sinusoid of the same frequency and some amplitude, which depends on !. This gives us a complex-valued function H(!), which is called the transfer function of the ¯lter.

The frequency response is the gain as a function of the frequency !. It is is equal to the magnitude of the transfer function. A ¯lter's frequency response is customarily graphed as in Figure 8.1 (part b). An incoming unit-amplitude sinusoid of frequency ! comes out of the ¯lter with magnitude jH(!)j.

It is sometimes also useful to know the phase response of the ¯lter, equal to 6 (H(!)). For a ¯xed frequency !, the ¯lter's output phase will be 6 (H(!)) ![ref4]![ref4]radians ahead of its input phase.

The design and use of ¯lters is a huge subject, because the wide range of uses a ¯lter might be put to suggests a wide variety of ¯lter design processes. In some applications a ¯lter must exactly follow a prescribed frequency response, in others it is important to minimize computation time, in others the phase response is important, and in still others the ¯lter must behave well when its parameters change quickly with time.

223

1. TAXONOMY OF FILTERS 230

gain![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.356.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.357.png)

(a) (b)

Figure 8.1: Representations of a ¯lter: (a) in a block diagram; (b) a graph of its frequency response.

1. Taxonomy of ¯lters

Over the history of electronic music the technology for building ¯lters has changed constantly, but certain kinds of ¯lters reappear often. In this section we will give some nomenclature for describing ¯lters of several generic, recurring types. Later we'll develop some basic strategies for making ¯lters with desired characteristics, and ¯nally we'll discuss some common applications of ¯lters in electronic music.

1. Low-pass and high-pass ¯lters

By far the most frequent purpose for using a ¯lter is extracting either the low- frequency or the high-frequency portion of an audio signal, attenuating the rest. This is accomplished using a low-pass or high-pass ¯lter.

Ideally, a low-pass or high-pass ¯lter would have a frequency response of one up to (or down to) a speci¯ed cuto® frequency and zero past it; but such ¯lters cannot be realized in practice. Instead, we try to ¯nd realizable approximations to this ideal response. The more design e®ort and computation time we put into it, the closer we can get.

Figure 8.2 shows the frequency response of a low-pass ¯lter. Frequency is divided into three bands, labeled on the horizontal axis. The passband is the region (frequency band) where the ¯lter should pass its input through to its output with unit gain. For a low-pass ¯lter (as shown), the passband reaches from a frequency of zero up to a certain frequency limit. For a high-pass ¯lter, the passband would appear on the right-hand side ofthe graph and would extend from the frequency limit up to the highest frequency possible. Any realizable ¯lter's passband will be only approximately °at; the deviation from °atness is called the ripple, and is often speci¯ed by giving the ratio between the highest

ripple![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.358.png)

stopband attenuation

passband stopband

transition band

Figure 8.2: Terminology for describing the frequency response of low-pass and high-pass ¯lters. The horizontal axis is frequency and the vertical axis is gain. A low-pass ¯lter is shown; a high-pass ¯lter has the same features switched from right to left.

ripple![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.359.png)

stopband attenuation

passband

stopband

stopband transition

bands![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.360.png)

Figure 8.3: Terminology for describing the frequency response of band-pass and stop-band ¯lters. The horizontal axis is frequency and the vertical axis is gain. A band-pass ¯lter is shown; a stop-band ¯lter would have a contiguous stopband surrounded by two passbands.

and lowest gain in the passband, expressed in decibels. The ideal low-pass or high-pass ¯lter would have a ripple of 0 dB.

The stopband of a low-pass or high-pass ¯lter is the frequency band over which the ¯lter is intended not to transmit its input. The stopband attenuation is the di®erence, in decibels, between the lowest gain in the passband and the highest gain in the stopband. Ideally this would be in¯nite; the higher the better.

Finally, a realizable ¯lter, whose frequency response is always a continuous function of frequency, must have a frequency band over which the gain drops from the passband gain to the stopband gain; this is called the transition band. The thinner this band can be made, the more nearly ideal the ¯lter.

2. Band-pass and stop-band ¯lters

A band-pass ¯lter admits frequencies within a given band, rejecting frequencies below it and above it. Figure 8.3 shows the frequency response of a band-pass ¯lter, with the key parameters labelled. A stop-band ¯lter does the reverse, rejecting frequencies within the band and letting through frequencies outside it.

bandwidth

center frequency![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.361.png)

Figure 8.4: A simpli¯ed view of a band-pass ¯lter, showing bandwidth and center frequency.

In practice, a simpler language is often used for describing bandpass ¯lters, as shown in Figure 8.4. Here there are only two parameters: a center frequency and a bandwidth. The passband is considered to be the region where the ¯lter has at least half the power gain as at the peak (i.e., the gain is within 3 decibels of its maximum). The bandwidth is the width, in frequency units, of the passband. The center frequency is the point of maximum gain, which is approximately the midpoint of the passband.

3. Equalizing ¯lters

In some applications, such as equalization, the goal isn't to pass signals of certain frequencies while stopping others altogether, but to make controllable adjust- ments, boosting or attenuating a signal, over a frequency range, by a desired gain. Two ¯lter types are useful for this. First, a shelving ¯lter (Figure 8.5) is used for selectively boosting or reducing either the low or high end of the frequency range. Below a selectable crossover frequency, the ¯lter tends toward a low-frequency gain, and above it it tends toward a di®erent, high-frequency one. The crossover frequency, low-frequency gain, and high-frequency gain can all be adjusted independently.

Second, a peaking ¯lter (Figure 8.6) is capable of boosting or attenuating signals within a range of frequencies. The center frequency and bandwidth (which together control the range of frequencies a®ected), and the in-band and out-of-band gains are separately adjustible.

Parametric equalizers often employ two shelving ¯lters (one each to adjust the low and high ends of the spectrum) and two or three peaking ¯lters to adjust bands in between.

2. ELEMENTARY FILTERS 236

high frequency gain![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.362.png)

low frequency gain

crossover frequency

Figure 8.5: A shelving ¯lter, showing low and high frequency gain, and crossover frequency.

bandwidth

in-band gain![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.363.png)

out-of-band gain

center frequency

Figure 8.6: A peaking ¯lter, with controllable center frequency, bandwidth, and in-band and out-of-band gains.

IN 

d=1![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.364.png)

Q  

OUT

Figure 8.7: A delay network with a single-sample delay and a complex gain Q. This is the non-recirculating elementary ¯lter, ¯rst form. Compare the non- recirculating comb ¯lter shown in Figure 7.3, which corresponds to choosing Q = ¡1 here.

2. Elementary ¯lters

We saw in Chapter 7 how to predict the frequency and phase response of delay networks. The art of ¯lter design lies in ¯nding a delay network whose transfer function (which controls the frequency and phase response) has a desired shape. We will develop an approach to building such delay networks out ofthe two types ofcomb ¯lters developed in Chapter 7: recirculating and non-recirculating. Here we will be interested in the special case where the delay is only one sample in length. In this situation, the frequency responses shown in Figures 7.6 and 7.10 no longer look like combs; the second peak recedes all the way to the sample rate, 2¼radians, when d = 1. Since only frequencies between 0 and the Nyquist frequency (¼radians) are audible, in e®ect there is only one peak when d = 1.

In the comb ¯lters shown in Chapter 7, the peaks are situated at DC (zero frequency), but we will often wish to place them at other, nonzero frequencies. This is done using delay networks|comb ¯lters|with complex-valued gains.

1. Elementary non-recirculating ¯lter

The non-recirculating comb ¯lter may be generalized to yield the design shown in Figure 8.7. This is the elementary non-recirculating ¯lter, of the ¯rst form. Its single, complex-valued parameter Q controls the complex gain of the delayed signal subtracted from the original one.

To ¯nd its frequency response, as in Chapter 7 we feed the delay network a complex sinusoid 1;Z;Z 2;::: whose frequency is ! = arg(Z). The nth sample of the input is Z n and that of the output is

(1 ¡ QZ ¡1)Zn

imaginary![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.365.png)

Z  

Z-Q Q  

r  

real 1  

QZ -1 

-1 1-QZ

Figure 8.8: Diagram for calculating the frequency response of the non- recirculating elementary ¯lter (Figure 8.7). The frequency response is given by the length of the segment connecting Z to Q in the complex plane.

so the transfer function is

H(Z) = 1 ¡ QZ ¡1

This can be analyzed graphically as shown in Figure 8.8. The real numbers r and ® are the magnitude and argument of the complex number Q:

Q = r ¢(cos(®) + i sin(®))

The gain of the ¯lter is the distance from the point Q to the point Z in the complex plane. Analytically we can see this because

j1 ¡ QZ ¡1j = jZjj1 ¡ QZ ¡1j = jQ ¡ Zj

Graphically, the number QZ ¡1 is just the number Q rotated backwards (clock- wise) by the angular frequency ! of the incoming sinusoid. The value j1¡QZ ¡1j is the distance from QZ ¡1 to 1 in the complex plane, which is equal to the dis- tance from Q to Z.

As the frequency of the input sweeps from 0 to 2¼, the point Z travels couterclockwise around the unit circle. At the point where ! = ®, the distance

gain

|Q|=1![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.366.png)

0\.5 0  

0   frequency 2  

Figure 8.9: Frequency response of the elementary non-recirculating ¯lter Figure 8.7. Three values of Q are used, all with the same argument (-2 radians), but with varying absolute value (magnitude) r = jQj.

is at a minimum, equal to 1 ¡ r. The maximum occurs which Z is at the opposite point of the circle. Figure 8.9 shows the transfer function for three di®erent values of r = jQj.

2. Non-recirculating ¯lter, second form

Sometimes we will need a variant of the ¯lter above, shown in Figure 8.10, called the elementary non-recirculating ¯lter, second form. Instead of multiplying the delay output by Q we multiply the direct signal by its complex conjugate Q. If

A = a + bi = r ¢(cos(®) + i sin(®))

is any complex number, its complex conjugate is de¯ned as:

A = a ¡ bi = r ¢(cos(®) ¡ i sin(®))![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.367.png)

Graphically this re°ects points of the complex plane up and down across the real axis. The transfer function of the new ¯lter is

H(Z) = Q ¡ Z ¡1![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.368.png)

This gives rise to the same frequency response as before since

jQ ¡ Z¡1j = jQ ¡ Z¡1j = jQ ¡ Zj![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.369.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.370.png)

Here we use the fact that Z = Z ¡1, for any unit complex number Z, as can be ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.371.png)veri¯ed by writing out ZZ in either polar or rectangular form.

Although the two forms of the elementary non-recirculating ¯lter have the same frequency response, their phase responses are di®erent; this will occasion- ally lead us to prefer the second form.

IN 

Q   d=1![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.372.png)

OUT

Figure 8.10: The elementary non-recirculating ¯lter, second form.

3. Elementary recirculating ¯lter

The elementary recirculating ¯lter is the recirculating comb ¯lter of Figure 7.7 with a complex-valued feedback gain P as shown in Figure 8.11 (part a). By the same analysis as before, feeding this network a sinusoid whose nth sample

is Z gives an output of:

n 1 ¡ P1Z¡1 Zn

so the transfer function is

1 H(Z) =

1 ¡ P Z¡1

The recirculating ¯lter is stable when jP j < 1; when, instead, jP j > 1 the output grows exponentially as the delayed sample recirculates.

The transfer function is thus just the inverse of that of the non-recirculating ¯lter (¯rst form). If you put the two in series with P = Q, the output the- oretically equals the input. (This analysis only demonstrates it for sinusoidal inputs; that it follows for other signals as well can be veri¯ed by working out the impulse response of the combined network).

4. Compound ¯lters

We can use the recirculating and non-recirculating ¯lters developed here to create a compound ¯lter by putting several elementary ones in series. If the parameters of the non-recirculating ones (of the ¯rst type) are Q1;:::;Qj and those of the recirculating ones are P1;:::;Pk, then putting them all in series, in any order, will give the transfer function:

H(Z) = (1 ¡ Q1Z¡1) ¢¢¢(1 ¡ Qj Z¡1) (1 ¡ P1Z¡1) ¢¢¢(1 ¡ PkZ¡1)

The frequency response of the resulting compound ¯lter is the product of those of the elementary ones. (One could also combine elementary ¯lters by adding

IN 

|P|=0.75![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.373.png)

0\.5![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.374.png)

OUT

d=1

0  P  

0   frequency 2  

(a) (b)

Figure 8.11: The elementary recirculating ¯lter: (a) block diagram; (b) fre- quency response.

their outputs, or making more complicated networks of them; but for most purposes the series con¯guration is the easiest one to work with.)

5. Real outputs from complex ¯lters

In most applications, we start with a real-valued signal to ¯lter and we need a real-valued output, but in general, a compound ¯lter with a transfer function as above will give a complex-valued output. However, we can construct ¯lters with non-real-valued coe±cients which nonetheless give real-valued outputs, so that the analysis that we carry out using complex numbers can be used to predict, explain, and control real-valued output signals. We do this by pairing each elementary ¯lter (with coe±cient P or Q) with another having as its coe±cient the complex conjugate P or Q.![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.375.png)

For example, putting two non-recirculating ¯lters, with coe±cients Q and Q, in series gives a transfer function equal to:![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.376.png)

H(Z) = (1 ¡ QZ ¡1) ¢(1 ¡ QZ ¡1)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.377.png)

which has the property that:

H(Z) = H(Z)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.378.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.379.png)

Now if we put any real-valued sinusoid:

X = 2re(AZ n ) = AZ n + AZn![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.380.png)

n

we get out: ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.381.png)

A ¢H(Z) ¢Zn + A ¢H(Z) ¢Z~~ n![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.382.png)

3. DESIGNING FILTERS 250

which, by inspection, is another real sinusoid. Here we're using two properties of complex conjugates. First, you can add and multiply them at will:

A + B = A + B AB![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.383.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.384.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.385.png) = A ¢B![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.386.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.387.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.388.png)

and second, anything plus its complex conjugate is real, and is in fact twice its real part:

A + A = 2re(A)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.389.png)

This result for two conjugate ¯lters extends to any compound ¯lter; in general, we always get a real-valued output from a real-valued input if we arrange that each coe±cient Qi and Pi in the compound ¯lter is either real-valued, or else appears in a pair with its complex conjugate.

6. Two recirculating ¯lters for the price of one

When pairing recirculating elementary ¯lters, it is possible to avoid computing one of each pair, as long as the input is real-valued (and so, the output is as well.) Supposing the input is a real sinusoid of the form:

AZ n + AZ ¡n![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.390.png)

and we apply a single recirculating ¯lter with coe±cient P . Letting a[n] denote the real part of the output, we have:

- ¸

a[n] = re 1~~ AZ n + 1~~ AZ¡n![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.391.png)

1 ¡ P Z¡1 1 ¡ P Z

- 1 + 1~~ AZ n

¸

- re~~ AZ n![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.392.png)

1 ¡ P Z¡1 1 ¡ P Z¡1

- ¸
- re 2 ¡ 2re(P )Z ¡1~~ AZ n![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.393.png)

(1 ¡ P Z¡1)(1 ¡ P Z¡1)

" #

1 ¡ re(P )Z¡1 n 1 ¡ re(P )Z~~ ¡1 ¡n![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.394.png)

- re (1 ¡ P Z¡1)(1 ¡ P Z¡1)AZ + (1 ¡ P Z¡1)(1 ¡ P Z¡1)AZ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.395.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.396.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.397.png)

(In the second step we used the fact that you can conjugate all or part of an expression, without changing the result, if you're just going to take the real part anyway. The fourth step did the same thing backward.) Comparing the input to the output, we see that the e®ect of passing a real signal through a complex one-pole ¯lter, then taking the real part, is equivalent to passing the signal through a two-pole, one-zero ¯lter with transfer function equal to:

1 ¡ re(P )Z¡1

H (Z) = ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.398.png)

re (1 ¡ P Z¡1)(1 ¡ P Z¡1)

A similar calculation shows that taking the imaginary part (considered as a real signal) is equivalent to ¯ltering the input with the transfer function:

im(P )Z¡1

Him (Z) = ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.399.png)

(1 ¡ P Z¡1)(1 ¡ P Z¡1)

So taking either the real or imaginary part of a one-pole ¯lter output gives ¯lters with two conjugate poles. The two parts can be combined to synthesize ¯lters with other possible numerators; in other words, with one complex recirculating ¯lter we can synthesize a ¯lter that acts on real signals with two (complex conjugate) poles and one (real) zero.

This technique, known as partial fractions, may be repeated for any number of stages in series as long as we compute the appropriate combination of real and imaginary parts of the output of each stage to form the (real) input of the next stage. No similar shortcut seems to exist for non-recirculating ¯lters; for them it is necessary to compute each member of each complex-conjugate pair explicitly.

3. Designing ¯lters

The frequency response ofa series ofelementary recirculating and non-recirculating ¯lters can be estimated graphically by plotting all the coe±cients Q1;:::;Qj and P1;:::;Pk on the complex plane and reasoning as in Figure 8.8. The overall frequency response is the product of all the distances from the point Z to each of the Qi, divided by the product of the distances to each of the Pi.

One customarily marks each of the Qi with an \o" (calling it a \zero") and each of the Pi with an \x" (a \pole"); their names are borrowed from the ¯eld of complex analysis. A plot showing the poles and zeroes associated with a ¯lter is unimaginatively called a pole-zero plot.

When Z is close to a zero the frequency response tends to dip, and when it is close to a pole, the frequency response tends to rise. The e®ect of a pole or a zero is more pronounced, and also more local, if it is close to the unit circle that Z is constrained to lie on. Poles must lie within the unit circle for a stable ¯lter. Zeros may lie on or outside it, but any zero Q outside the unit circle may be ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.400.png)replaced by one within it, at the point 1=Q, to give a constant multiple of the same frequency response. Except in special cases we will keep the zeros inside the circle as well as the poles.

In the rest of this section we will show how to construct several of the ¯lter types most widely used in electronic music. The theory of digital ¯lter design is vast, and we will only give an introduction here. A deeper treatment is available online from Julius Smith at ccrma.stanford.edu. See also [Ste96] for an introduction to ¯lter design from the more general viewpoint of digital signal processing.

half-power point![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.401.png) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.402.png)

p   

0   2  

(a) (b)

Figure 8.12: One-pole low-pass ¯lter: (a) pole-zero diagram; (b) frequency re- sponse.

1. One-pole low-pass ¯lter

The one-pole low-pass ¯lter has a single pole located at a positive real number p, as pictured in Figure 8.12. This is just a recirculating comb ¯lter with delay length d = 1, and the analysis of Section 7.4 applies. The maximum gain occurs at a frequency of zero, corresponding to the point on the circle closest to the point p. The gain there is 1=(1 ¡ p). Assuming p is close to one, if we move a

distance of 1 ¡ p units up or downp from the real (horizontal) axis, the distance increases![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.403.png) by a factor of about 2, and so we expect the half-power point to occur at an angular frequency of about 1 ¡ p.

This calculation is often made in reverse: if we wish the half-power point to lie at a given angular frequency !, we set p = 1 ¡ !. This approximation only works well if the value of ! is well under ¼=2, as it often is in practice. It is customary to normalize the one-pole low-pass ¯lter, multiplying it by the constant factor 1 ¡ p in order to give a gain of 1 at zero frequency; nonzero frequencies will then get a gain less than one.

The frequency response is graphed in Figure 8.12 (part b). The audible frequencies only reach to the middle of the graph; the right-hand side of the frequency response curve all lies above the Nyquist frequency ¼.

The one-pole low-pass ¯lter is often used to seek trends in noisy signals. For instance, if you use a physical controller and only care about changes on the order of 1/10 second or so, you can smooth the values with a low-pass ¯lter whose half-power point is 20 or 30 cycles per second.

p   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.404.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.405.png)

0  

(a) (b)

Figure 8.13: One-pole, one-zero high-pass ¯lter: (a) pole-zero diagram; (b) frequency response (from zero to Nyquist frequency).

2. One-pole, one-zero high-pass ¯lter

Sometimes an audio signal carries an unwanted constant o®set, or in other words, a zero-frequency component. For example, the waveshaping spectra of Section 5.3 almost always contain a constant component. This is inaudible, but, since it speci¯es electrical power that is sent to your speakers, its presence reduces the level of loudness you can reach without distortion. Another name for a constant signal component is \DC", meaning \direct current".

An easy and practical way to remove the zero-frequency component from an audio signal is to use a one-pole low-pass ¯lter to extract it, and then subtract the result from the signal. The resulting transfer function is one minus the transfer function of the low-pass ¯lter:

1 ¡ p 1 ¡ Z¡1 H(Z) = 1 ¡~~ = p

1 ¡ pZ ¡1 1 ¡ pZ ¡1

The factor of 1 ¡ p in the numerator of the low-pass transfer function is the normalization factor needed so that the gain is one at zero frequency.

By examining the right-hand side ofthe equation (comparing it to the general formula for compound ¯lters), we see that there is still a pole at the real number p, and there is now also a zero at the point 1. The pole-zero plot is shown in Figure 8.13 (part a), and the frequency response in part (b). (Henceforth, we will only plot frequency responses to the Nyquist frequency ¼; in the previous example we plotted it all the way up to the sample rate, 2¼.)

imaginary![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.406.png)

1-d

q  p  real ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.407.png)

1  

0  d  

(b)

(a)

Figure 8.14: One-pole, one-zero shelving ¯lter: (a) pole-zero diagram; (b) fre- quency response.

3. Shelving ¯lter

Generalizing the one-zero, one-pole ¯lter above, suppose we place the zero at a point q, a real number close to, but less than, one. The pole, at the point p, is similarly situated, and might be either greater than or less than q, i.e., to the right or left, respectively, but with both q and p within the unit circle. This situation is diagrammed in Figure 8.14.

At points of the circle far from p and q, the e®ects of the pole and the zero are nearly inverse (the distances to them are nearly equal), so the ¯lter passes those frequencies nearly unaltered. In the neighborhood of p and q, on the other hand, the ¯lter will have a gain greater or less than one depending on which of p or q is closer to the circle. This con¯guration therefore acts as a low-frequency shelving ¯lter. (To make a high-frequency shelving ¯lter we do the same thing, only placing p and q close to -1 instead of 1.)

To ¯nd the parameters ofa shelving ¯lter given a desired transition frequency

- (in angular units) and low-frequency gain g, ¯rst we choose an average distance d, as pictured in the ¯gure, from the pole and the zero to the edge of the circle. For small values of d, the region of in°uence is about d radians, so simply set d = ! to get the desired transition frequency.

p p ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.408.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.409.png)

Then put the pole at p = 1 ¡ d= g and the zero at q = 1 ¡ d g. The gain

P   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.410.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.411.png)

1   

P   

2   

0  

(a) (b)

Figure 8.15: Two-pole band-pass ¯lter: (a) pole-zero diagram; (b) frequency response.

at zero frequency is then

1 ¡ q

- g

1 ¡ p

as desired. For example, in the ¯gure, d is 0.25 radians and g is 2.

4. Band-pass ¯lter

Starting with the three ¯lter types shown above, which all have real-valued poles and zeros, we now transform them to operate on bands located o®the real axis. The low-pass, high-pass, and shelving ¯lters will then become band-pass, stop- band, and peaking ¯lters. First we develop the band-pass ¯lter. Suppose we want a center frequency at ! radians and a bandwidth of ¯. We take the low- pass ¯lter with cuto® frequency ¯; its pole is located, for small values of ¯, roughly at p = 1¡ ¯. Now rotate this value by ! radians in the complex plane, i.e., multiply by the complex number cos! + i sin !. The new pole is at:

P1 = (1 ¡ ¯)(cos ! + i sin !)

To get a real-valued output, this must be paired with another pole:

P2 = P1 = (1 ¡ ¯)(cos ! ¡ i sin !)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.412.png)

The resulting pole-zero plot is as shown in Figure 8.15.

The peak is approximately (not exactly) at the desired center frequency !, and the frequency response drops by 3 decibels approximately ¯ radians above and below it. It is often desirable to normalize the ¯lter to have a peak gain

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.413.png) 0  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.414.png)

(a) (b)

Figure 8.16: A peaking ¯lter: (a) pole-zero diagram; (b) frequency response. Here the ¯lter is set to attenuate by 6 decibels at the center frequency.

near unity; this is done by multiplying the input or output by the product of the distances of the two poles to the peak on the circle, or (very approximately):

- ¤ (¯ + 2!)

For some applications it is desirable to add a zero at the points 1 and ¡1, so that the gain drops to zero at angular frequencies 0 and ¼.

5. Peaking and stop-band ¯lter

In the same way, a peaking ¯lter is obtained from a shelving ¯lter by rotating the pole and the zero, and by providing a conjugate pole and zero, as shown in Figure 8.16. If the desired center frequency is !, and the radii of the pole and zero (as for the shelving ¯lter) are p and q, then we place the the upper pole and zero at

P1 = p ¢(cos ! + i sin !) Q1 = q¢(cos ! + i sin !)

As a special case, placing the zero on the unit circle gives a stop-band ¯lter; in this case the gain at the center frequency is zero. This is analogous to the one-pole, one-zero high-pass ¯lter above.

6. Butterworth ¯lters

A ¯lter with one real pole and one real zero can be con¯gured as a shelving ¯lter, as a high-pass ¯lter (putting the zero at the point 1) or as a low-pass ¯lter (putting the zero at ¡1). The frequency responses of these ¯lters are quite

blunt; in other words, the transition regions are wide. It is often desirable to get a sharper ¯lter, either shelving, low- or high-pass, whose two bands are °atter and separated by a narrower transition region.

A procedure borrowed from the analog ¯ltering world transforms real, one- pole, one-zero ¯lters to corresponding Butterworth ¯lters, which have narrower transition regions. This procedure is described clearly and elegantly in the last chapter of [Ste96]. The derivation uses more mathematics background than we have developed here, and we will simply present the result without deriving it.

To make a Butterworth ¯lter out of a high-pass, low-pass, or shelving ¯lter, suppose that either the pole or the zero is given by the expression

1 ¡ r2 (1 + r)2

where r is a parameter ranging from 1 to 1. If r = 0 this is the point 1, and if r = 1 it's ¡1.

Then, for reasons which will remain mysterious, we replace the point (whether pole or zero) by n points given by:

(1 ¡ r2) ¡ (2r sin(®))i 1 + r2 + 2r cos(®))

where ® ranges over the values:

- 1 ¼ 3 ¼ 2n ¡ 1

( ¡ 1); ( ¡ 1); :::; ( ¡ 1) 2 n 2 n 2 n

In other words, ®takes on n equally spaced angles between ¡¼=2 and ¼=2. The points are arranged in the complex plane as shown in Figure 8.17. They lie on a circle through the original real-valued point, which cuts the unit circle at right angles.

A good estimate for the cuto® or transition frequency de¯ned by these cir- cular collections of poles or zeros is simply the spot where the circle intersects the unit circle, corresponding to ®= ¼=2. This gives the point

(1 ¡ r2) ¡ 2ri

1 + r2

which, after some algebra, gives an angular frequency equal to

- = 2arctan(r)

Figure 8.18 (part a) shows a pole-zero diagram and frequency response for a Butterworth low-pass ¯lter with three poles and three zeros. Part (b) shows the frequency response of the low-pass ¯lter and three other ¯lters obtained by choosing di®erent values of ¯ (and hence r) for the zeros, while leaving the poles stationary. As the zeros progress from ¯ = ¼ to ¯ = 0, the ¯lter, which starts as a low-pass ¯lter, becomes a shelving ¯lter and then a high-pass one.

r=1

r=2 r=0.5![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.415.png)

- 3 /8 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.416.png)
- /8 
- - /8 
- -3 /8 

Figure 8.17: Replacing a real-valued pole or zero (shown as a solid dot) with an array of four of them (circles) as for a Butterworth ¯lter. In this example we get four new poles or zeros as shown, lying along the circle where r = 0:5.

shelf 2![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.417.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.418.png)

3  

hi-pass shelf 1 low-pass

0  

(b)

(a)

Figure 8.18: Butterworth low-pass ¯lter with three poles and three zeros: (a) pole-zero plot. The poles are chosen for a cuto® frequency ¯ = ¼=4; (b) fre- quency responses for four ¯lters with the same pole con¯guration, with di®erent placements of zeros (but leaving the poles ¯xed). The low-pass ¯lter results from setting ¯ = ¼ for the zeros; the two shelving ¯lters correspond to ¯ = 3¼=10 and ¯ = 2¼=10, and ¯nally the high-pass ¯lter is obtained setting ¯ = 0. The high-pass ¯lter is normalized for unit gain at the Nyquist frequency, and the others for unit gain at DC.

7. Stretching the unit circle with rational functions

In Section 8.3.4 we saw a simple way to turn a low-pass ¯lter into a band-pass one. It is tempting to apply the same method to turn our Butterworth low- pass ¯lter into a higher-quality band-pass ¯lter; but if we wish to preserve the high quality of the Butterworth ¯lter we must be more careful than before in the design of the transformation used. In this section we will prepare the way to making the Butterworth band-pass ¯lter by introducing a class of rational transformations of the complex plane which preserve the unit circle.

This discussion is adapted from [PB87], pp. 201-206 (I'm grateful to Julius Smith for this pointer). There the transformation is carried out in continuous time, but here we have adapted the method to operate in discrete time, in order to make the discussion self-contained.

The idea is to start with any ¯lter with a transfer function as before:

H(Z) = (1 ¡ Q1Z¡1) ¢¢¢(1 ¡ Qj Z¡1) (1 ¡ P1Z¡1) ¢¢¢(1 ¡ PkZ¡1)

whose frequency response (the gain at a frequency !) is given by:

jH(cos(!) + i sin(!))j

Now suppose we can ¯nd a rational function, R(Z), which distorts the unit circle in some desirable way. For R to be a rational function means that it can be written as a quotient of two polynomials (for example, the transfer function H is a rational function). That R sends points on the unit circle to other points on the unit circle is just the condition that jR(Z)j = 1 whenever Z = 1. It can easily be checked that any function of the form

R(Z) = U ¢An Zn + An¡1Zn¡1 + ¢¢¢+ A0 ![ref5]![ref5]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.420.png)A0Zn + A1Zn¡1 + ¢¢¢+ An

(where jUj = 1) has this property. The same reasoning as in Section 8.2.2 con¯rms that jR(Z)j = 1 whenever Z = 1.

Once we have a suitable rational function R, we can simply compose it with the original transfer function H to fabricate a new rational function,

J (Z) = H(R(Z))

The gain of the new ¯lter J at the frequency ! is then equal to that of H at a di®erent frequency Á, chosen so that:

cos(Á) + i sin(Á) = R(cos(!) + i sin(!))

The function R moves points around on the unit circle; J at any point equals H on the point R moves it to.

For example, suppose we start with a one-zero, one-pole low-pass ¯lter:

1 + Z¡1 H(Z) =

1 ¡ gZ¡1

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.421.png) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.422.png)

(a) (b)

Figure 8.19: One-pole, one-zero low-pass ¯lter: (a) pole-zero plot; (b) plot for the resulting ¯lter after the transformation R(Z) = ¡Z 2. The result is a band-

pass ¯lter with center frequency ¼=2.

and apply the function

R(Z) = ¡Z 2 = ¡ 1 ¢Z2 + 0 ¢Z + 0

0 ¢Z2 + 0 ¢Z + 1

Geometrically, this choice of R stretches the unit circle uniformly to twice its circumference and wraps it around itself twice. The points 1 and ¡1 are both sent to the point ¡1, and the points i and ¡i are sent to the point 1. The resulting transfer function is

1 ¡ Z¡2 (1 ¡ Z¡1)(1 + Z¡1)

J (Z) =~~ = p p ![ref6]![ref6]

1 + gZ¡2 (1 ¡ i gZ¡1)(1 + i gZ¡1)

The pole-zero plots of H and J are shown in Figure 8.19. From a low-pass ¯lter we ended up with a band-pass ¯lter. The points i and ¡i which R sends to 1 (where the original ¯lter's gain is highest) become points of highest gain for the new ¯lter.

8. Butterworth band-pass ¯lter

We can apply the transformation R(Z) = ¡Z 2 to convert the Butterworth ¯lter into a high-quality band-pass ¯lter with center frequency ¼=2. A further transformation can then be applied to shift the center frequency to any desired value ! between 0 and ¼. The transformation will be of the form,

aZ + b S(Z) =

bZ + a

where a and b are real numbers and not both are zero. This is a particular case of the general form given above for unit-circle-preserving rational functions. We have S(1) = 1 and S(¡1) = ¡1, and the top and bottom halves of the unit circle are transformed symmetrically (if Z goes to W then Z goes to W). The qualitative e®ect of the transformation S is to squash points of the unit circle toward 1 or ¡1.

In particular, given a desired center frequency !, we wish to choose S so that:

S(cos(!) + i sin(!)) = i

If we leave R = ¡Z 2 as before, and let H be the transfer function for a low-pass Butterworth ¯lter, then the combined ¯lter with transfer function H(R(S(Z))) will be a band-pass ¯lter with center frequency !. Solving for a and b gives:

- ! ¼ !

a = cos( ¡ ); b= sin( ¡ )

4 2 4 2

The new transfer function, H(R(S(Z))), will have 2n poles and 2n zeros (if n is the degree of the Butterworth ¯lter H).

Knowing the transfer function is good, but even better is knowing the lo- cations of all the poles and zeros of the new ¯lter, which we need to be able to compute it using elementary ¯lters. If Z is a pole of the transfer function J (Z) = H(R(S(Z))), that is, if J (Z) = 1, then R(S(Z)) must be a pole of H. The same goes for zeros. To ¯nd a pole or zero of J we set R(S(Z)) = W, where W is a pole or zero of H, and solve for Z. This gives:

- aZ + b¸2
- = W bZ + a

  aZ + b p ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.424.png)

- § ¡W

bZ + a

p

§a ¡W ¡ b Z = p ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.425.png)

¨b ¡W + a

(Here a and b are as given above and we have used the fact that a2 + b2 = 1). A sample pole-zero plot and frequency response of J are shown in Figure 8.20.

9. Time-varying coe±cients

In some recursive ¯lter designs, changing the coe±cients of the ¯lter can inject energy into the system. A physical analogue is a child on a swing set. The child oscillates back and forth at the resonant frequency of the system, and pushing or pulling the child injects or extracts energy smoothly. However, if you decide to shorten the chain or move the swing set itself, you may inject an unpredictable amount of energy into the system. The same thing can happen when you change the coe±cients in a resonant recirculating ¯lter.

The simple one-zero and one-pole ¯lters used here don't have this di±culty; if the feedback or feed-forward gain is changed smoothly (in the sense of an

3   3   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.426.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.427.png)

0  

(a) (b)

Figure 8.20: Butterworth band-pass ¯lter: (a) pole-zero diagram; (b) frequency response. The center frequency is ¼=4. The bandwidth depends both on center frequency and on the bandwidth of the original Butterworth low-pass ¯lter used.

amplitude envelope) the output will behave smoothly as well. But one subtlety arises when trying to normalize a recursive ¯lter's output when the feedback gain is close to one. For example, suppose we have a one-pole low-pass ¯lter with gain 0.99 (for a cuto® frequency of 0.01 radians, or 70 Hertz at the usual sample rate). To normalize this for unit DC gain we multiply by 0.01. Suppose now we wish to double the cuto® frequency by changing the gain slightly to 0.98. This is ¯ne except that the normalizing factor suddenly doubles. If we multiply the ¯lter's output by the normalizing factor, the output will suddenly, although perhaps only momentarily, jump by a factor of two.

The trick is to normalize at the input ofthe ¯lter, not the output. Figure 8.21 (part a) shows a complex recirculating ¯lter, with feedback gain P , normalized at the input by 1 ¡ jP j so that the peak gain is one. Part (b) shows the wrong way to do it, multiplying at the output.

Things get more complicated when several elementary recirculating ¯lters are put in series, since the correct normalizing factor is in general a function of all the coe±cients. One possible approach, if such a ¯lter is required to change rapidly, is to normalize each input separately as if it were acting alone, then multiplying the output, ¯nally, by whatever further correction is needed.

10. Impulse responses of recirculating ¯lters

In Section 7.4 we analyzed the impulse response of a recirculating comb ¯lter, of which the one-pole low-pass ¯lter is a special case. Figure 8.22 shows the result for two low-pass ¯lters and one complex one-pole resonant ¯lter. All are ele- mentary recirculating ¯lters as introduced in Section 8.2.3. Each is normalized

IN 

IN ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.428.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.429.png)

1-|P|

1-|P| OUT d=1

d=1 OUT

P  

P  

(a - right) (b - wrong)

Figure 8.21: Normalizing a recirculating elementary ¯lter: (a) correctly, by multiplying in the normalization factor at the input; (b) incorrectly, multiplying at the output.

to have unit maximum gain.

In the case of a low-pass ¯lter, the impulse response gets longer (and lower) as the pole gets closer to one. Suppose the pole is at a point 1 ¡ 1=n (so that the cuto® frequency is 1=n radians). The normalizing factor is also 1=n. After n points, the output diminishes by a factor of

µ 1¶n 1 1 ¡ ¼

n e

where e is Euler's constant, about 2.718. The ¯lter can be said to have a settling time of n samples. In the ¯gure, n = 5 for part (a) and n = 10 for part (b). In general, the settling time (in samples) is approximately one over the cuto® frequency (in angular units).

The situation gets more interesting when we look at a resonant one-pole ¯lter, that is, one whose pole lies o®the real axis. In part (c) of the ¯gure, the pole P has absolute value 0.9 (as in part b), but its argument is set to 2¼=10 radians. We get the same settling time as in part (b), but the output rings at the resonant frequency (and so at a period of 10 samples in this example).

A natural question to ask is, how many periods of ringing do we get before the ¯lter decays to strength 1=e? If the pole of a resonant ¯lter has magnitude 1 ¡ 1=n as above, we have seen in Section 8.2.3 that the bandwidth (call it b) is about 1=n, and we see here that the settling time is about n. The resonant frequency (call it !) is the argument of the pole, and the period in samples of the ringing is 2¼=!. The number of periods that make up the settling time is

4. APPLICATIONS 256

1/5![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.430.png)

(a)

1/(5e)

5   n  

1/10![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.431.png)

(b)

1/(10e)

10 

1/10![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.432.png)

(c)~~ 1/(10e)

10 

Figure 8.22: The impulse response of three elementary recirculating (one-pole) ¯lters, normalized for peak gain 1: (a) low-pass with P = 0:8; (b) low-pass with P = 0:9; (c) band-pass (only the real part shown), with jP j = 0:9 and a center frequency of 2¼=10.

thus:

n 1 ! q

- =

2¼=! 2¼ b 2¼

where q is the quality of the ¯lter, de¯ned as the center frequency divided by bandwidth. Resonant ¯lters are often speci¯ed in terms of the center frequency and \q" in place of bandwidth.

11. All-pass ¯lters

Sometimes a ¯lter is applied to get a desired phase change, rather than to alter the amplitudes of the frequency components of a sound. To do this we would need a way to design a ¯lter with a constant, unit frequency response but which changes the phase of an incoming sinusoid in a way that depends on its frequency. We have already seen in Chapter 7 that a delay of length d introduces a phase change of ¡d!, at the angular frequency !. Another class of ¯lters, called all-pass ¯lters, can make phase changes which are more interesting functions of !.

To design an all-pass ¯lter, we start with two facts: ¯rst, an elementary recirculating ¯lter and an elementary non-recirculating one cancel each other out perfectly if they have the same gain coe±cient. In other words, if a signal has been put through a one-zero ¯lter, either real or complex, the e®ect can be reversed by sequentially applying a one-pole ¯lter, and vice versa.

The second fact is that the elementary non-recirculating ¯lter of the second form has the same frequency response as that of the ¯rst form; they di®er only in phase response. So if we combine an elementary recirculating ¯lter with an elementary non-recirculating one of the second form, the frequency responses cancel out (to a °at gain independent of frequency) but the phase response is not constant.

To ¯nd the transfer function, we choose the same complex number P < 1 as coe±cient for both elementary ¯lters and multiply their transfer functions:

P ¡ Z¡1 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.433.png)H(Z) =

1 ¡ P Z¡1

The coe±cient P controls both the location of the one pole (at P itself) and the zero![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.434.png) (at 1=P ). Figure 8.23 shows the phase response of the all-pass ¯lter for four real-valued choices p of the coe±cient. At frequencies of 0, ¼, and 2¼, the phase response is just that of a one-sample delay; but for frequencies in between, the phase response is bent upward or downward depending on the coe±cient.

Complex coe±cients give similar phase response curves, but the frequencies at which they cross the diagonal line in the ¯gure are shifted according to the argument of the coe±cient P .

4. Applications

Filters are used in a broad range of applications both in audio engineering and in electronic music. The former include, for instance, equalizers, speaker

2  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.435.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.436.png)

0\.4

p=0.8

0  

-0.8

0  

0   ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.437.png) 2  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.438.png)

Figure 8.23: Phase response of all-pass ¯lters with di®erent pole locations p. When the pole is located at zero, the ¯lter reduces to a one-sample delay.

crossovers, sample rate converters, and DC removal (which we have already used in earlier chapters). Here, though, we'll be concerned with the speci¯cally musical applications.

1. Subtractive synthesis

Subtractive synthesis is the technique of using ¯lters to shape the spectral en- velope of a sound, forming another sound, usually preserving qualities of the original sound such as pitch, roughness, noisiness, or graniness. The spectral envelope of the resulting sound is the product of the spectral envelope of the original sound with the frequency response of the ¯lter. Figure 8.24 shows a possible con¯guration of source, ¯lter, and result.

The ¯lter may be constant or time-varying. Already in wide use by the mid 1950s, subtractive synthesis boomed with the introduction of the voltage- controlled ¯lter (VCF), which became widely available in the mid 1960s with the appearance of modular synthesizers. A typical VCF has two inputs: one for the sound to ¯lter, and one to vary the center or cuto® frequency of the ¯lter.

A popular use of a VCF is to control the center frequency of a resonant ¯lter from the same ADSR generator that controls the amplitude; a possible block diagram is shown in Figure 8.25. In this con¯guration, the louder portion of a note (loudness roughly controlled by the multiplier at the bottom) may also be made to sound brighter, using the ¯lter, than the quieter parts; this can mimic the spectral evolution of strings or brass instruments over the life of a note.

(a) amplitude![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.439.png)

frequency

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.440.png)

(c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.441.png)

Figure 8.24: Subtractive synthesis: (a) spectrum of input sound; (b) ¯lter fre- quency response; (c) spectrum of output sound.

frequency

center frequency![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.442.png)

OUT

Figure 8.25: ADSR-controlled subtractive synthesis.

2. Envelope following

It is frequently desirable to use the time-varying power of an incoming signal to trigger or control a musical process. To do this, we will need a procedure for measuring the power of an audio signal. Since most audio signals pass through zero many times per second, it won't su±ce to take instantaneous values of the signal to measure its power; instead, we must calculate the average power over an interval of time long enough that its variations won't show up in the power estimate, but short enough that changes in signal level are quickly reported. A computation that provides a time-varying power estimate of a signal is called an envelope follower.

The output of a low-pass ¯lter can be viewed as a moving average of its input. For example, suppose we apply a normalized one-pole low-pass ¯lter with coe±cient p, as in Figure 8.21, to an incoming signal x[n]. The output (call it y[n]) is the sum of the delay output times p, with the input times 1¡ p:

y[n] = p ¢y[n ¡ 1]+ (1 ¡ p) ¢x[n]

so each input is averaged, with weight 1¡p, into the previous output to produce a new output. So we can make a moving average of the square of an audio signal using the diagram of Figure 8.26. The output is a time-varying average of the instantaneous power x[n]2, and the design of the low-pass ¯lter controls, among other things, the settling time of the moving average.

IN 

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.443.png)

OUT

Figure 8.26: Envelope follower. The output is the average power of the input signal.

For more insight into the design of a suitable low-pass ¯lter for an envelope follower, we analyze it from the point of view of signal spectra. If, for instance, we put in a real-valued sinusoid:

x[n] = a ¢cos(®n)

the result of squaring is:

x[n]2 = a2 (cos(2®n) + 1)

2

and so if the low-pass ¯lter e®ectively stops the component of frequency 2® we will get out approximately the constant a2=2, which is indeed the average

power.

The situation for a signal with several components is similar. Suppose the input signal is now,

x[n] = a ¢cos(®n) + b¢cos(¯n)

whose spectrum is plotted in Figure 8.27 (part a). (We have omitted the two phase terms but they will have no e®ect on the outcome.) Squaring the signal produces the spectrum shown in part (b) (see Section 5.2).) We can get the desired ¯xed value of (a2+b2)=2 simply by ¯ltering out all the other components; ideally the result will be a constant (DC) signal. As long as we ¯lter out all the partials, and also all the di®erence tones, we end up with a stable output that correctly estimates the average power.

Envelope followers may also be used on noisy signals, which may be thought ofas signals with dense spectra. In this situation there will be di®erence frequen- cies arbitrarily close to zero, and ¯ltering them out entirely will be impossible;

257 CHAPTER 8. FILTERS

amplitude

1) b/2![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.444.png)

a/2

frequency

2  2  a +b![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.445.png)

2  (b)

0   -   2   +   2  

Figure 8.27: Envelope following from the spectral point of view: (a) an incoming signal with two components; (b) the result of squaring it.

we will always get °uctuations in the output, but they will decrease proportion- ally as the ¯lter's passband is narrowed.

Although a narrower passband will always give a cleaner output, whether for discrete or continuous spectra, the ¯lter's settling time will lengthen propor- tionally as the passband is narrowed. There is thus a tradeo® between getting a quick response and a smooth result.

3. Single Sideband Modulation

As we saw in Chapter 5, multiplying two real sinusoids together results in a sig- nal with two new components at the sum and di®erence of the original frequen- cies. If we carry out the same operation with complex sinusoids, we get only one new resultant frequency; this is one result of the greater mathematical simplicity of complex sinusoids as compared to real ones. If we multiply a complex sinu-

soid 1;Z;Z 2;::: with another one, 1;W;W 2;::: the result is 1;WZ;(WZ)2;:::, which is another complex sinusoid whose frequency, 6 (ZW), is the sum of the![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.446.png)

two original frequencies.

In general, since complex sinusoids have simpler properties than real ones, it is often useful to be able to convert from real sinusoids to complex ones. In other words, from the real sinusoid:

x[n] = a ¢cos(!n)

5. EXAMPLES 259

(with a spectral peak of amplitude a=2 and frequency !) we would like a way of computing the complex sinusoid:

X[n] = a (cos(!n) + i sin(!n)) so that

x[n] = re(X[n])

We would like a linear process for doing this, so that superpositions of sinusoids get treated as if their components were dealt with separately.

Of course we could equally well have chosen the complex sinusoid with fre- quency ¡!:

X 0[n] = a (cos(!n) ¡ i sin(!n))

and in fact x[n] is just half the sum of the two. In essence we need a ¯lter that will pass through positive frequencies (actually frequencies between 0 and ¼, corresponding to values of Z on the top half of the complex unit circle) from negative values (from ¡¼ to 0, or equivalently, from ¼ to 2¼|the bottom half of the unit circle).

One can design such a ¯lter by designing a low-pass ¯lter with cuto® fre- quency ¼=2, and then performing a rotation by ¼=2 radians using the technique of Section 8.3.4. However, it turns out to be easier to do it using two specially designed networks of all-pass ¯lters with real coe±cients.

Calling the transfer functions of the two ¯lters H1 and H2, we design the ¯lters so that

½

6 (H (Z)) ¡ 6 (H (Z)) ¼ 6![ref7]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.448.png)

¼=2 0 < (Z) < ¼![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.449.png)

1 2 ¡¼=2 ¡¼< 6 (Z) < 0

or in other words,

H1(Z) ¼ iH2(Z); 0 < 6 (Z) < ¼![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.450.png)

H1(Z) ¼ ¡iH2(Z); ¡¼< 6 (Z) < 0![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.451.png)

Then for any incoming real-valued signal x[n]we simply form a complex number a[n]+ ib[n] where a[n] is the output of the ¯rst ¯lter and b[n] is the output of the second. Any complex sinusoidal component of x[n] (call it Z n

transformed to (Z) + iH (Z) ¼ ½ 1(Z) 0 < (Z) < ¼ ) will be

H1 2 0 otherwise6

2H![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.452.png)

Having started with a real-valued signal, whose energy is split equally into positive and negative frequencies, we end up with a complex-valued one with only positive frequencies.

5. Examples

In this section we will ¯rst introduce some easy-to-use prefabricated ¯lters avail- able in Pd to develop examples showing applications from the previous section. Then we will show some more sophisticated applications that require specially designed ¯lters.

5. EXAMPLES 

noise~ white noise,![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.453.png)

test signal

0 <-- cutoff

lop~ low-pass filter |  

(OUT)

(a)

sinusoidal osc~ 220 test signal

+~ 1 add "DC"![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.454.png)

0

hip~ 5 high-pass filter |  

(OUT)

(b)

5. EXAMPLES 261

Figure 8.28: Using prefabricated ¯lters in Pd: (a) a low-pass ¯lter, with white noise as a test input; (b) using a high-pass ¯lter to remove a signal component of frequency 0.

Prefabricated low-, high-, and band-pass ¯lters

Patches H01.low-pass.pd, H02.high-pass.pd, and H03.band-pass.pd (Figure 8.28) show Pd's built-in ¯lters, which implement ¯lter designs described in Sections 8.3.1, 8.3.2 and 8.3.4. Two of the patches also use a noise generator we have not introduced before. We will need four new Pd objects:

lop~ : one-pole low-pass ¯lter. The left inlet takes a signal to be ¯ltered, and the![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.455.png) right inlet takes control messages to set the cuto® frequency of the ¯lter. The ¯lter is normalized so that the gain is one at frequency 0.

hip~ : one-pole, one-zero high-pass ¯lter, with the same inputs and outputs as![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.456.png) lop~, normalized to have a gain of one at the Nyquist frequency.

bp~ : resonant ¯lter. The middle inlet takes control messages to set the center ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.457.png)frequency, and the right inlet to set \q".

noise~ : white noise generator. Each sample is an independent pseudo- random![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.458.png) number, uniformly distributed from -1 to 1.

The ¯rst three example patches demonstrate these three ¯lters (see Figure 8.28). The lop~ and bp~ objects are demonstrated with noise as input; hip~ as shown is used to remove the DC (zero frequency) component of a signal.

Prefabricated time-varying band-pass ¯lter

Time-varying band-pass ¯ltering, as often used in classical subtractive synthesis (Section 8.4.1), can be done using the vcf~ object, introduced here:

vcf~ : a \voltage controlled" band-pass ¯lter, similar to bp~, but with a signal![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.459.png)

0 pitch mtof![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.460.png)

sawtooth phasor~ oscillator

0 sweep speed phasor~ LFO for sweep

0 sweep depth

\*~ 

0 base center frequency

+~  add base to sweep tabread4~ mtof convert to Hz.

0 Q (selectivity)

vcf~

|  (OUT)

Figure 8.29: The vcf~ band-pass ¯lter, with its center frequency controlled by an audio signal (as compared to bp~ which takes only control messages to set its center frequency.

inlet to control center frequency. Both bp~ and vcf~ are one-pole resonant ¯lters as developed in Section 8.3.4; bp~ outputs only the real part of the resulting signal, while vcf~ outputs the real and imaginary parts separately.

Example H04.¯lter.sweep.pd (Figure 8.29) demonstrates using the vcf~ ob- ject for a simple and characteristic subtractive synthesis task. A phasor~ object (at top) creates a sawtooth wave to ¯lter. (This is not especially good practice as we are not controlling the possibility of foldover; a better sawtooth generator for this purpose will be developed in Chapter 10.) The second phasor~ object (labeled \LFO for sweep") controls the time-varying center frequency. After adjusting to set the depth and a base center frequency (given in MIDI units), the result is converted into Hertz (using the tabread4~ object) and passed to vcf~ to set its center frequency. Another example of using a vcf~ object for subtractive synthesis is demonstrated in example H05.¯lter.°oyd.pd.

Envelope followers

Example H06.envelope.follower.pd shows a simple and self-explanatory realiza- tion of the envelope follower described in Section 8.4.2. An interesting ap- plication of envelope following is shown in Example H07.measure.spectrum.pd (Figure 8.30, part a). A famous bell sample is looped as a test sound. Rather

5. EXAMPLES 

r $0-loopf phasor~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.461.png)

\*~  r $0-totsamps +~ 1

tabread4~ $0-array signal to analyze

0 test frequency

0 Q  

bp~

bp~

|  (OUT)env~ 4096

0

measured strength

(a)

phasor~ 100

signal to analyze![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.462.png)

0 test frequency phasor~

+~ 0.25

cos~ cos~ modulate

to DC

\*~  \*~  0 responsiveness lop~ lop~ low-pass filter

r $0-tick snapshot~ snapshot~

0 0

real part imaginary part

(b)

5. EXAMPLES 263

Figure 8.30: Analyzing the spectrum of a sound: (a) band-pass ¯ltering a sam- pled bell sound and envelope-following the result; (b) frequency-shifting a partial to DC and reading o®its real and imaginary part.

than get the overall mean square power of the bell, we would like to estimate the frequency and power of each of its partials. To do this we sweep a band-pass ¯lter up and down in frequency, listening to the result and/or watching the ¯l- ter's output power using an envelope follower. (We use two band-pass ¯lters in series for better isolation of the partials; this is not especially good ¯lter design practice but it will do in this context.) When the ¯lter is tuned to a partial the envelope follower reports its strength.

Example H08.heterodyning.pd (part (b) of the ¯gure) shows an alternative way of ¯nding partial strengths of an incoming sound; it has the advantage of reporting the phase as well as the strength. First we modulate the desired partial down to zero frequency. We use a complex-valued sinusoid as a modulator so that we get only one sideband for each component of the input. The test frequency is the only frequency that is modulated to DC; others go elsewhere. We then low-pass the resulting complex signal. (We can use a real-valued low- pass ¯lter separately on the real and imaginary parts.) This essentially removes

sample loop for test signal![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.463.png)

pd bell-loop

pair of allpass 0 shift frequency

filters to make90 degree phase phasor~ cosine and sine waves shifted versions -~ 0.25 to form the real and

imaginary part of a

hilbert~ cos~ cos~ complex sinusoid

\*~  \*~  <-- complex multipier

(calculates real part)

-~ 

|  

(OUT)

Figure 8.31: Using an all-pass ¯lter network to make a frequency shifter.

all the partials except for the DC one, which we then harvest. This technique is the basis of Fourier analysis, the subject of Chapter 9.

Single sideband modulation

As described in Section 8.4.3, a pair of all-pass ¯lters can be constructed to give roughly ¼=2 phase di®erence for positive frequencies and ¡¼=2 for negative ones. The design of these pairs is beyond the scope of this discussion (see, for instance, [Reg93]) but Pd does provide an abstraction, hilbert~, to do this. Example H09.ssb.modulation.pd, shown in Figure 8.31, demonstrates how to use the hilbert~ abstraction to do signal sideband modulation. The Hilbert transform dates to the analog era [Str95, pp.129-132].

The two outputs of hilbert~, considered as the real and imaginary parts of

a complex-valued signal, are multiplied by a complex sinusoid (at right in the ¯gure), and the real part is output. The components of the resulting signal are those of the input shifted by a (positive or negative) frequency speci¯ed in the number box.

Using elementary ¯lters directly: shelving and peaking

No ¯nite set of prefabricated ¯lters could ¯ll every possible need, and so Pd provides the elementary ¯lters of Sections 8.2.1-8.2.3 in raw form, so that the user can supply the ¯lter coe±cients explicitly. In this section we will describe patches that realize the shelving and peaking ¯lters of Sections 8.3.3 and 8.3.5 directly from elementary ¯lters. First we introduce the six Pd objects that realize elementary ¯lters:

264

CHAPTER 8. FILTERS

zero pole (%) 0 0![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.464.png)

(IN) / 100 / 100

|  

rzero~

rpole~

|  (OUT)

(a)

0 angle (degrees)

zero and pole \* 3.14159![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.465.png)

radii (%)

/ 180

0 0

/ 100 / 100 cos sin

t b f t b f

(IN) \*   \*  

|   \*   \*  czero~

cpole~

|  

(OUT)

(b)

265

CHAPTER 8. FILTERS

Figure 8.32: Building ¯lters from elementary, raw ones: (a) shelving; (b) peak- ing.

rzero~ , rzero~~ rev~ , rpole~ : elementary ¯lters with real-valued coe±-![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.466.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.467.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.468.png)

cients operating on real-valued signals. The three implement non-recirculating ¯lters of the ¯rst and second types, and the recirculating ¯lter. They all have one inlet, at right, to supply the coe±cient that sets the location of the zero or pole. The inlet for the coe±cient (as well as the left inlet for the signal to ¯lter) take audio signals. No stability check is performed.

czero~ , czero~~ rev~ , cpole~ : elementary ¯lters with complex-valued![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.469.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.470.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.471.png)

coe±cients, operating on complex-valued signals, corresponding to the real- valued ones above. Instead of two inlets and one outlet, each of these ¯lters has four inlets (real and imaginary part of the signal to ¯lter, and real and imaginary part of the coe±cient) and two outlets for the complex-valued output.

The example patches use a pair of abstractions to graph the frequency and phase responses of ¯lters as explained in Example H10.measurement.pd. Exam- ple H11.shelving.pd (Figure 8.32, part a) shows how to make a shelving ¯lter. One elementary non-recirculating ¯lter (rzero~) and one elementary recircu- lating one (rpole~) are put in series. As the analysis of Section 8.3.9 might suggest, the rzero~ object is placed ¯rst.

Example H12.peaking.pd (part (b) of the ¯gure) implements a peaking ¯lter. Here the pole and the zero are rotated by an angle ! to control the center frequency of the ¯lter. The bandwidth and center frequency gain are equal to the shelf frequency and the DC gain of the corresponding shelving ¯lter.

Example H13.butterworth.pd demonstrates a three-pole, three-zero Butter- worth shelving ¯lter. The ¯lter itself is an abstraction, butterworth3~, for easy


8\.5. EXAMPLES

pole (%)

0![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.472.png)

/ 100

rzero\_rev~

rpole~

|  (OUT)

(a)

261

phasor~ 0.3![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.473.png)

expr~ abs($v1-0.5)

pd chord expr~ 0.97 - 0.6\*$v1\*$v1

rzero\_rev~ rpole~ rzero\_rev~ rpole~ rzero\_rev~

rpole~ rzero\_rev~ rpole~

+~ 

|   (b) (OUT)


Figure 8.33: All-pass ¯lters: (a) making an all-pass ¯lter from elementary ¯lters;

2) using four all-pass ¯lters to build a phaser.

reuse.

Making and using all-pass ¯lters

Example H14.all.pass.pd (Figure 8.33, part a) shows how to make an all-pass ¯lter out of a non-recirculating ¯lter, second form (rzero rev~) and a recir- culating![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.474.png) ¯lter (rpole~). The coe±cient, ranging from -1 to 1, is controlled in hundredths.

Example H15.phaser.pd (part b of the ¯gure) shows how to use four all-pass ¯lters to make a classic phaser. The phaser works by summing the input signal with a phase-altered version of it, making interference e®ects. The amount of phase change is varied in time by varying the (shared) coe±cient of the all-pass ¯lters. The overall e®ect is somewhat similar to a °anger (time-varying comb ¯lter) but the phaser does not impose a pitch as the comb ¯lter does.

262 CHAPTER 8. FILTERS

Exercises

1. A recirculating elementary ¯lter has a pole at i=2. At what angular fre- quency is its gain greatest, and what is the gain there? At what angular frequency is the gain least, and what is the gain there?
1. A shelving ¯lter has a pole at 0.9 and a zero at 0.8. What are: the DC gain; the gain at Nyquist; the approximate transition frequency?
1. Suppose a complex recirculating ¯lter has a pole at P . Suppose further that you want to combine its real and imaginary output to make a single, ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.475.png)real-valued signal equivalent to a two-pole ¯lter with poles at P and P . How would you weight the two outputs?
1. Suppose you wish to design a peaking ¯lter with gain 2 at 1000 Hertz and bandwidth 200 Hertz (at a sample rate of 44100 Hertz). Where, approximately, would you put the upper pole and zero?
1. In the same situation, where would you put the (upper) pole and zero to remove a sinusoid at 1000 Hertz entirely, while attenuating only 3 decibels at 1001 Hertz?
1. A one-pole complex ¯lter is excited by an impulse to make a tone at 1000 Hertz, which decays 10 decibels in one second (at a sample rate of 44100 Hertz). Where would you place the pole? What is the value of \q"?

Chapter 9

Fourier analysis and resynthesis

Among the applications of ¯lters discussed in Chapter 8, we saw how to use heterodyning, combined with a low-pass ¯lter, to ¯nd the amplitude and phase of a sinusoidal component of a signal (Page 257). In this chapter we will re- ¯ne this technique into what is called Fourier analysis. In its simplest form, Fourier analysis takes as input any periodic signal (of period N) and outputs the complex-valued amplitudes of its N possible sinusoidal components. These N complex amplitudes can theoretically be used to reconstruct the original signal exactly. This reconstruction is called Fourier resynthesis.

In this chapter we will start by developing the theory of Fourier analysis and resynthesis of periodic sampled signals. Then we will go on to show how to apply the same techniques to arbitrary signals, whether periodic or not. Finally, we will develop some standard applications such as the phase vocoder.

1. Fourier analysis of periodic signals

Suppose X[n] is a complex-valued signal that repeats every N samples. (We are continuing to use complex-valued signals rather than real-valued ones to simplify the mathematics.) Because of the period N, the values of X[n] for n = 0;:::;N ¡ 1 determine X[n] for all integer values of n.

Suppose further that X[n] can be written as a sum of complex sinusoids of frequency 0, 2¼=N, 4¼=N, :::, 2(N ¡ 1)¼=N. These are the partials, starting with the zeroth, for a signal of period N. We stop at the Nth term because the next one would have frequency 2¼, equivalent to frequency 0, which is already on the list.

Given the values ofX, we wish to ¯nd the complex amplitudes ofthe partials. Suppose we want the kth partial, where 0 · k < N. The frequency ofthis partial is 2¼k=N. We can ¯nd its complex amplitude by modulating X downward 2¼k=N radians per sample in frequency, so that the kth partial is modulated to

263

2. PROPERTIES OF FOURIER TRANSFORMS 273

frequency zero. Then we pass the signal through a low-pass ¯lter with such a low cuto® frequency that nothing but the zero-frequency partial remains. We can do this in e®ect by averaging over a huge number of samples; but since the signal repeats every N samples, this huge average is the same as the average of the ¯rst N samples. In short, to measure a sinusoidal component of a periodic signal, modulate it down to DC and then average over one period.

Let ! = 2¼=N be the fundamental frequency for the period N, and let U be the unit-magnitude complex number with argument !:

U = cos(!) + i sin(!)

The kth partial of the signal X[n] is of the form:

Pk[n] = Ak£Uk¤n

where Ak is the complex amplitude of the partial, and the frequency of the partial is:

6 (Uk) = k6 (U) = k!![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.476.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.477.png)

We're assuming for the moment that the signal X[n] can actually be written as a sum of the n partials, or in other words:

X[n] = A0£U0¤n + A1£U1¤n + ¢¢¢+ AN ¡1£UN ¡1¤n

By the heterodyne-¯ltering argument above, we expect to be able to measure each Ak by multiplying by the sinusoid of frequency ¡k! and averaging over a period:

A = 1 ³£U¡k¤0X[0]+ £U¡k¤1X[1]+ ¢¢¢+ £U¡k¤N ¡1X[N ¡ 1]´

k N

This is such a useful formula that it gets its own notation. The Fourier transform of a signal X[n], over N samples, is de¯ned as:

F T fX[n]g(k) = V0X[0]+ V1X[1]+ ¢¢¢+ VN ¡1X[N ¡ 1]

where V = U¡k. The Fourier transform is a function of the variable k, equal to N times the amplitude of the input's kth partial. So far k has taken integer values but the formula makes sense for any value of k if we de¯ne V more generally as:

V = cos(¡k!) + i sin(¡k!)

where, as before, ! = 2¼=N is the (angular) fundamental frequency associated with the period N.

1. Periodicity of the Fourier transform

If X[n] is, as above, a signal that repeats every N samples, the Fourier transform of X[n] also repeats itself every N units of frequency, that is,

F T fX[n]g(k + N) = F T fX[n]g(k)

for all real values of k. This follows immediately from the de¯nition of the Fourier transform, since the factor

V = cos(¡k!) + i sin(¡k!)

is unchanged when we add N (or any multiple of N) to k.

2. Fourier transform as additive synthesis

Now consider an arbitrary signal X[n] that repeats every N samples. (Previ- ously we had assumed that X[n]could be obtained as a sum of sinusoids, and we haven't yet found out whether every periodic X[n] can be obtained that way.) Let Y[k] denote the Fourier transform of X for k = 0;:::;N ¡ 1:

Y[k] = F T fX[n]g(k)

- ¤0 £ ¤1 £ ¤N ¡1
- U¡k X[0]+ U¡k X[1]+ ¢¢¢+ U¡k X[N ¡ 1]
- £U0¤kX[0]+ £U¡1¤kX[1]+ ¢¢¢+ hU¡(N ¡1) ikX[N ¡ 1]

In the second version we rearranged the exponents to show that Y[k] is a sum of complex sinusoids, with complex amplitudes X[m] and frequencies ¡m! for m = 0;:::;N ¡ 1. In other words, Y[k] can be considered as a Fourier series in its own right, whose mth component has strength X[¡m]. (The expression X[¡m] makes sense because X is a periodic signal). We can also express the amplitude of the partials of Y[k]in terms of its own Fourier transform. Equating the two gives:

1

F T fY[k]g(m) = X[¡m]

N

This means in turn that X[¡m] can be obtained by summing sinusoids with amplitudes Y[k]=N. Setting n = ¡m gives:

1

X[n] = F T fY[k]g(¡n)

N

- £U0 n Y[0]+ £U1¤n Y[1]+ ¢¢¢+ £UN ¡1¤n Y[N ¡ 1] ¤

This shows that any periodic X[n] can indeed be obtained as a sum of sinusoids. Further, the formula explicitly shows how to reconstruct X[n] from its Fourier transform Y[k], if we know its value for the integers k = 0;:::;N ¡ 1.

2. Properties of Fourier transforms

In this section we will investigate what happens when we take the Fourier trans- form of a (complex) sinusoid. The simplest one is \DC", the special sinusoid of frequency zero. After we derive the Fourier transform of that, we will develop some properties of Fourier transforms that allow us to apply the result to any other sinusoid.

1. Fourier transform of DC

Let X[n] = 1 for all n (this repeats with any desired integer period N > 1). From the preceding discussion, we expect to ¯nd that

½

N k = 0

F T fX[n]g(k) =

0  k = 1;:::;N ¡ 1

We will often need to know the answer for non-integer values of k however, and for this there is nothing better to do than to calculate the value directly:

F T fX[n]g(k) = V0X[0]+ V1X[1]+ ¢¢¢+ VN ¡1X[N ¡ 1]

where V is, as before, the unit magnitude complex number with argument ¡k!. This is a geometric series; as long as V 6= 1 we get:

VN ¡ 1 F T fX[n]g(k) =

V ¡ 1

We now symmetrize the top and bottom in the same way as we earlier did in Section 7.3. To do this let:

» = cos(¼k=N) ¡ i sin(¼k=N)

so that »2 = V. Then factoring appropriate powers of » out of the numerator and denominator gives:

F T fX[n]g(k) = »N ¡1 »N ¡ »¡N »¡ »¡1

It's easy now to simplify the numerator:

»N ¡ »¡N = (cos(¼k) ¡ i sin(¼k)) ¡ (cos(¼k) + i sin(¼k)) = ¡2i sin(¼k)

and similarly for the denominator, giving:

- ´ sin(¼k)

F T fX[n]g(k) = cos(¼k(N ¡ 1)=N) ¡ i sin(¼k(N ¡ 1)=N)

sin(¼k=N ) Whether V = 1 or not, we have

- ´

F T fX[n]g(k) = cos(¼k(N ¡ 1)=N) ¡ i sin(¼k(N ¡ 1)=N) DN (k)

where DN (k), known as the Dirichlet kernel, is de¯ned as

(

N k = 0

DN (k) = sin(¼k) k 6= 0; ¡N < k < N

sin(¼k=N )

Figure 9.1 shows the Fourier transform of X[n] = 1, with N = 100. The transform repeats every 100 samples, with a peak at k = 0, another at k = 100,

real![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.478.png)

-5  0   5   k  

imagi- nary

Figure 9.1: The Fourier transform of a signal consisting of all ones. Here N=100, and values are shown for k ranging from -5 to 10. The result is complex-valued and shown as a projection, with the real axis pointing up the page and the imaginary axis pointing away from it.

and so on. The ¯gure endeavors to show both the magnitude and phase behavior using a 3-dimensional graph projected onto the page. The phase term

cos(¼k(N ¡ 1)=N) ¡ i sin(¼k(N ¡ 1)=N)

acts to twist the values of F T fX[n]g(k) around the k axis with a period of approximately two. The Dirichlet kernel DN (k), shown in Figure 9.2, controls the magnitude of F T fX[n]g(k). It has a peak, two units wide, around k = 0. This is surrounded by one-unit-wide sidelobes, alternating in sign and gradually decreasing in magnitude as k increases or decreases away from zero. The phase term rotates by almost ¼ radians each time the Dirichlet kernel changes sign, so that the product of the two stays roughly in the same complex half-plane for k > 1 (and in the opposite half-plane for k < ¡1). The phase rotates by almost 2¼radians over the peak from k = ¡1 to k = 1.

2. Shifts and phase changes

Section 7.2 showed how time-shifting a signal changes the phases of its sinusoidal components, and Section 8.4.3 showed how multiplying a signal by a complex sinusoid shifts its component frequencies. These two e®ects have corresponding identities involving the Fourier transform.

First we consider a time shift. If X[n], as usual, is a complex-valued signal

3. FOURIER ANALYSIS OF NON-PERIODIC SIGNALS 279

-5  0   5  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.479.png)

frequency (bins) Figure 9.2: The Dirichlet kernel, for N = 100.

that repeats every N samples, let Y[n] be X[n] delayed d samples:

Y[n] = X[n ¡ d]

which also repeats every N samples since X does. We can reduce the Fourier transform of Y[n] this way:

F T fY[n]g(k) = V0Y[0]+ V1Y[1]+ ¢¢¢+ VN ¡1Y[N ¡ 1]

- V0X[¡d]+ V1X[¡d + 1]+ ¢¢¢+ VN ¡1X[¡d + N ¡ 1]
  - VdX[0]+ Vd+1 X[1]+ ¢¢¢+ Vd+N ¡1X[N ¡ 1]
- ¢
- Vd V0X[0]+ V1X[1]+ ¢¢¢+ VN ¡1X[N ¡ 1]
  - VdF T fX[n]g(k)

(The third line is just the second one with the terms summed in a di®erent order). We therefore get the Time Shift Formula for Fourier Transforms:

- ´

F T fX[n ¡ d]g(k) = cos(¡dk!) + i sin(¡dk!) F T fX[n]g(k)

The Fourier transform of X[n ¡ d] is a phase term times the Fourier transform of X[n]. The phase is changed by ¡dk!, a linear function of the frequency k.

Now suppose instead that we change our starting signal X[n] by multiplying it by a complex exponential Z n with angular frequency ®:

Y[n] = Zn X[n]

Z = cos(®) + i sin(®)

The Fourier transform is:

F T fY[n]g(k) = V0Y[0]+ V1Y[1]+ ¢¢¢+ VN ¡1Y[N ¡ 1]

- V0X[0]+ V1ZX[1]+ ¢¢¢+ VN ¡1ZN ¡1X[N ¡ 1]
- (VZ)0X[0]+ (VZ)1X[1]+ ¢¢¢+ (VZ)N ¡1X[N ¡ 1] ®
  - F T fX[n]g(k ¡ )

!

We therefore get the Phase Shift Formula for Fourier Transforms:

®N F T f(cos(®) + i sin(®))X[n]g(k) = F T fX[n]g(k ¡ ) 2¼

3. Fourier transform of a sinusoid

We can use the phase shift formula above to ¯nd the Fourier transform of any complex sinusoid Z n with frequency ®, simply by setting X[n] = 1 in the formula

and using the Fourier transform for DC:

F T fZn g(k) = F T f1g(k ¡ ®)

!

®

- [cos(©(k)) + i sin(©(k))] DN (k ¡ )

! where DN is the Dirichlet kernel and © is an ugly phase term:

®

©(k) = ¡¼¢(k ¡ ) ¢(N ¡ 1)=N

!

If the sinusoid's frequency ® is an integer multiple of the fundamental fre- quency !, the Dirichlet kernel is shifted to the left or right by an integer. In this case the zero crossings of the Dirichlet kernel line up with integer values of k, so that only one partial is nonzero. This is pictured in Figure 9.3 (part a).

Part (b) shows the result when the frequency ® falls halfway between two integers. The partials have amplitudes falling o®roughly as 1=k in both direc- tions, measured from the actual frequency ®. That the energy should be spread over many partials, when after all we started with a single sinusoid, might seem surprising at ¯rst. However, as shown in Figure 9.4, the signal repeats at a period N which disagrees with the frequency of the sinusoid. As a result there is a discontinuity at the beginning of each period, and energy is °ung over a wide range of frequencies.

3. Fourier analysis of non-periodic signals

Most signals aren't periodic, and even a periodic one might have an unknown period. So we should be prepared to do Fourier analysis on signals without making the comforting assumption that the signal to analyze repeats at a ¯xed period N. Of course, we can simply take N samples of the signal and make it periodic; this is essentially what we did in the previous section, in which a pure sinusoid gave us the complicated Fourier transform of Figure 9.3 (part b).

amplitude![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.480.png)

(a)

-5  0   5  

k->

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.481.png)

0   5  

-5 

Figure 9.3: Fourier transforms of complex sinusoids, with N = 100: (a) with frequency 2! ; (b) with frequency 1:5!. (The e®ect of the phase winding term is not shown.)

0   100 200![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.482.png)

Figure 9.4: A complex sinusoid with frequency ® = 1:5! = 3¼=N, forced to repeat every N samples. (N is arbitrarily set to 100; only the real part is shown.)

However, it would be better to get a result in which the response to a pure sinusoid were better localized around the corresponding value of k. We can accomplish this using the enveloping technique ¯rst introduced in Figure 2.7 (Page 38). Applying this technique to Fourier analysis will not only improve our analyses, but will also shed new light on the enveloping looping sampler of Chapter 2.

Given a signal X[n], periodic or not, de¯ned on the points from 0 to N ¡ 1, the technique is to envelope the signal before doing the Fourier analysis. The envelope shape is known as a window function. Given a window function w[n], the windowed Fourier transform is:

F T fw[n]X[n]g(k)

Much ink has been spilled over the design of suitable window functions for particular situations, but here we will consider the simplest one, named the Hann window function (the name is sometimes corrupted to \Hanning" in DSP circles). The Hann window is:

1  1

w[n] = ¡ cos(2¼n=N)

2  2

It is easy to analyze the e®ect of multiplying a signal by the Hann window before taking the Fourier transform, because the Hann window can be written as a sum of three complex exponentials:

w[n] = 1 ¡ 1Un ¡ 1U¡n

2 4 4

where as before, U is the unit-magnitude complex number with argument 2¼=N. We can now calculate the windowed Fourier transform of a sinusoid Z n with

angular frequency ® as before. The phases come out messy and we'll replace them with simpli¯ed approximations:

F T fw[n]Zn g(k)

- ¾
- F T 1Zn ¡ (UZ)n ¡ 1(U¡1Z)n (k) 1

2 4 4

®

- [cos(©(k)) + i sin(©(k))] M(k ¡ ) !

where the (approximate) phase term is:

®

©(k) = ¡¼¢(k ¡ )

!

and the magnitude function is:

- ¸ 1 1 1

2 N (k) + 4DN (k + 1) + 4DN (k ¡ 1) M(k) = D

amplitude![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.483.png)

M(k)

D (k) N  

D (k-1)

N  

-1  0   1   2   k->

Figure 9.5: The magnitude M(k) of the Fourier transform of the Hann window function. It is the sum of three (shifted and magni¯ed) copies of the Dirichlet kernel DN , with N = 100.

The magnitude function M(k) is graphed in Figure 9.5. The three Dirichlet kernel components are also shown separately.

The main lobe of M(k) is four harmonics wide, twice the width of the main lobe of the Dirichlet kernel. The sidelobes, on the other hand, have much smaller magnitude. Each sidelobe of M(k) is a sum of three sidelobes of Dn (k), one attenuated by 1=2 and the others, opposite in sign, attenuated by 1=4. They do not cancel out perfectly but they do cancel out fairly well.

The sidelobes reach their maximum amplitudes near their midpoints, and we can estimate their amplitudes there, using the approximation:

N sin(¼k) D (k) ¼

N ¼k

Setting k = 3=2;5=2;::: gives sidelobe amplitudes, relative to the peak height N, of:

2 2 2 2

- ¡13dB; ¼ ¡18dB; ¼ ¡21dB; ¼ ¡23dB;:::

3¼ 5¼ 7¼ 9¼

The sidelobes drop o®progressively more slowly so that the tenth one is only attenuated about 30 dB and the 32nd one about -40 dB. On the other hand, the Hann window sidelobes are attenuated by:

2 1 2 2

- [ + ] ¼ ¡32:30dB

5¼ 2 3¼ 7¼

and ¡42, ¡49, ¡54, and ¡59 dB for the next four sidelobes.

This shows that applying a Hann window before taking the Fourier transform will better allow us to isolate sinusoidal components. If a signal has many

real![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.484.png)

0   5   10  k  

imagi- nary

Figure 9.6: The Hann-windowed Fourier transform of a signal with two sinu- soidal components, at frequencies 5.3 and 10.6 times the fundamental, and with di®erent complex amplitudes.

sinusoidal components, the sidelobes engendered by each one will interfere with the main lobe of all the others. Reducing the amplitude of the sidelobes reduces this interference.

Figure 9.6 shows a Hann-windowed Fourier analysis of a signal with two sinusoidal components. The two are separated by about 5 times the fundamental frequency !, and for each we see clearly the shape of the Hann window's Fourier transform. Four points of the Fourier analysis lie within the main lobe of M(k) corresponding to each sinusoid. The amplitude and phase of the individual sinusoids are re°ected in those of the (four-point-wide) peaks. The four points within a peak which happen to fall at integer values k are successively about one half cycle out of phase.

To fully resolve the partials of a signal, we should choose an analysis size N large enough so that ! = 2¼=N is no more than a quarter of the frequency separation between neighboring partials. For a periodic signal, for example, the partials are separated by the fundamental frequency. For the analysis to fully resolve the partials, the analysis period N must be at least four periods of the signal.

In some applications it works to allow the peaks to overlap as long as the center of each peak is isolated from all the other peaks; in this case the four- period rule may be relaxed to three or even slightly less.

4. FOURIER ANALYSIS AND RECONSTRUCTION OF AUDIO SIGNALS275
4. Fourier analysis and reconstruction of audio signals

Fourier analysis can sometimes be used to resolve the component sinusoids in an audio signal. Even when it can't go that far, it can separate a signal into frequency regions, in the sense that for each k, the kth point of the Fourier transform would be a®ected only by components close to the nominal frequency k!. This suggests many interesting operations we could perform on a signal by taking its Fourier transform, transforming the result, and then reconstructing a new, transformed, signal from the modi¯ed transform.

Figure 9.7 shows how to carry out a Fourier analysis, modi¯cation, and reconstruction of an audio signal. The ¯rst step is to divide the signal into windows, which are segments of the signal, of N samples each, usually with some overlap. Each window is then shaped by multiplying it by a windowing function (Hann, for example). Then the Fourier transform is calculated for the N points k = 0;1;:::;N ¡ 1. (Sometimes it is desirable to calculate the Fourier transform for more points than this, but these N points will su±ce here.)

The Fourier analysis gives us a two-dimensional array of complex numbers. Let H denote the hop size, the number of samples each window is advanced past the previous window. Then for each m = :::;0;1;:::, the mth window consists of the N points starting at the point mH . The nth point of the mth window is mH + n. The windowed Fourier transform is thus equal to:

S[m; k] = F Tfw(n)X[n ¡ mH ]g(k)

This is both a function of time (m, in units of H samples) and of frequency (k, as a multiple of the fundamental frequency !). Fixing the frame number m and looking at the windowed Fourier transform as a function of k:

S[k] = S[m; k]

gives us a measure of the momentary spectrum of the signal X[n]. On the other hand, ¯xing a frequency k we can look at it as the kth channel of an N-channel signal:

C[m] = S[m; k]

From this point of view, the windowed Fourier transform separates the original signal X[n] into N narrow frequency regions, called bands.

Having computed the windowed Fourier transform, we next apply any de- sired modi¯cation. In the ¯gure, the modi¯cation is simply to replace the upper half of the spectrum by zero, which gives a highly selective low-pass ¯lter. (Two other possible modi¯cations, narrow-band companding and vocoding, are de- scribed in the following sections.)

Finally we reconstruct an output signal. To do this we apply the inverse of the Fourier transform (labeled \iFT" in the ¯gure). As shown in Section 9.1.2 this can be done by taking another Fourier transform, normalizing, and °ipping the result backwards. In case the reconstructed window does not go smoothly

INPUT

extract ... windows![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.485.png)

shape windows

Fourier

analysis FT  FT 

modifi-

cation ANYTHING ANYTHING Fourier

resynth- iFT iFT esis

shape windows again

overlap-

add ...

OUTPUT

Figure 9.7: Sliding-window analysis and resynthesis of an audio signal using Fourier transforms. In this example the signal is ¯ltered by multiplying the Fourier transform with a desired frequency response.

4. FOURIER ANALYSIS AND RECONSTRUCTION OF AUDIO SIGNALS277

to zero at its two ends, we apply the Hann windowing function a second time. Doing this to each successive window of the input, we then add the outputs, using the same overlap as for the analysis.

If we use the Hann window and an overlap of four (that is, choose N a multiple offour and space each window H = N=4 samples past the previous one), we can reconstruct the original signal faithfully by omitting the \modi¯cation" step. This is because the iFT undoes the work of the F T, and so we are multiplying each window by the Hann function squared. The output is thus the input, times the Hann window function squared, overlap-added by four. An easy check shows that this comes to the constant 3=2, so the output equals the input times a constant factor.

The ability to reconstruct the input signal exactly is useful because some types of modi¯cation may be done by degrees, and so the output can be made to vary smoothly between the input and some transformed version of it.

1. Narrow-band companding

A compander is a tool that ampli¯es a signal with a variable gain, depending on the signal's measured amplitude. The term is a contraction of \compressor" and \expander". A compressor's gain decreases as the input level increases, so that the dynamic range, that is, the overall variation in signal level, is reduced. An expander does the reverse, increasing the dynamic range. Frequently the gain depends not only on the immediate signal level but on its history; for instance the rate of change might be limited or there might be a time delay.

By using Fourier analysis and resynthesis, we can do companding individu- ally on narrow-band channels. If C[m] is one such band, we apply a gain g[m] to it, to give g[m]C[m]. Although C[m] is a complex number, the gain is a non- negative real number. In general the gain could be a function not only of C[m] but also of any or all the previous samples in the channel: C[m ¡ 1], C[m ¡ 2], and so on. Here we'll consider the simplest situation where the gain is simply a function of the magnitude of the current sample: jC[m]j.

The patch diagrammed in Figure 9.8 shows one very useful application of companding, called a noise gate. Here the gain g[m] depends on the channel amplitude C[m] and a noise °oor which is a function f of the channel number

k. For clarity we will apply the frequency subscript k to the gain, now written as g[m; k], and to the windowed Fourier transform S[m; k] = C[m]. The gain is given by: ½

1 ¡ f [k]=jS[m; k]j jS[m; k]j > f [k]

g[m; k] =

0 otherwise

Whenever the magnitude S[m; k] is less than the threshold f [k] the gain is zero and so the amplitude S[m; k] is replaced by zero. Otherwise, multiplying the amplitude by g[m; k] reduces the the magnitude downward to jS[m; k]j ¡ f [k]. Since the gain is a non-negative real number, the phase is preserved.

In the ¯gure, the gain is computed as a thresholding function of the ratio x = jS[m; k]j=f[k] of the signal magnitude to the noise °oor; the threshold is

IN 

extract and shape windows![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.486.png)

NOISE FT  FLOOR

|Z|

threshold function

iFT

overlap and add

OUT

Figure 9.8: Block diagram for narrow-band noise suppression by companding.

5. PHASE 289

FILTER CONTROL

INPUT INPUT

window![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.487.png)

FT 

|Z| |Z|

limiting function

iFT

overlap and add

OUT

Figure 9.9: Block diagram for timbre stamping (AKA \vocoding").

g(x) = 1 ¡ 1=x when x < 1 and zero otherwise, although other thresholding functions could easily be substituted.

This technique is useful for removing noise from a recorded sound. We either measure or guess values of the noise °oor f [k]. Because of the design of the gain function g[m; k], only amplitudes which are above the noise °oor reach the output. Since this is done on narrow frequency bands, it is sometimes possible to remove most of the noise even while the signal itself, in the frequency ranges where it is louder than the noise °oor, is mostly preserved.

The technique is also useful as preparation before applying a non-linear operation, such as distortion, to a sound. It is often best to distort only the most salient frequencies of the sound. Subtracting the noise-gated sound from the original then gives a residual signal which can be passed through undistorted.

2. Timbre stamping (classical vocoder)

A second application of Fourier analysis and resynthesis is a time-varying ¯lter capable of making one sound take on the evolving spectral envelope of another. This is widely known in electronic music circles as a vocoder, named, not quite

accurately, after the original Bell Laboratories vocal analysis/synthesis device. The technique described here is more accurately called timbre stamping. Two input signals are used, one to be ¯ltered, and the other to control the ¯lter via its time-varying spectral envelope. The windowed Fourier transform is used both on the control signal input to estimate its spectral envelope, and on the ¯lter input in order to apply the ¯lter.

A block diagram for timbre stamping is shown in Figure 9.9. As in the previous example, the timbre stamp acts by multiplying the complex-valued windowed Fourier transform of the ¯lter input by non-negative real numbers, hence changing their magnitudes but leaving their phases intact. Here the twist is that we want simply to replace the magnitudes of the original, jS[m; k]j, with magnitudes obtained from the control input (call them jT[m; k]j, say). The necessary gain would thus be,

jT[m; k]j g[m; k] =

jS[m; k]j

In practice it is best to limit the gain to some maximum value (which might depend on frequency) since otherwise channels containing nothing but noise, sidelobes, or even truncation error might be raised to audibility. So a suitable limiting function is applied to the gain before using it.

5. Phase

So far we have operated on signals by altering the magnitudes of their win- dowed Fourier transforms, but leaving phases intact. The magnitudes encode the spectral envelope of the sound. The phases, on the other hand, encode fre- quency and time, in the sense that phase change from one window to a di®erent one accumulates, over time, according to frequency. To make a transformation that allows independent control over frequency and time requires analyzing and reconstructing the phase.

In the analysis/synthesis examples of the previous section, the phase of the output is copied directly from the phase of the input. This is appropriate when the output signal corresponds in time with the input signal. Sometimes time modi¯cations are desired, for instance to do time stretching or contraction. Al- ternatively the output phase might depend on more than one input, for instance to morph between one sound and another.

Figure 9.10 shows how the phase of the Fourier transform changes from window to window, given a complex sinusoid as input. The sinusoid's frequency is ®= 3!, so that the peak in the Fourier transform is centered at k = 3. If the initial phase is Á, then the neighboring phases can be ¯lled in as:

6 S[0;2] = Á+ ¼ 6 S[0;3] = Á 6 S[0;4] = Á+ ¼![ref8]![ref8]![ref4]

6 S[1;2] = Á+ H®+ ¼ 6 S[1;3] = Á+ H® 6 S[1;4] = Á+ H®+ ¼ ![ref8]![ref8]![ref4]6 S[2;2] = Á+ 2H®+ ¼ 6 S[2;3] = Á+ 2H® 6 S[2;4] = Á+ 2H®+ ¼![ref7]![ref7]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.489.png)

(a)

real![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.490.png)

incoming sinusoid imaginary ...

windowed windowed windowed

FT  FT  FT 

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.491.png) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.492.png) ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.493.png)

S[0, 3] S[1, 3] S[2, 3]

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.494.png)

imaginary

real

S[0, 3]

H  

S[1, 3]

S[2, 3]

Figure 9.10: Phase in windowed Fourier analysis: (a) a complex sinusoid ana- lyzed on three successive windows; (b) the result for a single channel (k=3), for the three windows.

This gives an excellent way of estimating the frequency ®: pick any channel whose amplitude is dominated by the sinusoid and subtract two successive phase to get H®:

H®= 6 S[1;3]¡ 6 S[0;3]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.495.png)![ref3]

6 S[1;3]¡ 6 S[0;3]+ 2p¼![ref9]![ref10]

®=

H

where p is an integer. There are H possible frequencies, spaced by 2¼=H. If we are using an overlap of 4, that is, H = N=4, the frequencies are spaced by 8¼=N = 4!. Happily, this is the width of the main lobe for the Hann window, so no more than one possible value of ®can explain any measured phase di®erence within the main lobe of a peak. The correct value of p to choose is that which gives a frequency closest to the nominal frequency of the channel, k!.

When computing phases for synthesizing a new or modi¯ed signal, we want to maintain the appropriate phase relationships between successive resynthesis windows, and also, simultaneously, between adjacent channels. These two sets of relationships are not always compatible, however. We will make it our ¯rst obligation to honor the relations between successive resynthesis windows, and worry about phase relationships between channels afterward.

Suppose we want to construct the mth spectrum S[m; k] for resynthesis (having already constructed the previous one, number m ¡ 1). Suppose we wish the phase relationships between windows m ¡ 1 and m to be those of a signal x[n], but that the phases of window number m ¡ 1 might have come from somewhere else and can't be assumed to be in line with our wishes.

To ¯nd out how much the phase of each channel should di®er from the previous one, we do two analyses of the signal x[n], separated by the same hop size H that we're using for resynthesis:

T[k] = F T(W(n)X[n])(k) T0[k] = F T(W(n)X[n + H])(k)

Figure 9.11 shows the process of phase accumulation, in which the output phases each depend on the previous output phase and the phase di®erence for two windowed analyses of the input. Figure 9.12 illustrates the phase relationship in the complex plane. The phase of the new output S[m; k] should be that of the previous one plus the di®erence between the phases of the two analyses:

6 S[m; k] = 6 S[m ¡ 1;k]+ (6 T0[k]¡ 6 T[k])![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.498.png)![ref11]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.500.png)![ref11]

µ S[m ¡ 1;k]T0[k]¶

- 6![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.501.png)

T[k]

Here we used the fact that multiplying or dividing two complex numbers gives the sum or di®erence of their arguments.

If the desired magnitude is a real number a, then we should set S[m; k] to:

¯¯S[m ¡ 1;k]T0[k]¯¯¡1 S[m ¡ 1;k]T0[k] S[m; k] = a ¢ ¯¯ T[k] ¯ ¢ T[k]

¯

THIS INPUT

ANOTHER INPUT![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.502.png)

T[k] T'[k]

phase diff phase diff

phase accum phase accum S[m-1, k] S[m, k] S[m+1, k]

...

...

OUTPUT

Figure 9.11: Propagating phases in resynthesis. Each phase, such as that of S[m; k] here, depends on the previous output phase and the di®erence of the input phases.

imaginary![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.503.png)

T'[k] real

S[m-1, k] T[k]

S[m, k]

Figure 9.12: Phases of one channel of the analysis windows and two successive resynthesis windows.

The magnitudes of the second and third terms cancel out, so that the magnitude of S[m; k] reduces to a; the ¯rst two terms are real numbers so the argument is controlled by the last term.

If we want to end up with the magnitude from the spectrum T as well, we can set a = jT0[k]j and simplify:

¯¯ ¯¡ 1

¯S[m ¡ 1;k]¯¯ S[m ¡ 1;k]T0[k] S[m; k] = ¯ T[k] ¯ ¢ T[k]

9\.5.1 Phase relationships between channels

In the scheme above, the phase of each S[m; k] depends only on the previ- ous value for the same channel. The phase relationships between neighboring channels are left to chance. This sometimes works ¯ne, but sometimes the in- coherence of neighboring channels gives rise to an unintended chorus e®ect. We would ideally wish for S[m; k] and S[m; k + 1] to have the same phase rela- tionship as for T0[k] and T0[k + 1], but also for the phase relationship between S[m; k] and S[m ¡ 1;k] to be the same as between T0[k] and T[k].

These 2N equations for N phases in general will have no solution, but we can alter the equation for S[m; k] above so that whenever there happens to be a so- lution to the over-constrained system of equations, the reconstruction algorithm homes in on the solution. This approach is called phase locking [Puc95b], and has the virtue of simplicity although more sophisticated techniques are available [DL97]).


The desired output phase relation, at the frame m ¡ 1, is:

6 T[k + 1]¡ 6 T[k] = 6 S[m ¡ 1;k + 1]¡ 6 S[m ¡ 1;k] ![ref10]![ref9]![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.504.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.505.png)or, rearranging:

- ¾ ½ ¾ S[m ¡ 1;k + 1] S[m ¡ 1;k]

6 = 6![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.506.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.507.png)

T[k + 1] T[k]

In other words, the phase of the quotient S=T should not depend on k. With this in mind, we can rewrite the recursion formula for S[m; k]:

S[m; k] = jR[k]j¡1 ¢R[k]T0[k] with ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.508.png)

T[k] ¢ S[m ¡ 1;k] R[k] =

jS[m ¡ 1;k]j

and because of the previous equation, the R[k] should all be in phase. The trick is now to replace R[k] for each k with the sum of three neighboring ones. The computation is then:

S[m; k] = jR0[k]j¡ 1 ¢ R0[k]T0[k] with

R0[k] = R[k + 1]+ R[k]+ R[k ¡ 1]

If the channels are already in the correct phase relationship, this has no e®ect (the resulting phase will be the same as if only R[k] were used.) But in general the sum will share two terms in common with its neighbor at k + 1:

R0[k + 1] = R[k + 2]+ R[k + 1]+ R[k]

so that the R0 will tend to point more in the same direction than the R do. Applying this iteratively will eventually line all the R0 up to the same phase, as long as the phase relationships between the measured spectra T and T0 allow it.

6. Phase bashing

In Section 2.3 on enveloped sampling we saw how to make a periodic waveform from a recorded sound, thereby borrowing the timbre of the original sound but playing it at a speci¯ed pitch. If the window into the recorded sound is made to precess in time, the resulting timbre varies in imitation of the recorded sound.

One important problem arises, which is that if we take waveforms from di®erent windows of a sample (or from di®erent samples), there is no guarantee that the phases of the two match up. If they don't the result can be ugly, since the random phase changes are heard as frequency °uctuations. This can be corrected using Fourier analysis and resynthesis [Puc05].

6. PHASE BASHING 285

INPUT![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.509.png)



<table><tr><th colspan="1" rowspan="2"></th><th colspan="1" rowspan="2"></th><th colspan="1"></th></tr>
<tr><td colspan="2" valign="top"></td><td colspan="1"></td></tr>
</table>
...![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.510.png)

FT MAGNITUDE

(-1)k  

iFT

...

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.511.png)

PHASE-BASHED INPUT

Figure 9.13: Phase-bashing a recorded sound (here, a sinusoid with rising fre- quency) to give a series of oscillator wavetables.

(a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.512.png)

osc~ (c)

fft~ block~ 512![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.513.png)

tabwrite~ $0-imaginary inlet~

tabwrite~ $0-real tabreceive~ $0-hann

\*~ 

rfft~

(b)

0  <- frequency, \*~  \*~ 
* 10 tens of Hz. +~ 

osc~ click here and sqrt~

pd fft-analysis <- see tabwrite~ $0-magnitude

Figure 9.14: Fourier analysis in Pd: (a) the ®t » object; (b) using a subwindow to control block size of the Fourier transform; (c) the subwindow, using a real Fourier transform (the fft~object) and the Hann windowing function.

Figure 9.13 shows a simple way to use Fourier analysis to align phases in a series of windows in a recording. We simply take the FFT of the window and then set each phase to zero for even values of k and ¼for odd ones. The phase at the center of the window is thus zero for both even and odd values of k. To set the phases (the arguments of the complex amplitudes in the spectrum) in the desired way, ¯rst we ¯nd the magnitude, which can be considered a complex number with argument zero. Then multiplying by (¡1)k adjusts the amplitude so that it is positive and negative in alternation. Then we take the inverse Fourier transform, without even bothering to window again on the way back; we will probably want to apply a windowing envelope later anyway as was shown in Figure 2.7. The results can be combined with the modulation techniques of Chapter 6 to yield powerful tools for vocal and other imitative synthesis.

7. Examples

Fourier analysis and resynthesis in Pd

Example I01.Fourier.analysis.pd (Figure 9.14, part a) demonstrates computing the Fourier transform of an audio signal using the fft~ object:

fft~ : Fast Fourier transform. The two inlets take audio signals representing the![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.514.png) real and imaginary parts of a complex-valued signal. The window size N is given by Pd's block size. One Fourier transform is done on each block.

7. EXAMPLES 287

The Fast Fourier transform [SI03] reduces the computational cost of Fourier analysis in Pd to only that of between 5 and 15 osc~ objects in typical con¯gu- rations. The FFT algorithm in its simplest form takes N to be a power of two, which is also (normally) a constraint on block sizes in Pd.

Example I02.Hann.window.pd (Figure 9.14, parts b and c) shows how to control the block size using a block~ object, how to apply a Hann window, and a di®erent version of the Fourier transform. Part (b) shows the invocation of a subwindow which in turn is shown in part (c). New objects are:

rfft~ : real Fast Fourier transform. The imaginary part of the input is as- sumed![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.515.png) to be zero. Only the ¯rst N=2 + 1 channels of output are ¯lled in (the others are determined by symmetry). This takes half the computation time of the (more general) fft~object.

tabreceive~ : repeatedly outputs the contents of a wavetable. Each block of computation![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.516.png) outputs the same ¯rst N samples of the table.

In this example, the table \$0-hann" holds a Hann window function of length 512, in agreement with the speci¯ed block size. The signal to be analyzed appears (from the parent patch) via the inlet~ object. The channel amplitudes (the output of the rfft~ object) are reduced to real-valued magnitudes: the real and imaginary parts are squared separately, the two squares are added, and the result passed to the sqrt~ object. Finally the magnitude is written (controlled by a connection not shown in the ¯gure) via tabwrite~ to another table, \$0- magnitude", for graphing.

Example I03.resynthesis.pd (Figure 9.15) shows how to analyze and resyn- thesize an audio signal following the strategy of Figure 9.7. As before there is a sub-window to do the work at a block size appropriate to the task; the ¯gure shows only the sub-window. We need one new object for the inverse Fourier transform:

rifft~ : real inverse Fast Fourier transform. Using the ¯rst N=2 + 1 points ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.517.png)of its inputs (taken to be a real/imaginary pair), and assuming the appropriate values for the other channels by symmetry, reconstructs a real-valued output. No normalization is done, so that a rfft~/rifft~ pair together result in a gain of N. The ifft~ object is also available which computes an unnormalized inverse for the fft~ object, reconstructing a complex-valued output.

The block~ object, in the subwindow, is invoked with a second argument which speci¯es an overlap factor of 4. This dictates that the sub-window will run four times every N = 512 samples, at regular intervals of 128 samples. The inlet~ object does the necessary bu®ering and rearranging of samples so that its output always gives the 512 latest samples of input in order. In the other direction, the outlet~ object adds segments of its previous four inputs to carry out the overlap-add scheme shown in Figure 9.7.

The 512-sample blocks are multiplied by the Hann window both at the input and the output. If the rfft~ and rifft~ objects were connected without any modi¯cations in between, the output would faithfully reconstruct the input.

A modi¯cation is applied, however: each channel is multiplied by a (positive

block~ 512 4 512-sample block, 4-fold overlap (hop size 128).![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.518.png)

inlet~ now takes care of buffering and shifting for inlet~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.519.png) overlapped windowing.

\*~  tabreceive~ $0-hann Hann window as before

rfft~ real FT as before

tabreceive~ $0-gain read "gain" from a table in parent patch \*~  raise to 4th power (a more convenient scale)

\*~ 

/~ 768 renormalize: divide by window size 512 and an additional

factor of 3/2 to correct for twice-Hann-windowed

\*~  \*~  overlap-add in outlet~ below.

rifft~ real inverse fast Fourier transform (not normalized).

\*~  tabreceive~ $0-hann Hann window again on output.

outlet~ outlet~ does overlap-adding because of block~ setting above.

Figure 9.15: Fourier analysis and resynthesis, using block~ to specify an overlap of 4, and rifft~ to reconstruct the signal after modi¯cation.


9\.7. EXAMPLES

rfft~ real FT (a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.520.png)

\*~ \*~ compute power +~  (call it "s")

pd calculate-mask

subpatch shown in (b)

mask table tabreceive~ $0-mask

\*~ r mask-level -~  power ("s") minus

mask ("m")

max~ 0 force >= 0

+~ 1e-20 protect against division by zero

/~ 

sqrt((s-m)/s) q8\_sqrt~ (or 0 if s < m)

/~ 1536

\*~  \*~  normalize by 2/(3N) rifft~ real iFT

289

(b)

loop to number r make-mask![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.521.png)

of frames t b f r window-msec bang~

0  

spigot

hop size float + 1 /   / 4 in msec

- 0  number of

t f f frames

sel 0

expr 1/($f1+1) 0  

current 0   weight to average power new power into mask

inlet~

tabreceive~ $0-mask

-~  average current power into last mask to get new mask.

New value is weighted 1/n +~  \*~  on the nth iteration.

tabsend~ $0-mask


Figure 9.16: Noise suppression as an example of narrow-band companding: (a) analysis and reconstruction of the signal; (b) computation of the \mask".

real-valued) gain. The complex-valued amplitude for each channel is scaled by separately multiplying the real and imaginary parts by the gain. The gain (which depends on the channel) comes from another table, named \$0-gain". The result is a graphical equalization ¯lter; by mousing in the graphical window for this table, you can design gain-frequency curves.

There is an inherent delay introduced by using block~ to increase the block size (but none if it is used, as shown in Chapter 7, to reduce block size relative to the parent window.) The delay can be measured from the inlet to the outlet of the sub-patch, and is equal to the di®erence of the two block sizes. In this example the bu®ering delay is 512-64=448 samples. Blocking delay does not depend on overlap, only on block sizes.

7. EXAMPLES 300

Narrow-band companding: noise suppression

Example I04.noisegate.pd (Figure 9.16) shows an example of narrow-band com- panding using Fourier analysis/resynthesis. (This is a realization of the block diagram of Figure 9.8.) Part (a) of the ¯gure shows a ¯lter con¯guration similar to the previous example, except that the gain for each channel is now a function of the channel magnitude.

For each k, if we let s[k] denote the power in channel k, and let m[k] be a mask level (a level presumably somewhat higher than the noise power for channel k), then the gain in channel k is given by

( q ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.522.png)

s[k]¡m[k] s[k] > m[k]

s[k]

0 otherwise

The power in the kth channel is thus reduced by m[k] if possible, and otherwise replaced by zero.

The mask itself is the product of the measured average noise in each channel, which is contained in the table \$0-mask", multiplied by a value named \mask- level". The average noise is measured in a subpatch (pd calculate-mask), whose contents are shown in part (b) of the ¯gure. To compute the mask we are using two new new objects:

bang~ : send a bang in advance of each block of computation. The bang appears![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.523.png) at the logical time of the ¯rst sample in each block (the earliest logical

time whose control computation a®ects that block and not the previous one), following the scheme shown in Figure 3.2.

tabsend~ : the companion object for tabreceive~, repeatedly copies its input![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.524.png)

to the contents of a table, a®ecting up to the ¯rst N samples of the table.

The power averaging process is begun by sending a time duration in millisec- onds to \make-mask". The patch computes the equivalent number of blocks b and generates a sequence of weights: 1;1=2;1=3;:::;1=b, by which each of the b following blocks' power is averaged into whatever the mask table held at the previous block. At the end of b blocks the table holds the equally-weighted average of all b power measurements. Thereafter, the weight for averaging new power measurements is zero, so the measured average stops evolving.

To use this patch for classical noise suppression requires at least a fewseconds of recorded noise without the \signal" present. This is played into the patch, and its duration sent to \make-mask", so that the \$0-mask" table holds the average measured noise power for each channel. Then, making the assumption that the noisy part of the signal rarely exceeds 10 times its average power (for example), \mask-level" is set to 10, and the signal to be noise-suppressed is sent through part (a) of the patch. The noise will be almost all gone, but those channels in which the signal exceeds 20 times the noise power will only be attenuated by 3dB, and higher-power channels progressively less. (Of course, actual noise suppression might not be the most interesting application of the patch; one could try masking any signal from any other one.)

inlet~ filter input \*~  tabreceive~ $0-hann rfft~![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.525.png)

\*~  \*~  reciprocal

+~  modulus of inlet~ control source +~ 1e-20 filter input \*~  tabreceive~ $0-hann

amplitude

q8\_rsqrt~

rfft~

r squelch

\*~  \*~ 

expr 0.01\*$f1\*$f1 modulus

limit gain to +~ 

of control clip~ squelch\*squelch/100 q8\_sqrt~ amplitude

\*~  multiply the two amplitude

factors (for compression

and to apply new timbre)

/~ 1536

\*~  \*~ 

rifft~

\*~  tabreceive~ $0-hann outlet~

Figure 9.17: Timbre stamp.

Timbre stamp (\vocoder")

Example I05.compressor.pd (Figure 9.17) is another channel compander which is presented in preparation for Example I06.timbre.stamp.pd, which we will examine next. This is a realization of the timbre stamp of Figure 9.9, slightly modi¯ed.

There are two inputs, one at left to be ¯ltered (and whose Fourier transform is used for resynthesis after modifying the magnitudes), and one at right which acts as a control source. Roughly speaking, if the two magnitudes are f [k] for the ¯lter input and c[k] for the control source, we just \whiten" the ¯lter input, multiplying by 1=f[k], and then stamp the control magnitudes onto the result by further multiplying by c[k]. In practice, we must limit the gain to some reasonable maximum value. In this patch this is done by limiting the whitening factor 1=f[k] to a speci¯ed maximum value using the clip~ object. The limit

is controlled by the \squelch" parameter, which is squared and divided by 100 to map values from 0 to 100 to a useful range.

Another possible scheme is to limit the gain after forming the quotient c[k]=f[k]. The gain limitation may in either case be frequency dependent. It is also sometimes useful to raise the gain to a power p between 0 and 1; if 1, this is a timbre stamp and if 0, it passes the ¯lter input through unchanged, and values in between give a smooth interpolation between the two.

Phase vocoder time bender

The phase vocoder usually refers to the general technique of passing from (complex-valued) channel amplitudes to pairs consisting of (real-valued) magni- tudes and phase precession rates (\frequencies"), and back, as described in Fig- ure 9.11 (Section 9.5). In Example I07.phase.vocoder.pd (Figure 9.18), we use this technique with the speci¯c aim of time-stretching and/or time-contracting

a recorded sound under real-time control. That is, we control, at any moment in real time, the location in the recorded sound we hear. Two new objects are used:

lrshift~ : shift a block left or right (according to its creation argument). If![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.526.png) the argument is positive, each block of the output is the input shifted that number of spaces to the right, ¯lling zeros in as needed on the left. A negative argument shifts to the left, ¯lling zeros in at the right.

q8~~ rsqrt~ : quick and approximate reciprocal square root. Outputs the recip- ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.527.png)rocal of the square root of its input, good to about a part in 256, using much less computation than a full-precision square root and reciprocal would.

The process starts with a sub-patch, pd read-windows, that outputs two Hann-windowed blocks of the recorded sound, a \back" one and a \front" one 1/4 window further forward in the recording. The window shown uses the two outputs of the sub-patch to guide the amplitude and phase change of each channel of its own output.

The top two tabreceive~ objects recall the previous block of complex am- plitudes sent to the rifft~ object at bottom, corresponding to S[m ¡ 1;k] in the discussion of Section 9.5. The patch as a whole computes S[m; k] and then its Hann windowed inverse FT for output.

After normalizing S[m¡1;k], its complex conjugate (the normalized inverse) is multiplied by the windowed Fourier transform of the \back" window T[k], giving the product R[k] of Page 283. Next, depending on the value of the parameter \lock", the computed value of R[k] is conditionally replaced with the phase-locking version R0[k]. This is done using lrshift~ objects, whose outputs are added into R[k] if \lock" is set to one, or otherwise not if it is zero. The result is then normalized and multiplied by the Hann-windowed Fourier transform of the \front" window (T0[k]) to give S[m; k].

Three other applications of Fourier analysis/resynthesis, not pictured here, are provided in the Pd examples. First, Example I08.pvoc.reverb.pd shows how to make a phase vocoder whose output recirculates as in a reverberator, except

tabreceive~ prev-real recall previous output amplitude whose phase we©ll add to measured![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.528.png)

tabreceive~ prev-imag phase precession

\*~ \*~  normalize (divide by the magnitude).

The 1e-20 is to prevent overflows.

+~  +~ 1e-20

\*~  \*~  q8\_rsqrt~ Read two windows, one 1/4 length behind the other, of the input

pd read-windows sound, with Hann window function rfft~ Take FT of the window in back.

Multiply its conjugate by the

\*~  \*~  \*~  \*~  normalized previous output. Result

has the magnitude of the input sound.

+~  -~ 

lrshift~ 1 lrshift~ 1 If "lock" is on, add two neighboring complex amplitudes. The result will

lrshift~ -1 lrshift~ -1 tend toward the channel with the

strongest amplitude.

r lock

\*~ 

\*~ 

+~ 

+~ 

+~ 1e-15 Normalize again, taking care to salt

` `each channel with 1e-15 so that we get a unit \*~  \*~  complex number even if everything was zero.

Now take FT of the forward window

+~ 

and multiply it by the unit complex \*~  \*~  q8\_rsqrt~ number from above. Magnitude will

rfft~ be that of the forward window and phase will be previous output phase

\*~  \*~  \*~  \*~  plus the phase difference between the

two analysis windows, except that if -~  +~  "lock" is on, they will be changed to 

agree better with the inter-channel phase relationships of the input.

tabsend~ prev-imag

rifft~

tabsend~ prev-real r window-size \*~ tabreceive~ $0-hann![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.529.png)

\*~  r window-size set $1 4

'set' message to block

outlet~ expr 2/(3\*$f1) allows variable size block~

Figure 9.18: Phase vocoder for time stretching and contraction.

301 CHAPTER 9. FOURIER ANALYSIS AND RESYNTHESIS

that individual channels are replaced by the input when it is more powerful than what is already recirculating. The result is a more coherent-sounding reverberation e®ect than can be made in the classical way using delay lines.

Example I09.sheep.from.goats.pd demonstrates the (imperfect) technique of separating pitched signals from noisy ones, channel by channel, based on the phase coherence we should expect from a Hann-windowed sinusoid. If three adjacent channels are approximately ¼ radians out of phase from each other, they are judged to belong to a sinusoidal peak. Channels belonging to sinusoidal peaks are replaced with zero to extract the noisy portion of the signal, or all others are replaced with zero to give the sinusoidal portion.

Example I10.phase.bash.pd returns to the wavetable looping sampler of Fig- ure 2.7, and shows how to align the phases of the sample so that all components of the signal have zero phase at points 0, N, 2N, and so on. In this way, two copies of a looping sampler placed N samples apart can be coherently cross- faded. A synthetic, pitched version of the original sound¯le can be made using daisy-chained cross-fades.

Exercises

1. A signal x[n] is 1 for n = 0 and 0 otherwise (an impulse). What is its (N-point) Fourier transform as a function of k?
1. Assuming further that N is an even number, what does the Fourier trans- form become if x[n] is 1 at n = N=2 instead of at n = 0?
1. For what integer values of k is the Fourier transform of the N-point Hann window function nonzero?
1. In order to Fourier analyze a 100-Hertz periodic tone (at a sample rate of 44100 Hertz), using a Hann window, what value of N would be needed to completely resolve all the partials of the tone (in the sense of having non-overlapping peaks in the spectrum)?
1. Suppose an N-point Fourier transform is done on a complex sinusoid of frequency 2:5! where ! = 2¼=N is the fundamental frequency. What percentage of the signal energy lands in the main lobe, channels k = 2 and k = 3? If the signal is Hann windowed, what percentage of the energy is now in the main lobe (which is then channels 1 through 4)?


Chapter 10

Classical waveforms

Up until now we have primarily taken three approaches to synthesizing repetitive waveforms: additive synthesis (Chapter 1), wavetable synthesis (Chapter 2), and waveshaping (Chapters 5 and 6). This chapter introduces a fourth approach, in which waveforms are built up explicitly from line segments with controllable endpoints. This approach is historically at least as important as the others, and was dominant during the analog synthesizer period, approximately 1965-1985. For lack of a better name, we'll use the term classical waveforms to denote waveforms composed of line segments.

They include the sawtooth, triangle, and rectangle waves pictured in Figure 10.1, among many other possibilities. The salient features of classical waveforms are either discontinuous jumps (changes in value) or corners (changes in slope). In the ¯gure, the sawtooth and rectangle waves have jumps (once per cycle for the sawtooth, and twice for the rectangle), and constant slope elsewhere (negative for the sawtooth wave, zero for the rectangle wave). The triangle wave has no discontinuous jumps, but the slope changes discontinuously twice per cycle.

To use classical waveforms e®ectively, it is useful to understand how the shape of the waveform is re°ected in its Fourier series. (To compute these we need background from Chapter 9, which is why this chapter appears here and not earlier.) We will also need strategies for digitally synthesizing classical waveforms. These waveforms prove to be much more susceptible to foldover problems than any we have treated before, so we will have to pay especially close attention to its control.

In general, our strategy for predicting and controlling foldover will be to consider ¯rst those sampled waveforms whose period is an integer N. Then if we want to obtain a waveform of a non-integral period (call it ¿, say) we approximate ¿ as a quotient N=R of two integers. Conceptually at least, we can then synthesize the desired waveform with period N, and then take only one of each R samples of output. This last, down-sampling step is where the foldover is produced, and careful handling will help us control it.

295

1. SYMMETRIES AND FOURIER SERIES 306

(a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.530.png)

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.531.png)

(c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.532.png)

Figure 10.1: Classical waveforms: (a) the sawtooth, (b) the triangle, and (c) the rectangle wave, shown as functions of a continuous variable (not sampled).

1. Symmetries and Fourier series

Before making a quantitative analysis of the Fourier series of the classical wave- forms, we pause to make two useful observations about symmetries in waveforms and the corresponding symmetries in the Fourier series. First, a Fourier series might consist only of even or odd-numbered harmonics; this is re°ected in sym- metries comparing a waveform to its displacement by half a cycle. Second, the Fourier series may contain only real-valued or pure imaginary-valued coe±cients (corresponding to the cosine or sine functions). This is re°ected in symmetries comparing the waveform to its reversal in time.

In this section we will assume that our waveform has an integer period N, and furthermore, for simplicity, that N is even (if it isn't we can just up-sample by a factor of two). We know from Chapter 9 that any (real or complex valued) waveform X[n]can be written as a Fourier series (whose coe±cients we'll denote by A[k]):

X[n] = A[0]+ A[1]Un + ¢¢¢+ A[N ¡ 1]U(N ¡1)n

or, equivalently,

X[n] = A[0]+ A[1](cos(!n) + i sin(!n)) + ¢¢¢

+A[N ¡ 1](cos(!(N ¡ 1)n) + i sin(!(N ¡ 1)n)) where ! = 2¼=N is the fundamental frequency of the waveform, and

U = cos(!) + i sin(!)

is the unit-magnitude complex number whose argument is !.

To analyze the ¯rst symmetry we delay the signal X[n]by a half-cycle. Since UN=2 = ¡1 we get:

X[n + N=2] = A[0]¡ A[1]Un + A[2]U2n § ¢¢¢

+A[N ¡ 2]U(N ¡2)n ¡ A[N ¡ 1]U(N ¡1)n

In e®ect, a half-cycle delay changes the sign of every other term in the Fourier series. We combine this with the original series in two di®erent ways. Letting X 0 denote half the sum of the two:

0 X[n]+ X[n + N=2] 2n (N ¡2)n X [n] =~~ = A[0]+ A[2]U + ¢¢¢+ A[N ¡ 2]U

2

and X 00half the di®erence:

X 00[n] = X[n]¡ X[n + N=2] = A[1]Un + A[3]U3n + ¢¢¢+ A[N ¡ 1]U(N ¡1)n

2

we see that X 0 consists only of even-numbered harmonics (including DC) and X 00only of odd ones.

Furthermore, if X happens to be equal to itself shifted a half cycle, that is, if X[n] = X[n + N=2], then (looking at the de¯nitions of X 0 and X 00) we get

X 0[n] = X[n] and X 00[n] = 0. This implies that, in this case, X[n] has only even numbered harmonics. Indeed, this should be no surprise, since in this case X[n] would have to repeat every N=2 samples, so its fundamental frequency is twice as high as normal for period N.

In the same way, if X[n] = ¡X[n + N=2], then X can have only odd- numbered harmonics. This allows us easily to split any desired waveform into its even- and odd-numbered harmonics. (This is equivalent to using a comb ¯lter to extract even or odd harmonics; see Chapter 7.)

To derive the second symmetry relation we compare X[n] with its time reversal, X[¡n] (or, equivalently, since X repeats every N samples, with X[N ¡ n]). The Fourier series becomes:

X[¡n] = A[0]+ A[1](cos(!n) ¡ i sin(!n)) + ¢¢¢ +A[N ¡ 1](cos(!(N ¡ 1)n) ¡ i sin(!(N ¡ 1)n))

(since the cosine function is even and the sine function is odd). In the same way as before we can extract the cosines by forming X 0[n] as half the sum:

X 0[n] = X[n]+ X[¡n] = A[0]+ A[1]cos(!n) + ¢¢¢+ A[N ¡ 1]cos(!(N ¡ 1)n)

2

and X 00[n] as half the di®erence divided by i:

X 00[n] = X[n]¡ X[¡n] = A[1]sin(!n) + ¢¢¢+ A[N ¡ 1]sin(!(N ¡ 1)n)

2i

So if X[n] satis¯es X[¡n] = X[n] the Fourier series consists of cosine terms only; if X[¡n] = ¡X[n] it consists of sine terms only; and as before we can decompose any X[n] (that repeats every N samples) as a sum of the two.

10\.1.1 Sawtooth waves and symmetry

As an example, we apply the shift symmetry (even and odd harmonics) to a sawtooth wave. Figure 10.2 (part a) shows the original sawtooth wave and part (b) shows the result of shifting by a half cycle. The sum of the two (part c) drops discontinuously whenever either one of the two copies does so, and traces a line segment whenever both component sawtooth waves do; so it in turn becomes a sawtooth wave, of half the original period (twice the fundamental frequency). Subtracting the two sawtooth waves (part d) gives a waveform with slope zero except at the discontinuities. The discontinuities coming from the original sawtooth wave jump in the same direction (negative to positive), but those coming from the shifted one are negated and jump from positive to negative. The result is a square wave, a particular rectangle wave in which the two component segments have the same duration.

This symmetry was used to great e®ect in the design of Buchla analog synthesizers; instead of o®ering a single sawtooth generator, Buchla designed an oscillator that outputs the even and odd harmonic portions separately, so that cross-fading between the two allows a continuous control over the relative strengths of the even and odd harmonics in the analog waveform.

(a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.533.png)

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.534.png)

(c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.535.png)

(d)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.536.png)

Figure 10.2: Using a symmetry relation to extract even and odd harmonics from a sawtooth wave: (a) the original sawtooth wave; (b) shifted by 1/2 cycle; (c) their sum (another sawtooth wave at twice the frequency); (d) their di®erence (a square wave).


(a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.537.png)

L   L  

1   2   N  

(b) (c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.538.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.539.png)

Figure 10.3: Dissecting a waveform: (a) the original waveform with two discon- tinuities; (b and c) the two component sawtooth waves.

2. Dissecting classical waveforms

Among the several conclusions we can draw from the even/odd harmonic de- composition of the sawtooth wave (Figure 10.2), one is that a square wave can be decomposed into a linear combination of two sawtooth waves. We can carry this idea further, and show how to compose any classical waveform having only jumps (discontinuities in value) but no corners (discontinuities in slope) as a sum of sawtooth waves of various phases and amplitudes. We then develop the idea further, showing how to generate waveforms with corners (either in addi- tion to, or instead of, jumps) using another elementary waveform we'll call the parabolic wave.

Suppose ¯rst that a waveform of period N has discontinuities at j di®erent points, L1;:::;Lj , all lying on the cycle between 0 and N, at which the waveform jumps by values d1;:::;dj . A negative value of d1, for instance, would mean that the waveform jumps from a higher to a lower value at the point L1, and a positive value of d1 would mean a jump from a lower to a higher value.

For instance, Figure 10.3 (part a) shows a classical waveform with two jumps: (L1;d1) = (0:3N;¡0:3) and (L2;d2) = (0:6N;1:3). Parts (b) and (c) show sawtooth waves, each with one of the two jumps. The sum of the two sawtooth waves reconstructs the waveform of part (a), except for a possible constant (DC) o®set.

10\.2. DISSECTING CLASSICAL WAVEFORMS 301

1/12![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.540.png)

N  (N/2, -1/24)

Figure 10.4: The parabolic wave.

The sawtooth wave with a jump of one unit at the point zero is given by s[n] = n=N ¡ 1=2

over the period 0 · n · N ¡ 1, and repeats for other values of n. A sawtooth wave with a jump (L; d) is given by s0[n] = ds[n ¡ L]. The sum of all the

component sawtooth waves is:

x[n] = d1s[n ¡ L1]+ ¢¢¢+ dj s[n ¡ Lj ]

The slopes of the segments of the waveform of part (a) of the ¯gure are all the same, equal to the sum of the slopes of the component sawtooth waves:

- d1 + ¢¢¢+ dj N

Square and rectangle waves have horizontal line segments (slope zero); for this to happen in general the jumps must add to zero: d1 + ¢¢¢+ dj = 0.

To decompose classical waveforms with corners we use the parabolic wave, which, over a single period from 0 to N, is equal to

1 n 1 2 1 p[n] = ( ¡ ) ¡

2 N 2 24

as shown in Figure 10.4. It is a second-degree (quadratic) polynomial in the variable n, arranged so that it reaches a maximum halfway through the cycle at n = N=2, the DC component is zero (or in other words, the average value over one cycle of the waveform is zero), and so that the slope changes discontinuously by ¡1=N at the beginning of the cycle.

To construct a waveform with any desired number of corners (suppose they are at the points Mi;:::;Ml, with slope changes equal to c1;:::;cl), we sum up the necessary parabolic waves:

x[n] = ¡Nc1p[n ¡ M1]¡ ¢¢¢¡ Nclp[n ¡ Ml]

An example is shown graphically in Figure 10.5.

If the sum x[n] is to contain line segments (not segments of curves), the n2 terms in the sum must sum to zero. From the expansion of x[n] above, this implies that c1 + ¢¢¢+ cl = 0. Sums obtained from existing classical waveforms (as in the ¯gure) will always satisfy this condition because the changes in slope, over a cycle, must all add to zero for the waveform to connect with itself.

3. FOURIER SERIES OF THE ELEMENTARY WAVEFORMS 312

(a) (b) (c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.541.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.542.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.543.png)

Figure 10.5: Decomposing a triangle wave (part a) into two parabolic waves (b and c).

3. Fourier series of the elementary waveforms

In general, given a repeating waveform X[n], we can evaluate its Fourier series coe±cients A[k] by directly evaluating the Fourier transform:

1

A[k] = F TfX[n]g(k)

N

1 h i

- X[0]+ U¡kX[1]+ ¢¢¢+ U¡(N ¡1)kX[N ¡ 1]

N

but doing this directly for sawtooth and parabolic waves will require pages of algebra (somewhat less if we were willing resort to di®erential calculus). Instead, we rely on properties of the Fourier transform to relate the transform of a signal x[n] with its ¯rst di®erence, de¯ned as x[n]¡ x[n ¡ 1]. The ¯rst di®erence of the parabolic wave will turn out to be a sawtooth, and that of a sawtooth will be simple enough to evaluate directly, and thus we'll get the desired Fourier series.

In general, to evaluate the strength of the kth harmonic, we'll make the assumption that N is much larger than k, or equivalently, that k=N is negligible.

We start from the Time Shift Formula for Fourier Transforms (Page 267) setting the time shift to one sample:

F Tfx[n ¡ 1]g = [cos(k!) ¡ i sin(k!)]F Tfx[n]g

- (1 ¡ i!k)F T fx[n]g

Here we're using the assumption that, because N is much larger than k, k! = 2¼k=N is much smaller than unity and we can make approximations:

cos(k!) ¼ 1 ; sin(k!) ¼ k!

which are good to within a small error, on the order of (k=N)2. Now we plug this result in to evaluate:

F Tfx[n]¡ x[n ¡ 1]g ¼ i!kF T fx[n]g

1. Sawtooth wave

First we apply this to the sawtooth wave s[n]. For 0 · n < N we have:

½

1  1 n = 0

s[n]¡ s[n ¡ 1] = ¡ N + 0 otherwise

Ignoring the constant o®setof¡ 1 , this gives an impulse, zero everywhere except

N

one sample per cycle. The summation in the Fourier transform only has one term, and we get:

F Tfs[n]¡ s[n ¡ 1]g(k) = 1; k 6= 0; ¡N < k < N We then apply the di®erence formula backward to get:

1 ¡iN

F Tfs[n]g(k) ¼ =

i!k 2¼k

valid for integer values of k, small compared to N, but with k 6= 0 . (To get the second form of the expression we plugged in ! = 2¼=N and 1=i = ¡i.)

This analysis doesn't give us the DC component F Tfs[n]g(0), because we would have had to divide by k = 0. Instead, we can evaluate the DC term directly as the sum of all the points of the waveform: it's approximately zero by symmetry.

To get a Fourier series in terms of familiar real-valued sine and cosine func- tions, we combine corresponding terms for negative and positive values of k. The ¯rst harmonic (k = §1) is:

1 £F Tfs[n]g(1) ¢Un + F Tfs[n]g(¡1) ¢U¡n¤ N

- ¤
- ¡i Un ¡ U¡n

  2¼

  sin(!n) =

¼

and similarly the kth harmonic is

sin(k!n)

k¼

so the entire Fourier series is:

- ¸

1 sin(2!n) sin(3!n)

s[n] ¼ sin(!n) +~~ +~~ + ¢¢¢

- 2 3

(0,1)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.544.png)

N  

(N/2, -1)

Figure 10.6: Symmetric triangle wave, obtained by superposing parabolic waves with (M;c) pairs equal to (0;8) and (N=2;¡8).

2. Parabolic wave

The same analysis, with some di®erences in sign and normalization, works for parabolic waves. First we compute the di®erence:

( n ¡ 1 )2 ¡ ( n¡1 ¡ 1 )2 p[n]¡ p[n ¡ 1] = N 2 N 2

2

- ( Nn ¡ 2NN )2 ¡ ( Nn ¡ N2¡N2 )2

2

2n ¡ 1 + 1

- N 2 N N 2 2
- ¡s[n]=N:

So (again for k 6= 0, small compared to N) we get:

¡1 ¡iN

F Tfp[n]g(k) ¼ ¢ ¢F Tfs[n]g(k)

N 2¼k

¡1 ¡iN ¡iN

- ¢ ¢

  N 2¼k 2¼k

N

\=

4¼2k2

and as before we get the Fourier series:

- ¸

1 cos(2!n) cos(3!n)

p[n] ¼ cos(!n) +~~ +~~ + ¢¢¢

2¼2 4 9

3. Square and symmetric triangle waves

To see how to obtain Fourier series for classical waveforms in general, consider ¯rst the square wave,

N

x[n] = s[n]¡ s[n ¡ ]

2

(M, 1)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.545.png)

(N-M, -1)

Figure 10.7: Non-symmetric triangle wave, with vertices at (M;1) and (N ¡ M;¡1).

equal to 1=2 for the ¯rst half cycle (0 <= n < N=2) and ¡1=2 for the rest. We get the Fourier series by plugging in the Fourier series for s[n] twice:

·

1 sin(2!n) sin(3!n)

x[n] ¼ sin(!n) +~~ +~~ + ¢¢¢

- 2 3

¸ sin(2!n) sin(3!n)

¡sin(!n) + ¡ § ¢¢¢

2 3

- ¸

2 sin(3!n) sin(5!n)

- sin(!n) +~~ +~~ + ¢¢¢
- 3 5

The symmetric triangle wave (Figure 10.6) given by

N

x[n] = 8p[n]¡ 8p[n ¡ ]

2

similarly comes to

- ¸

8 cos(3!n) cos(5!n)

x[n] ¼ cos(!n) +~~ +~~ + ¢¢¢

¼2 9 25

4. General (non-symmetric) triangle wave

A general, non-symmetric triangle wave appears in Figure 10.7. Here we have arranged the cycle so that, ¯rst, the DC component is zero (so that the two corners have equal and opposite heights), and second, so that the midpoint of the shorter segment goes through the point (0;0).

The two line segments have slopes equal to 1=M and ¡2=(N ¡ 2M), so the decomposition into component parabolic waves is given by:

N 2

x[n] =~~ (p[n ¡ M]¡ p[n + M])

MN ¡ 2M 2

(here we're using the periodicity of p[n] to replace p[n¡ (N ¡ M)] by p[n+ M]).)

4. PREDICTING AND CONTROLLING FOLDOVER 318

The most general way of dealing with linear combinations of elementary (parabolic and/or sawtooth) waves is to go back to the complex Fourier series, as we did in ¯nding the series for the elementary waves themselves. But in this particular case we can use a trigonometric identity to avoid the extra work of converting back and forth. First we plug in the real-valued Fourier series:

·

N 2

x[n] =~~ cos(!(n ¡ M)) ¡ cos(!(n + M))

2¼2(MN ¡ 2M 2)

¸ cos(2!(n ¡ M)) ¡ cos(2!(n + M))

+ + ¢¢¢ 4

Now we use the identity,

b¡ a a + b

cos(a) ¡ cos(b) = 2sin(~~ ) sin(~~ )

2 2

so that, for example,

cos(!(n ¡ M)) ¡ cos(!(n + M)) = 2sin(2¼M=N) sin(!n)

(Here again we used the de¯nition of ! = 2¼=N.) This is a simpli¯cation since the ¯rst sine term does not depend on n; it's just an amplitude term. Applying the identity to all the terms of the expansion for x[n] gives:

x[n] = a[1]sin(!n) + a[2]sin(2!n) + ¢¢¢ where the amplitudes of the components are given by:

1 sin(2¼kM=N ) a[k] = ¼2(M=N ¡ 2(M=N)2) ¢ k2

Notice that the result does not depend separately on the values of M and N, but only on their ratio, M=N (this is not surprising because the shape of the waveform depends on this ratio). If we look at small values of k:

1

k <

4M=N

the argument of the sine function is less than ¼=2 and using the approximation sin(µ) ¼ µ we ¯nd that a[k] drops o®as 1=k, just as the partials of a sawtooth wave. But for larger values of k the sine term oscillates between 1 and -1, so that the amplitudes drop o®irregularly as 1=k2.

Figure 10.8 shows the partial strengths with M=N set to 0.03; here, our prediction is that the 1=k dependence should extend to k ¼ 1=(4 ¢0:03) ¼ 8:5, in rough agreement with the ¯gure.

Another way to see why the partials should behave as 1=k for low values of k and 1=k2 thereafter, is to compare the period of a given partial with the length

of the short segment, 2M. For partials numbering less than N=4M, the period

is at least twice the length of the short segment, and at that scale the waveform is nearly indistinguishable from a sawtooth wave. For partials numbering in excess of N=2M, the two corners of the triangle wave are at least one period apart, and at these higher frequencies the two corners (each with 1=k2 frequency dependence) are resolved from each other. In the ¯gure, the notch at partial 17 occurs at the wavelength N=2M ¼ 1=17, at which wavelength the two corners are one cycle apart; since the corners are opposite in sign they cancel each other.

4. Predicting and controlling foldover

Now we descend to the real situation, in which the period ofthe waveform cannot be assumed to be arbitrarily long and integer-valued. Suppose (for de¯niteness) we want to synthesize tones at 440 Hertz (A above middle C), and that we are using a sample rate of 44100 Hertz, so that the period is about 100.25 samples. Theoretically, given a very high sample rate, we would expect the ¯ftieth partial to have magnitude 1=50 compared to the fundamental and a frequency about 20 kHz. If we sample this waveform at the (lower) sample rate of 44100, then partials in excess of this frequency will be aliased, as described in Section 3.1. The relative strength of the folded-over partials will be on the order of -32 decibels|quite audible. If the fundamental frequency is raised further, more and louder partials reach the Nyquist frequency (half the sample rate) and begin to fold over.

Foldover problems are much less pronounced for waveforms with only corners (instead of jumps) because of the faster dropo®of higher partial frequencies; for instance, a symmetric triangle wave at 440 Hertz would get twice the dropo®, or -64 decibels. In general, though, waveforms with discontinuities are a better starting point for subtractive synthesis (the most popular classical technique). In case you were hoping, subtractive ¯ltering can't remove foldover once it is present in an audio signal.

1. Over-sampling

As a ¯rst line of defense against foldover, we can synthesize the waveform at a much higher sample rate, apply a low-pass ¯lter whose cuto® frequency is set to the Nyquist frequency (for the original sample rate), then down-sample. For example, in the above scenario (44100 sample rate, 440 Hertz tone) we could generate the sawtooth at a sample rate of 16 ¢44100 = 705600 Hertz. We need only worry about frequencies in excess of 705600 ¡ 20000 = 685600 Hertz (so that they fold over into audible frequencies; foldover to ultrasonic frequencies normally won't concern us) so the ¯rst problematic partial is 685600=440 = 1558, whose amplitude is -64dB relative to that of the fundamental.

This attenuation degrades by 6 dB for every octave the fundamental is raised, so that a 10 kHz. sawtooth only enjoys a 37 dB drop from the fundamental to the loudest foldover partial. On the other hand, raising the sample rate by an additional factor of two reduces foldover by the same amount. If we

magnitude (dB)

0  ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.546.png)

-10

-20 a/k

-30

b/k2  -40

-50

1   2   4   8   16  32 

partial number (k)

Figure 10.8: Magnitude spectrum of a triangle wave with M=N = 0:03. The two line segments show 1=k and 1=k2 behavior at low and high frequencies.

really wish to get 60 decibels of foldover rejection|all the way up to a 10 kHz. fundamental|we will have to over-sample by a factor of 256, to a sample rate

of about 11 million Hertz.

2. Sneaky triangle waves

For low fundamental frequencies, over-sampling is an easy way to get adequate foldover protection. If we wish to allow higher frequencies, we will need a more sophisticated approach. One possibility is to replace discontinuities by ramps, or in other words, to replace component sawtooth waves by triangle waves, as treated in Section 10.3.4, with values of M=N small enough that the result sounds like a sawtooth wave, but large enough to control foldover.

Returning to Figure 10.8, suppose for example we imitate a sawtooth wave with a triangle wave with M equal to two samples, so that the ¯rst notch falls on the Nyquist frequency. Partials above the ¯rst notch (the 17th partial in the ¯gure) will fold over; the worst of them is about 40 dB below the fundamental. On the other hand, the partial strengths start dropping faster than those of a true sawtooth wave at about half the Nyquist frequency. This is acceptable in some, but not all, situations.

The triangle wave strategy can be combined with over-sampling to improve the situation further. Again in the context of Figure 10.8, suppose we over- sample by a factor of 4, and set the ¯rst notch at the original sample rate. The partials up to the Nyquist frequency (partial 8, at the fundamental frequency shown in the ¯gure) follow those of the true sawtooth wave fairly well. Foldover sets in only at partial number 48, and is 52 dB below the fundamental. This overall behavior holds for any fundamental frequency up to about one quarter the sample rate (after which M exceeds N=2). Setting the notch frequency to the original sample rate is equivalent to setting the segment of length 2M to one sample (at the original sample rate).

3. Transition splicing

In the point of view developed in this chapter, the energy of the spectral com- ponents of classical waves can be attributed entirely to their jumps and corners. This is arti¯cial, of course: the energy really emanates from the entire wave- form. Our derivation of the spectrum of the classical waveforms uses the jumps and corners as a bookkeeping device, and this is possible because the entire waveform is determined by their positions and magnitudes.

Taking this ruse even further, the problem of making band-limited versions of classical waveforms can be attacked by making band-limited versions of the jumps and corners. Since the jumps are the more serious foldover threat, we will focus on them here, although the approach described here works perfectly well for corners as well.

To construct a band-limited step function, all we have to do is add the Fourier components of a square wave, as many as we like, and then harvest the step function at any one of the jumps. Figure 10.9 shows the partial Fourier

![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.547.png)

Figure 10.9: A square wave, band-limited to partials 1, 3, 5, 7, 9, and 11. This can be regarded approximately as a series of band-limited step functions arranged end to end.

sum corresponding to a square wave, using partials 1, 3, 5, 7, 9, and 11. The cuto® frequency can be taken as 12! (if ! is the fundamental frequency).

If we double the period of the square wave, to arrive at the same cuto® frequency, we would add twice as many Fourier partials, up to number 23, for instance. Extending this process forever, we would eventually see the ideal band-limited step function, twice per (arbitrarily long) period.

In practice we can do quite well using only the ¯rst two partials (one and three times the fundamental). Figure 10.10 (part a) shows a two-partial approx- imation of a square wave. The cuto® frequency is four times the fundamental; so if the period of the waveform is eight samples, the cuto® is at the Nyquist frequency. Part (b) of the ¯gure shows how we could use this step function to synthesize, approximately, a square wave of twice the period. If the cuto® frequency is the Nyquist frequency, the period of the waveform of part (b) is 16 samples. Each transition lasts 4 samples, because the band-limited square wave has a period of eight samples.

We can make a band-limited sawtooth wave by adding the four-sample-long transition to a ramp function so that the end of the resulting function meets smoothly with itself end to end, as shown in part (c) of the ¯gure. There is one transition per period, so the period must be at least four samples; the highest fundamental frequency we can synthesize this way is half the Nyquist frequency. For this or lower fundamental frequency, the foldover products all turn out to be at least 60 dB quieter than the fundamental.

Figure 10.11 shows how to generate a sawtooth wave with a spliced transi- tion. The two parameters are f , the fundamental frequency, and b, the band limit, assumed to be at least as large as f . We start with a digital sawtooth wave (a phasor) ranging from -0.5 to 0.5 in value. The transition will take place at the middle of the cycle, when the phasor crosses 0. The wavetable is traversed in a constant amount of time, 1=b, regardless of f . The table lookup is taken to be non-wraparound, so that inputs out of range output either -0.5 or 0.5.

At the end of the cycle the phasor discontinuously jumps from -0.5 to 0.5, but the output of the transition table jumps an equal and opposite amount, so the result is continuous. During the portion of the waveform in which the

(a)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.548.png)

(b)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.549.png)

(c)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.550.png)

Figure 10.10: Stretching a band-limited square wave: (a) the original waveform; (b) after splicing in horizontal segments; (c) using the same step transition for a sawtooth wave.

5. EXAMPLES 324

f  

0\.5 -0.5![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.551.png)

b/f

0\.5 -0.5

-0.5 0.5

OUT

Figure 10.11: Block diagram for making a sawtooth wave with a spliced transi- tion.

-- PHASES (percent) -- 0 0 0![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.552.png)

phasor~ / 100 / 100 / 100

phasor~ sawtooth wave -~  -~  -~ ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.553.png)

-~ 0.5 remove DC bias wrap~ wrap~ wrap~ wrap~ 1/2 cycle -~ 0.5 -~ 0.5 -~ 0.5

out of

-~ 0.5 phase AMPLITUDES (percent) +~  -~  sum and difference 0 0 0

/ 100 / 100 / 100

(a) \*~  \*~  \*~ 

+~ 

+~  (b)

|  

(OUT)

Figure 10.12: Combining sawtooth waves: (a) adding and subtracting sawtooth waves 1/2 cycle out of phase, to extract even and odd harmonics; (b) combining three sawtooth waves with arbitrary amplitudes and phases.

transition table is read at one or the other end-point, the output describes a straight line segment.

5. Examples

Combining sawtooth waves

Example J01.even.odd.pd (Figure 10.12, part a) shows how to combine saw- tooth waves in pairs to extract the even and odd harmonics. The resulting waveforms are as shown in Figure 10.3. Example J02.trapezoids.pd (part b of the ¯gure) demonstrates combining three sawtooth waves at arbitrary phases and amplitudes; the resulting classic waveform has up to three jumps and no corners. The three line segments are horizontal as long as the three jumps add to zero; otherwise the segments are sloped to make up for the the unbalanced jumps so that the result repeats from one period to the next.

Example J03.pulse.width.mod.pd (not shown) combines two sawtooth waves, of opposite sign, with slightly di®erent frequencies so that the relative phase

frequency -- PHASES (percent) --

0 0 0 0 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.554.png)phasor~ / 100 / 100 / 100

-~  -~  -~ wrap~ wrap~ wrap~ -~ 0.5 -~ 0.5 -~ 0.5

\*~  \*~  \*~ 

\*~ 0.5 \*~ 0.5 \*~ 0.5 -~ 0.0833 -~ 0.0833 -~ 0.0833

AMPLITUDES (percent)

0 0 0

/ 100 / 100 / 100

\*~  \*~  \*~ +~ 

+~ 

|  (OUT)

Figure 10.13: Combining parabolic waves to make a waveform with three cor- ners.

changes continuously. Their sum is a rectangle wave whose width varies in time. This is known as pulse width modulation (\PWM").

Example J04.corners.pd (Figure 10.13) shows how to add parabolic waves to make a combined waveform with three corners. Each parabolic wave is com- puted from a sawtooth wave (ranging from -0.5 to 0.5) by squaring it, multi- plying by 0.5, and subtracting the DC component of -1/12, or -0.08333. The patch combines three such parabolic waves with controllable amplitudes and phases. As long as the amplitudes sum to zero, the resulting waveform consists of line segments, whose corners are located according to the three phases and have slope changes according to the three amplitudes.

Strategies for band-limiting sawtooth waves

Example J05.triangle.pd (Figure 10.14, part a) shows a simple way to make a triangle wave, in which only the slope of the rising and falling segment are

frequency slopes![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.555.png)

0 up  down 0   frequency

phasor~ 0 0 phasor~

/ 100 / 100

0 slope of rise segment

\*~ -1+~ 1 \*~  \*~ 0 Duty cycle

\*~  / 100 make the phasor cross zero at the desired point of the cycle.

min~ -~  0 slope of decay segment

|  

(OUT) \* -1 multiply by desired slope, negating so that the segment points downward

\*~ 

(a) (b) minimum of rise and decay segments

min~ (makes a triangle wave)

clip~ 0 1 clip between 0 and 1 to make the

|   sustain and silent regions. (OUT)

Figure 10.14: Alternative techniques for making waveforms with corners: (a) a triangle wave as the minimum of two line segments; (b) clipping a triangle wave to make an \envelope".

speci¯ed. A phasor supplies the rising shape (its amplitude being the slope), and the same phasor, subtracted from one, gives the decaying shape. The minimum of the two linear functions follows the rising phasor up to the intersection of the two, and then follows the falling phasor back down to zero at the end of the cycle.

A triangle wave can be clipped above and below to make a trapezoidal wave, which can be used either as an audio-frequency pulse or, at a lower fundamen- tal frequency, as a repeating ASR (attack/sustain/release) envelope. Patch J06.enveloping.pd (Figure 10.14 part b) demonstrates this. The same rising shape is used as in the previous example, and the falling shape di®ers only in that its phase is set so that it falls to zero at a controllable point (not necessar- ily at the end of the cycle as before). The clip~ object prevents it from rising above 1 (so that, if the intersection of the two segments is higher than one, we get a horizontal \sustain" segment), and also from falling below zero, so that once the falling shape reaches zero, the output is zero for the rest of the cycle.

Example J07.oversampling.pd shows how to use up-sampling to reduce foldover when using a phasor~ object as an audio sawtooth wave. A subpatch, running at 16 times the base sample rate, contains the phasor~ object and a three- pole, three-zero Butterworth ¯lter to reduce the amplitudes of partials above the Nyquist frequency of the parent patch (running at the original sample rate) so that the output won't fold over when it is down-sampled at the outlet~ object. Example J08.classicsynth.pd demonstrates using up-sampled phasors as signal generators to make an imitation of a classic synthesizer doing subtractive synthesis.

Example J09.bandlimited.pd shows how to use transition splicing as an al- ternative way to generate a sawtooth wave with controllable foldover. This has the advantage of being more direct (and usually less compute-intensive) than the up-sampling method. On the other hand, this technique depends on using the reciprocal of the fundamental frequency as an audio signal in its own right (to control the amplitude of the sweeping signal that reads the transition table) and, in the same way as for the PAF technique of Chapter 6, care must be taken to avoid clicks if the fundamental frequency changes discontinuously.

Exercises

1. A phasor~ object has a frequency of 441 Hertz (at a sample rate of 44100). What is the amplitude of the DC component? The fundamental? The partial at 22050 Hertz (above which the partials fold over)?
1. A square wave oscillates between 1 and -1. What is its RMS amplitude?
1. In Section 10.3 a square wave was presented as an odd waveform whose Fourier series consisted of sine (and not cosine) functions. If the square wave is advanced 1/8 cycle in phase, so that it appears as an even function, what does its Fourier series become?
4. A rectangle wave is 1 for 1/4 cycle, zero for 3/4 cycles. What are the strengths of its harmonics at 0, 1, 2, 3, and 4 times the fundamental?
4. How much is 1 + 1=9 + 1=25 + 1=49 + 1=81 + ¢¢¢?

325 CHAPTER 10. CLASSICAL WAVEFORMS


Index

- » , 18 moses , 78 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.556.png)![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.557.png)bang » , 290 mtof , 22 block » , 213 noise » , 256 bp » , 256 notein , 83

  osc » , 18 catch » , 107

  clip » , 138 outlet , 102 cos » , 52 outlet » , 102 cpole » , 260 pack , 50 czero~~ rev » , 260 pipe , 77 czero » , 260 poly , 113

  dac » , 18 q8~~ rsqrt » , 292 delay , del , 77

  receive , 22 delread » , 209 receive » , 54

  delwrite » , 208

r®t » , 287

div , 113

ri®t » , 287 env » , 82

expr , 54 rpole » , 260

®t » , 286 rzero~~ rev » , 260

rzero » , 260 ¯ddle » , 135 r , 22

ftom , 22 r » , 54

hip » , 50, 256 samphold » , 54 inlet , 102 select , sel , 78 inlet » , 102 send , 23

line , 80 send » , 54

line » , 21 snapshot » , 82 loadbang , 54

stripnote , 83 lop » , 256

switch » , 213 lrshift » , 292 s , 23

makenote , 113 s » , 54

mod , 113 tabosc4 » , 47

319


tabread4 » , 48 ![](Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.558.png)tabreceive » , 287 tabsend » , 290 tabwrite » , 48 throw » , 110 trigger , t , 83

unpack , 107 until , 171 vcf » , 256 vd » , 209

vline » , 80 wrap » , 54

absolute value (of a complex num-

ber), 177

abstraction, 102

additive synthesis, 15

examples, 107, 110

ADSR envelope generator, 89 aliasing, 60

all-pass ¯lter, 193

amplitude, 1, 3

complex, 179

amplitude, measures of, 3 amplitude, peak, 3

amplitude, RMS, 3

angle of rotation, 190

argument (of a complex number),

177

arguments

creation, 16

audio signals, digital, 1

band-pass ¯lter, 226 bandwidth, 147, 227 beating, 24

Bessel functions, 141 box, 15

GUI, 16 message, 15 number, 16 object, 16

carrier frequency, 132, 148

carrier signal, 122

center frequency, 147, 227 Central Limit Theorem, 131 cents, 7

Chebychev polynomials, 140 class, 16

classical waveforms, 295 clipping, 27

clipping function, 127 coloration, 194

comb ¯lter, 183

recirculating, 185 compander, 276

complex conjugate, 231 complex numbers, 176 compound ¯lter, 232 continuous spectrum, 121 control, 61

control stream, 63

numeric, 64

covariance, 11

creation arguments, 16

DC, 121, 237

debouncing, 69

decibels, 4

delay

compound, 74

in Pd, 77

on control streams, 74 simple, 74

delay network

linear, 180

delay, audio, 180

digital audio signals, 1 Dirichlet kernel, 266 discrete spectrum, 119 distortion, 127

Doppler e®ect, 200

duty cycle, 40

dynamic, 6

dynamic range, 276

echo density, 194 elementary ¯lter

non-recirculating, 229


INDEX

recirculating, 232 encapsulation, 102 envelope follower, 69, 252 envelope generator, 10, 89

ADSR, 89

resetting, 95 equalization, 227

event, 63

event detection, 69

feedback, 160

¯lter, 183, 223

all-pass, 193, 249

band-pass, 226

Butterworth, 241

compound, 232

elementary non-recirculating, 229 elementary recirculating, 232 high-pass, 224

low-pass, 224

peaking, 227

shelving, 227

¯rst di®erence, 302

foldover, 60

formant, 147

Fourier analysis, 263

Fourier transform, 264

fast (FFT), 286

phase shift formula, 269

time shift formula, 268 windowed, 271

frequency

carrier, 132

modulation, 132

frequency domain, 180

frequency modulation, 24, 132 frequency response, 183

frequency, angular, 1

fundamental, 12

gain, 183

granular synthesis, 34 GUI box, 16

half-step, 7

Hann window function, 152

321

Hanning window function, 152, 271 harmonic signal, 119

harmonics, 12

high-pass ¯lter, 224

hop size, 274

imaginary part of a complex num-

ber, 176

impulse, 181, 303

impulse response, 185

index

of modulation, 132

waveshaping, 126, 140 inharmonic signal, 121

interference, 175

intermodulation, 130

Karplus-Strong synthesis, 213

logical time, 61 low-pass ¯lter, 224

magnitude (of a complex number),

177

merging control streams, 74

in Pd, 78

message box, 15

messages, 17, 77

MIDI, 7

modulating signal, 122

modulation

frequency, 24, 132

ring, 122

muting, 95

noise gate, 276

noisy spectrum, 121 number box, 16 numeric control stream

in Pd, 77

Nyquist theorem, 59

object box, 16 octave, 7 oscillator, 8

parabolic wave, 300


parent, 102

partials, 121

passband, 224

patch, 8, 15

peaking ¯lter, 227

period, 12

phase locking, 283

phase-aligned formant (PAF), 158 Pitch/Frequency Conversion formu-

las, 7

polar form (of a complex number),

177

pole-zero plot, 235

polyphony, 98

power, 3

power series, 130

pruning control streams, 74

in Pd, 78

quality (\q"), 249

real part of a complex number, 176 real time, 61

rectangle wave, 295

rectangular form (of a complex num-

ber), 177

re°ection, 191

resynchronizing control streams, 74

in Pd, 78

ring modulation, 122

ripple, 224

sample number, 1

sample rate, 1

sampling, 32

examples, 111 sawtooth wave, 28, 295 settling time, 247 shelving ¯lter, 227 sidebands, 122

sidelobes, 154, 267 signals, digital audio, 1 spectral envelope, 34, 121 spectrum, 119

square wave, 298

stable delay network, 185

stopband, 226

stopband attenuation, 226 subpatch, 102

subpatches, 102

subtractive synthesis, 250, 307 switch-and-ramp technique, 96

tags, 101

tasks, 98

threshold detection, 69

timbre stamping, 279

timbre stretching, 37, 149

time domain, 180

time invariance, 180

time sequence, 63

toggle switch, 24

transfer function, 94, 126, 223 transient generator, 89 transition band, 226

triangle wave, 295

unit generators, 8

unitary delay network, 189

vocoder, 278

voice bank, 98

von Hann window function, 271

wave packet, 154

waveshaping, 126

wavetable lookup, 27

non-interpolating, 28 wavetables

transposition formula for loop-

ing, 33

transposition formula, momen-

tary, 33

window, 3, 274

window function, 271

window size, 206


Bibliography

[Bal03] Mark Ballora. Essentials of Music Technology. Prentice Hall, Upper

Saddle River, New Jersey, 2003.

[Ble01] Barry Blesser. An interdisciplinary synthesis of reverberation view-

points. Journal of the Audio Engineering Society, 49(10):867{903, 2001.

[Bou00] Richard Boulanger, editor. The Csound book. MIT Press, Cambridge,

Massachusetts, 2000.

[Cha80] Hal Chamberlin. Musical applications of microprocessors. Hayden,

Rochelle Park, N.J., 1980.

[Cho73] John Chowning. The synthesis of complex audio spectra by means

of frequency modulation. Journal of the Audio Engineering Society, 21(7):526{534, 1973.

[Cho89] John Chowning. Frequency modulation synthesis of the singing voice.

In Max V. Mathews and John R. Pierce, editors, Current Directions in Computer Music Research, pages 57{64. MIT Press, Cambridge, 1989.

[DJ85] Charles Dodge and Thomas A. Jerse. Computer music : synthesis, composition, and performance. Schirmer, New York, 1985.

[DL97] Mark Dolson and Jean Laroche. About this phasiness business. In

Proceedings of the International Computer Music Conference, pages 55{58, Ann Arbor, 1997. International Computer Music Association.

[GM77] John M. Grey and James A. Moorer. Perceptual evaluations of syn-

thesized musical instrument tones. Journal of the Acoustical Society of America, 62:454{462, 1977.

[Har87] William M. Hartmann. Digital waveform generation by fractional

addressing. Journal of the Acoustical Society of America, 82:1883{ 1891, 1987.

[KS83] Kevin Karplus and Alex Strong. Digital synthesis of plucked-string

and drum timbres. Computer Music Journal, 7(2):43{55, 1983.

323

324 BIBLIOGRAPHY [Leb77] Marc Lebrun. A derivation of the spectrum of FM with a complex

modulating wave. Computer Music Journal, 1(4):51{52, 1977.

[Leb79] Marc Lebrun. Digital waveshaping synthesis. Journal of the Audio

Engineering Society, 27(4):250{266, 1979.

[Mat69] Max V. Mathews. The Technology of Computer Music. MIT Press,

Cambridge, Massachusetts, 1969.

[Moo90] F. Richard Moore. Elements of Computer Music. Prentice Hall,

Englewood Cli®s, second edition, 1990.

[PB87] T. W. Parks and C.S. Burrus. Digital ¯lter design. Wiley, New York,

1987\.

[Puc95a] Miller S. Puckette. Formant-based audio synthesis using nonlinear

distortion. Journal of the Audio Engineering Society, 43(1):224{227, 1995.

[Puc95b] Miller S. Puckette. Phase-locked vocoder. In IEEE ASSP Workshop

on Applications of Signal Processing to Audio and Acoustics, 1995. [Puc01] Miller S. Puckette. Synthesizing sounds with speci¯ed, time-varying

spectra. In Proceedings of the International Computer Music Con-

ference, pages 361{364, Ann Arbor, 2001. International Computer

Music Association.

[Puc05] Miller S. Puckette. Phase bashing for sample-based formant synthe-

sis. In Proceedings of the International Computer Music Conference, pages 733{736, Ann Arbor, 2005. International Computer Music As- sociation.

[Reg93] Phillip A. Regalia. Special ¯lter design. In Sanjit K. Mitra and

James F. Kaiser, editors, Handbook for digital signal processing, pages 907{978. Wiley, New York, 1993.

[RM69] Jean-Claude Risset and Max V. Mathews. Analysis of musical in-

strument tones. Physics Today, 22:23{40, 1969.

[RMW02] Thomas D. Rossing, F. Richard Moore, and Paul A. Wheeler. The Science of Sound. Addison Wesley, San Francisco, third edition, 2002.

[Roa01] Curtis Roads. Microsound. MIT Press, Cambridge, Massachusetts,

2001\.

[Sch77] Bill Schottstaedt. Simulation of natural instrument tones using fre-

quency modulation with a complex modulating wave. Computer Mu- sic Journal, 1(4):46{50, 1977.

BIBLIOGRAPHY 325 [SI03] Julius Orion Smith III. Mathematics of the Discrete Fourier Trans-

form (DFT), with Music and Audio Applications. W3K Publishing, Menlo Park, California, 2003.

[Ste96] Kenneth Steiglitz. A Digital Signal Processing Primer. Addison-

Wesley, Menlo Park, California, 1996.

[Str85] John Strawn, editor. Digital Audio Signal Processing. William Kauf-

mann, Los Altos, California, 1985.

[Str95] Allen Strange. Electronic music: systems, techniques, and controls.

W. C. Brown, Dubuque, Iowa, 1995.

[^1]: [t] = cos(!cn + a cos(!mn))
[ref1]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.267.png
[ref2]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.268.png
[ref3]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.292.png
[ref4]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.355.png
[ref5]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.419.png
[ref6]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.423.png
[ref7]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.447.png
[ref8]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.488.png
[ref9]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.496.png
[ref10]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.497.png
[ref11]: Aspose.Words.39de734b-8310-485c-b691-3f8d6b4844bd.499.png
