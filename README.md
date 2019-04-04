<meta charset="utf-8">

# Base-Dockerfile

Dockerfile to build my base test environment 🛠 .

## Build

```
# take `base` for example
$> cd base
$> docker build -t base_ubuntu .
```

## Base-Component

- wget✓
- curl✓
- bzip2✓
- unzip✓
- make✓
- gcc/g++ 7.3.0✓ (as of 2019/02/25)
- vim✓
- add-apt-repository✓
	- `python-software-properties` for 12.04
	- `software-properties-common` for 12.10 and above
- man-db✓
- inetutils-ping✓
- net-tools✓
- coreutils✓
- bsdmainutils✓
- tree✓
- screenfetch✓

## Advance_1-Component

- gcc/g++ 4.8.5<!-- ✓ -->
- TBA

## TODO

- [x] Optimize for Chinese ISP.
- [ ] "Advance_1": Base environment with gcc-4.8.5 enabled as primary.
- [ ] "Advance_2": Boost installed on top of "Advance_1" environment.