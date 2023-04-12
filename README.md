# RISC-V Acronyms

Notes of acronyms of RISC-V ISA.

## Register size (expressed as XLEN in spec)

| | |
| --- | --- |
| RV32   | 32bit register length |
| RV64   | 64bit register length |
| RV128  | 128bit register length |


## Supported ISA

| | |
| --- | --- |
| I  | Has  ISA for only Addition and Subtraction only on Integer |
| M  | Adds ISA for only Multiplication and Division only on Integer |
| F  | Adds ISA for calculating Single-Precision Floating-Point (32bit) |
| D  | Adds ISA for calculating Double-Precision Floating-Point (64bit) |
| A  | Adds ISA for Atomic Instructions |
| G  | Combining IMAFD above |
| C  | Adds ISA for Compressed Instructions |
| H  | Adds ISA for Hypervisor |
| B  | Adds ISA for Bit Manipulation |
| V  | Adds ISA for Vector Operations |


## Supported MMU (number of virtual address bits, mandatory to run Linux)

| | |
| --- | --- |
| Sv32 | 32bit address bits |
| Sv39 | 39bit address bits |
| Sv48 | 48bit address bits |

## Examples,

Typical combination for running Linux.

  RV64GCsv39

Many of single core RISC-V microcontrollers which do not have float.

  RV32IM

Many of multi core RISC-V microcontrollers which do not have float.

  RV32IMA
