# Pop Clutch Coffee on Squarespace: build sheet

This rebuilds the Pop Clutch one-pager (`pop-clutch-coffee.html` in this repo) inside Pop Clutch's own Squarespace site, using normal Squarespace sections and blocks, so the shop can keep editing it themselves. Nothing here is pasted in as one big code block.

Two files do the work:

- **This sheet:** every section, top to bottom, with the blocks to add, the exact text and which photo goes where.
- **`pop-clutch-custom.css`:** paste it once into Custom CSS for the fonts, button style, checkered race flags, colored menu cards and phone tweaks.

## Before you start

**Squarespace version.** Pop Clutch's live site uses features that only exist in version 7.1 with Fluid Engine (scrolling text blocks and the zigzag section divider), so everything here is written for **7.1**. I couldn't read the site's page code to confirm it 100%. If the editor shows a drag-and-drop grid when you edit a section, you're on 7.1.

**Build it on a hidden page first.** In Pages, add a new page under **Not linked**, call it `Home new`, build everything there, then set it as the homepage once Pop Clutch likes it. Their current site stays live the whole time.

**Plan check.** Everything in this sheet works on every plan, except the optional "Open now" badge in step 14, which runs JavaScript. JavaScript in code blocks needs the **Core, Plus or Advanced** plan (or some legacy plans).

**Hours: confirm with the shop before publishing.** Their own site says Tuesday to Friday 7am–4pm, Saturday 7am–2pm, closed Sunday and Monday. A third-party listing says Monday to Saturday 7am–4pm and lists Suite C instead of Suite B. This sheet uses their own site (Suite B).

**Photos.** Use the original photos already in Pop Clutch's Squarespace image library (they're sharper). The `images/` folder in this repo has web-size copies as a backup, named the same as below.

## Step 1: Site Styles (once, sitewide)

Open **Site Styles** (the paintbrush) and set:

**Colors → Edit palette**

| Palette slot | Hex | What it is |
|---|---|---|
| Lightest | `#FBF8F1` | Paper white background |
| Light | `#F7C600` | Pop Clutch yellow |
| Accent | `#F7C600` | Yellow (buttons, links) |
| Dark | `#4A4640` | Soft black for body text |
| Darkest | `#121110` | Logo black |

Section themes used below: **Lightest 1** (paper), **Light 1** (yellow), **Darkest 1** (black). After setting the palette, open each of those themes and check that headings and text read clearly (black on paper and yellow, paper or yellow on black).

**Fonts:** Headings `Archivo`, Paragraphs `Archivo`, Buttons `Archivo`. The CSS file then narrows the headings and widens the nav.

**Buttons:** Shape **Square**. The CSS adds the black outline and offset shadow.

**Animations:** None or Fade. Keep it light so the page loads fast.

## Step 2: Paste the CSS

In the editor, open **Pages**, scroll to **Website Tools** at the bottom, click **Custom CSS**, paste all of `pop-clutch-custom.css`, and click **Save**. You can also search "Custom CSS" in the panel's search.

If the editor complains about the first `@import` line, delete just that line and save. Headings will be a bit wider, everything else stays the same.

## Step 3: Header

**Header → Edit Site Header**

- **Logo:** the Pop Clutch logo (already on their site).
- **Navigation:** links to `#about` (About Us), `#menu` (Menu), `#gallery` (Gallery), `#visit` (Hours & Visit). To make a link jump to a section, add a Link in Navigation and paste the anchor, for example `/home-new#about` while building, then `/#about` once it's the homepage.
- **Button:** on, text `Directions`, link `https://www.google.com/maps/dir/?api=1&destination=922%20New%20York%20St%20Suite%20B%2C%20Redlands%2C%20CA%2092374`, open in new tab.
- **Fixed position:** on (Basic), so the header and its checkered strip stay on top while scrolling.
- **Color theme:** Lightest 1.

The thin checkered flag strip under the header comes from the CSS, there's nothing to add.

## Step 4: Ticker (scrolling announcements)

**New blank section** · Theme **Darkest 1** · Section height **Small**, drag the grid so it's one row tall.

Add a **Scrolling** block across the full width:

- Items: `Open Tue–Fri 7am–4pm · Sat 7am–2pm` / `922 New York St. Suite B, Redlands` / `Inside Good Trouble Supply Co.` / `House made syrups` / `For the love of coffee & motorcycles`
- Design: Direction left, Speed 1x, Text style Heading, Size S, Pause on hover on.

## Step 5: Hero

**New blank section** · Theme **Light 1** (yellow) · **Anchor link: `home`** (Section settings → Anchor link) · Bottom divider: **Wave** if you like the original's wavy edge.

Blocks, left to right on desktop:

1. **Text block** (Paragraph 3, small label, top left): `Open Tue–Sat in Redlands`
2. **Text block, Heading 1**, across most of the width, three lines:
   `POP`
   `CLUTCH`
   then a **Heading 3** line: `Coffee · Redlands`
3. **Text block** (Paragraph 1): `We're a coffee cart that believes in **strength** through espresso & community.` Bold the word "strength" and the CSS turns it into a black-and-yellow highlight.
4. **Button block** `Get directions` → the Google Maps link from Step 3, **Secondary** (black).
5. **Button block** `See the menu` → `#menu`, **Tertiary** (paper).
6. **Image block** on the right: `owners.jpg` (Marshall and Kapua behind the bar under their banner). The CSS gives it the arched top. Alt text: `Kapua and Marshall, owners of Pop Clutch Coffee, behind the bar under their Pop Clutch banner`.

On mobile view (phone icon at the top of the editor), stack it: label, POP / CLUTCH, text, both buttons full width, photo last.

## Step 6: "What's in the cup" badges

**New blank section** · Theme **Lightest 1** · height Small.

Six **Text blocks** in a row (3×2 on mobile). Each has a bold first line and a small second line:

| Bold line | Small line |
|---|---|
| House made syrups | Banana, orange, strawberry & more |
| Resolute Coffee | Columbia, plus Brazil decaf |
| Summit Tea | Jasmine green or Earl Grey |
| Your milk | Whole, oat or half & half |
| Double espresso | In every signature latte |
| Riders welcome | Born from a love of motorcycles |

## Step 7: About Us

### 7a. Checkered photo strip

**New blank section** · **Anchor link: `flag-photos`** · height Small.

Four **Image blocks** in a row with a gap between each, so the checkered background (from the CSS) shows around them: `crew.jpg`, `owners.jpg`, `moto-shop.jpg`, `lounge.jpg`.

Pop Clutch's own **Our Story** page already has a checkered photo header. If that section is easier to copy, use it here instead and skip this one.

### 7b. Story

**New blank section** · Theme **Lightest 1** · **Anchor link: `about`**.

- **Text block** (Paragraph 3 label): `About us`
- **Text block, Heading 2:** `For the love of coffee & motorcycles`
- **Text block** (Paragraph 1): `Pop Clutch Coffee is all about coffee, community, and a little bit of throttle.`

Left column, **Text block**:

> **Heading 3:** We're Pop Clutch Coffee. Let's drink!
>
> Pop Clutch Coffee was born from a love of motorcycles, community, and truly great coffee. Founded by Marshall and Kapua, two passionate riders and coffee enthusiasts. The journey began years ago with a simple barista job that sparked a lifelong love for the craft of coffee. Over the years, Marshall dove deep into the world of brewing methods, flavor profiles, quality beans, and small-batch roasters, developing a palate for the artistry behind every cup.
>
> **Heading 3:** Our story
>
> It started with Marshall and Kapua, a couple of motorcycle-loving coffee nerds who dreamed of creating a space where good coffee and good vibes come together.
>
> Marshall's coffee journey kicked off behind a barista bar in the 2000s and hasn't slowed down since. From mastering pour overs to pulling perfect espresso shots at home. Add a couple of Harleys to the mix, a lot of long rides, and endless talks about "what if we opened a shop?"… and Pop Clutch Coffee was born.
>
> In 2025, thanks to family, friends, and the awesome crew at Good Trouble Supply Co. in Redlands, we rolled out our first coffee cart. Now we're here to fuel your day with craft coffee, strong community, and the spirit and freedom of the open road.
>
> **Swing by, grab a cup, hang out, and be part of the ride.**

Right column, two **Image blocks** side by side, the second set a little lower: `moto-shop.jpg` (the blacked-out Harley by the Coffee Shop flag) and `cup.jpg` (latte cup on the motorcycle book).

Below, three **Text blocks** as fact cards in a row:

| Label (Paragraph 3) | Big line (Heading 3) | Text |
|---|---|---|
| The founders | Marshall & Kapua | Two passionate riders and coffee enthusiasts. |
| Rolling since | 2025 | First coffee cart rolled out in Redlands with help from family, friends and Good Trouble Supply Co. |
| Home base | Good Trouble Supply Co. | A foundation for the motorcycle community in the Inland Empire. |

To give a card a background, use the block's **Design → Background** fill if your editor has it: paper for the first, yellow for the second, black for the third.

Last, a **Quote block**: `What started as a passion, turned into an idea, turned into Pop Clutch Coffee.`

## Step 8: Checkered strip 1

**New blank section** · **Anchor link: `checker-1`** · leave it empty. The CSS turns it into a checkered flag band and shrinks it to 44px.

## Step 9: "Jumpstart your grind" band

**New blank section** · Theme **Darkest 1** · one row tall.

**Scrolling** block, items: `Jumpstart your grind` (just the one item, it repeats), Text style Heading, Size L, Speed 1x.

## Step 10: Drink menu

**New blank section** · Theme **Lightest 1** · **Anchor link: `menu`**.

- **Text block** (Paragraph 3 label): `Drink menu · House made syrups`
- **Text block, Heading 2:** `What's pouring`
- **Text block** (small): `Milk: Whole · Oat · Half & Half` / `Beans: Resolute Coffee: Columbia · Brazil (Decaf)` / `Sizes: 12 oz · 16 oz`
- **Menu block**, full width. Design: **Multi-column**, currency **$Dollar**.

Their current **Menu** page already has a Menu block with these drinks. The quickest route is to open that block, copy its text, and paste it into the new one. Otherwise paste this (Squarespace's menu format: a line of `===` after each menu name, `---` after each section name, then item name, description, price):

```
Signature
===
Signature drinks are served iced in 12 oz. & 16 oz.
Banana
---
Banana Covered Chocolate
Double espresso, milk, chocolate sauce, banana syrup, banana cold foam, Ceylon cinnamon topping
$7 / $8
Banana Matcha
Matcha, milk, banana syrup, banana cold foam, Ceylon cinnamon topping
$6 / $7
Banana Latte
Double espresso, milk, banana syrup, banana cold foam, Ceylon cinnamon topping
$6 / $7
Strawberry
---
Strawberry Covered Chocolate
Double espresso, milk, chocolate sauce, strawberry syrup, strawberry cold foam, strawberry topping
$7 / $8
Strawberry Matcha
Matcha, milk, strawberry syrup, strawberry cold foam, strawberry topping
$6 / $7
Strawberry Latte
Double espresso, milk, strawberry syrup, strawberry cold foam, strawberry topping
$6 / $7
Ube
---
Ube Covered Chocolate
Double espresso, milk, chocolate sauce, sugar in the raw syrup, ube cold foam
$7 / $8
Ube Matcha
Matcha, milk, sugar in the raw syrup, ube cold foam
$6 / $7
Ube Latte
Double espresso, sugar in the raw syrup, milk, ube cold foam
$6 / $7
Orange
---
Orange Grove Latte
Double espresso, orange syrup, milk, sweet cold foam, orange blossom essence spritz
$6 / $7
Cold Brew
---
Banana Bread Cold Brew
Cold brew, banana cold foam, cinnamon topping
$5 / $6
Honey Brew
Cold brew, honey, sweet cold foam
$6 / $7
Orange Grove Cold Brew
Cold brew, house made orange syrup, sweet cold foam, orange blossom essence spritz
$6 / $7
Cold Brew Lemonade
Cold brew, lemonade
$5 / $6
The Randos
---
The Dirtiest of Chai
Double espresso, chai latte, milk, sweet cream cold foam, Ceylon cinnamon
$7 / $8
Espresso Tonic
Double espresso, tonic water
$6 / $7
Iced Tea Lemonade Strawberry Cloud
Iced tea, lemonade, strawberry syrup, strawberry cold foam, strawberry topping
$5 / $6
Classic
===
Prices shown as 12 oz / 16 oz.
Coffee
---
Cold Brew
$4 / $5
Double Espresso
$4
Latte
$5 / $6
Mocha
$6 / $7
Cappuccino
$5 / $6
Cortado
$5
Americano
$4 / $5
Tea + Other
---
Matcha Latte
$5 / $6
Chai Tea Latte
$5 / $6
Hot Tea
$3 / $4
Iced Tea
$3 / $4
Lemonade
$3 / $4
Milk
$3.50 / $4.50
Make it yours
---
Syrups
Banana · Lavender · Orange · Sugar in the Raw · Strawberry · Vanilla
$0.50
Sauces
Chocolate · Caramel · Honey · Sugar Free French Vanilla
$0.50
Cold Foam
Banana · Strawberry · Sweet Cream · Ube
$1.00
Tea
Summit Tea: Jasmine Green · Earl Grey
```

If the Classic prices show up as descriptions instead of prices (those items have no description line), copy the Classic part from their current Menu page, which already has it formatted.

The CSS colors the flavor sections in order: banana yellow, strawberry pink, ube purple, orange, cold brew brown, and The Randos black. Keep the sections in this order so the colors match.

## Step 11: Gallery

**"Good coffee / Good people" band:** new blank section, Theme **Light 1** (yellow), one row tall, **Scrolling** block with items `Good coffee` and `Good people`, Direction right.

**Gallery section:** new blank section, Theme **Lightest 1**, **Anchor link: `gallery`**.

- **Text block, Heading 2:** `Be part of the ride`
- **Text block:** `Pop Clutch Coffee & Good Trouble Supply Co. A foundation for the motorcycle community in the Inland Empire.`
- Five **Image blocks** with captions (or a Gallery block, Grid layout):

| Photo | Caption |
|---|---|
| `lounge.jpg` | The lounge |
| `iced-concha.jpg` | Iced + a pan dulce |
| `carrier.jpg` | Coffee run |
| `crew.jpg` (make this one wider) | Moto community |
| `owners.jpg` | Marshall & Kapua |

## Step 12: Hours & visit

**New blank section** · Theme **Darkest 1** · **Anchor link: `visit`** · Top divider: **Wave**.

- **Text block** (Paragraph 3 label): `Hours & location`
- **Text block, Heading 2:** `Swing by, grab a cup, hang out`

Three columns:

**Find us** (Text block): Heading 3 `Find us`, then
`922 New York St. Suite B`
`Redlands, CA 92374`
`Inside Good Trouble Supply Co.`
Then a **Button block** `Get directions` (Primary, yellow) with the Google Maps link from Step 3.

**Hours** (Text block): Heading 3 `Hours`, then
`Tuesday 7am – 4pm`
`Wednesday 7am – 4pm`
`Thursday 7am – 4pm`
`Friday 7am – 4pm`
`Saturday 7am – 2pm`
`Sunday Closed`
`Monday Closed`
Small text: `Hours could vary based on private events happening at the shop or for unforeseen circumstances. Follow us on Instagram for updates.`
(Confirm these hours with the shop first, see the top of this sheet.)

**Get in touch** (Text block): Heading 3 `Get in touch`, then `info@popclutchcoffee.com` linked as an email, then a **Social links** block with Instagram, Facebook, Yelp and Linktree (Squarespace pulls these from Settings → Social links, which their site already has).

## Step 13: eGift cards & rewards

**New blank section** · Theme **Light 1** (yellow) · **Anchor link: `rewards`**.

Two columns:

- Heading 3 `eGift cards` · text `Send someone a coffee run. Pop Clutch eGift cards are sold online and land straight in their inbox.` · Button `Buy an eGift card` (Secondary) → `https://app.squareup.com/gift/MLQXA6TZWRZPC/order`
- Heading 3 `Customer rewards` · text `Sign up for Pop Clutch rewards and earn on every visit.` · Button `Join rewards` (Tertiary) → `https://squareup.com/customer-programs/enroll/XtS7j9NtG1qb`

## Step 14: Finish line

**New blank section** · **Anchor link: `finish-line`** · one row tall · one **Text block** centered:
`Finish line: Let's drink!` (Paragraph 1). The CSS draws the big checkered band and turns the text into a yellow tag.

**Mobile action bar (all plans):** in this same section, add a **Code block**, set it to **HTML**, and paste:

```html
<nav class="pc-actionbar" aria-label="Quick actions">
  <a href="https://www.google.com/maps/dir/?api=1&destination=922%20New%20York%20St%20Suite%20B%2C%20Redlands%2C%20CA%2092374" target="_blank" rel="noopener">Directions</a>
  <a href="#menu">Menu</a>
  <a href="#visit">Hours</a>
</nav>
```

It's invisible on desktop. On phones it pins a black Directions / Menu / Hours bar to the bottom of the screen. HTML-only code blocks work on every plan.

**Optional "Open now" badge (Core, Plus or Advanced plan only):** this needs JavaScript. If their plan allows it, add a Code block in the hero (Step 5) instead of the plain `Open Tue–Sat in Redlands` text:

```html
<p id="pc-status" style="display:inline-block;background:#121110;color:#F7C600;padding:8px 14px;font:800 13px/1 Archivo,Arial,sans-serif;text-transform:uppercase;letter-spacing:.06em">Open Tue–Sat in Redlands</p>
<script>
(function(){
  var H={2:[7,16],3:[7,16],4:[7,16],5:[7,16],6:[7,14]};
  var N=["Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"];
  function f(h){return (h>12?h-12:h)+(h>=12?"pm":"am");}
  try{
    var p={};new Intl.DateTimeFormat("en-US",{timeZone:"America/Los_Angeles",weekday:"short",hour:"numeric",minute:"numeric",hour12:false}).formatToParts(new Date()).forEach(function(x){p[x.type]=x.value;});
    var d=["Sun","Mon","Tue","Wed","Thu","Fri","Sat"].indexOf(p.weekday),t=(parseInt(p.hour,10)%24)+parseInt(p.minute,10)/60,el=document.getElementById("pc-status"),h=H[d];
    if(h&&t>=h[0]&&t<h[1]){el.textContent="Open now · until "+f(h[1])+" today";}
    else if(h&&t<h[0]){el.textContent="Closed now · opens today at "+f(h[0]);}
    else{for(var i=1;i<=7;i++){var n=(d+i)%7;if(H[n]){el.textContent="Closed now · opens "+(i===1?"tomorrow":N[n])+" at "+f(H[n][0]);break;}}}
  }catch(e){}
})();
</script>
```

If the hours change, update the numbers on the `var H=` line too (24-hour clock: `[7,16]` means 7am to 4pm; 2 = Tuesday … 6 = Saturday).

## Step 15: Footer

**Edit Footer** · Theme **Lightest 1**.

- Logo image (the Pop Clutch logo)
- Text: `Pop Clutch Coffee · 922 New York St. Suite B, Redlands, CA 92374` / `For the love of coffee & motorcycles.`
- Links: About Us (`/#about`), Menu (`/#menu`), Hours (`/#visit`), Instagram
- Their current site's big yellow `POP CLUTCH COFFEE` footer line can stay; it fits this design.

## Step 16: Check it, then go live

1. Preview on desktop and on the phone view in the editor. Check: checkered strip under the header, the checker bands, the colored menu cards, the bottom bar on phones.
2. Tap each nav link and the bottom bar buttons to make sure they jump to the right sections.
3. When Pop Clutch is happy: Pages → `Home new` → settings → **Set as Homepage**. Their old homepage stays in Pages, so they can switch back.

## If something doesn't look right

- **A section's style is missing:** its anchor name is probably spelled differently. Anchors must match the CSS exactly: `home`, `flag-photos`, `about`, `checker-1`, `checker-2`, `menu`, `gallery`, `visit`, `rewards`, `finish-line`.
- **Menu cards aren't colored or the tabs look plain:** Squarespace may use different class names for the Menu block on this site. The menu still works; send me a screenshot and I'll adjust the selectors.
- **Headings aren't narrow:** the font `@import` didn't load. Delete that line from Custom CSS; headings fall back to regular Archivo.
- **A second checkered strip** (`checker-2`) can go anywhere else you want a flag band, for example between Gallery and Hours.
