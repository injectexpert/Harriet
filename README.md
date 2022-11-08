# Harriet
This repo is a resource for various red teaming techniques and tools based on open source software and non-commerical tools.
 
![Screen Shot 2022-10-17 at 12 14 33 PM](https://user-images.githubusercontent.com/76174163/196229183-c96e9a38-8466-4ebd-81ab-35934877d559.png)

The payload framework is very effective when paired with my Covenant Randomizer script.

![Screen Shot 2022-10-17 at 12 15 10 PM](https://user-images.githubusercontent.com/76174163/196229270-49bb9d83-a18d-4cb6-b1b7-b798fca19d4c.png)

I was able to bypass Defender with Covenant with no problems.

![Screen Shot 2022-10-17 at 11 59 31 AM](https://user-images.githubusercontent.com/76174163/196239034-54866187-c461-4735-be81-9821c3a1e9a0.png)

I was also able to bypass Defender with a Meterpreter payload. This might not be as effective since Meterpreter is signatured so heavily. Your results will vary without modifying your Meterpreter payload's template inside Metasploit. Going with lesser used payloads will probably yield good results. 

**Modules**

![Screen Shot 2022-10-17 at 12 12 15 PM](https://user-images.githubusercontent.com/76174163/196239966-8d41b19b-6d66-4a80-a72c-4d1554197702.png)

There are four modules currently. As of this post, all of them bypass AV/Defender. 
 
AES Encrypted payload

AES Encrypted payload with process injection

QueueUserAPC shellcode execution

ThreadPoolWait shellcode execution. 

All of the modules use XOR encryption for strings and function obfuscation and AES encryption for payload exection. Once the payload is compiled, the script uses SigThief to sign the binary with a Microsoft certificate. 



