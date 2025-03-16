# Daily Commit Automation

This repository automates daily commits to keep your GitHub contribution graph active. The workflow leverages **GitHub Actions** to schedule automated commits with dynamic timestamps and commit counts.

## 🚀 Features
✅ Automated daily commits following a scheduled pattern.  
✅ Dynamic **commit number** tracking.  
✅ Displays **last commit timestamp** in `commit_info.md`.  
✅ Uses **PowerShell** for improved Windows compatibility.  
✅ Manual trigger supported via **workflow_dispatch**.

## 📂 Repository Structure
```
/
├── .github/
│   └── workflows/
│       └── daily_commit.yml
├── commit_info.md
├── .gitignore
├── README.md
```

## ⚙️ Setup Instructions
1. **Fork this repository** (or clone it into your own GitHub account).
2. Navigate to the repository and create the following path:
   - `.github/workflows/daily_commit.yml`
3. Copy the contents from `daily_commit.yml` into this newly created file.
4. Create a new file called `commit_info.md` (optional: add placeholder text).
5. Go to your repository's **Settings** → **Actions** → Enable workflows (if required).
6. Manually run the workflow by going to the **Actions** tab and selecting **Run Workflow**.

## 🕒 Commit Schedule
- **Monday:** 09:30 AM IST
- **Tuesday:** 10:30 AM IST
- **Wednesday:** 11:30 AM IST
- **Thursday:** 12:30 PM IST
- **Friday:** 01:30 PM IST
- **Saturday:** 02:30 PM IST
- **Sunday:** 03:30 PM IST

## 📋 `commit_info.md` Example Output
```
Hello Peoples
This is Commit Number: 5
Last Commit Time: 2025-03-28 13:30:00 IST
```

## 🚨 Important Notes
- Ensure the email and username in the `.yml` file match your GitHub account for accurate commit tracking.
- The workflow may fail if you disable repository actions or revoke GitHub's access permissions.
