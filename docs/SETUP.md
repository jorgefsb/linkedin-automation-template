# 📖 Setup Guide

Complete setup instructions for the LinkedIn Content Automation System.

---

## ⚡ Prerequisites

**Required:**
- AI tool access (Claude, ChatGPT, or similar)
- 10+ infographics or visual content to analyze
- LinkedIn account (obviously)

**Recommended:**
- Scheduling tool (Buffer, Hootsuite, or LinkedIn native)
- Image editing tool (Canva, Figma) for creating infographics
- Spreadsheet for tracking analytics

**Not Required:**
- Coding skills
- Design expertise
- Large budget

---

## 🚀 Step-by-Step Setup

### Step 1: Clone or Download This Template

```bash
# Option A: Clone with git
git clone https://github.com/[your-username]/linkedin-automation-template
cd linkedin-automation-template

# Option B: Download ZIP from GitHub
# Extract to your preferred location
```

---

### Step 2: Add Your Infographics

**Where to add them:**
```
01-infographics/categorized/
├── metrics/           # Add your metrics/data infographics here
├── topic-1/           # Rename to YOUR topic
├── topic-2/           # Rename to YOUR topic
└── ...
```

**How many do you need?**
- **Minimum:** 10-15 infographics to start
- **Comfortable:** 30-50 infographics
- **Ideal:** 100+ infographics

**Math:**
- 1 infographic → 4-8 posts
- 15 infographics = 60-120 posts
- = 1-2 months of content at 2-4 posts/day

**File naming convention:**
```
[topic]-[short-description].jpg

Examples:
metrics-12-key-kpis.jpg
framework-product-market-fit.png
case-study-company-growth.jpg
```

---

### Step 3: Customize Your Brand Voice

**Edit:** `02-templates/brand-adapters/personal-brand-TEMPLATE.md`

**Replace all [brackets] with your information:**

```markdown
### Personality:
- **Your expertise:** [e.g., "15+ years in software engineering"]
- **Your role:** [e.g., "Senior Product Manager at TechCo"]
- **Your approach:** [e.g., "Pragmatic problem solver"]
```

**Define your tone:**
```markdown
✅ [Your characteristic 1: e.g., "Direct and actionable"]
✅ [Your characteristic 2: e.g., "Data-driven"]
✅ [Your characteristic 3: e.g., "Friendly but professional"]

❌ [What to avoid 1: e.g., "Corporate jargon"]
❌ [What to avoid 2: e.g., "Overly technical without context"]
```

**Add your common phrases:**
```markdown
Common phrases you use:
- "[Your phrase 1: e.g., 'After X years in Y...']"
- "[Your phrase 2: e.g., 'Here's what I learned...']"
- "[Your phrase 3: e.g., 'The key insight is...']"
```

**Save this file** - it will be used to adapt all AI-generated content to your voice.

---

### Step 4: Update Categories for Your Niche

**Current categories (example - game industry):**
```
01-infographics/categorized/
├── metrics/
├── game-design/
├── retention/
├── monetization/
├── roblox/
├── marketing/
├── career/
└── business/
```

**YOUR categories should match YOUR industry:**

**Example for SaaS:**
```
├── metrics/
├── product-strategy/
├── user-onboarding/
├── pricing/
├── growth/
├── marketing/
├── career/
└── business/
```

**Example for Marketing:**
```
├── metrics/
├── content-strategy/
├── seo/
├── paid-ads/
├── social-media/
├── conversion/
├── career/
└── business/
```

**Rename folders:**
```bash
cd 01-infographics/categorized/
mv game-design/ YOUR-TOPIC-1/
mv retention/ YOUR-TOPIC-2/
# etc.
```

---

### Step 5: Track Content Credits

**Edit:** `01-infographics/credits-EXAMPLE.json`

**Save as:** `credits.json` (remove -EXAMPLE)

**For each infographic, add:**

```json
{
  "filename": "your-infographic.jpg",
  "category": "metrics",
  "original_author": "Author Name (if known)",
  "source_url": "https://...",
  "twitter_handle": "@author",
  "linkedin_handle": "linkedin.com/in/author",
  "license": "Creative Commons BY / All Rights Reserved / Unknown",
  "notes": "Where you found it, context, etc.",
  "verified": true,
  "research_priority": "high"
}
```

**Research tips:**
- Use reverse image search (Google Images, TinEye)
- Check watermarks on images
- Search for text snippets from the infographic
- Ask in relevant communities

**Why this matters:**
- Professional integrity
- Avoids legal issues
- Builds network with original creators
- Community goodwill

---

### Step 6: Customize Post Templates (Optional)

**Current templates work out-of-the-box, but you can customize:**

**Edit templates in:** `02-templates/post-templates/`

**Available templates:**
1. `educational.md` - Lists, tips, frameworks
2. `data-driven.md` - Benchmarks, numbers, ranges
3. `hot-take.md` - Controversial opinions
4. `case-study.md` - Real examples, analysis

**Customize:**
- Hook styles
- Body structure
- CTA patterns
- Hashtag strategy

**Or keep them as-is** - they're designed to work generically.

---

### Step 7: Generate Your First Batch

**Use the batch generator prompt with your AI tool:**

**Input to AI (e.g., Claude, ChatGPT):**

```
Generate 4 LinkedIn posts using this infographic about [TOPIC].

Context:
- I'm a [YOUR ROLE] with expertise in [YOUR AREAS]
- My audience is [WHO THEY ARE]
- My tone is [YOUR TONE]

Use the template at: 06-prompts/batch-generator.md

Include my brand voice from: 02-templates/brand-adapters/personal-brand.md

Generate:
1. Educational post
2. Data-driven post
3. Hot take post
4. Case study post

[Describe the infographic or attach image]
```

**AI will generate 4 posts** in different formats from the same infographic.

---

### Step 8: Review and Refine

**Quality checklist:**

- [ ] Does it sound like YOU (not generic AI)?
- [ ] Is there a unique insight from your experience?
- [ ] Is the tone consistent with your brand?
- [ ] Does it provide actionable value?
- [ ] Does the CTA invite real conversation?
- [ ] Are all sources credited properly?
- [ ] Are hashtags relevant to your audience?

**Save approved posts to:** `03-content-queue/2025-01/week-01/`

---

### Step 9: Publish and Track

**Schedule posts:**
- Use LinkedIn native scheduling OR
- Use Buffer, Hootsuite, etc.

**Recommended schedule (2 posts/day):**
- Post 1 (9:00 AM): Educational long-form with infographic
- Post 2 (5:00 PM): Quick insight or hot take

**Track in:** `07-analytics/engagement-log.csv`

**Metrics to track:**
- Views
- Likes
- Comments
- Shares
- DMs/leads generated
- Follower growth

---

### Step 10: Iterate Based on Data

**After 2 weeks (30 posts):**

**Review analytics:**
- Which topics get most engagement?
- Which formats perform best?
- Which times/days are optimal?

**Refine your approach:**
- Double down on high performers
- Adjust templates based on what works
- Update brand voice if needed

**Scale when ready:**
- Start: 2 posts/day
- After validation: 3 posts/day (if engagement >3%)
- After optimization: 4 posts/day (if engagement >4%)

---

## 🔧 Advanced Configuration

### Translation Setup (If Needed)

**Edit:** `06-prompts/translator.md`

**Customize for your target language:**
- Replace "español mexicano" with your dialect
- Adjust cultural references
- Modify tech term handling

### Multi-Brand Setup (Optional)

**If you manage multiple brands:**

1. Create brand adapters for each:
   - `brand-adapters/brand-a.md`
   - `brand-adapters/brand-b.md`

2. Use `06-prompts/brand-adapter.md` to generate variations

3. Never mix brands without clear separation

---

## 📋 Folder Organization Tips

**Monthly organization:**
```
03-content-queue/
├── 2025-01/
│   ├── week-01/
│   │   ├── monday/
│   │   ├── tuesday/
│   │   └── ...
│   ├── week-02/
│   └── ...
└── 2025-02/
```

**Or daily organization:**
```
03-content-queue/
├── 2025-01-15/
├── 2025-01-16/
└── ...
```

**Choose what works for you.**

---

## ⚠️ Common Issues

### Issue 1: Posts Don't Sound Like You

**Solution:**
- Spend more time on brand voice file
- Add more of YOUR characteristic phrases
- Include examples of your best posts
- Be more specific about tone

### Issue 2: Low Engagement

**Solution:**
- Test different post formats
- Experiment with posting times
- Try different topics
- Engage more in comments
- Make CTAs more specific

### Issue 3: Running Out of Content

**Solution:**
- Expand infographic library
- Reuse old posts (after 3+ months)
- Create new infographics
- Curate from other sources (with credits)

### Issue 4: AI Output Too Generic

**Solution:**
- Provide more context to AI
- Use more specific prompts
- Include examples of your voice
- Edit generated content before publishing

---

## ✅ Setup Complete Checklist

- [ ] Repo downloaded/cloned
- [ ] 10+ infographics added and categorized
- [ ] Brand voice file customized
- [ ] Categories renamed for your niche
- [ ] Credits system setup
- [ ] First batch generated (10+ posts)
- [ ] 2-3 posts published
- [ ] Analytics tracking started
- [ ] Engagement monitored

**Once all checked: You have a working content factory!**

---

## 🚀 Next Steps

After setup:
1. See `WORKFLOWS.md` for daily/weekly processes
2. See `CUSTOMIZATION.md` for advanced tweaks
3. See `FAQ.md` for common questions

---

**Questions? Issues? Suggestions?**
- Check FAQ.md
- Review template examples
- Modify prompts gradually
- Share your learnings with the community

---

**Setup time: 1-2 hours**
**Result: 1-2 months of content ready to publish**

**Let's go!** 🚀
