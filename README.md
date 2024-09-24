Here's the rewritten GitHub README in Markdown format:

---

# 🚀 Bulk Add Users to Microsoft Teams Private Channel using PowerShell

Automate adding multiple users to a Microsoft Teams team and its private channels with this PowerShell script! 🎉

## 📋 Prerequisites
Before you begin, ensure you have:

- Microsoft Teams PowerShell Module installed. 📦
- Global Administrator or Teams Administrator permissions. 🔑
- A CSV file containing the user email addresses. 📄

## 🛠️ Setup and Usage

### 1. **Install the Microsoft Teams PowerShell Module**

```powershell
Install-Module -Name MicrosoftTeams -Force
```

### 2. **Connect to Microsoft Teams**

```powershell
Connect-MicrosoftTeams
```

### 3. **Prepare Your CSV File**

Create a `users.csv` file with the following format:

```csv
UserEmail,Role
user1@example.com,Member
user2@example.com,Owner
user3@example.com,Member
```

### 4. **Update the Script Variables**

Replace the placeholders in the script with your actual values:

- `$teamName`: Your team name.
- `$channelName`: Your private channel name.
- `$usersCsvPath`: Path to your `users.csv` file.
- `$defaultRole`: "Member" or "Owner" for the channel role.
- `$reportFilePath`: Path where the report will be saved.

### 5. **Run the Script**

```powershell
# Connect to Microsoft Teams
Connect-MicrosoftTeams

# Define variables
$teamName = "Your Team Name"                      # Replace with your team name
$channelName = "Your Private Channel Name"        # Replace with your private channel name
$usersCsvPath = "C:\Path\To\users.csv"            # Replace with the path to your CSV file
$defaultRole = "Member"                           # Set default role to "Member" or "Owner"
$reportFilePath = "C:\Path\To\Report.txt"         # Path to save the report
$retryCount = 5                                   # Number of retries to check if the user is in the team
$retryDelay = 10                                  # Delay in seconds between retries

# Script to add users to private channel
```

### 6. **Check the Report**

After running the script, review the report file located at the path you specified. 📝

## 🎯 Features

- **Automated Bulk Addition:** Save time by adding multiple users at once. ⏱️
- **Progress Indicator:** Monitor the process with a real-time progress bar. 📊
- **Error Handling:** Logs any issues encountered during execution. ⚠️
- **Customizable Roles:** Assign users as Member or Owner of the private channel. 👥
- **Retry Mechanism:** Ensures users are added to the team before the channel. 🔄

## 🔔 Important Notes

- Ensure all users have the appropriate Microsoft 365 licenses. ✅
- You must have sufficient permissions to add users to teams and channels. 🔑
- Test the script with a small group before scaling up. 🧪

## 📄 License

This project is licensed under the MIT License. 📜

## 🤝 Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue. 🙌

## 📧 Contact

For questions or support, please open an issue or contact us at mez@mezbauddin.com ✉️

---

You can copy and paste this into your GitHub repository's `README.md` file!
