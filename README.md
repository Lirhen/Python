🔧 AWS Environment Variables Setup

To run this Python integration, you need to configure your AWS credentials as environment variables. This avoids hardcoding secrets inside your code.

Linux / macOS

Open your shell configuration file (e.g., ~/.bashrc or ~/.zshrc).

Add the following lines at the bottom of the file:

export AWS_ACCESS_KEY_ID="YOUR_ACCESS_KEY"
export AWS_SECRET_ACCESS_KEY="YOUR_SECRET_KEY"

Save the file and reload it:

source ~/.bashrc
# or
source ~/.zshrc

Windows
PowerShell

Run the following commands (they will persist across sessions):

setx AWS_ACCESS_KEY_ID "YOUR_ACCESS_KEY"
setx AWS_SECRET_ACCESS_KEY "YOUR_SECRET_KEY"

Command Prompt (temporary, current session only)
set AWS_ACCESS_KEY_ID=YOUR_ACCESS_KEY
set AWS_SECRET_ACCESS_KEY=YOUR_SECRET_KEY

Verification

You can verify that the variables are set correctly by running:

echo $AWS_ACCESS_KEY_ID        # Linux/macOS
echo $AWS_SECRET_ACCESS_KEY

echo $env:AWS_ACCESS_KEY_ID    # Windows PowerShell
echo $env:AWS_SECRET_ACCESS_KEY
