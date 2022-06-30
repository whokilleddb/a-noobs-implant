# Run That Shellcode!

This repository and all the code contained in it is part of my learning experience as I go through [RED TEAM Operator: Malware Development Essentials Course](https://institute.sektor7.net/view/courses/red-team-operator-malware-development-essentials/) try to obfuscate as much of the code as possible.

## Test 1 - The Raw Code

The executable was produced from direct code, i.e., no obfuscation methods were employed what so ever. The function calls and the payloads were kept intact without any funny business.

#### VirusTotal Score: **26/68**

![](images/1.png)

## Test 2 - Funny Functions

This time, all the function calls were obfuscated and the `GetProcAddress` was used along with some XOR'd function names. However, the payload wasn't modified at all.

#### VirusTotal Score: **23/68**

![](images/2.png)

## Test 3 - XOR it!

Now, its time to do some funny things with the payload. We begin with XOR'ing the payload with a string already available in the binary.

#### VirusTotal Score: **13/68**

![](images/3.png)

