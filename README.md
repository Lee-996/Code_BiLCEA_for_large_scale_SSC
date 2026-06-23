# Code_BiLCEA_for_large_scale_SSC
Large-scale sparse many-objective optimization for crowdsourced service allocation in cloud manufacturing

This is the code for the following paper. Please refer to the following reference when using the code.
%------------------------------- Reference --------------------------------
% Gui Li, Renbin Xiao, Zijun Wu, and Xi Chen, Large-scale sparse many-objective
% optimization for crowdsourced service allocation in cloud manufacturing, 
% Robotics and Computer-Integrated Manufacturing.

This project is based on PlatEMO 4.x. The specific file contents are as follows:
1)	The folder BiLCEA contains the codes related to the algorithm, including the implementation of all the pseudocode described in Section 4. This code is implemented based on the structure of PlatEMO 4.x. Simply copy this folder to the directory "Algorithm/Multi-objective optimization" of PlatEMO 4.x and it can be used directly.
2)	The folder SSC contains the code related to problems and datasets. SSCReal1-4 represents the implementation of a refrigerator design case with different constraints. The folder RealDataSet contains the real data that has been sorted out from the service data of ZBJ.COM. The code for problems are also implemented based on PlatEMO 4.x. The relevant files can be stored in the "Problems/Multi-objective optimization" of PlatEMO 4.x. It is worth noting that, due to the unknown CPF, the calculation of the HV metric is based on a reference point. The calculation of the HV metric for all MOEAs using the same reference point ensures fairness.
3)	The folder Metric store the evaluation metrics used in the comparative experiments, including the HV and IGD that have been open-sourced in PlatEMO, as well as the multiplicative epsilon metric implemented by authors. These codes should be stored in the folder Metric of PlatEMO 4.x.
4)	The folder Comparison store comparison MOEAs that have been open-sourced in PlatEMO.
