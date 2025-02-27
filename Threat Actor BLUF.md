Threat Actor: UNC4536

Create Process: This step involves spawning the cmd.exe process to inject the malicious code by redirecting STDIN and STDOUT to pipes. 
Notably, this process isn't suspended, making it appear less suspicious.
Waiting to read input from the pipe, the NtReadFile syscall sets its main thread's state to Waiting 
and _KWAIT_REASON to Executive, signifying that it's awaiting the execution of kernel code operations and their return.

Mitigation on sever exploit

Change all passwords of the host and ensure the use of strong passwords.
Strong passwords should contain upper case letters, lower case letters,
digits, punctuation marks, and other symbols. Remove any unrecognizable files, software, or services.

Hunt and Intel Research #3

Threat Actor BLUF: Threat Actor: UNC4536     A new variant of the HijackLoader malware has been reported by CrowdStrike, showcasing enhanced evasion techniques and persistence mechanisms[.] This malware is known for deploying additional payloads and has become more sophisticated in evading detection

Date: 12FEB2024

IP Address = 4 (3.125.197[.]172, 172.67.198[.]249, 104.168.48[.]208 )

Hash Values = 1 (6f345b9fda1ceb9fe4cf58b33337bb9f820550ba08ae07c782c2e142f7323748)

Domain/URL = 3 (gcdnb.pbrd.co, nginx.org, onlinetechdesk.com )
