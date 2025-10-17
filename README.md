# 💥Ignite — TryHackMe

TryHackMe writeup for the **Ignite** box. This repo shows how I exploited a pre-auth Remote Code Execution in Fuel CMS 1.4.1 (CVE-2018-16763), got a shell, and escalated to root.

## Quick summary
- Target: Fuel CMS 1.4.1 (vulnerable)  
- Vuln: CVE-2018-16763 — PHP code evaluation via `pages/select` filter or `preview` data parameters.
- Exploit: public Python exploit (Exploit-DB); used to run commands and spawn a reverse shell.
- Outcome: user shell → found config/credentials → root.

## Disclaimer
For educational use only (TryHackMe lab). Don’t use these techniques on systems you don’t own or have explicit permission to test.

## References
- Exploit-DB — Fuel CMS 1.4.1 RCE PoC.  
- NVD — CVE-2018-16763. 
