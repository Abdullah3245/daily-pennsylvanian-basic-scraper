# Cron Syntax Explanation

Cron expressions consist of five fields that represent units of time, separated by spaces. Each field specifies when a task should run:

1. **Minute** (0 - 59): The minute of the hour the task should run.
2. **Hour** (0 - 23): The hour of the day the task should run.
3. **Day of the Month** (1 - 31): The specific day of the month the task should run.
4. **Month** (1 - 12 or JAN-DEC): The month during which the task should run.
5. **Day of the Week** (0 - 6 or SUN-SAT): The day of the week the task should run.

### Special Characters

- **`*` (any value):** Represents "every" possible value for that field.  
  Example: `* 10 * * *` runs the task every minute during the 10th hour of every day.

- **`,` (multiple values):** Specifies multiple specific values.  
  Example: `10,15 * * * *` runs the task at the 10th and 15th minutes of every hour.

- **`-` (range):** Represents a range of values.  
  Example: `* 10-12 * * *` runs the task every minute during the 10th, 11th, and 12th hours.

- **`/` (step values):** Specifies increments.  
  Example: `*/5 * * * *` runs the task every 5 minutes.

### Example Interpretation

The cron expression `0 3 * * *` means the job runs at **3:00 AM UTC every day**.  
- `0` → At the 0th minute (on the hour).  
- `3` → During the 3rd hour of the day.  
- `*` → Every day of the month.  
- `*` → Every month.  
- `*` → Every day of the week.  
****
