Project Goal
To conduct a comprehensive study of the architecture and internal components of the Windows operating system to understand the principles of process operation, memory management, and code execution mechanisms, as well as to develop practical tools for interacting with system structures.

Project Description
Methodology and Approach
During the research, I developed a multi-level analysis methodology combining:

Static Analysis:

Investigation of PE file structure using Detect It Easy

Analysis of executable file headers and memory sections

Study of import/export tables of system libraries

Dynamic Analysis:

Real-time system activity monitoring using Process Monitor

Tracing process and thread creation

Analysis of dynamic library loading

Practical Experimentation:

Development of utilities for interacting with Windows API

Testing memory management mechanisms

Creation of proof-of-concept tools to demonstrate theoretical concepts

Key Research Findings
1. Windows Process Architecture
I conducted a detailed study of the internal structure of Windows processes. During experiments with the notepad.exe process, I discovered interesting dependencies between parent and child processes. The analysis of process integrity levels was particularly interesting, where I found that notepad.exe runs with high privilege levels, opening possibilities for further research into security mechanisms.

2. Memory Management Mechanisms
I conducted a series of experiments on virtual memory analysis, during which I:

Determined base loading addresses of critical system components

Investigated address space distribution between user and system components

Analyzed the impact of system architecture (32-bit vs 64-bit) on memory organization

3. Dynamic Libraries and Their Loading
My work on DLL analysis revealed a complex system of dependencies between system components. I tracked the loading chain of 51 dynamic libraries for the relatively simple notepad.exe application, demonstrating the complexity of modern operating systems.

4. Executable File Format
I developed a methodology for analyzing PE files that enables:

Identifying program entry points

Analyzing the structure of executable file sections

Identifying critical strings and resources

Practical Development
Based on the acquired theoretical knowledge, I created the inject-poc.exe tool, which demonstrates:

Techniques for working with Windows API for process management

Mechanisms for allocating and managing virtual memory

Practical application of knowledge about internal process structure

The development successfully passed testing and confirmed theoretical concepts, demonstrating the possibility of controlled interaction with system structures.

Conclusions
The conducted research allowed me to deeply understand the architectural principles of the Windows operating system. The most significant results were:

Systematic Understanding of Windows internal mechanisms, from process level to memory management

Practical Skills in working with low-level APIs and system structures

Analysis Methodology for complex system components

The acquired knowledge has practical significance for developing system software, security analysis, and creating system activity monitoring tools. The research demonstrates that understanding operating system internal mechanisms is critically important for creating efficient and secure applications.

Further research is planned to focus on analyzing memory protection mechanisms and studying modern process isolation technologies in Windows.

