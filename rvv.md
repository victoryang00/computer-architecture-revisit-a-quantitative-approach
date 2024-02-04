# Is VLIW view of commiting the GPU good or bad?
Why RISC-V Vector Extension is VLIW? Let's see the operand. It requires we set some MSR register before we launch a bunch of kernel to the Vector Unit. The control flow is more like lunching cuda kernels with added GPU context like blocks and SM parameters. The Vector Unit implemented in the BOOMv3 is using a accelerator protocol called RoCC, which is a VLIW-like protocol. // shall use two 

# Tenstorrent way of dealing RISC-V Vector Extension

## Reference
1. [BOOMv3 RoCC](https://github.com/riscv-boom/riscv-boom)
2. [Tenstorrent Vector Engine](https://www.youtube.com/watch?v=H253qdZjbhQ)