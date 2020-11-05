# CalibPars
Those Calibration parameters are generated using the filter of J20v1, data from J20v2.

Notes:

      1: To get integral parameters, I use COTIwaverec method, its parameter: --NTimesRMS should set higher than default(1.5) to avoid noise peak in charge spectrum. 
         In my case, I set to 2, but there still is one bin of noise peak at 0 ns in charge spectrum. 
         So if you want to use simple integral method(COTIwaverec)'s charge spectrum information, pay attention to abandon it.
      
      2：In J20v2, 30ns delay is added to MCP PMTs while do electronics simulation, so MCP PMTs' timeOffset values are larger and seperated from dynode PMTs' timeOffset values.
         Furthermore, PMT's TTS is a variable of angle in J20v2.
      
      3: The deconvolution's filter is from J20v1, new filter is still checking, maybe soon I will get the right filter. 
      
      4: 600 to 1000ns time window is used to calculate dark noise rate as before. However, that's not proper, little LS slow light will be in the calculation. 
         I will update this strategy after getting the right filter.
      
      
      
      
Detector and electronics simulation files are at: /junofs/production/data-production/Pre-Releases/J20v2r0-Pre0/

More files details see: https://juno.ihep.ac.cn/mediawiki/index.php/Offline:Data_production/calibration
