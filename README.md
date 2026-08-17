This React component is a Digital Clock that displays the current time in a 12-hour format and updates every second.

Here, useState(new Date()) initializes the clock with the current date and time, whilst useEffect sets up a setInterval when the component loads.
Every 1,000 milliseconds (1 second), setTime(new Date()) runs to update the state and trigger a re-render.
To clean up, clearInterval(intervalId) runs when the component disappears to prevent memory leaks.Lastly, formatTime converts 24-hour time to 12-hour time (AM/PM) and uses padZero to keep numbers as double-digits (e.g., "05" instead of "5").

