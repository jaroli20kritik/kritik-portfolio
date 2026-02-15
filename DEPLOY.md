# How to Deploy to GitHub Pages

1.  **Create a Repository on GitHub**
    *   Go to [github.com/new](https://github.com/new).
    *   Name it `kritik-portfolio` (or anything you like).
    *   Initialize it **without** a README, .gitignore, or license (empty repo).

2.  **Push your code**
    Open your terminal in the project folder (`kritik-portfolio`) and run:
    ```bash
    git init
    git add .
    git commit -m "Initial commit"
    git branch -M main
    git remote add origin https://github.com/<YOUR-USERNAME>/kritik-portfolio.git
    git push -u origin main
    ```
    *(Replace `<YOUR-USERNAME>` with your actual GitHub username)*

3.  **Enable GitHub Pages**
    *   Go to your repository **Settings** tab.
    *   Click on **Pages** in the left sidebar.
    *   Under **Source**, select `Deploy from a branch`.
    *   Under **Branch**, select `main` and fold `/ (root)`.
    *   Click **Save**.

4.  **View your site**
    *   Review the "GitHub Pages" section at the top of the settings page. It will show you the live URL (e.g., `https://<user>.github.io/kritik-portfolio/`).
