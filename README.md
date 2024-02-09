# Python-alarm-clock

import time

def alarm_clock(hour, minute):
  while True:
    # Get the current time
    current_time = time.localtime()
    # Check if the current time is equal to the alarm time
    if current_time.tm_hour == hour and current_time.tm_min == minute:
      print("Wake up!")
      break
    # Sleep for a minute before checking the time again
    time.sleep(60)

# Set the alarm for 7:30 AM
alarm_clock(7, 30)
