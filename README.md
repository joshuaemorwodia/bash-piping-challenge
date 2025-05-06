# bash-piping-challenge
# ALX Bash Piping Challenge

## a) The Piping Challenge
I explored how to use Bash piping to find the most common word in a text file. The focus was on understanding how to chain commands like `tr`, `sort`, and `uniq` using `|`.

### Objective:
- Break down text into individual words
- Sort and count the frequency
- Display the most repeated word

## b) AI Tool & Strategy Used
- **Tool:** ChatGPT (OpenAI)
- **Strategy:** I used ChatGPT to explain piping logic step by step and help correct command syntax.

## c) AI Interaction Evidence

### Prompt 1:
**Q:** How do I find the most repeated word in a text file using Bash piping?  
**A:**  
```bash
tr -s ' ' '\n' < file.txt | sort | uniq -c | sort -nr | head -n 1
cat file.txt | tr -d '[:punct:]' | tr -s ' ' '\n' | sort | uniq -c | sort -nr | head -n 1

---

### **Additional Files to Upload to GitHub**
1. `commands.sh`  
   (Contains your Bash piping commands)  
   Example:
   ```bash
   #!/bin/bash
   cat file.txt | tr -d '[:punct:]' | tr -s ' ' '\n' | sort | uniq -c | sort -nr | head -n 1
