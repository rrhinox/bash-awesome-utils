# 📦 Command-Line Shells awesome for day by day!

## Intro & Documentation

***What are Cmd and Powershell for Windows?***

Windows has two command-line shells: the Command shell and PowerShell. Each shell is a software program that provides direct communication between you and the operating system or application, providing an environment to automate IT operations.

[Microsoft Learn][cmd1]

[cmd1]: https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/windows-commands

[Microsoft Command-line Shells][cmd2]

[cmd2]: https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/windows-commands#command-line-shells


## Example 

*Get Processor and System Information*

`Get-WmiObject -Class Win32_Processor -ComputerName. | Select-Object -Property [a-z]*`

`Get-WmiObject -Class Win32_ComputerSystem -ComputerName. | Select-Object -Property SystemType`

[credit][cred]

[cred]: https://www.action1.com/how-to-get-cpu-information-in-windows-powershell/
