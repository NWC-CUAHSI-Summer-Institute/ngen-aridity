## Tables:
#### Table S1: Parameter configuration used for CFE calibration

| Parameter Name | Unit | Definition | Lower Calibration Parameter Range | Upper Calibration Parameter Range |
| :------------: | :--: | :--------: | :-------------------------------: | :-------------------------------: | 
| bb | (-) | Exponent on Clapp-Hornberger (1978) function | 0 | 21.94 | 
| smcmax | m^3/m^3 | Maximum soil moisture content | 0.20554 | 1 | 
| satdk | m/hr | Saturated hydraulic conductivity | 0 | 0.000726 | 
| slop | (-) | Slope coefficient | 0 | 1 | 
| max_gw_storage | m | Max groundwater storage | 0.01 | 0.25 | 
| expon | (-) | A primary groundwater nonlinear reservoir exponential constant | 1 | 8 | 
| Cgw | m/hr | A primary groundwater nonlinear reservoir constant | 1.8e-6 | 1.8e-3 | 
| K_lf | (-) | Lateral flow coefficient | 0 | 1 | 
| K_nash | (-) | Nash cascade discharge coefficient | 0 | 1 | 

#### Table S2: Parameters and attributes included in differentiable LGAR

| Parameter Name | Unit | Definition | 
| :------------: | :--: | :--------: |
| $\alpha$ | cm^-1 | Van Genuchten parameter representing the inverse of air-entry| 
| n | m3/m3 | Van Genuchten shape parameters | 
| $K_{sat}$ | cm/hr | Effective saturated hydraulic conductivity | 
| $\theta_{s}$ | (-) | Water content at effective saturation |
| $\theta_{r}$ | (-) | Residual water content |
| $d_{p}$ | cm | Maximum ponded depth | 
| % Clay | % | Percent of soil layer composed of clay | 
| % Silt | % | Percent of soil layer composed of silt | 
| % Sand | % | Percent of soil layer composed of sand | 
| pH | N/A | Soil layer pH | 
| Organic Matter | (-) | Percent of organic matter within the soil layer | 

#### Table S3: Parameters and attributes included in differentiable LGAR

| Parameter Name | Unit | Definition | 
| :------------: | :--: | :--------: |
| refkdt | (-) |  Runoff partitioning parameter | 
| satdk | m/hr |  Saturated hydraulic conductivity | 
| slope | (-) | Slope index | 
| vcmx25 |  umol CO2^m-2 s^-1  |  Maximum rate of carboxylation at 25C |
| mfsno | (-) |  Snowmelt m parmaeter |
| cwpvt | (-) | Empirical canopy wind parameter | 

## Figures:
#### Figure S1: A flowchart showing the integration of LGAR and the parameter-learning NN

the scheme used to generate lumped catchment soil parameters from n POLARIS sampling points
<img width="574" alt="image" src="https://github.com/NWC-CUAHSI-Summer-Institute/ngen-aridity/assets/16233925/26fad83b-1a25-4522-8544-cdd09c179d8e">

#### Figure S2: A flowchart showing the integration of LGAR and the parameter-learning NN
the scheme used to generate CFE parameters from a CAMELS basin
<img width="574" alt="image" src="https://github.com/NWC-CUAHSI-Summer-Institute/ngen-aridity/assets/52061672/015aa99c-de19-4ac3-bab4-d639802f6922">

#### Figure S3: A CDF plot showing the KGE percentage distribution through CDF.
<img width="574" alt="image" src="https://github.com/NWC-CUAHSI-Summer-Institute/ngen-aridity/assets/74229990/3c72c6c6-8434-49ae-bbe9-8528a9f8f25b">

#### Figure S4: A CDF plot showing the NSE percentage distribution through CDF.
<img width="574" alt="image" src="https://github.com/NWC-CUAHSI-Summer-Institute/ngen-aridity/assets/74229990/b1291581-a422-409e-a0e0-66654db2de44">

#### Figure S5: A Violin+Box plot showing the KGE distribution.
<img width="574" alt="image" src="https://github.com/NWC-CUAHSI-Summer-Institute/ngen-aridity/assets/74229990/c7794f10-8157-4665-8bc1-74f776d09aaa">

#### Figure S6: A Violin+Box plot showing the NSE distribution.
<img width="574" alt="image" src="https://github.com/NWC-CUAHSI-Summer-Institute/ngen-aridity/assets/74229990/38577a81-ce40-4a70-ac72-44d9ea6e45f0">

#### Figure S7: A visualization of the gradient chain from CFE-classic
See the PDF https://github.com/NWC-CUAHSI-Summer-Institute/ngen-aridity/blob/main/CFE_gradient_chain_demo.pdf
