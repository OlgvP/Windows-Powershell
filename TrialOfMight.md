# Exercise Powershell CLI - Trial of might

## *password lvl 1-2:* 
*Used command:* $PSVersionTable

## *password lvl 2-3:* 
*Used command:* ls, get-command

## *password lvl 3-4:* 
*Used command:* **ls and counted manually, not very well method but in this case the fastest for me**

## *password lvl 4-5:* 
*Used command:* dir, cd

## *password lvl 5-6:* 
*Used command:* $env:USERDOMAIN, dir

## *password lvl 6-7:* 
*Used command:* **This time was too much folders to count manually so I found and used:**
		(Get-ChildItem -Directory | Measure-Object). Count
		
## *password lvl 7-8:* 
*Used command:* Get-Childitem –Path C:\ -Include *readme* -Recurse -ErrorAction SilentlyContinue
	**after I was checking all the files readme this command showed with "cat"**

## *password lvl 8-9:* 
*Used command:* $A = $( foreach ($line in Get-Content C:\users\century8\desktop\unique.txt) {
    $line.tolower().split(" ")
  }) | Sort-Object | Get-Unique
$A.count	

## *password lvl 9-10:* 
*Used command:*
$content = Get-Content -Path "C:\users\century9\desktop\Word_File.txt"
$words = $content -split ' '    **<-spliting lines into a words**
$item = $words[160]		**<-in powershell position 161 has index 160 (cause it starts from 0)**
Write-Output $item

## *password lvl 10-11:* 
*Used command:*
 $wuauserv = Get-WmiObject -Class Win32_Service | Where-Object { $_.Name -eq "wuauserv" }
 $description = $wuauserv.Description
 Write-Output $description
 
## *password lvl 11-12:* 
*Used command:* get-childitem -force -recurse

## *password lvl 12-13:* 
*Used command:* 
	**Import the Active Directory module**
	Import-Module ActiveDirectory

	**Get the domain controller object**
	$domainController = Get-ADComputer -Filter {PrimaryGroupID -eq 516} -Properties Description

	**Output the description**
	$domainController.Description
	
## *password lvl 13-14:* 
Used commands: **I had a little problem with this exercise, so i decided to copy content the file 
and use script to count the words:**

$content = @"
<file content>
"@

$wordCount = ($content -split '\s+' | Where-Object { $_ -ne '' }).Count

Write-Host "Number of words in the file: $wordCount"

## *password lvl 14-15:* 
*Used commands:* 
		$path = "C:\users\century14\desktop\countpolos"
		$word = "polo"

		$content = Get-Content -Path $path -Raw
		$count = ($content | Select-String -Pattern "\b$word\b" -AllMatches).Matches.Count

		Write-Host "Number of word '$word': $count"













