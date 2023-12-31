# Welcome to my Quantum Step Sequencer!

As quantum computing continues to advance, there is a growing interest in exploring its applications in the field of music technology. This project develops a 16-step sequencer that introduces quantum algorithms into the process of generating sound, and it aims to propose an easy approach for the self-development of quantum instruments. You can run this instrument on your own computer by following this README.

## Abstract: what is this project about?

The step-sequencer employs a Launchpad X interface to control the generation of MIDI notes, which are then processed in Python. The resulting commands are sent to either a Pd patch or the DAW Cubase for sound synthesis. The interface consists of an eight by eight grid of buttons, with the first three rows associated with qubits. Different gates can be manually chosen and applied to these qubits, allowing for intuitive manipulation of quantum systems. The step-sequencer divides the Launchpad X into two halves, with each half representing eight steps. While the qubits operate under quantum principles, the fourth row of the interface is dedicated to chords and bass as “classical instruments”. This combination of quantum and classical instruments enables the generation of both steady and repetitive sequences, as well as counterintuitive and surprising musical patterns. The paper attached provides detailed explanations of the interface, code, and sound synthesis components, highlighting the functionality and capabilities of the quantum step-sequencer.

A simple sketch of this instrument is presented here: 

<img src="https://github.com/maria-aguado/Quantum-Step-Sequencer/assets/114862739/d84418f6-1896-458f-b961-6066412c9172" width="400" />

## Getting Started

I suggest going through the .pdf document I have attached. A detailed explanation of this project and its various parts is presented in it. 

### What do you need?

* **A Launchpad X** as an interface (it can be substituted by any alternative MIDI device, but subsequent modifications should be performed in the code).
* **An environment to run Python notebooks** (ex: Visual Studio Code).
* **To install either Cubase Pro 12 or Pure Data** for sound synthesis.
* **A Focusrite Interface:** I used it to connect with Cubase but not to connect with Pure Data. This is a personal choice depending on your operating system and computational efficiency.

### Executing program

To run the step sequencer, ensure that each of the following bullet points is satisfied:

* Your Launchpad X should be connected in _Programmer Mode_ to your computer.
* You should open the Cubase Project in Cubase Pro 12 or the Pure Data patches. You can choose your own VTS plugins and sounds for the Cubase project. The melody, the chords, and the bass require plugins, whereas the kick, the snare, and the hi-hat can be sampled. For Pure Data, the melody, chords, and bass rely on their own patches, whereas the percussion is again sampled. I have uploaded the .wav files I used in PD. You need to load them in the main patch (QuantumStep).
* Once your interface and Cubase/PD are ready, you have to run the launchpad.ipynb notebook. This is where the main program loop takes place. Ensure that all of the MIDI ports are correctly configured (there is a section for this purpose within the code). If the step sequencer is running properly, the Launchpad should be displaying a light setup, and you should be able to hear sound.

## Contact & Help

You can contact me if you have any questions at mariaaguyan@gmail.com. I will be glad to help!

## Acknowledgments

This project was made possible thanks to the publication of the book _Quantum Computer Music: Foundations and Initial Experiments_. I drew inspiration from the initial chapters (1-7). This book provides an introduction to different ways of applying quantum computing in music and proposes algorithms and methods to do so.
