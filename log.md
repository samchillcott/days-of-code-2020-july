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
