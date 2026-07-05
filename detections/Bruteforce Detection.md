# Bruteforce Detection 
## Objective 
The objective of this detection is to find failed login attempts in Windows Security Event which leads to a Bruteforce detection against Windows user account.I have analyzed using Windows Security Event ID 4625 how failed attempts are recorded and how can they or will be investigated by a SOC Analyst.

## Attack Simulation 
In order to simulate a BruteForce attack scenario,a local user account 'attacker' has been created.Five incorrect password attempts were made before entering the correct password.This led to in generating failed logon events that were recorded in the Windows Security Event logs.

## Log Source 
- Log name : Windows Security Event log
- Event ID : 4625
- Event description : An account failed to log on

## Event Analysis 
The Event ID 4625 which generated contains useful information for investigating the failed attempts based on:
- Account that failed to log on
- Logon type
- Failure reason
- Status codes
- Workstation source
- Time of the failed attempts

