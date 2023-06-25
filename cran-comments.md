# CRAN submission ACNE 0.9.0

on 2023-06-215

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
── ACNE 0.8.1-9004: OK

  Build ID:   ACNE_0.8.1-9004.tar.gz-f8aaff4e18bc417b949d721859e2b781
  Platform:   Debian Linux, R-devel, clang, ISO-8859-15 locale
  Submitted:  12m 28.1s ago
  Build time: 12m 11.6s

0 errors ✔ | 0 warnings ✔ | 0 notes ✔

── ACNE 0.8.1-9004: OK

  Build ID:   ACNE_0.8.1-9004.tar.gz-4366037b9cbc417ca37e0cb8d50a042b
  Platform:   Fedora Linux, R-devel, GCC
  Submitted:  12m 28.1s ago
  Build time: 8m 18.9s

0 errors ✔ | 0 warnings ✔ | 0 notes ✔

── ACNE 0.8.1-9004: OK

  Build ID:   ACNE_0.8.1-9004.tar.gz-42b70d71f7354077abecce5cb4ac0bbf
  Platform:   Debian Linux, R-patched, GCC
  Submitted:  12m 28.1s ago
  Build time: 11m 21.3s

0 errors ✔ | 0 warnings ✔ | 0 notes ✔

── ACNE 0.8.1-9004: WARNING

  Build ID:   ACNE_0.8.1-9004.tar.gz-c7130b3147094f148f97757949a785fa
  Platform:   Windows Server 2022, R-release, 32/64 bit
  Submitted:  12m 28.1s ago
  Build time: 4m 6.7s

❯ checking whether package 'ACNE' can be installed ... WARNING
  See below...

0 errors ✔ | 1 warning ✖ | 0 notes ✔

── ACNE 0.8.1-9004: NOTE

  Build ID:   ACNE_0.8.1-9004.tar.gz-f58076e6c3ce4de7ad4c7d5c9040d43b
  Platform:   Windows Server 2022, R-devel, 64 bit
  Submitted:  12m 28.1s ago
  Build time: 2m 54s

❯ checking package dependencies ... NOTE
  Package suggested but not available for checking: 'DNAcopy'

0 errors ✔ | 0 warnings ✔ | 1 note ✖
```
