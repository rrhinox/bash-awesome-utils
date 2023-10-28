# 📦  PowerShell awesome command line for day by day!

[Microsoft Learn][cmd]

[cmd]: https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/windows-commands

## Example 

*Get Processor Information*

Get-WmiObject -Class Win32_Processor -ComputerName. | Select-Object -Property [a-z]*

