### #daysofcode 20/7/20 ⁣
⁣
**Today's Progress**⁣
- SSL reading. My SiteGround hosting account will cover this for portfolio site.⁣
- Updating Project 1 so GitHub Pages uses the latest build version.⁣
- npm run build - understanding what React builds actually do to the files and folders.⁣
⁣
**Thoughts** ⁣
- Good to come back refreshed. Not had 2 days off without either having headache or hangover for 7 months.⁣
- #daysofcode means I continue my learning publicly but with less pressure and commitments. ⁣
- My knowledge of build systems and folders should help me get my Weather app up and running correctly now.⁣
- Build and static server working on fix branch but build folder seems to dissapear when I merge back to dev and master?! VSCode doesn't prompt for changes/deletions? Discovered git ignore was ignoring the build folder!⁣
- Master is running build ok but strange "<<<<<<< HEAD" appearing at the top? Updated few files - fixed.⁣
- GHP has updated deployment but still shows old version. I have 3x index.html files in the project (1 in build, public and static folders) - not sure what the diffs are and guessing GHP is using the wrong one.⁣
- Further understanding of package.json should help me here. ⁣
- I'm slowly untangling the mess but going forward with other projects, I'll know what to monitor as I go.⁣
- I think "Let me just get it working and worry about it later" from a few weeks back has caught up with me. All good.⁣
- GHP giving a 404 even though projects seems fine. I'm close. Now its a link and my read me displaying? Got it working using ghp branch.⁣
- Although I have spent 5.5 hours trying to solve the issue I have learned a lot about builds, serves and deployment.

### #daysofcode 21/7/20 ⁣
⁣
**Today's Progress**⁣
- Portfolio Updates:⁣
- Created gifs for weather and coaching apps and embedded.⁣
- Subdomain hosting - point portfolio.samchillcott.com to show the hosted Netlify portfolio.⁣
- Deployment and DNS (Domain Name System) reading.⁣
- Added CNAME record in DNS Zone Editor to point to Netlify portfolio.⁣
⁣
**Thoughts** ⁣
- I'm enjoying the reduced pressure of not doing a challenge. Although, I am aware of the added pressure I did put on myself.⁣
- Still a bit vague on DNS but not covered deployment yet (the final part of compile, build, deploy). ⁣
- Trying to work out where I set things up (name servers, A Record, CNAME record) and what I point where.⁣
- Turns out I didn't need to create the subdomain in SiteGround but the CNAME would kinda do that for me (as far as I can work out). The record seems to be added ok so may have to wait 24 hrs for it to propagate. Doesn't seem to have worked - "www.portfolio.samchillcott.com’s server IP address could not be found. DNS_PROBE_FINISHED_NXDOMAIN".⁣
- Another day of spending a few (3+) hours to complete 1 small task (easy when you know how) but learned a lot about peripheral concepts related to hosting and deployment.

### #daysofcode 22/7/20 ⁣
⁣
**Today's Progress**⁣
- Portfolio Updates:⁣
- Subdomain DNS setup.⁣
- package-lock.json reading⁣.
⁣
**Thoughts** ⁣
- Mentor chat/code review with @voyzan yesterday brought up some great feedback and tweaks for the portfolio - manly around UX and reducing some of the clicks. Added suggestions to todo list.⁣
- I can't add a CNAME for portfolio because the "name is already reserved" (I created the portfolio subdomain again in cPanel). I can't add an A record because I don't have the IP of my Netlify app (and they suggest using a CNAME). Wtf?⁣
- If I delete the subdomain I can add the CNAME. But then I can't add the subdomain back? Grr.⁣
- Called Siteground customer support who confirmed I only need the CNAME record (no need to create subdomain) and I just need to wait for propagation. Guess that's the downside of DNS - you have to wait to 24 hrs to see if your tweak worked! And it turned out I had it right yesterday but then changed it.⁣
- I have learned to keep an eye on how long to spend on each task and when to ask for help. I guess usually I can get instant feedback on whether I was successful - DNS doesn't give me that so don't wait 24hrs for that feedback.⁣
- Feel strangely tired today. Slept well but focus and energy not there after 2 hrs for some reason. Calling it after 3 hrs. Possibly mental fatigue from last few days where I have done way above average (for me) hours of coding?

### #daysofcode 23/7/20 

**Today's Progress**
- Day Off.
- Fixed subdomain.

**Thoughts** 
- Was irked by subdomain not working so couldn't enjoy my day. Contacted hosting company who gave me the real reason it wasn't working. Missing www. From the CNAME record! Changed it, instantly worked. Can sleep well now.

### #daysofcode 24/7/20 ⁣
⁣
**Today's Progress**⁣
- HTTPS (SSL/TLS) setup on portfolio site. Padlock in place.⁣
- TLS - Transport Layer Security (TLS) is the successor protocol to SSL.⁣
- gitignore reading.⁣
- Added site title using React Helmet.⁣
- Look at better options to host Resume (which constantly gets updated).⁣
⁣
**Thoughts** ⁣
- I'm getting into the habit of searching the docs (if I am using a certain platform or tech) before using google.⁣
- Netlify makes the TLS process nice and easy - gotta love abstraction.⁣
- Realised public folder was in gitignore. Read up on what usually gets ignored.⁣
- Trying to add a title tag in index.html but Gatsby develop keeps removing it (leaving the title as the url). Might need to use React helmet or add an SEO component but also looked into the Gatsby-config.js file and what that does. ⁣
- Tried to figure out why some hover links work and some don't. Baffling me.⁣
- My resume page currently links to a pdf in my google drive which works great. Until I then edit the resume. Wondering if I can host somewhere and point a subdomain to that.⁣
- Feels like a day of spending a lot of time but not changing much. I know I've learned a bit though.⁣
- MVP portfolio now complete! I can now go back and do phase 2 which will improve the UX and styling.

### #daysofcode 25/7/20 ⁣
⁣
**Today's Progress**⁣
- Portfolio Updates:⁣
- Put Resume .pdf in the public folder rather than linking externally. That way the link stays the same in the code and to update I just add the updated pdf with the same filename to the project to overwrite the existing pdf.⁣
- Attempt to add Open Graph tags (using Helmet) to display better image in social media.⁣
- New branch for Sass tweaks.⁣
- Tidied Header component spacing.⁣
- About Page containers tidy up.⁣
- Uniform size of tech icons.⁣
- Add extra tech icons.⁣
- Updated main media query.⁣
⁣
**Thoughts** ⁣
- After all the hard work on presentation, when I add the link to my LinkedIn profile it displays the worst image from my project (the firebasic screenshot which is just an html form with no css). What a woeful first impression! I want to be able to change this. Wonder if there is a setting to just use a live preview of the home page? Turns out it used one of the gifs once I submitted so that'll do. Couldn't get og tags working as planned.⁣
- I'm finding myself avoiding the Sass editing because someone else wrote it and I don't yet know their structure. Tempted to rewrite from scratch so I know where everything should be and what the class names are.⁣
- Got head around what template designer was trying to do and starting to write my own Sass where needed.⁣
- A lot happier now its a little tidier.⁣
- Discovered a strange bug where the SVGs don't load on page refresh. Quick look to find a solution (no joy) but leaving for now. Chances of that being recreated are slim.
