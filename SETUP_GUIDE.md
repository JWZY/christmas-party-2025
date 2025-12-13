# Christmas Party Site - Setup Guide

## 🎨 Visual Updates

The site has been redesigned with a modern, polished look inspired by Partiful:
- Beautiful gradient background (forest green to dark green)
- Modern card-based layout with hover effects
- Improved typography and spacing
- Better mobile responsiveness
- Subtle shadows and animations

## 📝 Setting Up Google Form for Potluck Submissions (FREE!)

Here's how to set up the potluck submission system:

### Step 1: Create a Google Form

1. Go to [Google Forms](https://forms.google.com)
2. Click **+ Blank** to create a new form
3. Title it: "Christmas Party Potluck Sign-up"

### Step 2: Add Form Fields

Add these questions:
- **Name** (Short answer, Required)
- **What are you bringing?** (Short answer, Required)
- **Category** (Multiple choice: Appetizer, Main Dish, Side Dish, Dessert, Drinks, Other)
- **Dietary Info** (Short answer, Optional) - e.g., "Vegetarian", "Gluten-free", "Contains nuts"

### Step 3: Connect Form to Your Spreadsheet

1. In your Google Form, click the **Responses** tab
2. Click the Google Sheets icon (green spreadsheet icon)
3. Select **"Select existing spreadsheet"**
4. Choose your spreadsheet: `Christmas Party Potluck 2025`
5. Click **Select**

Now when people submit the form, it automatically adds to your spreadsheet!

### Step 4: Get the Form Link

1. Click the **Send** button (top right)
2. Click the link icon (🔗)
3. Check "Shorten URL" if you want
4. Copy the link
5. Replace the placeholder link in `index.html` (line 42):
   ```html
   <a href="YOUR_FORM_LINK_HERE" class="btn" target="_blank">
   ```

### Step 5: Customize the Spreadsheet Display (Optional)

If you want to hide the timestamp column or rearrange columns:
1. Open your Google Sheet
2. Right-click the "Timestamp" column → **Hide column**
3. Rearrange columns as desired
4. The embedded view will update automatically!

---

## 🚀 Deploying to GitHub Pages

### Step 1: Create a GitHub Repository

```bash
# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - Christmas party website"

# Create a new repository on GitHub (via web)
# Then connect it:
git remote add origin https://github.com/YOUR_USERNAME/christmas-party-2025.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 2: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**

### Step 3: Access Your Site

Your site will be live at:
```
https://jwzy.github.io/christmas-party-2025/
```

It may take 1-2 minutes to deploy. You'll see a green checkmark when it's ready!

### Step 4: Update the Site

Whenever you make changes:
```bash
git add .
git commit -m "Update party details"
git push
```

Changes will appear on your site in 1-2 minutes.

---

## 🎯 Quick Customization Checklist

- [ ] Replace Google Form link in `index.html` (line 42)
- [ ] Update RSVP form link if you have a separate RSVP form (line 35)
- [ ] Verify Google Sheet embed URL is correct (line 48)
- [ ] Update guest list as people RSVP
- [ ] Test the site locally before deploying
- [ ] Push to GitHub and enable Pages

---

## 🆘 Troubleshooting

**Google Form not showing submissions?**
- Make sure the form is connected to the correct spreadsheet
- Check that the spreadsheet is published (File → Share → Publish to web)

**Spreadsheet embed not loading?**
- Make sure the sharing settings are "Anyone with the link can view"
- Try republishing: File → Share → Publish to web → Republish

**GitHub Pages not updating?**
- Check the Actions tab in GitHub to see if the deployment succeeded
- Clear your browser cache
- Wait 2-3 minutes and refresh

---

## 💡 Pro Tips

1. **Custom Domain**: You can use a custom domain with GitHub Pages (e.g., `christmas2025.yourdomain.com`)
2. **QR Code**: Generate a QR code for your site URL to easily share
3. **Form Notifications**: In Google Forms, click ⋮ → Get email notifications to be notified of new submissions
4. **Backup**: Your Google Sheet serves as a backup of all potluck submissions

Enjoy your party! 🎄✨



