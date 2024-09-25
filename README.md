# Measuring the Distance to the Large Magellanic Cloud using Cepheid Variables

## Summary
In this project, I used astronomical data from the Gaia mission and OGLE light curves to calculate the distance to a nearby galaxy. This required extensive Python analysis and SQL queries into the databases. For the full report, read this [pdf](https://nbviewer.org/github/kylesoni/calculating-distance-to-the-lmc/blob/main/annotated-ASTRON_321_final_report.pdf). I also provided the abstract below and an example figure from the paper.

## Abstract
The Large Magellanic Cloud (LMC) is a nearby satellite galaxy of the Milky Way. Measuring its distance from Earth is important for understanding the broader structure of the universe and how galaxies interact. Since the LMC contains many Cepheid variables, the fixed period-luminosity (P-L) relationship of Cepheids is useful in calculating this distance. 

To calibrate this relationship, I used parallax measurements from the Gaia mission to find distances to Cepheids in the galactic disk. I then used light curves from the Optical Gravitational Lensing Experiment (OGLE) to find the pulsation period (via Lomb-Scargle) and apparent magnitudes of these Cepheids, successfully calibrating the P-L relationship as $M = (-2.15 \pm 0.04) \log(P) + (-2.35 \pm 0.01)$, where $M$ is absolute magnitude and $P$ is period. Using OGLE light curves from LMC Cepheids, I found their pulsation periods, allowing me to calculate their absolute magnitudes as well. 

Combining this with the apparent magnitude data from OGLE yielded distance measurements for these stars. The median of these measurements was 41.24 $\pm$ 2.23 kiloparsec (kpc), showing that the distance to the LMC is comparable to the size of the Milky Way.

![alt text](https://github.com/kylesoni/calculating-distance-to-the-lmc/blob/main/figures/fig1.png)

Graphical representation of calibrated Period-Luminosity relation. The fitted line follows equation $M = (−2.15 ± 0.04) \log(P) + (−2.35 ± 0.01)$.
