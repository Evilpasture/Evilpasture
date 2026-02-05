I’m a Data Science undergrad who spends a lot of time in Python's C API. I like making Python fast by offloading the heavy lifting to C and modern hardware. (totally not obsessed)

### Current status

#### [Culverin](https://github.com/Evilpasture/Culverin)
A Jolt Physics wrapper for Python that focuses on **memory-mapped performance**.
- **The Pitch:** Most wrappers are slow because they copy data. This one uses C shadow buffers to let you read 10,000 objects in 0.02ms.
- **Modern Features:** It's built for **Python 3.13t (Free-Threaded)**. It releases the GIL so physics and logic actually run on different cores.
- **Truth:** I don't really know C++, so I wrote a C wrapper for the C++ parts and spent 3 days fighting CMake until it worked on Windows/Linux/macOS.

#### [HyperGL](https://github.com/Evilpasture/HyperGL)
A heavily refactored fork of **ZenGL**, revamped for AZDO, compute shading, SSBO, etc. and Free-Threaded Python.
- **What changed:** I took the core of ZenGL and stripped it down to support **Approaching Zero Driver Overhead (AZDO)** workflows and bindless textures. Only took a few extra thousands of lines and a very, very cruciating C development where I have to merge with an old working version and a broken new version.
- **Thread Safety:** Rewrote the context management to handle multi-threaded migrations for Python's new no-GIL mode.

---

### Technical Survival Skills
- **Languages:** Python, C (and enough C++ to get Jolt to compile).
- **Specialties:** Python C-Extensions, memoryview tricks, and some low-level OpenGL (AZDO/Bindless).
- **Tools:** CMake (I brute-forced it), GitHub Actions (for cross-platform wheels), and NumPy.

### AI usage
I use AI. Extensively. But I'm not the type of person to just let an IDE open and somehow it codes for you like magic. It's just as time-consuming to fix bugs AI left for you to fix like a puzzle, except that said puzzles are hiding right underneath my nose. It's still a force multiplier, though... and I do think it makes things that used to be "impossible" for me now becomes plausible. Like my projects above.

### Currently learning
- Better ways to handle concurrency in Python 3.14.
- Half-trying on learning how C++ actually works so I don't have to keep being stupid. (will never touch C++ for real)
- Building a game engine using Culverin + HyperGL.

### Contacts
I have a Discord account. My handle is "enwifi". This is probably where I will 99% get in touch.
