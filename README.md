# MEM_PS_Installer
Simple Intune Software Package Framework

<#
.SYNOPSIS
  This script performs the installation or uninstallation of [PACKAGENAME]
  
.DESCRIPTION
  This script is a framework and standardisation for installing apps focussed on Intune.
  It performs an install or uninstall depending on the "type" parameter
   
.INPUTS
  -Type		The type of deployment to perform. Options: [Install, Uninstall]. Default is: Install.
 
.OUTPUTS
  Transcript logfile: c:\programdata\$BrandName\Log\$logfile
  Registry Enry: HKLM\SOFTWARE\$BrandName\Packages\
 
.EXAMPLE
	powershell.exe -executionpolicy bypass -noprofile -noninteractive -file ".\IntuneSetup.ps1 -Type "Install""
	powershell.exe -executionpolicy bypass -noprofile -noninteractive -file ".\IntuneSetup.ps1 -Type "Uninstall"
 
.NOTES
  Version:        1.7
  Author:         Marcus Jaken ~ Microsoft Cloud Consultant @ Advantive B.V
  Creation Date:  2021-05-19
  
#>
