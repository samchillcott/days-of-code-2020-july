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

### #daysofcode 26/7/20 

**Today's Progress**
- N/A.

**Thoughts** 
- First day of with low stress levels and no guilt or urge to get back to coding.
- Should have portfolio finished ready for job apps this week. Bring it on.

### #daysofcode 27/7/20 

**Today's Progress**
- Portfolio Updates:
- Move projects out of clickable animation to display on load.

**Thoughts** 
- Although the MVP does a job, the UX is the next area to focus on. The projects could do with a bit more description of what they do and what tech I used and not be hidden behind a click. I realise now there is a balance to find between minimalism and UX.
- I'm struggling to understand how the template creator has set up the animation transition. Its an area I've never really covered as I have concentrated on "more important things to learn" (imo). Rather than tweak it, I am temped to strip it all out and start from scratch (like I did with the About page).
- Stripped out existing code and sorted layout from scratch. Brought back in elements that I needed for consistency.
- Again, the classname setup is confusing af because I didn't write it. Stripped that back too.
- Content overflowing from container is something I still have happening from time to time. This is great practice to understand why.
- I think keys are causing me some confusion as to why some of my links don't have a hover state any more. Noted to read up on keys for a refresher.
- Feel a bit better now the projects are on display from the get go.

### #daysofcode 28/7/20 ⁣
⁣
**Today's Progress**⁣
- Portfolio Updates:⁣
- Create gifs for Firebasic & Portfolio projects.⁣
- Merged all back in to master branch.⁣
- Complete Readme docs for all projects. Now has sections for intro, Tech Used, Features, What I learned, Challenges, Improvements, Watch Me Build This (links to IG videos for the time I was building that project) and Original Spec (by my mentor).⁣

**Thoughts** ⁣
- Can't figure out why the hover states don't work any more. Am spending too much time on this so will move on as it is a minor detail. Albeit it annoys the perfectionist in me.⁣
- Using gifs has solved the issue of non-uniform image height (which affected the project wrapper height).⁣
- Readmes took a long time but worth it. Might even start using readme as note taking doc within the projects. That way I can just tidy up my notes/reflections rather than having them dotted around my google doc for the project.⁣
- Few tiny tweaks to make but 99% of portfolio is now done. Sweet.

### #daysofcode 29/7/20 

**Today's Progress**
- Command Line learning - Navigate the file system, create/move/edit folders and files and how to kill a process.
- rm doesn't send to trash so be careful!

**Thoughts** 
- CLI/Terminal is on my Job Prep list and I thought today would be a good time to spend a few mins getting used to it before I move onto my next phase.
- I am pretty comfortable with Git nowadays but it dawned on me that I have been using GitGraph exclusively and not actually using the CL (or even GH Desktop) for git actions. React and npm do use the command line but they tend to be the same repeated commands. Will have a go at using it a bit more going forward. But then again, it seems so long winded compared to using a GUI and a few clicks?!
- I always prefer GUIs so I can SEE what I am doing. It's that fear I still have of editing or deleting something by accident.

### #daysofcode 30/7/20 

**Today's Progress**
- Testing:
- E2E - Create end-to-end (e2e) functional tests for automated click-testing of critical paths instead of relying on your users to do it for you.
- Integration - Develop integration tests to audit your application holistically and make sure everything works together correctly in harmony.
- Unit - Write effective unit tests that target the critical behaviour and functionality of your application.
- Static - Use a static type system and a linter to capture basic errors like typos and syntax.
- Ask: Is the trade-off worth it?
- Stub & Driver - Incremental Approach is carried out by using dummy programs called Stubs and Drivers. Stubs and Drivers do not implement the entire programming logic of the software module but just simulate data communication with the calling module.
- Had a play with updating dependencies and checking vulnerabilities.
- Looked a basic Jest tut.

**Thoughts** 
- Mentor chat yesterday going over next steps. Wissam @designingforscale who is a Senior Engineering Manager at GitHub had a look at our "Job Prep List" and suggested adding testing to it so will be doing some reading and a quick challenge over the coming days.
- My aim is to have some knowledge in testing concepts around unit tests, end-to-end tests, and integration tests. "You don't have to be an expert, but this is something that companies tend to look for".
- Cloned testing tut via the GH desktop app which I haven't used before. I usually clone via zip. Thought this would make sync setup quicker but looks like a fork rather than a clone because I can't push to the remote. Think it was because the remote was already setup as part of the clone so reconfigured using the GH quick setup page.
- GH Dependabot merge requests on testing clone. Have had a few alerts via email for 1 one of my projects too. Cool to see what this process does and to do the PRs. Updates dependencies and deletes the branch.

### #daysofcode 31/7/20 

**Today's Progress**
- Jest unit & integration testing (Test Runner & Assertion Library).
- Puppeteer e2e testing (Headless Browser).
- One of the benefits of using Headless Chrome (as opposed to testing directly in Node) is that your JavaScript tests will be executed in the same environment as users of your site. This gives you a real browser context without the memory overhead of running a full version of Chrome.
- Double checks can check for false positives or opposites.
- Drill down and write unit tests for the smallest levels. Then the integration test just relies on the units being tested.

**Thoughts** 
- Experimenting with having my first coffee of the day a little later. Have been sleeping well this week but still feeling tired. Also due to minimal physical exercise this week I imagine. Crashed early so had coffee (90 mins later than usual) - will bring the delay forward and see what works best.
- I like how you can watch using Jest so can catch failed tests as you go.
- I'm following along the concepts ok but not fully understanding the code/syntax just yet. Spent a while reading all the code in the tut project to understand what each part and file does. Makes more sense now. Reminds me that jumping straight in on a follow-along will catch up with you! Also highlights a point made by @emmabostian in her Honeypot video to read other people's code (because that is what you will be doing most of the time in a job - as opposed to being self taught and only writing your own code).
- Cool to play with 3 more new technologies. Was unsure of the reasons behind using Chromium and not Chrome so did some reading on why we use headless browsers.
