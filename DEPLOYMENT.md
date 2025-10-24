# Deployment Instructions for GitHub Pages

## Step-by-Step Guide to Deploy the Delphi Workshop Website

### Prerequisites
- GitHub account with access to the AthensDiaCorpus organization
- Git installed on your computer (optional, can use GitHub web interface)

### Method 1: Using GitHub Web Interface (Easiest)

1. **Login to GitHub**
   - Go to https://github.com
   - Sign in with your account

2. **Navigate to AthensDiaCorpus Organization**
   - Click on your profile icon (top right)
   - Select "Your organizations"
   - Click on "AthensDiaCorpus"

3. **Create New Repository**
   - Click the green "New" button
   - Repository name: `Delphi2025` (with capital D as requested)
   - Description: "International Workshop - Corpora and Diachrony 2025"
   - Set to **Public**
   - Do NOT initialize with README
   - Click "Create repository"

4. **Upload Files**
   - Click "uploading an existing file"
   - Drag and drop all website files:
     - index.html
     - secure.html
     - css folder (with style.css inside)
     - js folder (with main.js inside)
     - README.md
   - Write commit message: "Initial website upload"
   - Click "Commit changes"

5. **Enable GitHub Pages**
   - Go to repository Settings (top menu)
   - Scroll down to "Pages" (left sidebar)
   - Under "Source", select "Deploy from a branch"
   - Branch: select "main"
   - Folder: select "/ (root)"
   - Click "Save"

6. **Wait for Deployment**
   - GitHub will show a message with your site URL
   - Wait 2-5 minutes for the site to go live
   - Your site will be available at: https://athensdiacorpus.github.io/Delphi2025

### Method 2: Using Git Command Line

1. **Clone the repository**
   ```bash
   git clone https://github.com/AthensDiaCorpus/Delphi2025.git
   cd Delphi2025
   ```

2. **Add all website files**
   ```bash
   # Copy all files to the repository folder
   git add .
   git commit -m "Initial website upload"
   git push origin main
   ```

3. **Enable GitHub Pages**
   - Follow steps 5-6 from Method 1

### Important Notes

- **Password for secure area**: The current password is `delphi2025` (hardcoded in secure.html)
- **Images**: Add open access images to the `images/` folder when available
- **Updates**: To update the site, simply edit files and commit changes
- **Custom Domain**: If you want a custom domain later, add a CNAME file

### Troubleshooting

If the site doesn't appear after 10 minutes:
1. Check Settings > Pages for any error messages
2. Ensure the repository is public
3. Check that index.html is in the root directory
4. Try clearing your browser cache

### Next Steps

After deployment:
1. Test all navigation links
2. Check the secure area with password
3. Add open access images of Delphi
4. Update contact email if needed
5. Share the link: https://athensdiacorpus.github.io/Delphi2025

For any issues, contact the technical team or check GitHub's documentation at https://docs.github.com/pages