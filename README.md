# GW151226_samples
Posterior samples for the GW151226 binary black hole event described in [arxiv:2105.06486](https://arxiv.org/abs/2105.06486): "Signs of higher multipoles and orbital precession in GW151226".

The default parameter estimation samples are found in ```GW151226_IASprior.pkl```, whereby the effects of orbital precession and higher order radiative multipoles are included in the likelihood evaluation in the ```IMRPhenomXPHM``` waveform model [(arxiv:2004.06503)](https://arxiv.org/abs/2004.06503). ```GW151226_IASprior_noHM.pkl``` and ```GW151226_IASprior_noPre.pkl``` contain the samples where the higher multipoles and orbital precession are disabled respectively. In the three cases above, the spin prior is uniform in $`\chi_{\rm eff}`$. For ```GW151226_LVCprior.pkl``` the spin prior is isotropic in spin components and uniform in component spin magnitudes, while the effects or orbital precession and higher multipoles are included in the likelihood evaluation.

The data is contained in ```pandas.DataFrame```, with the column names defined as follows:  

```mchirp```: detector frame chirp mass  
```mchirp_source```: source frame chirp mass  
               ```mtot```: detector frame total mass  
               ```mtot_source```: source frame total mass  
               ```m1```: detector frame primary mass  
               ```m2```: detector frame secondary mass  
               ```m1_source```: source frame primary mass  
               ```m2_source```: source frame secondary mass  
               ```q```: mass ratio,  
               ```d_luminosity```: luminosity distance (Mpc)  
               ```d_comoving```: comoving distance (Mpc)  
               ```z```: redshift  
               ```chieff```: effective aligned spin  
               ```s1x```: x spin component of primary component  
               ```s1y```: y spin component of primary component  
               ```s1z```: z spin component of primary component  
               ```s2x```: x spin component of secondary component  
               ```s2y```: y spin component of secondary component  
               ```s2z```: z spin component of secondary component  
               ```ra```: right ascension (rad)  
               ```de```': declination (rad)  
               ```psi```: polarization phase (rad)  
               ```vphi```: orbital Phase (rad)  
               ```iota```: inclination (rad)  
               ```tgps_geocenter```: GPS time (s) at geocenter  
               ```tgps_H```: GPS time at Hanford  
               ```tgps_L```: GPS time at Livingston  
               ```tgps_V```: GPS time at Virgo  
               ```f_ref```: reference frequency (Hz)  
               ```f_lo```: minimum frequency (Hz)  
               ```f_hi```: maximum frequency (Hz)  
               ```lnl```: log likelihood  
               ```lnl_aux_H```: Hanford log likelihood  
               ```lnl_aux_L```: Livingston log likelihood  
               ```lnl_aux_V```: Virgo log likelihood  
               ```asd_drift_H```: Hanford amplitude spectral density drift correction  
               ```asd_drift_L```: Livingston amplitude spectral density drift correction  
               ```asd_drift_V```: Virgo Aaplitude spectral density drift correction
