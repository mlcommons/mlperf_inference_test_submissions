*Check [MLC MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: Linux-6.17.0-1015-azure-x86_64-with-glibc2.39
* CPU version: x86_64
* Python version: 3.13.13 (main, Apr 30 2026, 14:44:12) [GCC 13.3.0]
* MLC version: unknown

## MLC Run Command

See [MLC installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U mlcflow

mlc rm cache -f

mlc pull repo mlcommons@mlperf-automations --checkout=b0fe3b0c241d5c095955751f6eef373cbdf27e47


```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf,
 you should simply reload mlcommons@mlperf-automations without checkout and clean MLC cache as follows:*

```bash
mlc rm repo mlcommons@mlperf-automations
mlc pull repo mlcommons@mlperf-automations
mlc rm cache -f

```

## Results

Platform: gh_ubuntu-latest_x86-reference-cpu-tf_v2.21.0-default_config

Model Precision: fp32

### Accuracy Results 
`acc`: `76.0`, Required accuracy for closed division `>= 75.6954`

### Performance Results 
`Samples per second`: `28.3454`
