# DevOps_task
This respositry mainly is to submit the assessment task as a first phase of Fawry DevOps Internship process

# Q1 : Custom Command (mygrep.sh)
1. 🧪 Hands-On Validation

![Screenshot from 2025-04-28 20-03-40](https://github.com/user-attachments/assets/b98460eb-f234-4062-8349-ed3cc62c746a)
![Screenshot from 2025-04-28 20-03-49](https://github.com/user-attachments/assets/2b77f972-7714-4d73-b150-89af42101ba5)
![Screenshot from 2025-04-28 20-03-55](https://github.com/user-attachments/assets/1ea249d1-00d0-428e-a668-911cb5cbe118)
![Screenshot from 2025-04-28 20-04-07](https://github.com/user-attachments/assets/47c1ae32-4931-48bd-88d3-a17d363a2728)

2. 🧠 Reflective Section
Argument Handling:

- The script uses getopts to parse command-line options -n and -v. It checks for invalid options and provides usage information if necessary.
After parsing options, it checks if the required arguments (search string and file) are provided. If not, it displays an error message and usage instructions.
It verifies if the specified file exists before proceeding with the search.
Supporting Regex or Additional Options:

- To support regex, I would modify the grep command to include the -E option for extended regex patterns. For options like -i (case-insensitive), -c (count matches), or -l (list filenames), I would add additional flags in the option parsing section and adjust the grep command accordingly to handle these cases.

- Hardest Part to Implement: Actually the challenging part was to remind myself with some syntax and manipulations in Bash scripting to ensure that the script works normally without any error or exception
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Q2 : Scenario
1.  Verify DNS Resolution:
![Screenshot from 2025-04-28 20-47-22](https://github.com/user-attachments/assets/e6c61bef-7f1f-4ad0-b801-40fd7f3fb2d6)
![Screenshot from 2025-04-28 20-47-55](https://github.com/user-attachments/assets/ffd7ca5a-82f9-4a85-9cd2-5e09df85c0c4)

2. Diagnose Service Reachability:
![Screenshot from 2025-04-28 20-48-27](https://github.com/user-attachments/assets/3061447a-dc5b-4724-842d-ad4a3ee4b4b6)


3.  Trace the Issue – List All Possible Causes
- Host Configuration:
  Issue : Incorrect hostname resolution in /etc/hosts.
  Solution : Update the configuration file with adding the resolved ip of the hostname that we have captured from step 2
4. Propose and Apply Fixes
  4.1.  Explain how you would confirm it's the actual root cause
       using #sudo command to be the root
  4.2.  Show the exact Linux command(s) you would use to fix it
       using nano, vim or cat to update the conf file
  ![Screenshot from 2025-04-28 20-48-55](https://github.com/user-attachments/assets/f5c00ec1-1e02-47bd-9b47-46b579283f72)

Verify the resolution is working normally 
![Screenshot from 2025-04-28 20-49-19](https://github.com/user-attachments/assets/d90ce02c-9ac2-4161-865f-9ca6a9b208f7)
![Screenshot from 2025-04-28 20-50-55](https://github.com/user-attachments/assets/b15ef5aa-fc86-4e28-be07-e0c3680d1c0a)

