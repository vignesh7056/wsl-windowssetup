# wsl-windowssetup
cheat sheet to proper enable of wsl in windows using powershell


step1 

RUN POWERSHELL as administrator
step2
 type in powershell =   Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
 
 step3
 
 RESTART system
 
 step4 
 
 RUN POWERSHELL as administrator
 
  type in powershell = dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
  
  type in powershell =  dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
  
  step5
  
  restart
  
  step6 
  
  Download Linux Kernel: https://aka.ms/wsl2kernel
  
  double click & install
  
  step7
  
  run powershell as administrator
  
  step8
  
 type in powershell = wsl --set-default-version 2
  
  type in powershell = wsl --list --verbose
  
