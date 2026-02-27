*Check [MLC MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: Linux-6.14.0-1017-azure-x86_64-with-glibc2.39
* CPU version: x86_64
* Python version: 3.13.12 (main, Feb  4 2026, 13:48:12) [GCC 13.3.0]
* MLC version: unknown

## MLC Run Command

See [MLC installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U mlcflow

mlc rm cache -f

mlc pull repo amd@mlperf-automations --checkout=183369cf11d61f41d3477d3ee4e8492d7363caec


```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf,
 you should simply reload amd@mlperf-automations without checkout and clean MLC cache as follows:*

```bash
mlc rm repo amd@mlperf-automations
mlc pull repo amd@mlperf-automations
mlc rm cache -f

```

## Results

Platform: gh_ubuntu-latest_x86-mlcommons_cpp-cpu-onnxruntime-default_config

Model Precision: fp32

### Accuracy Results 
`acc`: `76.0`, Required accuracy for closed division `>= 75.6954`

### Performance Results 
`Samples per second`: `23.094`
