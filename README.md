# Degree-v-Degree-
Coding Mistakes
import time
import sys

def animate(text, delay=0.1):
    for char in text:
        sys.stdout.write(char)
        sys.stdout.flush()
        time.sleep(delay)
    print()

def rip_degree(friend_name):
    animate(f"Locating {friend_name}'s Computer Science Degree...", 0.06)
    time.sleep(0.5)
    animate("Found! Initiating extraction sequence... 💔", 0.07)
    time.sleep(0.5)
    animate("Ripping out the heart of the degree...", 0.04)
    for i in range(3):
        animate("💔", 0.3)
    animate("\nDegree successfully extracted!\n", 0.07)
    time.sleep(0.5)

def show_certificate(your_name):
    certificate = f"""
    ┌─────────────────────────────┐
    │      MASTER OF COOL         │
    │  Presented to: {your_name}     │
    │                             │
    │  For: Out-coding CS grads   │
    └─────────────────────────────┘
    """
    print(certificate)
    time.sleep(0.5)
    animate("No degree for your friend. Sorry not sorry 😎", 0.08)

if __name__ == "__main__":
    friend_name = "Your CS Friend"
    your_name = "HotKeyNerd"
    rip_degree(friend_name)
    show_certificate(your_name)
