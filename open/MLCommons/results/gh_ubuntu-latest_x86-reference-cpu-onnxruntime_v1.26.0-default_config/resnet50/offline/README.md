*Check [MLC MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: Linux-6.17.0-1013-azure-x86_64-with-glibc2.39
* CPU version: x86_64
* Python version: 3.13.13 (main, Apr 30 2026, 14:44:12) [GCC 13.3.0]
* MLC version: unknown

## MLC Run Command

See [MLC installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U mlcflow

mlc rm cache -f

mlc pull repo YasirKhokhar@mlperf-automations --checkout=5a4591957c32a0b91b6d730a45b1737cae4a64d2


```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf,
 you should simply reload YasirKhokhar@mlperf-automations without checkout and clean MLC cache as follows:*

```bash
mlc rm repo YasirKhokhar@mlperf-automations
mlc pull repo YasirKhokhar@mlperf-automations
mlc rm cache -f

```

## Results

Platform: gh_ubuntu-latest_x86-reference-cpu-onnxruntime_v1.26.0-default_config

Model Precision: fp32

### Accuracy Results 
`acc`: `76.0`, Required accuracy for closed division `>= 75.6954`

### Performance Results 
`Samples per second`: `21.0825`
