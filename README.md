# Microsoft Ignite Scripts
> 作者：陈希章 

这个脚本库是 `Microsoft Ignite` 相关的脚本，包括可以用来下载视频和PPT的脚本和其他的。


## 下载所有的Microsoft Teams开发相关课程

``` Powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://raw.githubusercontent.com/chenxizhang/ignitescripts/master/Download-Resources.ps1') -replace '\$PSScriptRoot','(Get-Location).Path' -replace '\$sessionCodes = ""','$sessionCodes = "THR4005,BRK3160,MDEV30,THR2005R,THR3149,BRK1077,BRK3225,BRK3215,THR3040,THR3041,BRK1090"')
```