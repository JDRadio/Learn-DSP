## Module 0: Introduction to my approach

### Module objectives

- Describe the target audience
- Explain the approach used throughout this course
- Present a sample problem


### Target audience and the intuitive approach

Having worked myself in the field of satellite communications, it's easy for me to throw out mathematical formulas and complex diagrams if I'm explaining to another engineer who really should know about this -- this is how most books I've read on the topic are written. That method is great when you already have an understanding and are looking either for confirmation or to extend your knowledge, but it's not so great when you're facing the problem for the first time.

The audience I'm targetting with this guide ranges from the neophyte to the hobbyist, but also includes some engineers working in this field. I've come to realize that most engineers working with digital signal processing are not trained in the field and are expected to learn quickly the various concepts that would be useful for their job. They are often placed in such a position due to necessity caused by the difficulty of finding qualified experts. Digital signal processing in itself is very widespread, but most of the references target a hardware implementation, whereas this guide focuses on a fully software approach.

Traditional methods will usuall have you memorize formulas and throw them up on your exam just to never remember any of them afterwards. I advocate for an intuitive approach to learning, where you first start with understanding the concepts at a high level and only then can you solidify that knowledge with mathematics if you so desire. I believe it is possible to learn digital signal processing without having a deep understanding of the mathematics involved, rather going by intuition.

Here's a quick example of this approach:
> Create a system that will recover the keys pressed from the sound of a telephone.

An intuitive approach would want you to understand that when you press the digits on your telephone, it uses dual-tone multi-frequency signaling (DTMF), which is a fancy way of saying you have two tones playing at once. If you can identify which two tones are playing at the same time, you can match the pair to a key on the telephone. To identify the tones, since they have different frequencies, you need to list the frequencies present in the signal. Considering there are only 7 or 8 frequencies you are interested in, there are multiple approaches you could take: have a bank of filters (one per frequency), perform a fast Fourier transform (FFT), use the Goertzel algorithm, use cross-correlation with the expected tones, etc.

The goal of this guide is not to provide you with the most optimal solution, but rather to allow you to find a solution to any problem.

### Next module

#### [Module 1: Introduction to Digital Signal Processing](module1.md)
