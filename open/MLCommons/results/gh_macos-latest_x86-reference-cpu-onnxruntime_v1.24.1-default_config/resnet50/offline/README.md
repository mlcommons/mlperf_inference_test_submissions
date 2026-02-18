*Check [MLC MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: macOS-15.7.3-arm64-arm-64bit-Mach-O
* CPU version: arm
* Python version: 3.13.12 (v3.13.12:1cbe4818347, Feb  3 2026, 13:36:53) [Clang 16.0.0 (clang-1600.0.26.6)]
* MLC version: unknown

## MLC Run Command

See [MLC installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U mlcflow

mlc rm cache -f

mlc pull repo rafalop@mlperf-automations --checkout=a6860f916adc2f68ce6fe1a14d384f36be7c9c38


```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf,
 you should simply reload rafalop@mlperf-automations without checkout and clean MLC cache as follows:*

```bash
mlc rm repo rafalop@mlperf-automations
mlc pull repo rafalop@mlperf-automations
mlc rm cache -f

```

## Results

Platform: gh_macos-latest_x86-reference-cpu-onnxruntime_v1.24.1-default_config

Model Precision: fp32

### Accuracy Results 
`acc`: `76.0`, Required accuracy for closed division `>= 75.6954`

### Performance Results 
`Samples per second`: `12.8007`
