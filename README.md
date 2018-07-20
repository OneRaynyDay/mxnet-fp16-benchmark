# mxnet-fp16-benchmark

## Environment info

Running on a p3.8xlarge

```
nvidia-smi:

+-----------------------------------------------------------------------------+
| NVIDIA-SMI 384.130                Driver Version: 384.130                   |
|-------------------------------+----------------------+----------------------+
| GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
| Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
|===============================+======================+======================|
|   0  Tesla V100-SXM2...  Off  | 00000000:00:1B.0 Off |                    0 |
| N/A   46C    P0    53W / 300W |   5100MiB / 16152MiB |      6%      Default |
+-------------------------------+----------------------+----------------------+
|   1  Tesla V100-SXM2...  Off  | 00000000:00:1C.0 Off |                    0 |
| N/A   42C    P0    34W / 300W |     10MiB / 16152MiB |      0%      Default |
+-------------------------------+----------------------+----------------------+
|   2  Tesla V100-SXM2...  Off  | 00000000:00:1D.0 Off |                    0 |
| N/A   39C    P0    37W / 300W |     10MiB / 16152MiB |      0%      Default |
+-------------------------------+----------------------+----------------------+
|   3  Tesla V100-SXM2...  Off  | 00000000:00:1E.0 Off |                    0 |
| N/A   40C    P0    37W / 300W |     10MiB / 16152MiB |      0%      Default |
+-------------------------------+----------------------+----------------------+

+-----------------------------------------------------------------------------+
| Processes:                                                       GPU Memory |
|  GPU       PID   Type   Process name                             Usage      |
|=============================================================================|
|    0     44367      C   /opt/conda/envs/user/bin/python             2152MiB |
|    0     56344      C   /opt/conda/envs/user/bin/python              906MiB |
|    0     61965      C   /opt/conda/envs/user/bin/python             1188MiB |
|    0     79156      C   /opt/conda/envs/user/bin/python              844MiB |
+-----------------------------------------------------------------------------+
```

```
(dockerized)[ray_zhang@i-0555fc08518f7d737 bighead]$ pip freeze | grep mx
You are using pip version 9.0.1, however version 10.0.1 is available.
You should consider upgrading via the 'pip install --upgrade pip' command.
keras-mxnet==2.2.0
mxnet-cu90==1.3.0b20180715
```

```
(dockerized)[ray_zhang@i-0555fc08518f7d737 bighead]$ python --version
Python 3.6.3 :: Intel Corporation
```

```
(dockerized)[ray_zhang@i-0555fc08518f7d737 bighead]$ lsb_release -a
No LSB modules are available.
Distributor ID:	Ubuntu
Description:	Ubuntu 16.04.4 LTS
Release:	16.04
Codename:	xenial
```
