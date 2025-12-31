# 🔄 Workflows Guide

Step-by-step processes for daily, weekly, and monthly content operations.

---

## 📊 Overview

This system has 3 main workflows:

1. **Batch Generation** - Create 30-60 posts in one session (monthly)
2. **Daily Publishing** - Schedule and publish 2-4 posts/day (10 min)
3. **Performance Review** - Analyze and optimize (weekly/monthly)

**Time investment:**
- Month 1: ~7 hours total
- Month 3: ~5 hours total
- Month 6: ~3 hours total

**Output:**
- 60-120 posts/month
- Consistent daily presence
- Data-driven optimization

---

## 🎯 Workflow 1: Batch Generation (Monthly)

**Frequency:** Once per month
**Time:** 2-3 hours
**Output:** 60-120 posts ready to publish

### Step-by-Step Process:

#### 1. Select Infographics (15 min)

**For 2 posts/day (60 posts/month):**
- Select 15 best infographics
- 4 variations each = 60 posts

**For 4 posts/day (120 posts/month):**
- Select 30 infographics
- 4 variations each = 120 posts

**Selection criteria:**
- Mix of topics (don't pick all from same category)
- High-quality visuals
- Data-rich content
- Align with your expertise

**Organize selection:**
```
Create folder: batch-prep/2025-01/
Copy selected infographics there
```

#### 2. Research Credits (30 min)

**For each infographic:**

```bash
# Use reverse image search
# Check watermarks
# Search for text snippets
# Document in credits.json
```

**Update:** `01-infographics/credits.json`

```json
{
  "filename": "infographic-name.jpg",
  "original_author": "Author Name",
  "source_url": "https://...",
  "verified": true
}
```

**Priority:**
- High: Infographics you'll use this month
- Medium: Next month's candidates
- Low: Library backlog

#### 3. Generate Posts (60-90 min)

**Use AI tool with batch generator prompt:**

**For each infographic, use this prompt:**

```
Generate 4 LinkedIn posts using this infographic about [TOPIC].

Context from my brand voice file:
[Paste key sections from personal-brand.md]

Generate:
1. Educational post (list/tips format)
2. Data-driven post (benchmarks/numbers)
3. Hot take post (controversial insight)
4. Case study post (real example)

Infographic description:
[Describe the infographic content]

Requirements:
- Spanish/[YOUR LANGUAGE]
- Include proper credits
- Match my tone and voice
- 3-5 relevant hashtags
- Strong CTA for engagement
```

**AI generates 4 posts per infographic.**

**Save to:** `03-content-queue/2025-01/week-01/`

#### 4. Review and Edit (30-45 min)

**Quality checklist for each post:**

- [ ] Sounds like your voice (not generic AI)
- [ ] Has unique insight from your experience
- [ ] Provides actionable value
- [ ] Credits included correctly
- [ ] Hashtags relevant
- [ ] CTA invites conversation
- [ ] No typos or errors

**Edit rate expectations:**
- Month 1: 50-70% need edits
- Month 3: 20-30% need edits
- Month 6: 5-10% need edits

**As you refine your brand voice file and prompts, quality improves.**

#### 5. Organize by Week/Day (15 min)

**Option A: Weekly organization**
```
03-content-queue/2025-01/
├── week-01/
│   ├── post-01-monday-am.md
│   ├── post-02-monday-pm.md
│   ├── post-03-tuesday-am.md
│   └── ...
├── week-02/
└── ...
```

**Option B: Daily organization**
```
03-content-queue/2025-01/
├── 15-monday/
│   ├── am-educational.md
│   └── pm-hot-take.md
├── 16-tuesday/
└── ...
```

**Theme rotation (recommended):**
- Monday: Metrics/Analytics
- Tuesday: Core Topic 1
- Wednesday: Core Topic 2
- Thursday: Case Studies
- Friday: Industry Trends
- Saturday: Career Advice
- Sunday: Personal/Behind-the-scenes

#### 6. Create Posting Schedule (15 min)

**Create calendar:**

**2 posts/day schedule:**
- Post 1: 9:00 AM - Educational (with infographic)
- Post 2: 5:00 PM - Quick insight or hot take

**4 posts/day schedule (only after validation):**
- Post 1: 8:00 AM - Educational
- Post 2: 12:00 PM - Quick tip
- Post 3: 4:00 PM - Case study
- Post 4: 7:00 PM - Engagement post

**Document in:** `03-content-queue/2025-01/schedule.md`

```markdown
# January 2025 Schedule

## Week 1
- Jan 15 (Mon) 9:00 AM - Metrics educational
- Jan 15 (Mon) 5:00 PM - Retention hot take
- Jan 16 (Tue) 9:00 AM - Case study
...
```

---

## 📤 Workflow 2: Daily Publishing (Daily)

**Frequency:** Daily
**Time:** 8-10 minutes
**Output:** 2-4 posts scheduled/published

### Step-by-Step Process:

#### Option A: Batch Schedule (Recommended)

**Once per week (30 min):**

1. Open scheduling tool (Buffer, Hootsuite, or LinkedIn)
2. Open folder: `03-content-queue/2025-01/week-01/`
3. For each post:
   - Copy text
   - Attach infographic image
   - Set scheduled time
   - Add to queue
4. Review week's schedule
5. Done - autopilot for 7 days

**Advantages:**
- ✅ Consistent posting
- ✅ No daily effort
- ✅ Can batch in focused session

#### Option B: Daily Manual (Not Recommended)

**Each morning (10 min):**

1. Open today's posts folder
2. Copy post text
3. Open LinkedIn
4. Create post
5. Attach image
6. Publish or schedule
7. Repeat for second post

**Disadvantages:**
- ❌ Daily commitment required
- ❌ Higher chance of missing days
- ❌ Context switching

**Use this only if:**
- You want real-time flexibility
- You're responding to current events
- You're testing different times

---

## 📊 Workflow 3: Performance Review (Weekly/Monthly)

### Weekly Review (15 min)

**Every Sunday or Monday:**

#### 1. Check Analytics

**Track in:** `07-analytics/engagement-log.csv`

**For each post from the week:**
- Views
- Likes
- Comments
- Shares
- DMs/leads
- Follower change

**Quick spreadsheet:**
```csv
Date,Topic,Format,Views,Likes,Comments,Shares,DMs,Engagement%
2025-01-15,Metrics,Educational,1200,45,8,3,2,4.8%
2025-01-15,Retention,Hot Take,800,67,15,5,1,10.9%
...
```

**Engagement % = (Likes + Comments*2 + Shares*3) / Views * 100**

#### 2. Identify Patterns

**Questions to ask:**
- Which topics got most engagement?
- Which formats performed best?
- Which days/times were optimal?
- Which CTAs drove most comments?
- Any posts that underperformed? Why?

**Note insights in:** `07-analytics/insights.md`

```markdown
# Week of Jan 15-21

## Top Performers
1. Hot take about [X] - 10.9% engagement
2. Case study about [Y] - 8.2% engagement

## Learnings
- Controversial opinions drive 2X more comments
- Tuesday 9 AM posts get 50% more views
- Posts with questions in CTA get 3X more comments

## Adjustments for Next Week
- Add more hot takes (1 per day instead of 2 per week)
- Schedule more posts for Tuesday
- Always include question in CTA
```

#### 3. Quick Optimizations

**If something is working:**
- Create more of that format
- Post at that time more often
- Use similar topics

**If something isn't working:**
- Try different format
- Test different time
- Switch topics

---

### Monthly Review (45-60 min)

**First weekend of each month:**

#### 1. Deep Analytics Review

**Calculate monthly KPIs:**

```markdown
# January 2025 Results

## Volume
- Posts published: 60
- Time invested: 6.5 hours

## Growth
- Followers start: 850
- Followers end: 987
- Net growth: +137 (+16%)

## Engagement
- Total views: 45,230
- Total likes: 1,823
- Total comments: 287
- Total shares: 94
- Average engagement: 4.9%

## Business Impact
- DMs received: 23
- Leads generated: 8
- Meetings booked: 3

## ROI
- Leads per hour: 1.23
- Cost per lead: ~$0 (time only)
```

#### 2. Identify Best Performers

**Top 10 posts by engagement:**

```markdown
1. [Post title/topic] - 12.3% engagement
   - Why it worked: [Analysis]
   - Replicate: [Action items]

2. [Post title/topic] - 10.9% engagement
   - Why it worked: [Analysis]
   - Replicate: [Action items]

...
```

**Save top performers to:** `07-analytics/best-performers.md`

#### 3. Refine Templates

**Update post templates based on data:**

**If data shows:**
- Shorter posts (150 words) outperform long posts (300+ words)
  → Update templates to be more concise

- Questions drive 3X more engagement
  → Add more questions to CTAs

- Numbered lists get 2X more saves
  → Prioritize educational list format

**Edit templates in:** `02-templates/post-templates/`

#### 4. Refine Brand Voice

**Update brand voice file with learnings:**

**Add to:** `02-templates/brand-adapters/personal-brand.md`

```markdown
## What's Working (Based on Data)

### Hook Styles That Perform:
- "After [X years/projects]..." - 8.5% avg engagement
- "The data shows..." - 7.2% avg engagement

### CTAs That Drive Comments:
- "What's your experience with [X]?" - 3X more comments
- "Which of these [X] do you disagree with?" - 5X more comments

### Tone Adjustments:
- Controversial but respectful works better than neutral
- Specific numbers (12, 7) better than vague (many, several)
```

#### 5. Plan Next Month

**Decide on:**

- [ ] Should I scale volume? (2 → 3 or 3 → 4 posts/day)
- [ ] Which topics to double down on?
- [ ] Which formats to prioritize?
- [ ] Which posting times are optimal?
- [ ] Do I need new infographics? How many?

**Scaling decision criteria:**

**Scale from 2 → 3 posts/day IF:**
- ✅ Average engagement >3%
- ✅ Follower growth >10%/month
- ✅ No signs of audience fatigue
- ✅ Can maintain quality

**Scale from 3 → 4 posts/day IF:**
- ✅ Average engagement >4%
- ✅ Follower growth >15%/month
- ✅ High demand (lots of DMs/comments)
- ✅ Can maintain quality

**Do NOT scale if:**
- ❌ Engagement declining
- ❌ Follower growth stalling
- ❌ Comments dropping
- ❌ Quality suffering

---

## 🔄 Complete Monthly Cycle

**Month 1 Timeline:**

**Week 1:**
- Setup (2 hours) - one time
- Generate first batch (2 hours) - 30 posts
- Publish daily (10 min/day)
- Weekly review (15 min)

**Week 2:**
- Publish daily (10 min/day)
- Weekly review (15 min)

**Week 3:**
- Publish daily (10 min/day)
- Weekly review (15 min)
- Generate next batch (2 hours) - 30 more posts

**Week 4:**
- Publish daily (10 min/day)
- Weekly review (15 min)

**Month End:**
- Monthly review (60 min)
- Refine system (30 min)

**Total time: ~7 hours**
**Output: 60 posts published**

---

**Month 3+ Timeline:**

**Week 1:**
- Generate batch (90 min) - improved process
- Publish daily (automated)
- Weekly review (10 min)

**Weeks 2-4:**
- Publish daily (automated)
- Weekly review (10 min each)

**Month End:**
- Monthly review (45 min)
- Quick optimizations (15 min)

**Total time: ~4 hours**
**Output: 60-90 posts published**

---

## 📋 Workflow Checklists

### Monthly Batch Generation Checklist

- [ ] Select 15-30 infographics
- [ ] Research and update credits
- [ ] Generate 4 posts per infographic (AI)
- [ ] Review and edit posts
- [ ] Organize by week/day
- [ ] Create posting schedule
- [ ] Load into scheduling tool

**Time: 2-3 hours**

---

### Weekly Scheduling Checklist

- [ ] Open scheduling tool
- [ ] Open week's content folder
- [ ] Schedule all 14-28 posts
- [ ] Attach images to each
- [ ] Set correct times
- [ ] Review full week schedule
- [ ] Done for 7 days

**Time: 30 min**

---

### Weekly Analytics Checklist

- [ ] Export data from LinkedIn
- [ ] Update engagement-log.csv
- [ ] Calculate engagement rates
- [ ] Identify top 3 performers
- [ ] Identify bottom 3 performers
- [ ] Note insights
- [ ] Make 1-2 quick adjustments

**Time: 15 min**

---

### Monthly Review Checklist

- [ ] Calculate all KPIs
- [ ] Identify top 10 posts
- [ ] Analyze what worked / didn't work
- [ ] Update templates based on data
- [ ] Update brand voice file
- [ ] Decide on scaling (if applicable)
- [ ] Plan topics for next month
- [ ] Generate next month's content

**Time: 60-90 min**

---

## 🎯 Success Metrics by Month

### Month 1 (Validation)
- ✅ 60 posts published
- ✅ 3%+ average engagement
- ✅ +100 followers
- ✅ 5-10 leads generated
- ✅ <7 hours invested

### Month 3 (Optimization)
- ✅ 60-90 posts published
- ✅ 4%+ average engagement
- ✅ +300 followers total
- ✅ 20-30 leads generated total
- ✅ <5 hours/month invested

### Month 6 (Scaling)
- ✅ 90-120 posts published
- ✅ 5%+ average engagement
- ✅ +500 followers total
- ✅ 50+ leads generated total
- ✅ <4 hours/month invested
- ✅ System mostly automated

---

## ⚠️ Common Workflow Problems

### Problem: Can't Keep Up with Daily Publishing

**Solution:**
- Use scheduling tool (Buffer, Hootsuite)
- Batch schedule weekly, not daily
- Reduce volume (4 → 3 or 3 → 2 posts/day)

### Problem: Running Out of Content

**Solution:**
- Generate 2 months ahead instead of 1
- Expand infographic library
- Reuse top performers after 90 days
- Create new infographics

### Problem: Engagement Declining

**Solution:**
- Review what changed
- Return to formats that worked
- Reduce posting frequency
- Refresh content mix
- Increase personal insights (less generic)

### Problem: Too Much Time on Reviews

**Solution:**
- Review weekly, not daily
- Automate data collection
- Focus on top/bottom performers only
- Use templates for note-taking

---

## 💡 Pro Tips

**Batch everything:**
- Don't generate 1 post at a time
- Don't schedule 1 post at a time
- Don't review 1 post at a time
- Batch = efficiency

**Use templates:**
- Workflow checklists
- Analytics templates
- Insight note templates
- Saves time and mental energy

**Automate ruthlessly:**
- Scheduling (Buffer, Hootsuite)
- Analytics export (LinkedIn API if available)
- Reminders (calendar)

**Track relentlessly:**
- You can't improve what you don't measure
- Weekly reviews prevent drift
- Monthly reviews drive optimization

**Iterate constantly:**
- Month 1 = validation
- Month 2 = iteration
- Month 3+ = optimization
- Never stop improving

---

**These workflows get EASIER and FASTER over time.**

**Month 1: Learning**
**Month 3: Optimizing**
**Month 6: Autopilot**

**Stick with it.** 🚀
