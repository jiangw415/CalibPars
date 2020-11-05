# CalibPars
Those Calibration parameters are generated using the filter of J20v1, data from J20v2.

Notes:
      1: To get integral parameters, I use COTIwaverec method, its parameter: --NTimesRMS should set higher than default(1.5) to avoid noise peak in charge spectrum, in my case, I set to 2, but there still is one bin of noise peak at 0 ns in charge spectrum, so if you want to use simple integral method(COTIwaverec)'s charge spectrum information, pay attention to abandon it.
      2: The deconvolution's filter is from J20v1, new filter is still checking, maybe soon I will get the right filter. 
      3: 600 to 1000ns time window is used to calculate dark noise rate as before. However, that's not proper, little LS slow light will be in the calculation. I will update this strategy after getting the right filter.
      
Detector and electronics simulation files are at: /junofs/production/data-production/Pre-Releases/J20v2r0-Pre0/
More files details see: https://juno.ihep.ac.cn/mediawiki/index.php/Offline:Data_production/calibration
