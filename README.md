# RISC-V Cheat Sheet on ISA naming convention of Extension and Acronyms

Notes of acronyms of RISC-V ISA.

## Register size (expressed as XLEN in spec)

| Base Name | Length Register (XLEN) |
| --- | --- |
| RV32   | 32bit register length |
| RV64   | 64bit register length |
| RV128  | 128bit register length |


## Supported ISA

| Extension Name | Detail Description
| --- | --- |
| I  | Addition and Subtraction Arithmetic only on Integer (Mandatory) |
| M  | Multiplication and Division Arithmetic only on Integer |
| F  | FP32 (float) Single precision floating point arithmetic |
| D  | FP64 (double) double precision floating point arithmetic |
| A  | Atomic Instructions |
| G  | Combination of IMAFD above |
| C  | Adds 16bit length Compressed Instructions |
| H  | Adds Hypervisor  |
| B  | Adds Bit Manipulation |
| P  | Adds Traditional SIMD instruction |
| V  | Adds Vector Operations |
| Q  | Adds Quad (128bit) precision floating point arithmetic |


## Supported MMU (number of virtual address bits, mandatory to run Linux)

| Virtual Memory (MMU) | Size of Virtual address |
| --- | --- |
| none | No MMU |
| Sv32 | 32bit address (4 GB) |
| Sv39 | 39bit address (512 GB) |
| Sv48 | 48bit address (256 TB) |
| Sv57 | 57bit address (128 PB) |

## Examples,

A typical combination for running OS requires MMU.
[For Linux capability]

  RV64GCsv39

Many of single core RISC-V microcontrollers do not have float.
[For bare metal programming or RTOS]

  RV32IM

Many of multi core RISC-V microcontrollers do not have float.
[For bare metal programming or RTOS]

  RV32IMA
