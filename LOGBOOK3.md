
# Trabalho realizado na Semana #3

## Identificação

- CVE-2019-0708, also known as BlueKeep

- A Vulnerability in Remote Desktop Services when an unauthenticated attacker
  connects to the target system using RDP and sends specially crafted requests

- Aplicações/Sistemas Operativos Relevantes
  1. Windows 2003
  1. Windows XP
  1. Windows Vista
  1. Windows 7
  1. Windows Server 2008

## Catalogação

- CVSS 3.x Severity and Metrics: Base Score 9.8 Critical

- CVSS 2.0 Severity and Metrics: Base Score 10.0 High

- CWE-416 - Use After Free - Referencing memory after it has been freed can
  cause a program to behave unexpectedly/execute code.

- Bluekeep vulnerability was first noted by the UK National Cyber Security
  Centre (14th May 2019).

## Exploit

- There are multiple exploits and Proof of Concepts available on metasploit or
  git repositories

- msf5 exploit(windows/rdp/cve\_2019\_0708\_bluekeep\_rce) > run

- [Ekultek Bluekeep PoC](https://github.com/Ekultek/BlueKeep)

- Metasploit DoS [exploit-db](https://www.exploit-db.com/exploits/47120)

## Ataques

- On 2019 a hacker group used BlueKeep to search for open RDP
  ports and deploy a payload that mines cryptocurrencies

- Affected countries include France,Russia,Italy,Spain,Ukraine,Germany and the
  UK

- On 8 November 2019, Microsoft confirmed a BlueKeep attack, and urged users to
  immediately patch their Windows systems.
