# Zhussup

Systems programmer focused on high-performance computing and computational
science: fast native cores, decoupled architecture, honest benchmarks.

I build systems in layers — a headless simulation daemon with independent
terminal and graphical clients on top of one snapshot protocol, a C++ compute
core with an ergonomic Python layer above it — and profile the hot paths down
to the assembly level.

## Focus

- **High-performance C++ (C++20) and C** — memory layout, SIMD, CUDA; profiling hot paths with GDB and perf on Linux.
- **Architecture** — decoupled multi-process designs: daemons over IPC, independent UI clients, strict module boundaries, API/ABI as a deliberate interface.
- **Native × Python interop** — C/C++ cores exposed to Python through the C-API.
- **Scientific computing** — computational biology, physics simulation, compiler analysis.

## Selected work

- **[BioFasting](https://github.com/Zhussup/BioFasting)** — a C++ core for FASTQ/FASTA and sequence ops, built to close the 7–10× gap Biopython leaves on hot paths. SIMD-dispatched native parsing and `libdeflate` for compressed data underneath an ergonomic Python API — the *numpy layer* of bioinformatics.
- **[rocketlab](https://github.com/Zhussup/rocketlab)** — an open-source spaceflight sandbox in C++20. The simulator is a headless daemon; the terminal dashboard (FTXUI) and the graphical map view (ImGui/GLFW) are independent clients over the same snapshot protocol. Assemble rockets, write their flight software in Lua.
- **[ProteinGPU-Studio](https://github.com/Zhussup/ProteinGPU-Studio)** — in-silico protein mutagenesis backed by real structure prediction (OmegaFold), with an honest CPU vs GPU benchmark.
- **[decay_chain_simulator](https://github.com/Zhussup/decay_chain_simulator)** — radioactive decay physics: event-driven Monte-Carlo simulation overlaid with the analytic Bateman solution; the curves matching is the physical validation of both models.
- **[kind_picture](https://github.com/Zhussup/kind_picture)** — given a compiler listing, recover C that behaves the same — and prove it mechanically.

**Languages:** C++20 · C · Python · CUDA · x86-64 assembly
**Tooling:** Linux · CMake · GDB · perf · Catch2

---

Reach me: [@Zhussup](https://github.com/Zhussup) · Codewars: [![](https://www.codewars.com/users/Zhussup/badges/micro)](https://www.codewars.com/users/Zhussup)
