# How does traffic emissions affect Air quality in Europe

## A model comparison across chemical complexity

Contact: <august.thomasson@fysik.lu.se>

This is a repository used to showcase results from a model comparison of traffic emissions effect on air quality in Europe. This is a project within the Horizon Europe project PAREMPI [parmepi.eu].

---

## Introduction & Method

- Traffic emission cause complex non-linear effects on atmospheric chemistry
- Therefore, it is unclear how traffic emissions affect air quality in Europe
- We utilize two different models to quantity the effect of traffic emissions and to understand how the model chemical complexity affect the conclusions.
- Each model is run for 2018 with and without traffic emissions

**TM5-MP - Global Eularian Model**

- Reduced chemstry and aersol dynamics
- Novel SOA formation from anthropogenic VOCs
- Ammonia-sulfuric acid NPF included

**ADCHEM - Lagrangian column model**

- Near explicit chemistry and detailed aerosol dynamics
- 25 000 trajectories remapped to annual grid

---

## Key takeaways

- ~10 % PM2.5 and ~5% PN from traffic in Europe
- NO3 and NH4 dominate the mass
- Largest impact in urban areas and during winter
- Higher chemically complexity captures more non-linear effects

---

## Model evaluation

The models match observed concentrations of several tracers well. We evaluate with normalized Mean Absolute Error and Pearson’s correlation coefficient of yearly average concentration for all available sites in Europe. The difference in the model can be attributed to both differences in chemical complexity and emission inventory used. TM5 perform best against PM2.5 measurements (nMAE = 0.18, r = 0.81, N = 41), BC (nMAE = 0.46, r = 0.56, N = 34), NO3 (nMAE = 0.44, r = 0.86, N = 22) and NH4 (nMAE = 0.45, r = 0.86, N= 19), while ADCHEM recover observed OA (nMAE = 0.33, r = 0.83, N= 20) and particle size distributions better.

---

## Results

### Seasons PM2.5 from TM5-MP

**Traffic PM2.5**
![season_PM25_tm5](figures/TM5/season_PM25_tm5.png)

**NO3+NH4**
![season_SIA_tm5](figures/TM5/season_SIA_tm5.png) 

**BC+POA**
![season_Primary_tailpipe_tm5](figures/TM5/season_Primary_tailpipe_tm5.png)

**Non-exhaust emissions**
![season_NEE_tm5](figures/TM5/season_NEE_tm5.png)

**SOA**
![season_SOA_tm5](figures/TM5/season_SOA_tm5.png)

---

### Traffic PM2.5 mean for 2018 and its components

**Traffic PM2.5**
![](figures/TM5/map_PM25_tm5.png) 
![](figures/ADCHEM/map_PM25_adchem.png)

**NO3 + NH4**
![](figures/TM5/map_SIA_tm5.png)  
![](figures/ADCHEM/map_SIA_adchem.png)

**POA + BC**
![](figures/TM5/map_Primary_tailpipe_tm5.png) 
![](figures/ADCHEM/map_Primary_tailpipe_adchem.png)

**Non-exhaust emissions**
![](figures/TM5/map_NEE_tm5.png) 
 ![](figures/ADCHEM/map_NEE_adchem.png)

**Secondary Organic Aerosols**
![](figures/TM5/map_SOA_tm5.png)  
![](figures/ADCHEM/map_SOA_adchem.png)

**Others, mostly seasalt**
![](figures/TM5/map_Others_tm5.png) 
 ![](figures/ADCHEM/map_Others_adchem.png)

---

### Traffic Particle Number median for 2018

**All Particle number**
![](figures/TM5/map_PN_tm5.png)  
![](figures/ADCHEM/map_PN_adchem.png)

**Ultra-fine Particles**
![](figures/TM5/map_UFP_tm5.png) 
![](figures/ADCHEM/map_UFP_adchem.png)

---
