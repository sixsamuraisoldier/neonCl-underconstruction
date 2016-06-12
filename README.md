# What's this branch?

This is a port in progress of nervana neon Kepler convolution kernels to OpenCL.

The original neon, documentation etc is at https://github.com/nervanasystems/neon

## How to run something with it?

Test code is at:
- [test_perf.py](test_perf.py)  For timings
- [test_correctness.py](test_correctness.py)   For fprop correctness
- [test_correctness_bprop.py](test_correctness_bprop.py)    For gradInput backprop correctness

## Plan

It's a port of neon convolutions to OpenCL (in progress)

## Status

Latest news:
- fprop is working!
- backprop gradInputs is working!

Next steps, in no particular order:
- port also backprop weights
- port dim_shuffle (?)
- migrate everything to opencl (ie remove the insane cuda-cpu-cl copying currently involved in running
cl kernels against cuda buffers...)

## License

Apache 2.0, per original neon

