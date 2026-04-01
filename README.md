# Academic Projects Portfolio

This repository highlights selected academic projects I completed as part of my computer science coursework at the University of San Diego.

Because several of these assignments are reused in future semesters, I am not publishing the source code publicly. Instead, this portfolio summarizes the project goals, technologies used, key implementation details, and selected outputs or visuals where appropriate.

## Project Areas
- Systems Programming
- Networking
- Computer Architecture / Digital Design

## Featured Projects
- [ToreroServe](#toreroserve)
- [Iterative DNS Resolver](#iterative-dns-resolver)
- [Sensor Network Protocol Reverse Engineering & Client](#sensor-network-protocol-reverse-engineering--client)
- [Unix Shell Project](#unix-shell-project)
- [Pipelined RISC-V Processor](#pipelined-risc-v-processor)

---

## ToreroServe

**Area:** Networking / Systems  
**Tech:** C++, TCP sockets, HTTP, multithreading, Linux

ToreroServe is a multithreaded HTTP web server built in C++. The server was designed to serve files from a configurable document root and support multiple simultaneous client connections.

### What I Built
- Implemented HTTP request parsing and response handling for valid and invalid requests
- Served multiple content types including HTML, CSS, images, PDFs, JSON, and plain text
- Added support for 404 responses, directory index handling, and auto-generated directory listings
- Implemented concurrent client handling with worker threads and a bounded-buffer model

### What I Learned
This project strengthened my understanding of TCP communication, HTTP request/response structure, concurrency, and systems debugging. It also gave me hands-on experience validating correctness with checksum-based testing and debugging memory issues with Valgrind.

### Screenshots / Outputs
Add browser screenshots, terminal output, or directory listing screenshots here.

---

## Iterative DNS Resolver

**Area:** Networking  
**Tech:** Python, UDP sockets, DNS, logging

This project involved building an iterative DNS resolver capable of resolving both A and MX records by querying root, top-level domain, and authoritative name servers.

### What I Built
- Sent and received DNS queries over UDP sockets
- Parsed raw DNS responses and extracted records including A, CNAME, NS, MX, SOA, and AAAA
- Implemented referral handling, CNAME chaining, timeout behavior, and retries across multiple servers
- Logged resolution steps to make the lookup process transparent and easier to debug

### What I Learned
This project gave me a much deeper understanding of how DNS actually works under the hood, especially the difference between recursive and iterative resolution. It also helped me practice protocol parsing and building reliable networked software in Python.

### Screenshots / Outputs
Add terminal screenshots showing A and MX record resolution here.

---

## Sensor Network Protocol Reverse Engineering & Client

**Area:** Networking / Protocol Analysis  
**Tech:** C, POSIX sockets, TCP/IP, Wireshark, tshark

In this project, I reverse-engineered a custom sensor network protocol by observing packet captures and reconstructing the client/server message flow. After analyzing the protocol, I reimplemented the client in C using sockets.

### What I Built
- Used Wireshark and tshark to analyze packet contents, connection flow, and application-layer message structure
- Reconstructed the protocol sequence and created a client that matched the original protocol behavior
- Reimplemented the client using the BSD sockets API in C
- Validated correctness through live server communication and debugging

### What I Learned
This project taught me how to reason about undocumented protocols by combining observation, inference, and testing. It also gave me strong practice with socket programming and low-level networking tools.

### Screenshots / Outputs
Add sequence diagram, tshark output, or terminal screenshots here.

---

## Unix Shell Project

**Area:** Systems Programming  
**Tech:** C, Linux, processes, signals

This project involved building a Unix-like shell in C that supported core command-line functionality, process management, and signal handling.

### What I Built
- Implemented command execution using `fork` and `execvp`
- Added support for built-in commands and background process execution
- Handled `SIGINT` and `SIGCHLD` for interactive shell control and child-process management
- Implemented process tracking and exit-status reporting

### What I Learned
This project helped me understand how shells manage processes, signals, and interactive behavior. It also gave me practical experience working directly with operating system primitives in C.

### Screenshots / Outputs
Add terminal screenshots showing command execution and background jobs here.

---

## Pipelined RISC-V Processor

**Area:** Computer Architecture / Digital Design  
**Tech:** SystemVerilog, RISC-V, Quartus, Questa

This project focused on building and debugging a 5-stage pipelined RISC-V processor with support for hazard handling.

### What I Built
- Added forwarding, stalls, and flushes to correctly handle data and control hazards
- Integrated a hazard unit into the processor controller/datapath design
- Tested dependency scenarios including load-use hazards, branch hazards, and store-related forwarding behavior
- Verified correctness through simulation and waveform analysis in Questa

### What I Learned
This project deepened my understanding of pipelined processor design, datapath/control interaction, and hardware verification. It also improved my ability to debug complex logic using simulations and targeted test cases.

### Screenshots / Outputs
Add waveform screenshots or architecture visuals here.

---

## Why the Source Code Is Not Public

These projects were completed as part of coursework that may be reused in future semesters. To respect academic integrity and course reuse policies, I am not publishing the source code publicly.

I’m still happy to discuss:
- implementation details
- design decisions
- debugging process
- technical challenges
- tools and technologies used

---

## About Me

I’m a Computer Science senior at the University of San Diego graduating in May 2026. I’m interested in software engineering roles across systems, networking, backend, and data-focused applications.

Other public projects can be found on my GitHub profile, including full-stack, Java, and data science work.

## Contact
- **GitHub:** https://github.com/ethanhaug
- **LinkedIn:** https://www.linkedin.com/in/haugethan/
