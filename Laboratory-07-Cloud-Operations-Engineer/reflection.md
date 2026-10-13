
# Reflection

## 1. Why check the host server's resources even if containers run perfectly?

Containers use the resources of the host server. If the host runs out of memory or disk space, every container on it can slow down or stop. My host has 1.9 GiB of RAM and 19 GB of storage, so I need to know these limits before a traffic surge. Checking the host first helps me find problems early, before users are affected.

## 2. How would docker logs help if a user cannot log in?

The logs show each request and the answer from the server. I can look for error codes like 401, 403, or 500 around the time the user tried to log in. For example, many 500 errors would tell me the problem is in the application and not with the user. This shows me what failed and where to fix it.

## 3. Logs vs. metrics

Logs record events, such as a request that returned 404. Metrics are numbers that show how much the system is using, such as CPU and memory. Logs tell me what happened. Metrics tell me how the system is doing.

## 4. How do large companies monitor thousands of containers?

They use tools like Prometheus to collect metrics from all containers automatically. They then use Grafana to show the data in dashboards and to send alerts when something goes wrong. This way, they do not need to check each container by hand.

## 5. How has my troubleshooting improved?

I learned to check the host first with free, df, and top. I can now read docker logs to find HTTP 200 and 404 codes, and use docker stats to check CPU and memory. In this lab, the container used only 2.719MiB of memory and 0.00% CPU, which shows the server is ready. I feel more confident finding the cause of a problem step by step.
