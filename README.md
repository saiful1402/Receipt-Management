# Project (Prepared for GitHub)

This archive is prepared to be pushed to GitHub safely.

## What I changed / added
- Added `.gitignore` to ignore `database.php`, `.env` and other common files.
- Created example DB files: admin bill page/config/database.php.example, admin bill page/admin/database.php.example.

## How to finish setup locally
1. Unzip and open the folder in VS Code.
2. Copy `database.php.example` → `database.php` and fill your real credentials (DO NOT commit).
3. Initialize git:
   ```bash
   git init
   git add .
   git commit -m "Initial commit - sanitized"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
4. Keep real `database.php` on the server outside the repo or add it to `.gitignore`.

## Import DB (if you exported SQL)
Use phpMyAdmin or:
```
mysql -u username -p database_name < dump.sql
```
