*Check [MLC MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: macOS-15.7.4-arm64-arm-64bit-Mach-O
* CPU version: arm
* Python version: 3.13.12 (v3.13.12:1cbe4818347, Feb  3 2026, 13:36:53) [Clang 16.0.0 (clang-1600.0.26.6)]
* MLC version: unknown

## MLC Run Command

See [MLC installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U mlcflow

mlc rm cache -f

mlc pull repo amd@mlperf-automations --checkout=3d6508fa9ecaba958354d71680f64b3a0e58492a


```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf,
 you should simply reload amd@mlperf-automations without checkout and clean MLC cache as follows:*

```bash
mlc rm repo amd@mlperf-automations
mlc pull repo amd@mlperf-automations
mlc rm cache -f

```

## Results

Platform: gh_macos-latest_x86-reference-cpu-onnxruntime_v1.24.3-default_config

Model Precision: fp32

### Accuracy Results 
`acc`: `76.0`, Required accuracy for closed division `>= 75.6954`

### Performance Results 
`Samples per second`: `12.667`
