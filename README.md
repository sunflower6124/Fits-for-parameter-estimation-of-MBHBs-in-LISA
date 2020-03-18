# Analytic parameter estimation for MBHBs in LISA

This repository is intended to contain the data presented in the work arXiv: (insert link) with an additional tutorial to show how these data can be used. <br />
The repository contains several folders and .tar:

## 1. The folder `data` 
contains the median, 68\% and 95\% uncertainties for:
- Sky position <img src="https://render.githubusercontent.com/render/math?math=\Delta \Omega \, [deg^2]"> ('skyloc.txt')
- Luminosity distance <img src="https://render.githubusercontent.com/render/math?math=\Delta{d_L/d_L}" >  ('dl.txt')
- Chirp mass <img src="https://render.githubusercontent.com/render/math?math=\Delta\mathcal{M}/\mathcal{M}"> ('mchirp.txt')
- Mass-ratio <img src="https://render.githubusercontent.com/render/math?math=\Delta{q/q}"> ('mass_ratio.txt')
- S/N ('SNR.txt')
    
assuming the standard LISA sensitivity curve, as described in Sec.II of (link to arxiv). Refer to the file with ' *_degraded.txt ' for the same quantites computed with the degraded LISA sensitivity. <br />
We report the values at 7 times from coalescence: 1 month, 1 week, 3 days, 1 day, 10 hours, 5 hours and 1 hour.
For the <img src="https://render.githubusercontent.com/render/math?math=\Delta \Omega"> and <img src="https://render.githubusercontent.com/render/math?math=\Delta{d_L/d_L}" > uncertainties we report also the uncertainties at the merger obtained from eq. (12-13). We provide also the S/N for the full signal. <br />
The files 'skyloc.txt', 'dl.txt', 'SNR.txt' are organized in 42 columns as follow: <br />
log10(mtot/msun) - redshift - median (1 month) - median (1 week) -  ... median (1 hour) - median (merger) - 68% lower (1 month)  - ... - 68% lower (merger) - 68% upper (1 month) - ... - 68% upper (merger) - 95% lower (1 month)  ... - 95% lower (merger) - 95% upper (1 month) - ... - 95% upper (merger) 

The files 'mchirp.txt' and 'mass_ratio.txt' are organized in the same way withour the 'merger' columns, i.e. they have 37 columns

## 2. The folder `fits`
contains modules where we already implemented the fits. The names shoudl be self-explanatory. 
however we notice that `the area uncertainties provided by the corresponding formula are in steradians`.

## 3. the `distribution.tar` and `distribution_degr.tar`
contain the <img src="https://render.githubusercontent.com/render/math?math=\Delta \Omega \, [deg^2]">, <img src="https://render.githubusercontent.com/render/math?math=\Delta{d_L/d_L}" >, <img src="https://render.githubusercontent.com/render/math?math=\Delta\mathcal{M}/\mathcal{M}">, <img src="https://render.githubusercontent.com/render/math?math=\Delta{q/q}"> and S/N distribution for the whole set of parameters explored at different time from coalescence.  <br />


