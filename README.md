# LogClean-Ps

### STATUS: 
Working. Early version, functional but pending further development and testing.

### DESCRIPTION
LogClean-Ps is a straightforward and efficient batch and PowerShell script combination designed for cleaning `.log` files in a given directory by removing ANSI codes. This tool is particularly handy for users who regularly work with log files that contain cluttered and hard-to-read ANSI escape sequences. By automating the cleaning process, LogClean-Ps saves time and effort, making log files more readable and easier to analyze. Intended for NotePad++ input of error.log files into GPT.

### FEATURES
- **Automated Cleaning**: Automatically finds and cleans the first `.log` file in the current directory, removing all ANSI codes.
- **Simplicity in Use**: Simple and direct functionality, ideal for quick and hassle-free log file cleaning.
- **Direct Feedback**: Provides real-time progress updates and completion messages, enhancing the user interaction experience.
- **Sleep Intervals**: Intentional short pauses after each major action for better tracking of the script's progress.

### PREVIEW
From this...
```
[31;1mGet-GPUList: [0mD:\GameTools\AllTexConFO4-Ps\AllTexConFO4-Ps v0.05\main.ps1:124[0m
[31;1m[0m[36;1mLine |[0m
[31;1m[0m[36;1m[36;1m 124 | [0m     $gpuList = [36;1mGet-GPUList[0m
[31;1m[0m[36;1m[36;1m[0m[36;1m[0m[36;1m     | [31;1m                ~~~~~~~~~~~[0m
[31;1m[0m[36;1m[36;1m[0m[36;1m[0m[36;1m[31;1m[31;1m[36;1m     | [31;1mNo '<adapter>:' line found in output.[0m
```
...to this...
```
Get-GPUList: D:\GameTools\AllTexConFO4-Ps\AllTexConFO4-Ps v0.05\main.ps1:124
Line |
 124 |      $gpuList = Get-GPUList
     |                 ~~~~~~~~~~~
     | No '<adapter>:' line found in output.
```
...come on say it...WOW!

### USAGE
1. Drop the "LogClean-Ps" batch and PowerShell scripts in the same directory as your `.log` files.
2. Run the "LogClean-Ps.Bat" file.
3. The script will automatically identify and process the first `.log` file in the directory.
4. After completion, review the cleaned log file, which will have the same name as the original.
5. When you have solved your errors, then delete the files.

### REQUIREMENTS
- Windows environment with Batch and PowerShell support.
- The scripts should be in the same directory as the `.log` files intended for cleaning.

### NOTATION
-This program will require a re-visit at some point, it just does what I need for now.

### DISCLAIMER
This program is provided "as is" without warranties or support. Users are responsible for the content they, download and use, as well as, any resulting damage to, hardware or sanity.
