# BRIX events: how the team adds them

The team fills in a Google Form. Each event appears on **brixldn.com/events** within 5 minutes and drops off automatically after its date.

## One-time setup (about 5 minutes)

**1. Update the script**
- In the BRIX Website Forms Sheet, go to **Extensions → Apps Script**.
- Replace all the code with the new **Code.gs**, then **Save**.

**2. Build the team form**
- In the function dropdown pick **createEventsForm**, then click **Run**.
- Approve the new permissions: **Review → Advanced → Allow**. This time it also asks for Forms and Drive.
- Open the **Execution log** at the bottom. It shows two links:
  - **EDIT the form**: open this one now.
  - **TEAM LINK**: this is the link the BRIX team uses. Save it.
- Your Sheet now has a new **Events** tab.

**3. Add the image question (Google won't let a script do this bit)**
- In the form editor, click **+ Add question** and name it **Image**.
- Change the type to **File upload**. Continue if Google asks.
- Set **Maximum number of files** to **1**, **Maximum file size** to **10 MB**, and allow **Image** only.
- Turn on **Required**.

**4. Publish the update**
- In Apps Script go to **Deploy → Manage deployments → pencil → Version: New version → Deploy**. The link stays the same, so forms.js doesn't change.

**5. Upload the website pages**
- Upload the 11 .html files to the repo root on GitHub.

## Day to day, for the team
- Open the **TEAM LINK** and fill in the event name, date, start time, optional label (e.g. *Live music*, *SIXT33N*), description, booking link and image. Submit.
- **Images:** portrait 4:5 looks best. 1080 × 1350 is an Instagram post, so the post artwork works as-is.
- **To edit an event:** change the text in its row in the **Events** tab. It updates on the site straight away.
- **To remove an event:** delete its row in the **Events** tab.
- Past events disappear from the site by themselves.
- Uploading a file needs a Google sign-in, and anyone with the team link can add an event, so keep that link inside the team.

If there are no upcoming events, the page shows a short "New dates landing soon" message with links to Instagram and the BRIX list.
