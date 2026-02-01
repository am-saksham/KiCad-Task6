# How to Upload SpiralGen Pro to GitHub

I have already initialized the Git repository for you locally. Follow these steps to put it online:

### 1. Create the Repository on GitHub
1.  Go to [github.com/new](https://github.com/new).
2.  **Repository name:** `SpiralGen-Pro` (or `KiCad-Task6`).
3.  **Description:** "KiCad 9 Plugin for generating planar spiral inductors (Task 6 Submission)."
4.  **Public/Private:** Choose **Public** (easier for sharing).
5.  **Do NOT check** "Initialize with README" (we already have one).
6.  Click **Create repository**.

### 2. Connect and Push
Once the repository is created, copy the URL (it will look like `https://github.com/YOUR_USERNAME/SpiralGen-Pro.git`).

Open your terminal and run these commands (replace `YOUR_URL` with the one you copied):

```bash
cd /Users/am.sakshamgupta/Desktop/Task6

git remote add origin YOUR_URL_HERE

git branch -M main

git push -u origin main
```

### 3. Verify
Refresh your GitHub page. You should see all your files (`SpiralGen/`, `README.md`, etc.).

### 4. Final Step
Copy the link to your new repository and paste it into `proposal_details.txt`.
