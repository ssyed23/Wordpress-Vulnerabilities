# week-7-8
wordpress vulnerabilities
Time spent: 8 hours spent in total

> Objective: Find, analyze, recreate, and document 3-5 vulnerabilities affecting an old version of WordPress

## Pentesting Report

1. User Enumeration
  - [ ] Summary: 
    - Vulnerability types: User Enumeration
    - Tested in version: 4.2
    - Fixed in version: 
  - [ ] GIF Walkthrough:(video) https://github.com/ssyed23/week-7-8/blob/master/user%20enum.mp4 
  - [ ] Steps to recreate: 
  Try combinations of possible users and passwords. Look for message that implies the username exists even if the password is incorrect.
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
