# week-7-8
wordpress vulnerabilities
Time spent: 8 hours spent in total

> Objective: Find, analyze, recreate, and document 3-5 vulnerabilities affecting an old version of WordPress

## Pentesting Report

1. User Enumeration
  - [ ] Summary: 
    - Vulnerability types: User Enumeration
    - Tested in version: 4.2
    - Fixed in version: 4.5
  - [ ] GIF Walkthrough:https://github.com/ssyed23/week-7-8/blob/master/userenum.gif
  - [ ] Steps to recreate: 
  Try combinations of possible users and passwords. Look for message that implies the username exists even if the password is incorrect.
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
    
    
    2. Cross-Site Scripting (XSS)
  - [ ] Summary: 
    - Vulnerability types: XXS in URL embed
    - Tested in version: 4.0
    - Fixed in version: 4.7
  - [ ] GIF Walkthrough:https://github.com/ssyed23/week-7-8/blob/master/xxs1.gif 
  - [ ] Steps to recreate: 
  1. Log into account that is able to make posts.
  2. Edit a post and write code such as, [embed src='https://www.youtube.com/embed/video\x3csvg onload=alert("XSS Found!")\x3e'][/embed]
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
    
    
    3. Cross-Site Scripting (XSS)
  - [ ] Summary: 
    - Vulnerability types: XXS - allows users to inject potentially harmful code 
    - Tested in version: 4.2
    - Fixed in version: 4.6.1
  - [ ] GIF Walkthrough:
  - [ ] Steps to recreate: 
  1. Log into account that allows user to make/edit posts.
  2. Make a new post and write code such as <img src=image oneerror=alert("XSS!")>
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
