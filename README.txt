RAJPALWAN COMMUNITY WEBSITE — NETLIFY + SECURE CMS SETUP

What this package includes
- index.html: public village website
- content/site.json: editable introduction, announcements, gallery and contact link
- admin/: Decap CMS admin interface
- uploads/: destination for photos uploaded in the CMS

IMPORTANT: This CMS is not ready to authenticate until you complete the account-connection steps below. Do not share the admin URL as a security measure; access is controlled by Decap Turbo site permissions.

LOW-COST PUBLISHING STEPS

1. Create/sign in to GitHub at https://github.com/ and create a NEW repository named rajpalwan-village.
   For a public village website, the repository can be public; never put passwords, private phone numbers, or secrets in it.
2. Upload the CONTENTS of this folder (not the outer folder) to the repository. Keep the main file named index.html and keep admin/ and content/ at the repository root. Commit to the main branch.
3. Sign in to Netlify at https://app.netlify.com/ and choose Add new project / Import an existing project. Connect GitHub and select rajpalwan-village. Publish from branch main with publish directory "." and no build command.
4. Copy the public Netlify URL after deployment.
5. Sign up/sign in to Decap Turbo at https://decapcms.org/ (Turbo link in the Decap CMS site). Create a site, connect the GitHub repository you just made, and grant your own account editor/owner access.
6. In the Decap Turbo site settings, add the admin URL exactly, for example:
   https://YOUR-SITE-NAME.netlify.app/admin/
   Use your actual Netlify site name, not the example.
7. Copy the Turbo site ID shown in the Turbo site overview. Edit admin/config.yml and replace REPLACE_WITH_DECAP_TURBO_SITE_ID with that ID. Commit the change to GitHub. Netlify will redeploy automatically.
8. Open https://YOUR-SITE-NAME.netlify.app/admin/ and log in with Decap Turbo. Only accounts explicitly granted access to this site should be able to edit.
9. To add news, open Village content. To add photos, edit Village photo gallery, upload a file, add a caption, and publish. A commit triggers a Netlify redeploy; it may take a short time for the live site to refresh.

PHOTO UPLOAD NOTES
- The included setup uploads photos into the Git repository under uploads/. This is the lowest-cost simple route and avoids the separate Decap Turbo Media Library, which is a Pro feature according to its documentation.
- Compress photos before uploading (e.g. JPG/WebP, ideally 0.5–1.5 MB each) to keep the repository small.
- Ask permission before posting identifiable people, especially children. Do not publish private phone numbers or addresses.

GOVERNMENT UPDATES
The website contains official links to Kangra/Himachal government pages. It does NOT automatically scrape or republish government notices. Add a dated community item manually only after checking the original official notice and include the official source link in the text when possible. Do not present this community site as a government website.

COST AND LIMITS
- Netlify currently offers a Free plan with a monthly credit allowance and hard limit; check your dashboard usage before frequent redeploys.
- GitHub account/repository and Decap CMS are free to start; Decap Turbo starts on Free and has plan limits. Check current terms before relying on it long term.
- A custom domain is optional and normally costs extra.
- I cannot sign into your accounts or publish on your behalf. Never send passwords or access tokens in chat.

If you get stuck, send a screenshot of the current Netlify/GitHub/Decap Turbo screen (hide email, tokens, and private details) and I can guide the next click.


LATEST CUSTOMISATIONS
- Added a village map section with embedded 2D map, a Google Maps pin, satellite-view link, directions link and Google Earth 3D link. The pin is an approximate village-level location (32.02262, 75.82918); verify it locally before treating it as definitive.
- Added public website credit: Created & maintained by Ajay Mehra, phone 9518085026, email amehra488@gmail.com, as explicitly requested by the site owner. This contact information will be visible to all visitors.

SIMPLE PUBLISH CHECKLIST
1. Download and extract this ZIP on your computer.
2. In GitHub, open your rajpalwan-village repository. Upload/replace the package contents at the repository root (index.html, admin folder, content folder; keep folder names unchanged) and commit the changes.
3. Netlify will deploy automatically if it is connected to that GitHub repository. If not, in Netlify choose Add new project > Import an existing project and connect the repository.
4. Open your Netlify public URL and check the Village map section and footer credit.
5. To publish new photos and updates, complete the Decap Turbo CMS connection described above and open /admin/. Do not share passwords or access tokens.
