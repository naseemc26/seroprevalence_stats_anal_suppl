<h1>Sentinel seroprevalence of Sars-CoV-2 in Gauteng province, South Africa, August - October 2020: Statistical analysis supplement</h1>

<p></p>

The study reports the crude anti-SARS-CoV-2 antibody positivity (seroprevalence) for COVID-19 infection for Gauteng province and then focuses more specifically on the City of Johannesburg district because the bulk of samples were from this district. Since the data was collected non-randomly, using sentinel surveillance, we adjusted the prevalence by using a model-based population weighted framework. 

<p></p>

The multilevel logistic regression with poststratification, generally referred to as Multilevel Regression and Poststratification (MRP) was used (Gelman et al, 2016). The model uses age-sex distributions in each region as weights. The population weights were in 238 age-sex-region strata (17 age categories, 2 sex levels and 7 regions). The sentinel survey used samples from all population age groups. The 2011 Johannesburg population from Census data were used for the poststratification weights. The MLP model was also used to adjust for sensitivity and specificity of the assay (Uyoga et al, 2021; Gelman et al, 2016).

<p></p>

To estimate the stratum seroprevalence we fitted a Bayesian Multilevel Logistic Regression with poststratification that included sex as a fixed effect, and age and region as random effects (Downes et al, 2018; Uyoga et al, 2021). The model was fit in RJags, a package in R version 3.6.3 (Foundation for Statistical Computing, Vienna, Austria). Vague or weakly informative priors were used for all parameters and hyperparameters. The Bayesian Multilevel Logistic regression and poststratification model is implemented in two steps:
<p></p>
<p></p>

![Stats supplement Text with formulae](https://user-images.githubusercontent.com/84568779/133573938-d3a84f4d-06ce-4afc-987c-3bb2a37aaa43.jpg)

<p></p>

<h2>References</h2>

1.	Gelman, A., Lax, J., Phillips, J., Gabry, J., & Trangucci, R. (2016). Using multilevel regression and poststratification to estimate dynamic public opinion. Unpublished manuscript, Columbia University, 2. http://www.stat.columbia.edu/~gelman/research/unpublished/MRT(1).pdf (access date 12 January 2021).
2.	Uyoga, S., Adetifa, I. M., Karanja, H. K., Nyagwange, J., Tuju, J., Wanjiku, P., ... & Warimwe, G. M. (2021). Seroprevalence of anti–SARS-CoV-2 IgG antibodies in Kenyan blood donors. Science, 371(6524), 79-82. https://doi.org/10.1126/science.abe1916
3.	Downes, M., Gurrin, L. C., English, D. R., Pirkis, J., Currier, D., Spittal, M. J., & Carlin, J. B. (2018). Multilevel regression and poststratification: A modeling approach to estimating population quantities from highly selected survey samples. American journal of epidemiology, 187(8), 1780-1790. https://doi.org/10.1093/aje/kwy070
4.	Leeflang, M. M., Rutjes, A. W., Reitsma, J. B., Hooft, L., & Bossuyt, P. M. (2013). Variation of a test's sensitivity and specificity with disease prevalence. CMAJ : Canadian Medical Association journal = journal de l'Association medicale canadienne, 185(11), E537–E544. https://doi.org/10.1503/cmaj.121286
5.	Larremore DB, Fosdick BK, Bubar KM, Zhang S, Kissler SM, Metcalf CJE, et al. (2021). Estimating SARS-CoV-2 seroprevalence and epidemiological parameters with uncertainty from serological surveys. eLife. 1;10: e64206. https://doi.org.10.7554/eLife.64206
