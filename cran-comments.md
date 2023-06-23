# CRAN submission aroma.apd 0.7.0

on 2023-06-21

Thanks in advance


## Notes not sent to CRAN

### R CMD check validation

The package has been verified using `R CMD check --as-cran` on:

| R version     | GitHub | R-hub | mac/win-builder |
| ------------- | ------ | ----- | --------------- |
| 4.1.x         | L      |       |                 |
| 4.2.x         | L M W  |       |                 |
| 4.3.x         | L M W  | L . W | M1 W            |
| devel         | L M W  | L   W |    W            |

*Legend: OS: L = Linux, M = macOS, M1 = macOS M1, W = Windows*


R-hub checks:

```r
res <- rhub::check(platforms = c(
  "debian-clang-devel", 
  "fedora-gcc-devel",
  "debian-gcc-patched", 
  "windows-x86_64-release",
  "windows-x86_64-devel"
))
print(res)
```

gives

```

── aroma.apd 0.6.1-9001: OK

  Build ID:   aroma.apd_0.6.1-9001.tar.gz-335761c136af4df884d50021abd4c384
  Platform:   Debian Linux, R-devel, clang, ISO-8859-15 locale
  Submitted:  7m 28.3s ago
  Build time: 6m 15.5s

0 errors ✔ | 0 warnings ✔ | 0 notes ✔

── aroma.apd 0.6.1-9001: OK

  Build ID:   aroma.apd_0.6.1-9001.tar.gz-1a077969e0324d8f9602087b9acc3b65
  Platform:   Fedora Linux, R-devel, GCC
  Submitted:  7m 28.3s ago
  Build time: 5m 43.4s

0 errors ✔ | 0 warnings ✔ | 0 notes ✔

── aroma.apd 0.6.1-9001: OK

  Build ID:   aroma.apd_0.6.1-9001.tar.gz-9c07be858d9345828bb8b8a3296b73c8
  Platform:   Debian Linux, R-patched, GCC
  Submitted:  7m 28.3s ago
  Build time: 6m 27.6s

0 errors ✔ | 0 warnings ✔ | 0 notes ✔

── aroma.apd 0.6.1-9001: OK

  Build ID:   aroma.apd_0.6.1-9001.tar.gz-66b994a6e1d442c3b379d3f9d0321516
  Platform:   Windows Server 2022, R-release, 32/64 bit
  Submitted:  7m 28.3s ago
  Build time: 3m 5.4s

0 errors ✔ | 0 warnings ✔ | 0 notes ✔

── aroma.apd 0.6.1-9001: NOTE

  Build ID:   aroma.apd_0.6.1-9001.tar.gz-725c53cb415f4df18c705909420fb547
  Platform:   Windows Server 2022, R-devel, 64 bit
  Submitted:  7m 28.3s ago
  Build time: 2m 57.1s

❯ checking package dependencies ... NOTE
  Package suggested but not available for checking: 'affxparser'

❯ checking Rd cross-references ... NOTE
  Package unavailable to check Rd xrefs: 'affxparser'

0 errors ✔ | 0 warnings ✔ | 2 notes ✖
```
