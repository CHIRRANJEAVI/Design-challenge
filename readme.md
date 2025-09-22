Project proposal: evaluating Microwatt CPU as a measurement-type CPU

We propose a reproducible study to evaluate the Microwatt open-source Power ISA core as the on-chip “lab controller” for silicon measurements. Many SoC projects need a small, dependable CPU to configure peripherals, sweep stimuli, log data, and orchestrate verification loops. Microwatt is a serious contender because it is auditable, and actively maintained. Our goal is to determine if it delivers the best balance of ease-of-integration, performance, and resource cost for measurement-heavy chips.
Method: we integrate Microwatt with a tiny reconfigurable logic block (a LUT/PLA “logic sandbox”) and a set of fixed standard-cell reference blocks on SKY130. Microwatt runs bare-metal code that programs the sandbox, applies vectors, timestamps operations, and records outputs. We compare fabric versus fixed implementations and profile the CPU’s own overhead. Metrics include area, timing (Fmax/latency), power and energy per operation, bring-up friction, and developer effort (scripts, LOC, prompt logs).
Why do this: teams repeatedly reinvent test controllers. If Microwatt proves fast to bring up, and measurement-friendly, it can become a standard for open silicon projects. Deliverables include RTL, testbenches, OpenLane results, a how-to video.

Clarence Luo, Chirranjeavi Moorthi
9/21/2025
