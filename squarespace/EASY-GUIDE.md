# Your new Pop Clutch homepage: an easy step-by-step guide

Hi Marshall and Kapua! This guide walks you through building the new Pop Clutch homepage yourselves, inside your own Squarespace site. You don't need to know any code. Every step is one small action, and after each part you'll see what it should look like.

You'll build the new page on a hidden practice page first, and only swap it in when you're happy. One heads-up: Parts 2 and 3 (colors, fonts and the design file) change the look of your whole site, including the pages that are live now, as soon as you click **Save**. Do them at a quiet time, and plan to finish the new page soon after.

## Before you start

- **Use a computer, not a phone.** The Squarespace phone app can't do all of these steps.
- **Set aside about 2 hours.** You can stop and come back anytime, as long as you click **Save** first.
- **Have your real hours ready.** This guide shows the hours from your current website as an example. Type in whatever your hours really are.
- **Keep this link handy.** It has the one file you'll copy and paste:
  https://github.com/StayChwispyIG/Pop-Clutch-Coffee/blob/main/squarespace/pop-clutch-custom.css

## A few words you'll see

- **Section:** a full-width band of the page, like the yellow top part or the black hours part. The page is a stack of sections.
- **Block:** one piece of content inside a section: a text box, a photo, a button, a menu.
- **Site Styles:** the paintbrush menu where you set colors, fonts and button shapes for the whole site.
- **Section theme:** the color scheme of one section (for example, black background with light text).
- **Anchor link:** a short name you give a section, like `menu`. The menu buttons use it to jump to that section. It also tells the design file which section to decorate, so type each one exactly as shown.
- **Custom CSS:** a box in Squarespace where you paste the design file. It adds the checkered flags, colored menu cards and other touches.
- **Code block:** a block that holds a small piece of code. You'll use one, for the phone menu bar.

## Three moves you'll repeat

You'll do these over and over, so here they are once:

**Add a section**

1. Hover your mouse over the page where you want the new section.
2. Click the **Add Section** button that appears.
3. At the top of the list, click **Add a Blank Section**.

**Give a section its settings (theme and anchor link)**

1. Hover over the section and click the pencil icon on its right side (**Edit Section**).
2. Under **Colors**, click the theme the guide names.
3. Find **Anchor Link** and type the name the guide gives, all lowercase, exactly as written.
4. Click anywhere outside the panel to close it.

**Add a block**

1. While editing a section, click **Add Block** (top left of the section).
2. Pick the block type the guide names (Text, Image, Button and so on).
3. Drag the block where you want it. Drag its corners to resize it.

When you add a **Text** block, the toolbar above it has a style menu (it usually says *Paragraph 2*). That's where you choose **Heading 1**, **Heading 2**, **Heading 3** or a **Paragraph** size.

---

## Part 1: Make a hidden practice page

1. Log in at squarespace.com and click your Pop Clutch site.
2. Click **Website**, then **Pages**.
3. Scroll to the **Not linked** heading and click the **+** next to it.
4. Click **Page**, then **Blank**.
5. Name it `Home new` and press Enter.
6. Hover over the page preview on the right and click **Edit**.

**You should see:** an empty page with your header and footer. Nobody can find this page on your site yet.

## Part 2: Set your colors, fonts and buttons

1. While editing, click the paintbrush icon at the top right (**Site Styles**).
2. Click **Colors**.
3. At the top, click the row of color circles (**Edit palette**).
4. Click each circle and type its code:

   | Circle | Type this | What it is |
   |---|---|---|
   | Lightest | `#FBF8F1` | Paper white |
   | Light | `#F7C600` | Pop Clutch yellow |
   | Accent | `#F7C600` | Yellow again |
   | Dark | `#4A4640` | Soft black |
   | Darkest | `#121110` | Logo black |

5. Click the back arrow, then click **Fonts**.
6. Set **Headings**, **Paragraphs** and **Buttons** to **Archivo**.
7. Click the back arrow, then click **Buttons**, and set **Shape** to **Square**.
8. Click **Save** at the top left.

**You should see:** your site's colors change to the yellow, cream and black of the new design. Older pages may look a little different too, and that's normal. Check one or two of them.

## Part 3: Paste the design file

**Copy it from GitHub:**

1. Open the link from "Before you start" in a new browser tab.
2. Above the code, on the right, click the button that looks like two overlapping squares (**Copy raw file**).

   If you don't see it, click **Raw** instead. Press **Ctrl+A** (Mac: **Cmd+A**) to select everything, then **Ctrl+C** (Mac: **Cmd+C**) to copy it.

**Paste it into Squarespace:**

3. Back in Squarespace, click **Website**, then **Pages**.
4. Scroll all the way down to **Website Tools** and click **Custom CSS**. On some accounts this is under **Design**, then **Custom CSS**.
5. Click inside the big box and press **Ctrl+V** (Mac: **Cmd+V**) to paste.
6. Click **Save**.

**You should see:** a thin black-and-white checkered strip under your header. Headings get bolder and narrower. The rest shows up as you build the sections.

## Part 4: Build the page, top to bottom

Work on your `Home new` page. For each section below, do the three moves: **add a section**, **give it its settings**, then **add the blocks**. Click **Save** after each section.

### Section 1: Scrolling announcement bar

- **Theme:** Darkest 1. **Anchor link:** none.
1. In **Edit Section**, under **Format**, set the height to **Small**.
2. Add a **Scrolling** block and stretch it across the full width.
3. Click the block and type these items, one per line:
   `Open Tue–Fri 7am–4pm · Sat 7am–2pm` (your real hours)
   `922 New York St. Suite B, Redlands`
   `Inside Good Trouble Supply Co.`
   `House made syrups`
   `For the love of coffee & motorcycles`
4. In the block's **Design** settings, set direction to **left** and speed to **1x**.

**You should see:** a black bar with text gliding across it.

### Section 2: The big yellow welcome

- **Theme:** Light 1 (yellow). **Anchor link:** `home`
1. Add a **Text** block, set to **Paragraph 3**: `Open Tue–Sat in Redlands`
2. Add a **Text** block, set to **Heading 1**, with two lines: `POP` and `CLUTCH`. Make it big, across most of the section.
3. Under it, add a **Text** block, set to **Heading 3**: `Coffee · Redlands`
4. Add a **Text** block, set to **Paragraph 1**: `We're a coffee cart that believes in strength through espresso & community.`
5. Select the word **strength** and click **B** to make it bold. The design turns it into a black-and-yellow highlight.
6. Add a **Button** block. Set the text to `Get directions`, then paste this link: `https://www.google.com/maps/dir/?api=1&destination=922%20New%20York%20St%20Suite%20B%2C%20Redlands%2C%20CA%2092374`. Turn on **Open in new tab**. Set its style to **Secondary**.
7. Add a **Button** block. Set the text to `See the menu` and the link to `#menu`. Set its style to **Tertiary**.
8. Add an **Image** block on the right and pick the photo of the two of you behind the bar.

**You should see:** a yellow section with huge POP CLUTCH lettering, a black button, a cream button, and your photo with a rounded arch on top.

### Section 3: What's in the cup

- **Theme:** Lightest 1. **Anchor link:** none.
1. Add six small **Text** blocks in a row. In each one, type the first line, make it bold, then type the second line under it:

   | Bold line | Second line |
   |---|---|
   | House made syrups | Banana, orange, strawberry & more |
   | Resolute Coffee | Columbia, plus Brazil decaf |
   | Summit Tea | Jasmine green or Earl Grey |
   | Your milk | Whole, oat or half & half |
   | Double espresso | In every signature latte |
   | Riders welcome | Born from a love of motorcycles |

### Section 4: Checkered photo strip

- **Theme:** any. **Anchor link:** `flag-photos`
1. Add four **Image** blocks in a row, leaving a small gap between each one. Use your crew photo, the photo of the two of you, the Harley by the Coffee Shop flag, and the lounge.

**You should see:** your four photos sitting on a checkered race flag background.

### Section 5: About us

- **Theme:** Lightest 1. **Anchor link:** `about`
1. Add a **Text** block, set to **Paragraph 3**: `About us`
2. Add a **Text** block, set to **Heading 2**: `For the love of coffee & motorcycles`
3. Add a **Text** block on the left for your story. Paste in the text from your **Our Story** page (open that page, select its text, copy it, and paste it here).
4. Add two **Image** blocks on the right: the Harley by the Coffee Shop flag, and the latte on the motorcycle book.
5. Add a **Quote** block: `What started as a passion, turned into an idea, turned into Pop Clutch Coffee.`

### Section 6: Checkered flag band

- **Anchor link:** `checker-1`
1. Leave it empty. Don't add any blocks.

**You should see:** a thin checkered race flag band across the page.

### Section 7: "Jumpstart your grind" bar

- **Theme:** Darkest 1. **Anchor link:** none.
1. Set the height to **Small**.
2. Add a **Scrolling** block with one item: `Jumpstart your grind`

### Section 8: Drink menu

- **Theme:** Lightest 1. **Anchor link:** `menu`
1. Add a **Text** block, set to **Paragraph 3**: `Drink menu · House made syrups`
2. Add a **Text** block, set to **Heading 2**: `What's pouring`
3. Add a **Text** block with three lines:
   `Milk: Whole · Oat · Half & Half`
   `Beans: Resolute Coffee: Columbia · Brazil (Decaf)`
   `Sizes: 12 oz · 16 oz`
4. Copy your current menu:
   1. In another tab, open your current **Menu** page and click **Edit**.
   2. Double-click the menu, click inside its text, and press **Ctrl+A** then **Ctrl+C** (Mac: **Cmd+A**, **Cmd+C**).
   3. Close that page without changing anything.
5. Back on `Home new`, add a **Menu** block across the full width.
6. Double-click it, click inside its text, press **Ctrl+A** to select the sample text, then **Ctrl+V** to paste your menu over it.
7. In the block's **Design** settings, pick **Multi-column**.

Keep the flavor groups in this order: Banana, Strawberry, Ube, Orange, Cold Brew, The Randos. The design colors them in that order: yellow, pink, purple, orange, brown, then black.

If your menu needs re-typing, the full menu text is in `BUILD-SHEET.md`, Step 10, in the same folder as this guide.

**You should see:** each flavor group in its own colored, rounded card.

### Section 9: "Good coffee / Good people" bar

- **Theme:** Light 1 (yellow). **Anchor link:** none.
1. Set the height to **Small**.
2. Add a **Scrolling** block with two items: `Good coffee` and `Good people`. Set its direction to **right**.

### Section 10: Gallery

- **Theme:** Lightest 1. **Anchor link:** `gallery`
1. Add a **Text** block, set to **Heading 2**: `Be part of the ride`
2. Add a **Text** block: `Pop Clutch Coffee & Good Trouble Supply Co. A foundation for the motorcycle community in the Inland Empire.`
3. Add five **Image** blocks. Click each one and add a caption:

   | Photo | Caption |
   |---|---|
   | The lounge | `The lounge` |
   | Iced drink with a pan dulce | `Iced + a pan dulce` |
   | Drink carrier | `Coffee run` |
   | Crew photo (make this one wider) | `Moto community` |
   | The two of you | `Marshall & Kapua` |

### Section 11: Hours & visit

- **Theme:** Darkest 1. **Anchor link:** `visit`
1. Add a **Text** block, set to **Heading 2**: `Swing by, grab a cup, hang out`
2. Make three columns of **Text** blocks:
   - **Column 1:** Heading 3 `Find us`, then `922 New York St. Suite B`, `Redlands, CA 92374` and `Inside Good Trouble Supply Co.` Under it, add a **Button** block `Get directions` with the same Google Maps link as Section 2, style **Primary**.
   - **Column 2:** Heading 3 `Hours`, then one line per day with **your real hours**. Under that, in smaller text: `Hours could vary based on private events happening at the shop or for unforeseen circumstances. Follow us on Instagram for updates.`
   - **Column 3:** Heading 3 `Get in touch`. Then type `info@popclutchcoffee.com`, select it, click the link button, and choose **Email**. Under it, add a **Social Links** block, which shows your Instagram, Facebook and other icons automatically.

**You should see:** a black section with yellow headings.

### Section 12: Gift cards & rewards

- **Theme:** Light 1 (yellow). **Anchor link:** `rewards`
1. Make two columns:
   - **Left:** a Heading 3 `eGift cards`, the text `Send someone a coffee run. Pop Clutch eGift cards are sold online and land straight in their inbox.`, and a **Button** `Buy an eGift card` (style **Secondary**) linked to `https://app.squareup.com/gift/MLQXA6TZWRZPC/order`
   - **Right:** a Heading 3 `Customer rewards`, the text `Sign up for Pop Clutch rewards and earn on every visit.`, and a **Button** `Join rewards` (style **Tertiary**) linked to `https://squareup.com/customer-programs/enroll/XtS7j9NtG1qb`

### Section 13: Finish line

- **Anchor link:** `finish-line`
1. Set the height to **Small**.
2. Add one **Text** block in the middle: `Finish line: Let's drink!`

**You should see:** a big checkered band with a yellow tag in the middle that says "Finish line: Let's drink!"

## Part 5: Add the phone menu bar

This adds a black bar with **Directions**, **Menu** and **Hours** buttons to the bottom of the screen on phones. It works on every Squarespace plan.

1. In the **Finish line** section, click **Add Block**, then **Code**.
2. Double-click the code block and delete the sample text inside it.
3. Make sure the menu above the box says **HTML**.
4. Copy and paste this, exactly as it is:

```html
<nav class="pc-actionbar" aria-label="Quick actions">
  <a href="https://www.google.com/maps/dir/?api=1&destination=922%20New%20York%20St%20Suite%20B%2C%20Redlands%2C%20CA%2092374" target="_blank" rel="noopener">Directions</a>
  <a href="#menu">Menu</a>
  <a href="#visit">Hours</a>
</nav>
```

5. Click outside the box, then click **Save**.

**You should see:** nothing new on a computer, which is correct. You'll check it on a phone in Part 6.

## Part 6: Check it

1. Click the phone icon at the top of the editor to see the phone version.
2. Look for the black **Directions / Menu / Hours** bar at the bottom.
3. Scroll through the whole page. If something is squished on the phone view, drag it into place. Changes you make here only affect phones.
4. Click **Save**, then **Exit**.
5. On your own phone, open the page: your website address followed by `/home-new`.
6. Tap **Menu** and **Hours** on the bottom bar to make sure they jump to the right spots.

## Part 7: Make it your homepage

Do this only when you're both happy with it.

1. Click **Website**, then **Pages**.
2. Hover over **Home new** and click the gear icon (**Page settings**).
3. Click **Set as Homepage**.
4. Optional: put your **About Us**, **Menu** and **Hours** links in the top menu. In **Pages**, click the **+** next to your main menu, choose **Link**, and use `/#about`, `/#menu` and `/#visit`.

**You should see:** the new page when you visit your site's main address. Your old homepage is still in **Pages** if you ever want it back.

---

## If something looks wrong

- **A section has no checkered flags or special colors:** its anchor link is probably misspelled. Open **Edit Section** and check it's exactly one of these, all lowercase: `home`, `flag-photos`, `about`, `checker-1`, `menu`, `gallery`, `visit`, `rewards`, `finish-line`.
- **Headings aren't narrow and bold:** the special font didn't load. Open **Custom CSS** and delete just the first line (it starts with `@import`). Click **Save**. Headings will be a little wider, and everything else stays the same.
- **The colors are off:** go back to **Site Styles**, then **Colors**, then **Edit palette**, and recheck the five codes in Part 2. Then open each section's **Edit Section** and recheck its theme.
- **Menu cards aren't colored:** the menu still works fine. Send Chwispy a screenshot and he'll adjust the design file.
- **The bottom bar shows on a computer or not on a phone:** make sure the code block is set to **HTML** and you pasted the whole thing, from `<nav` to `</nav>`.
- **You pasted the design file twice:** open **Custom CSS**, select everything, delete it, and paste it again once.

## How to undo

- **Undo your last change:** press **Ctrl+Z** (Mac: **Cmd+Z**) while editing.
- **Turn off the whole new design:** open **Custom CSS**, select everything, delete it, and click **Save**. Your site goes back to plain Squarespace styling. Paste the file again anytime to bring it back.
- **Go back to your old homepage:** **Pages**, hover over your old home page, gear icon, **Set as Homepage**.
- **Start the practice page over:** hover over `Home new` in **Pages**, click the trash can, and begin again at Part 1. Your colors and design file stay in place.

## If your hours change later

Update them in two places: the scrolling bar at the top (Section 1) and the **Hours** column (Section 11).

Questions? Send Chwispy a screenshot of what you see, and he'll help.
