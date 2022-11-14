Hostname | Out-File „C:\IseseisevÜL.txt“ -Append
Get-Host | Select-Object Version | Out-File „C:\IseseisevÜL.txt“ -Append
Get-WMIObject win32_operatingsystem | Select Version | Out-File „C:\IseseisevÜL.txt“ -Append
#2#
Get-NetIPAddress -AddressFamily IPv4 | ft -AutoSize | Out-File „C:\IseseisevÜL.txt“ -Append
Get-CimInstance -Class Win32_NetworkAdapterConfiguration -Filter "DHCPEnabled=$true" | Out-File „C:\IseseisevÜL.txt“ -Append
Sort-Object DHCPEnabled | Out-File „C:\IseseisevÜL.txt“ -Append
get-netadapter | Format-List -Property "Name", "InterfaceDescription", "MacAddress" | Out-File „C:\IseseisevÜL.txt“ -Append
[PSCustomObject]@{
  SystemName = hostname
  Name = $processor.Name
}
#Ram#
$CompObject.FreePhysicalMemory/1024/1024 | Out-File „C:\IseseisevÜL.txt“ -Append
Get-WmiObject win32_VideoController | Out-File „C:\IseseisevÜL.txt“ -Append
Get-CimInstance -ClassName Win32_LogicalDisk | Out-File „C:\IseseisevÜL.txt“ -Append 
#Get-WmiObject –Class Win32_PnpSignedDriver | Where-Object

{$_.DeviceID –like „PCI*“} | Select-Object Description,
DriverVersion | Sort-Object Description | Format-Table –AutoSize | Out-File „C:\IseseisevÜL.txt“ -Append
Get-LocalUser | Out-File „C:\IseseisevÜL.txt“ -Append
Get-Process | Format-List * | Out-File „C:\IseseisevÜL.txt“ -Append
Get-Date | Out-File „C:\IseseisevÜL.txt“ -Append




