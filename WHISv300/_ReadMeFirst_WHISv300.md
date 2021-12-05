%% ======================================================================  
%%
%% README file for Wadai (Wakayama University) Hearing Impairment Simulator (WHIS)  
%% 和大模擬難聴システム  
%% Copyright (c) 2010-20xx  Wakayama University   
%% All rights reserved.　  
%% by Toshio Irino , 5-Dec-2021   
%%  
%% ======================================================================  



1. Software and setting

- You need GCFBv231. Set local directory as follows.
   - [LocalDir]/WHIS/WHISv300  
   - [LocalDir]/gammachirp-filterbank/GCFBv231  
   - See GCFBv231 for Seting of hearing loss (HL) 

- WHISv300_GUI :  GUI version of WHIS

- WHISv300_Batch: Batch version of WHIS

- testWHISv300v226_Batch.m : test program for WHISv300 (dtvf & fbas) & v226 for comparison

- StartupWHIS.m : setting path for tools of WHIS and GCFB

- Snd_Hello123.wav :   Sample sound

- ShowIOfunc_WHISv300CamHLS_GCFBv231.m  
    Calculation of Input-Output function using GCFB, WHIS, and CambHLS_(Not provided here)

- ShowSpec_WHISv300CamHLS_GCFBv231.m  
    Calculation of spectrogram using GCFB, WHIS, and CambHLS_(Not provided here)

- ShowIOfunc_GCFBWHISCamHLS.m  
    Showing IO function after finishing ShowIOfunc_WHISv300CamHLS_GCFBv231.m

- There are some other programs.

---

2. GUI version of WHIS
- WHISv300_GUI
  - See WHIS_GUImanual_v225-300.pdf

- Execution:   
 ＞＞　StartupWHIS  
 ＞＞  WHISv300_GUI  
 
- The following directory will be produced automatically.  
	Mac:	/Users/[UserName]/Data/WHIS   
	Win:  C:¥Users¥[UserName]¥Data¥WHIS  
    You can change the directory when the data is saved.

- You need to calibrate the SPL. --> See section 4.

---

3. Batch version of WHIS

- WHISv300_Batch
  - Batch processing program is also provided to produce many sound files for psychoacoustic experiments.
  - See testWHISv300v226_Batch.m 

---

4. Internal digital level and SPL of real environment

- Calibration tone:  sin wave with diginal RMS level of -26 dB
    - Specify SPL (Leq) of this sound in dB.

- In the case of WHISv300_GUI, it is set to 80 dB SPL.  
  -	[Intenal digital RMS level  -26 dB]  == [Outside SPL (Leq) 80 dB]

- You may specify this value when using WHISv300_Batch


--- 

  - Toshio Irino  
e-mail: irino@sys.wakayama-u.ac.jp


