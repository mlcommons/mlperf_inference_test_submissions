*Check [MLC MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: Linux-6.17.0-1013-azure-x86_64-with-glibc2.39
* CPU version: x86_64
* Python version: 3.12.13 (main, Mar  4 2026, 02:26:36) [GCC 13.3.0]
* MLC version: unknown

## MLC Run Command

See [MLC installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U mlcflow

mlc rm cache -f

mlc pull repo mlcommons@mlperf-automations --checkout=1666d59b5a9729c97cd3f384048996a4e8d5c3b4


```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf,
 you should simply reload mlcommons@mlperf-automations without checkout and clean MLC cache as follows:*

```bash
mlc rm repo mlcommons@mlperf-automations
mlc pull repo mlcommons@mlperf-automations
mlc rm cache -f

```

## Results

Platform: gh_ubuntu-latest_x86-mlcommons_cpp-cpu-onnxruntime-default_config

Model Precision: fp32

### Accuracy Results 
`acc`: `76.0`, Required accuracy for closed division `>= 75.6954`

### Performance Results 
`Samples per second`: `23.2674`
