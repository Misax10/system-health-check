# 📅 Automate Script Execution with Cron

This guide explains how to automatically run the `health_check.sh` script daily using `cron`, the built-in job scheduler available on macOS and Linux.

---

## ✅ Step 1: Make the Script Executable

Open your terminal and run:

```bash
chmod +x /full/path/to/health_check.sh
```

Replace /full/path/to/health_check.sh with actual absolute path of your script

## ✅ Step 2: Get the Full Script Path

Run the following in your script's directory to get the absolute path:

```bash
pwd
```

Then append /health_check.sh to that path.

Example:

```bash
/Users/khoa/Projects/system-health-check/health_check.sh
```

---

## ✅ Step 3: Edit Your Crontab

Open your crontab configuration:

```bash
crontab -e
```

If prompoted, choose your preferred editor (e.g, nano or vim).

---

## ✅ Step 4: Add the Cron Job

At the bottom of the crontab file, add this line:

```bash
0 9 * * * /Users/khoa/Projects/system-health-check/health_check.sh
```

This runs the script every day at 9:00 AM

Cron Format Explained:

```
┬ ┬ ┬ ┬ ┬
│ │ │ │ └─── Day of the week (0 - 6) [Sunday = 0 or 7]
│ │ │ └───── Month (1 - 12)
│ │ └─────── Day of the month (1 - 31)
│ └───────── Hour (0 - 23)
└─────────── Minute (0 - 59)
```

---

## ✅ Step 5: Save and Exit

- If using nano:
  - Press Ctrl + O to save, then Ctr + X to exit.
- If using vim:
  - Type :wq and press Enter

---

## Step 6: Verify Cron Job is Scheduled
Run:
```bash
crontab -l
```

You should see your scheduled line listed.
