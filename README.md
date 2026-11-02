# Arduino Projects

Microcontroller experiments connecting small displays, animation, and embedded programming.

**Status: documentation stage.** This repository describes the experiments and their test criteria. Reviewed sketches and hardware demonstrations have not yet been published.

## Project directions

| Experiment | Purpose | Engineering considerations |
| --- | --- | --- |
| OLED animated eyes | Explore expressive display animation for a robotics interface | Frame timing, input handling, state transitions, and idle behavior |
| Rotating tesseract | Explore projecting a four-dimensional object onto a small display | Projection math, numerical limits, clipping, and animation rate |
| Portable display demo | Run a standalone animation from a power source | Startup behavior, reset recovery, and power compatibility |

The intended starting hardware is an Arduino Uno with a small OLED module. The display controller, pixel dimensions, interface, supply requirements, and library versions must be confirmed before a wiring guide or build instructions are released.

## What a sketch release should include

- A complete, reviewed sketch with explicit pin assignments
- Board selection and exact dependency versions
- A wiring diagram for the actual module
- Build instructions and any configurable parameters
- Known limitations, including SRAM and display-buffer use
- Attribution for libraries and reused animation techniques

## Planned verification

1. Compile for the stated board and record warnings and memory use.
2. Confirm reset and startup behavior on the hardware.
3. Measure frame timing and check long-running animation behavior.
4. Exercise input boundaries where input is supported.
5. Record the power source and configuration used for the demonstration.

These checks are planned. No compile result, frame rate, or hardware reliability claim is published yet.

See the [portfolio documentation standards](https://github.com/jackjavo826-source/jackjavo826-source/blob/main/PORTFOLIO_STANDARDS.md).
