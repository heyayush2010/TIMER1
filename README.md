# TIMER1
import time

def countdown_timer(seconds):
    while seconds:
        mins, secs = divmod(seconds, 60)
        timer = '{:02d}:{:02d}'.format(mins, secs)
        print(timer, end="\r")
        time.sleep(1)
        seconds -= 1
    
    print('Time’s up!')

# Example usage
countdown_time = 60  # 1 minute
countdown_timer(countdown_time)
