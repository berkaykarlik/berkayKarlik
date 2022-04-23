---
layout: post
title:  "First steps toward emulation"
date:   2022-04-23 20:10:00 +0300
---

Past couple of months, I had been working on my first emulator project, a CHIP-8 interpreter.
It's not exactly finished as there are still some bugs to solve and improvements to make but it's
rather on a stable point now, so I have decided to share what I have learned so far.

# What's an emulator?

An emulator is a program that can simulate a given system on a hardware/software level.
If you are like me, you might had tried to play gameboy games on PC when you were a kid and discovered
some Gameboy emulators. However any system can be emulated (theoretically) Gameboy, Nes, arcade machines, micro chips even playstation and computers.
There are two general approaches toward emulation. Low Level Emulation (LLE) and High Level Emulation (HLE).
LLE aims to imitate whatever target systems hardware can do. While HLE tries to imitate the capability of the target systems software. Also these approaches are not binary but a range, LLE ,for example, can be implemented on component level (like cpu, ram...) or can be implemented down to its very basics like transistors or even atoms if you have the means...
You could research further into existing methodologies but at this point you are at a good point to get your hands dirty.

# Where to begin?

Every resource I could find on the internet seem to recommend CHIP-8 as the hello world of emulation. Thus I have started from there as well.
[CHIP-8](https://en.wikipedia.org/wiki/CHIP-8) is not a system but rather an interpreted programming language developed by Joseph Weisbecker. It was meant for microcomputers like COSMAC VIP and Telmac 1800. Few variations and extensions appeared later on.

The simplicity of the system makes it excellent for beginners. It only has:
* 36 instructions
* 4K memory
* 64x32 display
* 16 8-bit registers & special 16-bit register I
* Stack pointer
* 2 8-bit timers
* Stack of 16 16-bit values & 8-bit Stack pointer (SP)
* 16-bit program counter (PC)
* 16-key hexadecimal keypad

List might look like a lot but believe me this is one of the simplest systems you can get. If you are interested
and would like to give a shoot on writing your own chip-8 interpreter, I can recommend resources I relied on:

* [Cowgod's Chip-8 Technical Reference](http://devernay.free.fr/hacks/chip8/C8TECH10.HTM)
* [Tobias v. Langhoff's Guide to making a CHIP-8 emulator](https://tobiasvl.github.io/blog/write-a-chip-8-emulator/#0nnn-execute-machine-language-routine)
* Reddit [r/EmuDev](https://www.reddit.com/r/EmuDev/) and it's [discord](https://discord.com/invite/dkmJAes) has a very helpful community as well.

I will conclude this post after this short introduction to Emulator development and Chip-8. I'm planning to
write more about [my own implementation](https://github.com/berkaykarlik/Chip8py) in future posts so stay tuned.
Thanks for reading.