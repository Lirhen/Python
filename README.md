# Python

AWS Environment Variables Setup
Overview
To run this Python integration, you need to configure your AWS credentials as environment variables.
Linux / macOS Setup

Open your shell configuration file:
bashnano ~/.bashrc    # For bash
# OR
nano ~/.zshrc     # For zsh

Add the following lines at the bottom of the file:
bashexport AWS_ACCESS_KEY_ID="YOUR_ACCESS_KEY"
export AWS_SECRET_ACCESS_KEY="YOUR_SECRET_KEY"
export AWS_DEFAULT_REGION="us-east-1"  # Optional but recommended

Save the file and reload it:
bashsource ~/.bashrc
# OR
source ~/.zshrc


Windows Setup
PowerShell (Persistent across sessions)
powershellsetx AWS_ACCESS_KEY_ID "YOUR_ACCESS_KEY"
setx AWS_SECRET_ACCESS_KEY "YOUR_SECRET_KEY"
setx AWS_DEFAULT_REGION "us-east-1"
Command Prompt (Temporary, current session only)
cmdset AWS_ACCESS_KEY_ID=YOUR_ACCESS_KEY
set AWS_SECRET_ACCESS_KEY=YOUR_SECRET_KEY
set AWS_DEFAULT_REGION=us-east-1
Verification
Verify that the variables are set correctly:
Linux/macOS
bashecho $AWS_ACCESS_KEY_ID
echo $AWS_SECRET_ACCESS_KEY
echo $AWS_DEFAULT_REGION
Windows PowerShell
powershellecho $env:AWS_ACCESS_KEY_ID
echo $env:AWS_SECRET_ACCESS_KEY
echo $env:AWS_DEFAULT_REGION
