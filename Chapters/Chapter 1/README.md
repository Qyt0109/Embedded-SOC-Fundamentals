# Chapter 1. A Memory-centric System Model

Chapter 1 introduces embedded systems from a high-level hardware and software perspective. We cover basic systems built on microcontroller-based architectures before moving to SoC-based designs.

###### In this first chapter, we will review the basics of a computer system.

## 1.1. Global Computing Systems

Nowadays, computing is pervasive throughout the entire world:
- Wide area network
- Cloud computing
- Servers
- IoT
- ...

The expandsion of IoT is one of the new technology revolutions, also including the field of robotics, automotive, AI,... with many areas of research and numerous new industrial products.

<figure>
  <img src="./images/1.1.png">
  <figcaption style="text-align:center;">
    High-level component view of a global computing system
  </figcaption>
</figure>

However, the majority of this technology is hidden from the average human user. Typically, large servers will have thousands of processing units in form of microprocessors together with huge amounts of memory and specific accelerators (GPUs, FPGAs,...).

## 1.2. General Computer Architecture

Computer architecture at the hardware level is a system composed basic elements:
- __Processor(s)__ or __Microprocessor(s)__ for data management and program execution.
- __Memories__ for code, data, and operational (stack, heap,...) storage.
- __I/O devices__ for comunication with internal facilities and external world though __programmable interfaces__.

Connection between these elements:
- __Address bus__ is used to specify which requestor unit to access and which element within this unit.
- __Data bus__ is used to tranfer data between a requestor unit and a completer unit.
- __Control bus__ is used to specify what to do: the direction of data transfers (read or write) from the requestor unit's POV and when to do it in terms of timing.

Other mandatory functions and signals are also requires such as __clock__ to synchonize data transfers, a __reset__ to initialize the system, __power supply__ lines, __interrupt__ lines.

<figure>
  <img src="./images/1.2.png">
  <figcaption style="text-align:center;">
    General computer architecture with minimum of elements
  </figcaption>
</figure>

