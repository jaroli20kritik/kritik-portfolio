# How to Deploy Your Portfolio to GitHub Pages

Follow these exact steps to get your website online.

## Step 1: Create a Repository on GitHub
1.  Log in to your [GitHub account](https://github.com/).
2.  Click the **+** icon in the top-right corner and select **New repository**.
3.  **Repository name**: Enter `kritik-portfolio` (or any name you prefer).
4.  **Description**: (Optional) e.g., "My personal portfolio website".
5.  **Public/Private**: Select **Public** (Github Pages is free for public repos).
6.  **Initialize this repository with**: Leave all these unchecked (No README, No .gitignore, No License). **This is important.**
7.  Click **Create repository**.

## Step 2: Push Your Code
Now that you have an empty repository on GitHub, you need to upload your local code to it.

1.  Copy the HTTPS URL of your new repository from the Quick Setup page (it looks like `https://github.com/YOUR-USERNAME/kritik-portfolio.git`).
2.  Open your terminal or command prompt in your project folder.
3.  Run the following commands (replace `<YOUR_REPO_URL>` with the URL you copied):

```bash
git remote add origin <YOUR_REPO_URL>
git push -u origin main
```

*Note: If `git push` asks for a password, you might need to use a Personal Access Token or sign in via the browser if prompted.*

## Step 3: Enable GitHub Pages
Once your code is pushed:

1.  Go to your repository on GitHub.
2.  Click on the **Settings** tab (top right of the repo menu).
3.  In the left sidebar, click on **Pages**.
4.  Under **Build and deployment** > **Source**, select **Deploy from a branch**.
5.  Under **Branch**, confirm it says **main** and folder is **/(root)**.
6.  Click **Save**.

## Step 4: View Your Live Site
*   Refresh the Pages settings page.
*   You should see a message at the top: "Your site is live at..."
*   Click the link to view your portfolio!

## Troubleshooting
**Error: "fatal: not a git repository (or any of the parent directories): .git"**
This means your terminal is not inside the project folder. Run this command first:

```powershell
cd "C:\Users\HP\.gemini\antigravity\scratch\projects\kritik-portfolio"
```


## How to Update Your Site
Whenever you make changes to your code (e.g., changing text, images, or styles), run these 3 commands in your terminal to update the live site:

1.  **Stage your changes:**
    ```bash
    git add .
    ```
2.  **Commit your changes** (replace "Updated content" with a short description):
    ```bash
    git commit -m "Updated content"
    ```
3.  **Push to GitHub:**
    ```bash
    git push
    ```

*After running `git push`, wait 1-2 minutes and update your live website.*
