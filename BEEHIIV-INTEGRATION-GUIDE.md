# Beehiiv × New Life Capital Partners
## Complete Integration & Content Automation Guide

> **Your role in this system: minimal.** There is one setup phase that takes about 15–20 minutes — done once, never again. After that, Claude writes, schedules, and publishes everything. Articles go live on your website and land in subscriber inboxes automatically.

---

## How the System Works (Plain English)

You have a Beehiiv account. Beehiiv is your content command center — it stores your articles, manages your subscriber list, and sends email newsletters. Your website (newlifecapitalpartners.com on GitHub Pages) is where the public reads those articles. The two are connected via two bridges:

1. **Beehiiv's RSS feed** automatically feeds published articles into your website's Insights section — no manual copy-paste, no uploading.
2. **Beehiiv's embed form** lets website visitors subscribe to your newsletter with a single click.

Claude operates as your SEO specialist and content writer through Beehiiv's API. When it's time for a new article, Claude writes it, formats it for SEO, and publishes or schedules it directly into Beehiiv — which then triggers everything else automatically.

---

## PART 1 — One-Time Setup (You Do This Once)

This is everything you personally need to do. Each step is self-contained and clearly marked with how long it takes.

---

### STEP 1 — Confirm Your Beehiiv Plan (2 minutes)

The API access Claude needs is available on Beehiiv's **Scale plan** ($99/month) or higher. The free and Launch plans do not include API access.

**What to check:**
1. Log in at [app.beehiiv.com](https://app.beehiiv.com)
2. Click your profile icon → **Settings** → **Billing**
3. Confirm your current plan

**If you're on the free or Launch plan:** Upgrade to Scale to unlock the API. The Scale plan is worth it — it also unlocks advanced analytics, custom automations, and unlimited posts.

> 💡 The RSS feed (which feeds articles to your website) is available on ALL plans. So if you want a simpler setup without API access for now, we can use a manual-publish workflow and still automate the website side.

---

### STEP 2 — Get Your Beehiiv API Key (3 minutes)

This is the "password" Claude uses to publish articles on your behalf. You generate it once and share it privately.

**Steps:**
1. In Beehiiv, go to **Settings** (gear icon, bottom left)
2. Click **Integrations** in the left sidebar
3. Scroll to **API Keys** section
4. Click **Generate New API Key**
5. Give it a name: `Claude Content Writer`
6. Copy the key — it looks like: `bh_api_xxxxxxxxxxxxxxxxxxxxx`
7. Keep it in a safe place (like a password manager)

**Important:** The API key is shown only once. If you close the window, you'll need to generate a new one.

---

### STEP 3 — Find Your Publication ID (1 minute)

This is your Beehiiv publication's unique identifier. Claude needs it to know which publication to publish to.

**Steps:**
1. Go to your Beehiiv publication dashboard
2. Look at the URL in your browser — it looks like:
   `https://app.beehiiv.com/p/pub_XXXXXXXXXXXXXXXX`
3. The part that starts with `pub_` is your Publication ID
4. Copy it and save it alongside your API key

---

### STEP 4 — Share Your Credentials With Claude (1 minute)

In a new chat message, simply send Claude the following:

> "Here are my Beehiiv credentials:
> API Key: [paste your key]
> Publication ID: [paste your pub_xxx]"

Claude will store these securely in project memory and use them going forward. You will never need to provide them again in this project.

---

### STEP 5 — Set Up Your Beehiiv Publication Profile (10 minutes)

Before Claude starts publishing, configure a few things in Beehiiv's settings:

**A. Publication Name & Description**
- Settings → Publication → Name: `New Life Capital Partners Insights`
- Description: `Real estate education, market strategy, and investment insights for savvy investors and property owners.`
- Category: Real Estate

**B. Sender Information (for newsletters)**
- Settings → Email → From Name: `New Life Capital Partners`
- From Email: `info@newlifecapitalpartners.com` (verify this — Beehiiv will send a verification email)
- Reply-to: `info@newlifecapitalpartners.com`

**C. Custom Domain for Beehiiv (Optional but recommended)**
If you want your Beehiiv publication to be accessible at `insights.newlifecapitalpartners.com` instead of the default Beehiiv URL:
- Settings → Publication → Custom Domain
- Enter: `insights.newlifecapitalpartners.com`
- Follow Beehiiv's instructions to add a CNAME record in your domain's DNS settings (takes ~10 min, done through your domain registrar — Claude can walk you through this if needed)

**D. Email Sending Schedule**
- Settings → Sending → Default send day/time
- Recommended: **Tuesday at 9:00 AM Central** (highest open rates for B2B real estate content)

---

### STEP 6 — Claude Wires Up the Website (Automatic — No Action Needed)

Once you share your credentials, Claude will:

1. **Add the RSS feed reader to your Insights page** — Articles from Beehiiv automatically appear on your website within minutes of publishing. No manual updates needed.
2. **Embed the Beehiiv subscribe form** — A newsletter signup section is added to your website so visitors can subscribe directly.
3. **Push the changes to GitHub** — The website updates automatically via your existing GitHub Pages setup.
4. **Test the connection end-to-end** — Claude will publish a test draft and verify it appears on the website.

This entire step takes Claude about 30–45 minutes and requires nothing from you except sharing the credentials in Step 4.

---

## PART 2 — The Ongoing Content Workflow (Fully Automated)

After setup, this is how the system runs week to week. Your involvement: review if you want to, otherwise nothing.

---

### How Claude Operates as Your Content Specialist

Claude will create and maintain a **content calendar** aligned to your business strategy. Every article serves a purpose — educating potential investors, establishing authority, improving search rankings, and building your subscriber list.

**Content pillars (mapped to your Insights categories):**

| Category | What It Covers | Audience |
|---|---|---|
| Market Trends | Cap rates, local market data, economic indicators | Active investors |
| Property Acquisition | Deal analysis, due diligence, negotiation | Buyers & flippers |
| Property Management | Tenant relations, maintenance, profitability | Landlords & owners |
| Investing 101 | First-time investor education, terminology, concepts | New investors |

**Publishing cadence (recommended):**
- 2 articles per week (Tuesday and Thursday)
- 1 newsletter per week (Tuesday, bundles the week's article + brief market insight)
- 1 in-depth piece per month (long-form, pillar content for SEO)

---

### What Happens When an Article Is Published

Here is the exact sequence — nothing manual required after setup:

1. **Claude writes the article** — SEO-optimized headline, meta description, structured headings, internal links, keyword targeting for real estate searches relevant to your market.
2. **Claude publishes via API** — Article goes into Beehiiv as a scheduled post at the optimal day and time.
3. **Beehiiv sends the newsletter** — At the scheduled time, Beehiiv emails the article to every subscriber.
4. **RSS feed updates** — Your website's Insights section pulls the new article within minutes.
5. **Article is live** — A visitor on your website sees the article. If they subscribe, they're added to Beehiiv and receive future newsletters.

---

### How to Request a Specific Article

Any time you want a specific topic covered, simply message Claude:

> "Write an article about [topic] — [any context, angle, or specific points you want included]"

Claude will write it, optimize it for SEO, and publish or schedule it. No further action needed from you.

---

## PART 3 — Beehiiv Platform Overview

Here's a quick reference for the Beehiiv interface so you can navigate it confidently.

---

### Key Areas of Beehiiv

**Dashboard** — Your overview. Shows recent posts, subscriber growth, and engagement metrics.

**Posts** — All your articles. Statuses: Draft, Scheduled, Published. Claude manages all of these.

**Audience** — Your subscriber list. You can see who subscribed, when, and how they engaged.

**Email** — Where you configure how newsletters look and are delivered. Claude handles the content; you control the branding.

**Analytics** — Open rates, click-through rates, subscriber growth over time. Review this monthly to see what's resonating.

**Automations** — Advanced: can trigger emails based on subscriber behavior (e.g., welcome email when someone subscribes). Claude can set these up for you.

**Monetization** — Beehiiv's built-in feature if you ever want to add a paid tier or premium content. Not needed now, but good to know it exists.

---

### Beehiiv Subscriber Forms

Beehiiv gives you an embed code for a signup form. It looks like this:

```html
<iframe src="https://embeds.beehiiv.com/[your-form-id]" 
  data-test-id="beehiiv-embed" 
  width="100%" height="320" frameborder="0" scrolling="no">
</iframe>
```

Claude will copy this into the right place on your website during setup (Step 6). You don't need to touch any code.

---

## PART 4 — Content Strategy (How Claude Thinks About Your Articles)

---

### SEO Approach

Every article Claude writes targets specific search terms your ideal clients use when searching Google. For New Life Capital Partners, the focus is:

- Geographic: Louisiana, Baton Rouge area real estate (based on your business location)
- Intent-based: People researching investment properties, property management, passive income through real estate
- Education-first: Articles that answer real questions — Google rewards depth and usefulness

**Example target keywords Claude will build articles around:**
- "how to analyze a rental property investment"
- "what is cap rate in real estate"
- "property management tips for landlords"
- "passive income through real estate investing"
- "how to buy investment property with little money down"

---

### Article Structure (Every Time)

Each article Claude writes follows this structure for maximum readability and SEO:

1. **Headline** — Contains the target keyword. Clear, compelling, specific.
2. **Meta description** — 155 characters for Google search results.
3. **Introduction** — Hooks the reader, states what they'll learn.
4. **Body** — Organized with H2 and H3 subheadings, 1,000–2,000 words.
5. **Key Takeaways** — Bullet summary for skimmers.
6. **Call to Action** — Soft prompt to subscribe or contact New Life Capital Partners.
7. **Tags** — Mapped to your four category pillars.

---

### First Three Articles (Planned)

Once credentials are provided, Claude will start with these three high-impact articles to launch the Insights section with substance:

**Article 1:** *"The 5 Financial Metrics Every Real Estate Investor Must Understand Before Buying a Property"*
— Target: Investing 101 / first-time investors, high SEO demand

**Article 2:** *"What Baton Rouge's 2025 Rental Market Means for Property Owners"*
— Target: Market Trends / local authority content

**Article 3:** *"From Single-Family to Portfolio: How New Life Capital Partners Approaches Property Acquisition"*
— Target: Property Acquisition / brand storytelling + SEO

---

## PART 5 — Frequently Asked Questions

---

**Q: What if I don't like an article Claude published?**
Every article can be edited or unpublished directly in Beehiiv's Posts section. You can also message Claude: "Edit the article about [X] to change [Y]." Claude will update it via the API.

**Q: Can I approve articles before they go live?**
Yes. Claude can be configured to save every article as a **Draft** in Beehiiv instead of scheduling it. You'd then log in, review it, and click "Schedule" or "Send" yourself. Just let Claude know if you prefer this workflow.

**Q: What if someone unsubscribes?**
Beehiiv handles this automatically. Unsubscribes are instant and comply with CAN-SPAM law. You don't need to do anything.

**Q: Can subscribers reply to newsletters?**
Yes — replies go to your configured reply-to email (info@newlifecapitalpartners.com). This is a great opportunity for lead generation.

**Q: Will the Insights section of my website look different from the rest of the site?**
No. Claude will match the styling of your existing Insights page. Articles will display in the same card format as the current design, just automatically populated from Beehiiv.

**Q: What if Beehiiv is down or the API isn't available?**
The website will simply show whatever articles were last loaded. Claude can also save articles directly to the website's HTML files as a backup. No content is ever lost.

**Q: Can I grow my subscriber list other ways?**
Absolutely. Beehiiv has a referral program, a recommendations network, and you can share your signup link (e.g., `newlifecapitalpartners.beehiiv.com/subscribe`) on social media, in email signatures, and in your other communications. Claude can create a "Subscribe" page for your website as well.

---

## PART 6 — Summary Checklist

### Your One-Time Tasks:
- [ ] Confirm you're on Beehiiv Scale plan (or upgrade)
- [ ] Generate API Key in Beehiiv → Settings → Integrations
- [ ] Copy your Publication ID from the Beehiiv URL
- [ ] Share both with Claude in a message
- [ ] Configure your Publication Profile (name, email, sender info)
- [ ] Verify your sending email address (Beehiiv sends you a verification link)

### Claude Does the Rest:
- [ ] Wires RSS feed into your Insights page
- [ ] Embeds the subscribe form on the website
- [ ] Pushes changes to GitHub → site goes live
- [ ] Publishes first three articles
- [ ] Sets content calendar for ongoing publishing
- [ ] Manages SEO, scheduling, and newsletter sending indefinitely

---

*Guide version 1.0 — New Life Capital Partners × Claude Content System*
*Last updated: May 2026*
