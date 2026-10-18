# Laboratory 08 - Cloud Security Engineer

## Mission Overview

In this lab, I acted as a Cloud Security Engineer at CloudNova Technologies. I deployed an Nginx web app, turned on the UFW firewall with a Default Deny policy, and opened only the ports the client needs.

## Objectives

- Understand the attack surface and the Principle of Least Privilege.
- Check active network ports on a Linux server.
- Set up UFW with a Default Deny policy.
- Allow only SSH and port 8080.
- Document firewall rules in Markdown.
- Add to my GitHub Cloud Computing Portfolio.

## Commands Executed

| Command | Purpose |
|---|---|
| `docker run -d --name secure-web-app -p 8080:80 nginx` | Start the Nginx container |
| `curl http://localhost:8080` | Test the web app |
| `sudo ufw allow ssh` | Allow SSH (port 22) |
| `sudo ufw default deny incoming` | Block all incoming traffic by default |
| `sudo ufw default allow outgoing` | Allow all outgoing traffic |
| `sudo ufw enable` | Turn on the firewall |
| `sudo ufw status verbose` | Check the firewall status |
| `sudo ufw allow 8080/tcp` | Allow web traffic on port 8080 |
| `sudo ufw status numbered` | Show the rules with numbers |

## Skills Learned

- Setting up a firewall with UFW.
- Using a Default Deny policy.
- Allowing only the ports a service needs.
- Allowing SSH first so I do not get locked out.
- Writing security documentation in Markdown.

## Files

- [Security Audit Report](security-audit-report.md)
- [Firewall Configuration](firewall-configuration.md)
- [Reflection](reflection.md)
