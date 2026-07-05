*Check [MLC MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: macOS-26.4-arm64-arm-64bit-Mach-O
* CPU version: arm
* Python version: 3.13.14 (v3.13.14:fd17997c386, Jun 10 2026, 08:55:00) [Clang 21.0.0 (clang-2100.1.1.101)]
* MLC version: unknown

## MLC Run Command

See [MLC installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U mlcflow

mlc rm cache -f

mlc pull repo amd@mlperf-automations --checkout=13580c087656b8ffdbb7b86fec3bef2b5170fa12


```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf,
 you should simply reload amd@mlperf-automations without checkout and clean MLC cache as follows:*

```bash
mlc rm repo amd@mlperf-automations
mlc pull repo amd@mlperf-automations
mlc rm cache -f

```

## Results

Platform: gh_macos-latest_x86-mlcommons_cpp-cpu-onnxruntime-default_config

Model Precision: fp32

### Accuracy Results 
`acc`: `76.0`, Required accuracy for closed division `>= 75.6954`

### Performance Results 
`Samples per second`: `9.48716`
