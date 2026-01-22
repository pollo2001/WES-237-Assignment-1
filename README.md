# WES-237-Assignment-1

### Includes
- Technical Report: A PDF detailing top-down design, frequency testing, and troubleshooting.

- Perception Plot: A graph demonstrating the non-linear Weber-Fechner Law.

- Jupyter Notebook: Source code with inline C++ for MicroBlaze and Python for system logic.

### Includes within Code
- Hardware Control: Uses MicroBlaze C++ for low-latency GPIO toggling on PMODB.

- WM Logic: Emulates analog voltage with corner-case handling for 0% and 100% duty cycles.

- Concurrency: Uses asyncio to blink the LED and poll buttons for color changes simultaneously.

- State Management: Prevents color contamination by resetting all pins before each state change.
  
- Optimization: Operates at 40Hz to exceed the human flicker-fusion threshold
