*Check [MLC MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: Linux-6.17.0-1018-azure-x86_64-with-glibc2.39
* CPU version: x86_64
* Python version: 3.12.13 (main, Jun 16 2026, 22:05:08) [GCC 13.3.0]
* MLC version: unknown

## MLC Run Command

See [MLC installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U mlcflow

mlc rm cache -f

mlc pull repo DeepakP-amd@mlperf-automations --checkout=c728b364bcba773744895c46dc5fb6bcee9fa5bf


```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf,
 you should simply reload DeepakP-amd@mlperf-automations without checkout and clean MLC cache as follows:*

```bash
mlc rm repo DeepakP-amd@mlperf-automations
mlc pull repo DeepakP-amd@mlperf-automations
mlc rm cache -f

```

## Results

Platform: gh_ubuntu-latest_x86-reference-cpu-tf_v2.21.0-default_config

Model Precision: fp32

### Accuracy Results 
`acc`: `76.0`, Required accuracy for closed division `>= 75.6954`

### Performance Results 
`Samples per second`: `28.3584`
