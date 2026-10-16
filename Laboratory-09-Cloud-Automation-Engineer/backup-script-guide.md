# Backup Script Guide

## 1. Backup Script

The following Bash script automates the backup of the application data directory. It creates a backup folder if it does not exist and compresses the application data into a `.tar.gz` file with a timestamp.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. File Permissions

The command `chmod +x backup.sh` gives the script executable permission. This allows Linux to run the file as a program using `./backup.sh`.

## 3. Cron Job Configuration

The cron expression used is:

```bash
0 2 * * * /root/backup.sh
```

### Meaning of the Five Time Fields

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | Run at minute zero |
| Hour | `2` | Run at 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

The cron job schedules the backup script to run every day at 2:00 AM without requiring someone to start it manually.
