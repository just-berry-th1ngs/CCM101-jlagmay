# Reflection

## 1. How does a host-based firewall protect a server if the physical network perimeter is breached?

A host-based firewall runs on the server itself. If an attacker gets past the network perimeter, the firewall still checks every connection to the server. With Default Deny, anything I did not allow is blocked, so the attacker cannot reach other services.

## 2. Why is managing open network ports critical to reducing the attack surface?

Each open port is an entry point into the server. A service on an open port can have bugs or weak passwords that an attacker can use. When I close the ports I do not need, there are fewer entry points to attack. In this lab, I opened only port 22 for SSH and port 8080 for the web app.

## 3. Why is it dangerous to leave a database port like 3306 open to the public internet?

A database holds important data, such as customer records. If port 3306 is open to the public, anyone can try to guess the password or use a known bug. Automated tools scan the internet for open database ports all the time. The database should only be reachable from the application server on a private network.

## 4. How did this mission change my perspective on how easily a server can be compromised?

Before this lab, I thought a server was safe until something went wrong. Now I know a new server with no firewall is exposed right away. I also learned that one wrong order of commands, like turning on the firewall before allowing SSH, can lock me out of my own server. Security needs careful steps.

## 5. How does my GitHub portfolio look with eight completed missions?

My portfolio now has eight lab folders. Each one has a README, reports, and screenshots as proof. It shows my progress from basic cloud ideas to deployment, monitoring, and security. I want to keep my files clean and well organized as I add more work.
