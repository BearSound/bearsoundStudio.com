---
layout: default
title: Choosing the Right Microphone
author: matt
categories: guide
tags: microphone
---

# Choosing the Right Microphone
## Pre-Amble
When you've taken the plunge to record your own podcast one of the first items on your shopping list really should be a good quality microphone. This doesn't necessarily need to break the bank, after all, a well treated room will significant improve your audio recordings as opposed to adding an extra £200 onto an already serviceable microphone. When you're in the market for microphones, there's a bunch of jargon you need to get your head around first. This won't be an in-depth discussion on the topics, but enough to understand what they mean and how they affect the microphones in your shopping basket.

## Glossary of terms
* **Dynamic** - A type of microphone which operates using air-pressure resistance.
* **Condenser** - A type of microphone which utilises electrical currents from _Phantom Power_.
* **Hybrid** - Technically my own term for _Dynamic_ microphones which can benefit from the input of _Phantom Power_ such as the [_Aston Microphone Stealth_][f12df6e7].
* **Phantom Power** - usually a switch found on most audio interfaces which activates a 48v current to power electrical components in _Condenser_ and _Hybrid_ microphones.
* **Polar Pattern** - The Polar Pattern of a microphone represents how the microphone listens to sound, and from what 'general' direction it can hear.
* **USB Microphone** - As the name suggests, a USB microphone is a plug-and-play microphone with some form of built in Analogue-to-Digital (ADC) converter, forgoing the need for an audio interface.
* **Sensitivity** - Usually accompanied by numbers and the measurement `dBV` or `mV/Pa`. Essentially this tells us how quiet a sound the microphone can pick up (or conversely how loud you need to be to create listenable sound). The lower the negative number the less sensitive a microphone is in `dBV`. Conversely `mV/Pa`, the higher the number the more more sensitive the microphone.
* **Frequency Response** - How a microphone captures the intensity of individual frequency bands, some frequencies may appear louder, or 'boosted', compared to others.
* **Off-Axis** -
* **Proximity Effect** -

## Consider Your Applications
First and foremost in your mind should be how you intend your podcast to sound. Is it going to be group discussion, is it going to be journalistic, is it going to be solo, are you planning on a close-sounding NPR-style, or is this going to possibly get loud. These questions may sound arbitrary at first, however can have implications down the line if the ultimate purchase is of the wrong polar pattern, for example. <br>

### Remember Sound Reflects
I should clearly state that sound emits from a source-object in radials, much like dropping a pebble in still water. Therefore, the sounds in your room are constantly bouncing off walls, furniture, and anything else you might have in there. Just bear that in mind going forward. To get the cleanest recordings you need the quietest place.

## Polar Patterns
* ### Cardioid
The most common _Polar Pattern_ used for podcasting and broadcasting is the _Cardioid_, named after the apparent heart-shape it hears.
<br>

![Cardioid Polar Pattern](/public/images/polarPatternCardioid.png)

From the above diagram, you should be able to see that _Cardioid_ handles sound extremely well from the front, whilst providing a good _Off-Axis_ rejection of sound. What this translates to in the real world, is that sounds coming from behind the microphone are dampened, and less likely to be heard in your recordings, such as typing keyboards. Cardioid microphones also suffer from the _Proximity Effect_ and should be positioned slightly further away from your sound source to get a more neutral and representational sound. _Cardioid_ microphones also come in other exciting flavours, such as _Hypercardioid_ and/or _Supercardioid_, which are the same initial heart-shape, but more directional. Most commonly these types of microphones are long, thin, shotgun-style for use in very noisy environments.

* ### Omnidirectional
Less common in the broadcasting and podcasting world, _omnidirectional, or omni_ microphones can 'hear' in a 360<sup>o</sup> arc, great for catching discussions from around the table.
![Omnidirectional Polar Pattern](/public/images/polarPatternOmni.png)<br>
 Because of its construction, _Omnidirectional_ microphones have little _Proximity Effect_ issues, and can be placed much closer to a sound source.

* ### Figure of Eight
The _figure of eight_ polar pattern is a weird and wonderful type of microphone which offers almost unparalleled _off-axis_ rejection from the side.<br>

![Figure of Eight Polar Pattern](/public/images/polarPatternFigureOfEight.png)

Most commonly used in stereo mic-ing, as the name suggests, this polar pattern will pick up sound from the front **and** the back, resulting in a great microphone for an interviewer sitting across from their interviewee. Unfortunately the _Proximity Effect_ should be taken into consideration with this type of microphone.

## Dynamic or Condenser?
Both types of microphone have their pros and cons. For my own podcasting usage, I have consistently used dynamic microphones for their tendency to create a warm sound (due to the 16kHz roll off due to their design), the slightly lower sensitivity (as I have a loud and booming voice), and the fact that they are rugged little machines. All my own vocals are recorded on a [Rode Procaster](http://en.rode.com/microphones/procaster).

bearSound Studio however, keeps a troupe of [Sontronic STC-3](http://sontronics.com/stc3xpack.htm)s for clientelle location recording, and those occasional times when Sonic Signatures has guests. The flexibility of having a sensitive microphone allows for quiet voices and/or sound sources to be recorded at acceptable levels, rather than boosting the gain in post, amplifying any noise. Usually condenser mics will have a `pad` switch which knocks a good 20dB off of the sensitivity of the microphone meaning that you can use them for loud situations as well.

## A Word about Frequency Response
Frequency response, as previously alluded to, is how a microphone reacts to varying frequencies. In ideal world, a microphone would have a _flat frequency response_, i.e. listen to all frequencies (20Hz - 20kHz) with the same intensity. However, this is not an ideal world. Take, for instance, the Rode Procaster below:

![Rode Procaster Frequency Response](/public/images/procasterFrequencyResponse.jpg)

It's designed from the start as a vocal mic, therefore there is no need for the mic to capture the sub-bass, and it only pics up frequencies above 45Hz. As the mic hears frequencies between 100Hz -200Hz there is a slight boost in presence. 200Hz - 1kHz is actually quite flat and natural, before a little boost until 14kHz where it tails off. <br>
Each microphone has it's own frequency response, and as such, is the reason why no two microphones sound exactly the same. If you're recording your own vocals, I've found a good exercise is to take a short recording of your voice and run it through a spectral analyser such as [SpeK](http://spek.cc), or [FFMPEG](https://www.ffmpeg.org) if you're feeling command-line savvy, and notice the natural frequencies of your voice. As you can see from my own spectral analysis, there is a very strong presence in the 0-3.5kHz range, as well as the 7-18kHz range.

![Vocal Spectral Analysis](/public/images/vocalSpectrumAnalysis.png)

If we compare this to the Procaster frequency response, we can determine that the 300Hz -1.5kHz flat response will accurately capture the majority of the tone of my voice. With the dip around 14kHz, the sound will loose a little of the 'air' attributed to a recording (sometimes also referred as 'space'). This sound is exactly what I'm looking for. A nice, clean sound which has a certain tightness. Not quite NPR proximity effect, but just a little.

## The Battle of USB and XLR
### TL;DR
 - I will _always_ advocate XLR microphones over USB. That is my own personal opinion, of course, but the pros outweigh the cons considerably. If you want something that just works out-of-the-box, go USB, if you feel that 

So far, I have talked about how microphones listen, how they represent different frequencies, and whether they require a little extra electrical juice or not. The next big question is how do I connect the darn thing to my PC/Mac. Until recently, with the boon of live streaming, USB microphones were nothing really to write home about. They would capture your voice, but it would not sound great. Todays landscape is completely different. Prodigious audio companies like [Blue Microphones](https://www.blue-designs.co.uk/#) actively innovate in the USB microphone market. It really is the epitome of ease-of-use: just plug it in and on you go.

The downside in my book is the lack of choice. For a microphone to transmit your audio into a computer, it needs to make use of an Analogue to Digital Converter, or an ADC. As you can imagine, trying to fit _the best_ ADC into a small, self-contained piece of equipment whilst trying to make it as small as possible, and look good... well you get the gist. The Blue Microphones [Snowball Ice](https://www.blue-designs.co.uk/products/snowball-ice/) (which I have used on many occasions, don't get me wrong) is one such microphone which will only record in 44.1kHz sample rate, at 16 bits. I realise that I have not talked about these terms before, and I will not get into it here. But for me, the fact I cannot choose the sample and bit rate of the audio going into my computer is a great let down. I use several plug-ins as I produce podcasts and having the more information stored in even 48kHz audio allows for a better editing experience. Rant over.

Now, after all that negativity, USB microphones are fantastic choices if all you want to do is get a decent sound recorded with little-to-no faff. As I previously mentioned, I've used the Snowball Ice on and off for four years as a great quality Skype mic, even after catastrophic failures during Discord RPG games - the Snowball became my go-to.


  [f12df6e7]: https://www.astonmics.com/EN/product/Mics/Stealth "Aston Microphone Stealth"
