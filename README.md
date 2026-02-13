                                        WhatsApp Automation Project Documentation
1. Project Overview
This project uses Python to automate sending WhatsApp messages. It utilizes the pywhatkit library to interact with a web browser and WhatsApp Web to deliver messages to specific contacts or groups.

2. Technical Setup
IDE: PyCharm (JetBrains).

Language: Python 3.x.

Library: pywhatkit.

External Requirements: WhatsApp Web logged in via a default browser.

3. Step-by-Step Execution Process
Step 1: Environment Preparation
Created a new Python project in PyCharm located at C:\Users\Chandrakala\PycharmProjects\PythonProject.

Attempted installation via Terminal using pip install pywhatkit, which resulted in a "command not found" error.

Resolved by installing the package through PyCharm Settings: File > Settings > Python Interpreter > Available Packages > pywhatkit > Install Package.

Step 2: Writing the Automation Script
Developed code in main.py using the sendwhatmsg and sendwhatmsg_instantly functions.

Learned to handle the 24-hour clock format and international phone number prefixes (e.g., +91).

Step 3: Troubleshooting and Refinement
Issue: Messages were appearing as drafts but not sending.

Solution: Increased the wait_time parameter to allow the browser more time to load and automatically trigger the "Enter" key press.

Step 4: Version Control and GitHub Integration
Created a GitHub account (mythili886).

Authorized the JetBrains IDE Integration to connect PyCharm to GitHub.

Created a new repository named whatsapp-automation-python on GitHub.

Cloned the repository to the local machine using GitHub  Desktop.

Pushed the final main.py code to the cloud using the Commit and Push origin workflow.

4. Final Code Structure
Python
import pywhatkit

# Function to send message immediately
pywhatkit.sendwhatmsg_instantly("+910000000000", "Hello! This is an automated message.", wait_time=20)
