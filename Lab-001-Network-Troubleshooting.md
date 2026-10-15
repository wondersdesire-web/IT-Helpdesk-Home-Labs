# Lab 001: Network Connectivity and DNS Troubleshooting

## Objective
Learn how to diagnose basic internet connectivity problems using macOS Terminal.

## Lab Environment
- Device: MacBook Air
- Operating System: macOS
- Tools: Terminal, Google Chrome
- Skill Level: Beginner

## Problem
During my home lab, my computer was unable to access websites. I investigated the connection using networking commands and browser tests.

## Troubleshooting Steps

### 1. Tested Website Connectivity
Command: `ping -c 4 google.com`

Initial result: Unknown host.

This indicated that my computer could not resolve the website name.

### 2. Tested IP Connectivity
Command: `ping -c 4 8.8.8.8`

Initial result:
- 4 packets transmitted
- 0 packets received
- 100% packet loss
- No route to host

This suggested a network connectivity or routing problem.

### 3. Checked Wi-Fi and Browser
I inspected my Wi-Fi connection and tested Google Chrome.

Chrome initially displayed `ERR_INTERNET_DISCONNECTED`.

Later, Google search results loaded successfully.

### 4. Verified Network Connectivity
I repeated the ping test to `8.8.8.8`.

Final result:
- 4 packets transmitted
- 4 packets received
- 0% packet loss
- Average response time: approximately 19.26 ms

### 5. Tested DNS Resolution
Command: `nslookup google.com`

Result: The DNS server at `8.8.8.8` successfully returned IP addresses for google.com.

## Outcome
Internet connectivity and DNS resolution were working during the final tests. The original cause of the temporary connection failure was not determined.

## Skills Learned
- Basic macOS Terminal commands
- Command syntax troubleshooting
- Network connectivity testing
- Understanding packet loss
- DNS resolution testing
- Documenting technical issues
- Verifying troubleshooting results

## Reflection
This was my first hands-on IT support home lab. I learned how to investigate network connectivity issues systematically instead of guessing at the cause.

This project is part of my journey toward becoming an entry-level IT Support Technician.
