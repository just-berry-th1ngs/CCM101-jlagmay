# Security Audit Report

## Principle of Least Privilege (PoLP)

PoLP means a user or account gets only the minimum access needed to do its job. It is important for cloud accounts because if one account is hacked or makes a mistake, the damage stays small.

## Attack Surface

Attack surface is all the possible entry points an attacker can use to get into a system. For a virtual machine, this means open ports, running services, and remote login like SSH. The more things that are exposed, the easier it is to attack.

## Default Deny Policy

Default deny means all incoming traffic is blocked unless it is allowed by a rule. It is safer than blocking hackers one by one because attackers can change their address anytime, and I cannot know every bad address. With default deny, anything I did not allow is blocked.
