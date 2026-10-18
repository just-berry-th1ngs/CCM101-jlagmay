# Laboratory 09 - Cloud Automation Engineer

## Mission Overview

In this lab, I acted as a Cloud Automation Engineer at CloudNova Technologies. I wrote a Bash script that backs up a folder, made it executable, and set a cron job to run it every night at 2:00 AM.

## Objectives

- Understand the basics of a Bash script, including variables.
- Use nano to write and save a script.
- Change file permissions with chmod.
- Understand cron scheduling.
- Document the script and cron job in Markdown.
- Finish my GitHub Cloud Computing Portfolio.

## Commands Executed

| Command | Purpose |
|---|---|
| `mkdir app-data` | Create the dummy data folder |
| `echo "..." > app-data/data.txt` | Create a test file |
| `nano backup.sh` | Write the backup script |
| `./backup.sh` | Run the script |
| `chmod +x backup.sh` | Make the script executable |
| `ls -l backups/` | Check the backup file |
| `crontab -l` | View the cron jobs |
| `env EDITOR=nano crontab -e` | Edit the cron jobs |

## Skills Learned

- Writing a Bash script with variables.
- Making a script executable with chmod.
- Creating a compressed backup with tar.
- Scheduling tasks with cron.
- Reading the five cron time fields.
- Writing technical guides in Markdown.

## Files

- [Automation Research](automation-research.md)
- [Backup Script Guide](backup-script-guide.md)
- [Reflection](reflection.md)
