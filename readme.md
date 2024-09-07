# Achie Discord Bot Webpage

This README file provides instructions on how to update various elements of the Achie Discord Bot webpage, including links, logo, and bot name, as well as how to host the site.

## Project Structure

- `index.html`: The main HTML file.
- `style.css`: The stylesheet for styling the webpage.
- `links.js`: The JavaScript file that dynamically sets the links.

## 1. Editing Links

### Files Affected
- `links.js`
- `index.html`

### Steps

1. **Open `links.js`**:
   - Locate the `links.js` file in your project directory.

2. **Update Link URLs**:
   - Find the following code snippet in `links.js`:
     ```javascript
     const inviteLink = 'https://discord.com/oauth2/authorize?client_id=1267591670619312230&permissions=10587093855999&scope=bot%20applications.commands';
     const supportServerLink = 'https://discord.gg/jCgweFSBXy';
     ```
   - Replace the URLs with the new invite link and support server link:
     ```javascript
     const inviteLink = 'NEW_INVITE_LINK_HERE';
     const supportServerLink = 'NEW_SUPPORT_SERVER_LINK_HERE';
     ```

3. **Check HTML**:
   - Ensure that the `id` attributes for the links in `index.html` match those in `links.js`:
     ```html
     <a id="invite-link" href="#">Invite Now</a>
     <a id="support-link" href="#">Support Server</a>
     ```

4. **Save Changes**:
   - Save the `links.js` and `index.html` files after updating the links.

## 2. Updating the Logo

### Files Affected
- `index.html`
- `style.css` (if needed)
- Image files (e.g., `discord.png` and `logo.gif`)

### Steps

1. **Prepare Your New Logo**:
   - Ensure your new logo files are in the correct format (e.g., `.png`, `.gif`).

2. **Replace Logo Files**:
   - Replace the existing logo files in your project directory with the new logo files. Ensure they have the same names or update the filenames in the HTML accordingly.

3. **Update Image Source in `index.html`**:
   - Open `index.html` and find the `<img>` elements for the logos:
     ```html
     <img src="discord.png" alt="Logo" width="30" height="30" class="h-10 w-10 text-white">
     <img src="logo.gif" alt="Logo" class="h-full w-full object-cover rounded-full">
     ```
   - Update the `src` attributes if the filenames have changed:
     ```html
     <img src="NEW_LOGO_FILENAME.png" alt="Logo" width="30" height="30">
     <img src="NEW_LOGO_FILENAME.gif" alt="Logo">
     ```

4. **Save Changes**:
   - Save the `index.html` file after updating the image sources.

## 3. Changing the Bot Name

### Files Affected
- `index.html`

### Steps

1. **Open `index.html`**:
   - Locate and open the `index.html` file in your project directory.

2. **Find and Update the Bot Name**:
   - Locate the section where the bot name is displayed:
     ```html
     <h1 class="text-3xl font-bold tracking-tighter text-white sm:text-5xl xl:text-6xl mb-4">
         Achie: A Powerful Discord Bot
     </h1>
     ```
   - Update the bot name to the new name:
     ```html
     <h1 class="text-3xl font-bold tracking-tighter text-white sm:text-5xl xl:text-6xl mb-4">
         NEW_BOT_NAME: A Powerful Discord Bot
     </h1>
     ```

3. **Save Changes**:
   - Save the `index.html` file after updating the bot name.

## 4. Hosting the Website

### Steps

1. **Sign Up or Log In to Netlify**:
   - Go to [Netlify](https://www.netlify.com/).
   - Create a new account or log in with your existing account.

2. **Upload Your Code**:
   - Once logged in, click on "Sites" > "Add New Site" > "Deploy Manually" > "Drag & drop your site output folder here".
   - If you choose to upload manually, drag and drop your project files (including `index.html`, `style.css`, and `links.js`) into the upload area. Netlify will automatically build and deploy your site.

3. **Using GitHub for Automatic Deployment**:
   - Alternatively, you can use GitHub to host your code. First, push your code to a GitHub repository.
   - In Netlify, select "Sites" > "Add New Site" > "Import An Existing Project" and choose GitHub as the source.
   - Connect your GitHub account and select the repository containing your project.
   - Netlify will automatically deploy your site. It will also automatically update the live site whenever you push new changes to your GitHub repository.

4. **Automatic Updates**:
   - If you use GitHub, Netlify will handle updates automatically. Every time you push changes to your GitHub repository, Netlify will redeploy your site with the latest code changes without any additional steps from you.

- Note:
   ```html
   Netlify offers up to 100 GB of bandwidth for free. Beyond this limit, you’ll need to pay for additional usage. If you anticipate needing more bandwidth or prefer a different hosting solution, consider alternatives. I chose Netlify for its ease of use and suitability for short-term hosting. After this period, I plan to migrate the site to a web server or VPS.
   ```

## Conclusion

By following these steps, you can update the links, logo, and bot name on your Achie Discord Bot webpage and host it using Netlify. Ensure you test the webpage after making changes to confirm that everything is working correctly.

## Need Help?

If you encounter any issues or have questions, feel free to reach out for support:

[Contact Support](https://discord.gg/jCgweFSBXy)

---

**Developed by Console**
