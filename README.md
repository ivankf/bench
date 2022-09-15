# Bench

## Usage

Disk benchmark for Linux system

1. Benchmark the disk in the current path

```shell
curl -sL https://raw.githubusercontent.com/ivankf/bench/main/iops.sh | bash
```


2. Benchmark the disk on the specified path

```shell
curl -sL https://raw.githubusercontent.com/ivankf/bench/main/iops.sh | bash -s -- <target_path>
```

## What metrics are counted?

```shell
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#                   Disk-Bench-Script                #
#                     v2022-09-13                    #
#           https://github.com/ivankf/bench          #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
Wed Sep 14 23:39:11 EDT 2022
Basic System Information:
---------------------------------
Uptime     : 0 days, 18 hours, 44 minutes
Processor  : Intel(R) Xeon(R) Gold 5218 CPU @ 2.30GHz
CPU cores  : 4 @ 2294.609 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 15.6 GiB
Swap       : 6.4 GiB
Disk       : 57.5 GiB
Distro     : CentOS Linux 7 (Core)
Kernel     : 5.19.8-1.el7.elrepo.x86_64
fio Disk Speed Tests (Mixed R/W 30/70):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
------   | ---            ----  | ----           ----
Read       | 88.68 MB/s   (22.1k) | 148.09 MB/s   (2.3k)
Write      | 207.27 MB/s  (51.8k) | 347.56 MB/s   (5.4k)
Total      | 295.95 MB/s  (73.9k) | 495.66 MB/s   (7.7k)
|                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
------   | ---            ----  | ----           ----
Read       | 140.92 MB/s    (275) | 130.41 MB/s    (127)
Write      | 340.90 MB/s    (665) | 319.23 MB/s    (311)
Total      | 481.82 MB/s    (940) | 449.64 MB/s    (438)
```