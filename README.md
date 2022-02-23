# Secode

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FAliasgarSabunwala%2FSecode%2F&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=TOOL+VIEWS&edge_flat=false)](https://hits.seeyoufarm.com)

<p align="center">
       <b> In a Nutshell </b>
</p>

- Secode is an Static Code Analyzer, that analyzes your code, to find anomalies, currently only limited to "Insecure Functions" in your codes
- But, it doesn't stop there - as a precautionary measure, it provides you with safer function as an alternative - like instead of using `strcpy()` which is vulnerable to Buffer Overflow, it provides you with safer function as an alternative like `lstrcy()`, which is not vulnerable to Buffer Overflow, that you can implement on your code, to make it secure

# How is it different?
- Secode is powered by a **stringent and comprehensive ruleset**, that can detect vulnerabilities pretty easily, which will be updated regularly, 
as more vulnerabilities and exploits emerge
- Secode enforces the concept of "**Secure Coding" and "Secure Software Development Life Cycle (Secure SDLC)"** which is now gaining much needed traction during the 
development process of any software


# What does a Secode scan on the Code(s) you provide, give you?
Your Code Report provides you information about-

- Hit count of vulnerable functions (total count)
- Vulnerability at hand
- CWE Number associated with it
- A brief description about the vulnerability
- Risk level of your code (graded from 1 - 5,on the severity basis)
- Secure alternative(s) that you must use which are totally safe from exploits


## Installation Guide
Refer to the [INSTALL.md](INSTALL.md) file for an in-depth walkthrough on how to install the tool, on your Linux distro


# Under the hood
- More technically, secode uses lexical scanning to find tokens (such as function names) that suggest likely vulnerabilities, estimates their level of risk (e.g., by the text of function calls), and reports the results
- Secode does not use or have access to information about control flow, data flow, or data types
- Thus, secode will necessarily produce many false positives for vulnerabilities and fail to report many vulnerabilities
- On the other hand, secode can find vulnerabilities in programs that cannot be built or cannot be linked
- Secode also doesn't get as confused by macro definitions and other oddities that more sophisticated tools have trouble with


## Roadmap
- Dockerize it to provide support across all platforms
- Extending Scanning functionalities within the tool to: 
    1. Web Technologies like HTML, CSS, Js and PHP
    2. App Development languages like Java and Kotlin
- GitHub Actions workflows Integration


# Contributions
We love contributions! For more information on contributing, see the file [CONTRIBUTING.md](CONTRIBUTING.md)


# License
Secode is released under the GNU GPL license version 2 or later (GPL-2.0+). See the [LICENSE](LICENSE) file for license information.
