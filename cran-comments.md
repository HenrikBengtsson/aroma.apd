# CRAN submission aroma.apd 0.6.1

on 2022-07-18

This submission addresses Rd issues detected by R-devel.

Thanks in advance


## Notes not sent to CRAN

### R CMD check validation

The package has been verified using `R CMD check --as-cran` on:

| R version     | GitHub | R-hub    | mac/win-builder |
| ------------- | ------ | -------- | --------------- |
| 4.0.x         | L      |          |                 |
| 4.1.x         | L M W  |          |                 |
| 4.2.x         | L M W  | . M M1 . | M1 W            |
| devel         | L M W  | .        |    W            |

*Legend: OS: L = Linux, M = macOS, M1 = macOS M1, W = Windows*


R-hub checks:

```r
res <- rhub::check(platform = c(
#  "debian-clang-devel", "debian-gcc-patched", "linux-x86_64-centos-epel",
  "macos-highsierra-release-cran", "macos-m1-bigsur-release"
#  "windows-x86_64-release"
))
print(res)
```

gives

```
── aroma.apd 0.6.1: OK

  Build ID:   aroma.apd_0.6.1.tar.gz-0eeba727283a4bb09f15627beeff4fcf
  Platform:   macOS 10.13.6 High Sierra, R-release, CRAN's setup
  Submitted:  2m 4.2s ago
  Build time: 1m 12.8s

0 errors ✔ | 0 warnings ✔ | 0 notes ✔

── aroma.apd 0.6.1: OK

  Build ID:   aroma.apd_0.6.1.tar.gz-9a2ff9276a744ce6b9984c8ee00661ad
  Platform:   Apple Silicon (M1), macOS 11.6 Big Sur, R-release
  Submitted:  2m 4.3s ago
  Build time: 1m 40.4s

0 errors ✔ | 0 warnings ✔ | 0 notes ✔
```
