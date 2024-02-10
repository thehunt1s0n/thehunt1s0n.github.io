---
title: WordMacrosGenerator
date: 2024-02-09 11:00:00 -500
categories: [writeup]
# TAGS should always be lowercase
---



# What are word macros?

According to Microsoft: A macro is a series of commands and instructions that you group together as a single command to accomplish a task automatically.

Word macros can be used to deliver and execute malicious code. While macros can be beneficial for legitimate purposes, they can also be exploited by malicious actors to deliver malware, such as viruses, trojans, or ransomware.

Malicious macros typically rely on social engineering techniques to trick users into enabling or running them. For example, an attacker might send a Word document containing a macro disguised as a legitimate file, such as an invoice or a job application. When the user opens the document and enables macros, the malicious code embedded in the macro can be executed, potentially leading to unauthorized access, data theft, or system compromise.

# Automating the process using powershell.

><span style="color:green; font-style:Bold; font-family: Times New Roman, sans-serif; font-size: larger">Note : The script I used won't be shared because it can be used for malicious acts and it could harm some individuals and companies.</span>


For this to work we will need a windows machine and another machine of your choosing (I chose kali).

Step 1 : Configure the Network

Both machines should be configured to NAT


<div style="text-align:center;">
  <img src="https://github.com/thehunt1s0n/media/blob/main/WordMacroGenerator/image%20(1).png?raw=true" alt="gif 1" width="400"/>
</div>

Step 2 : Start a listener

<div style="background-color: #1e2124; padding: 10px;">
$<span style="color:red"> rlwrap nc -nvlp 1234</span></div>

<div style="text-align:center;">
  <img src="https://github.com/thehunt1s0n/media/blob/main/WordMacroGenerator/image%20(2).png?raw=true" alt="gif 1" width="400"/>
</div>
<br>

Step 3 : Execute the command

<div style="background-color: #1e2124; padding: 10px;">
$<span style="color:red"> ip a</span></div>

<div style="text-align:center;">
  <img src="https://github.com/thehunt1s0n/media/blob/main/WordMacroGenerator/image%20(3).png?raw=true" alt="gif 1" width="400"/>
</div>

<div style="background-color: #1e2124; padding: 10px;">
PS C:\Users\Public><span style="color:red"> .\script.ps1 192.168.142.131 1234</span></div>

<div style="text-align:center;">
  <img src="https://github.com/thehunt1s0n/media/blob/main/WordMacroGenerator/image%20(4).png?raw=true" alt="gif 1" width="400"/>
</div>


<div style="text-align:center;">
  <img src="https://github.com/thehunt1s0n/media/blob/main/WordMacroGenerator/image%20(5).png?raw=true" alt="gif 1" width="400"/>
</div>

<br>
Step 4 : Execute the malicious word document
<br>

<div style="text-align:center;">
  <img src="https://github.com/thehunt1s0n/media/blob/main/WordMacroGenerator/image%20(6).png?raw=true" alt="gif 1" width="400"/>
</div>
<br>

<div style="text-align:center;">
  <img src="https://github.com/thehunt1s0n/media/blob/main/WordMacroGenerator/image%20(7).png?raw=true" alt="gif 1" width="400"/>
</div>
