---
layout: page
title: Pilot
permalink: /pilot/
---

# The Pilot Framework

Pilot is a framework that is designed for collecting precise benchmark
results in the shortest possible time. This is useful when a designer
or administrator needs to evaluate many candidate parameters. Pilot
analyzes time series data in real time and tells you when the desired
width of confidence interval is reached. Pilot can also automate many
benchmark chores, such as measuring the overhead, detecting warm-up
and tear-down phases, discovering bottlenecks of the system, and
comparing very close benchmark results. Pilot is in BSD 3-clause or
GPLv2+ license, and comes with easy-to-use scriptable and CLI
interfaces with C/C++/Python bindings.

## Just take me to the code!

- [GitHub project](https://github.com/ascar-io/pilot-bench)
- [MASCOTS'16 paper (PDF)](/assets/pdf/pilot-mascots16-final2.pdf)

## Pilot Helps To Answer These Questions

- How long shall I run this benchmark to get a precise result?
- Is my new algorithm really 3% faster than baseline or is that an error?

## Pilot Is Designed To

- help testers who may not have enough statistics knowledge,
- get accurate, precise, repeatable results,
- and get results using the shortest possible time while still meeting statistical requirements.

## Pilot Can Be Used By

- researchers, engineers, testers, users

## Pilot's Function

- can handle statistical stuff so your benchmark results are statistically valid
  - measure and reduce the autocorrelation among samples
  - calculate the confidence interval (CI)
  - use t-distribution to calculate the required number of samples to achieve the desired CI
- can detect (and remove) warm-up and cool-down phases using multiple methods
- can compare benchmarks that have very close results
- is optimized to get results using the shortest time (for both measurement and comparison)
- provides many easy-to-use interfaces
- is extensible through plug-ins
- and more!

## Publication

Our [MASCOTS'16 paper](/assets/pdf/pilot-mascots16-final2.pdf) contains
technical details of Pilot. See also the related SC17 materials:
[paper](/assets/pdf/li-capes-sc17.pdf) ·
[slides](/assets/pdf/li-capes-sc17-slides.pdf).

## Acknowledgments

Pilot was a research project from the [Storage Systems Research
Center](http://www.ssrc.ucsc.edu/) at [UC Santa
Cruz](http://ucsc.edu/) from 2015 to 2016. This research was supported
in part by the National Science Foundation under awards IIP-1266400,
CCF-1219163, CNS-1018928, CNS-1528179, by the Department of Energy
under award DE-FC02-10ER26017/DESC0005417, by a Symantec Graduate
Fellowship, by a [grant from Intel
Corporation](https://software.intel.com/en-us/articles/intel-parallel-computing-center-baskin-school-of-engineering-at-uc-santa-cruz),
and by industrial members of the Center for Research in Storage
Systems.

This project does not reflect the opinion or endorsement of the
sponsors listed above.
