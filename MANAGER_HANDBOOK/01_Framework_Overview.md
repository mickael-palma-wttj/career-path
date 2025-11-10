# Framework Overview: Understanding the IC Evaluation Grid

This guide explains how the IC Career Development Framework works, how to interpret the evaluation grid, and how to use it effectively with your team.

---

## 📊 The Evaluation Grid Structure

The framework evaluates Individual Contributors across **3 core pillars**, broken down into **specific criteria**, with **different weights at each career level**.

### Data Source
All data lives in: [`IC_evaluation_grid_template - raw_weights.csv`](../IC_evaluation_grid_template%20-%20raw_weights.csv)

---

## 🏛️ The 3 Pillars

### 1. Engineering Craft (Technical Excellence)
**Weight:** 40-70% depending on level

The core technical capabilities that make someone an effective engineer.

**Categories:**
- **Writing Code** - Code quality, documentation, language proficiency
- **Testing** - Testing practices, coverage, quality assurance
- **Technical Understanding & Prioritisation** - Domain knowledge, work breakdown
- **Software Architecture** - Design patterns, system thinking
- **Security** - Security principles, data handling
- **Debugging & Monitoring** - Troubleshooting, observability

**Why it matters:** This is the foundation. Strong technical craft enables everything else.

**How weight changes:**
- **Junior/Confirmed:** 65-70% - Building technical foundation
- **Senior/Staff:** 55-65% - Proven technical ability, expanding influence
- **Senior Staff/Principal:** 40-60% - Technical excellence assumed, organizational impact becomes primary

---

### 2. Soft Skills (Collaboration & Communication)
**Weight:** 25-40% depending on level

The interpersonal capabilities that make someone an effective team member and collaborator.

**Categories:**
- **Empathy & Humility** - Understanding others, sharing credit
- **Communication** - Clarity, timeliness, stakeholder management
- **Initiative** - Self-direction, problem-solving, follow-through
- **Objectivity & Adaptability** - Decision-making, handling change
- **Business Acumen** - Understanding business context and impact

**Why it matters:** Technical skill without collaboration capability limits impact and scope.

**How weight changes:**
- **Junior/Confirmed:** 25-30% - Learning to work effectively with others
- **Senior/Staff:** 30-40% - Collaboration becomes crucial for broader impact
- **Senior Staff/Principal:** 40% - Organizational influence requires exceptional soft skills

---

### 3. Leadership (Influence & Impact)
**Weight:** 5-20% depending on level

The ability to influence, guide, and develop others, whether or not you're a people manager.

**Categories:**
- **Hiring & Org Design** - Recruiting, building teams
- **Stakeholder Management** - Setting expectations, protecting teams
- **Team Leadership** - Reliability, difficult conversations
- **Developing Others** - Mentoring, coaching, feedback
- **Culture & Togetherness** - Building positive environments

**Why it matters:** Senior ICs multiply their impact by influencing and enabling others.

**How weight changes:**
- **Junior:** 5% - Minimal expectation, focus on learning
- **Confirmed:** 5% - Beginning to help others
- **Senior:** 10% - Expected to mentor and lead by example
- **Staff:** 20% - Leading across teams, significant influence
- **Senior Staff/Principal:** 20% - Shaping organizational direction

---

## 📏 The Rating Scale

### Understanding Ratings: 0.0 to 4.0+

| Rating | Descriptor | What It Means | Typical Level |
|--------|-----------|---------------|---------------|
| **0.0** | Not Applicable | This criterion doesn't apply at this level | Junior (for advanced criteria) |
| **0.5 - 1.0** | Developing | Learning, needs significant guidance and support | Junior |
| **1.0 - 1.5** | Basic Competency | Can do this with help, inconsistent | Junior → Confirmed |
| **1.5 - 2.0** | Competent | Reliable performance with occasional support | Confirmed |
| **2.0 - 2.5** | Proficient | Consistent, independent execution | Confirmed → Senior |
| **2.5 - 3.0** | Strong | Consistently excellent, beginning to mentor | Senior |
| **3.0 - 3.5** | Expert | Deep expertise, influences multiple teams | Staff → Senior Staff |
| **3.5 - 4.0** | Authority | Organization-wide impact and influence | Senior Staff → Principal |
| **4.0+** | Industry Leader | External reputation, pushing field forward | Principal |

### Important Notes on Ratings

**✅ Ratings Are Contextual**
- A 2.0 in "Writing Code Quality" for a Senior means something different than for a Junior
- Always read the full criterion description, not just the number

**✅ No One Is Perfect**
- It's normal to have variation across criteria
- Strengths in some areas, development opportunities in others
- The overall pattern matters more than any single rating

**✅ 0.0 ≠ Bad**
- For Junior Developers, many advanced criteria show 0.0
- This means "not expected at this level," not "failing"
- Example: Junior Developers have 0.0 for "Mentoring" in many areas—that's appropriate

---

## ⚖️ Understanding Weights

Weights determine the relative importance of each criterion within its section.

### How Weights Work

```
Engineering Craft (70% of Junior Developer evaluation)
  ├── Writing Code (45% of Engineering Craft = 31.5% of total)
  │   ├── Quality (50% of Writing Code = 15.75% of total)
  │   ├── Documentation (25% of Writing Code = 7.875% of total)
  │   └── Language (25% of Writing Code = 7.875% of total)
  ├── Testing (15% of Engineering Craft = 10.5% of total)
  └── ...
```

### Reading Weights in the CSV

The CSV has several weight columns:
- **"Role model Rating"** - The benchmark rating for this level/criterion
- **"Weights"** - The percentage this criterion counts within its parent section

**Example from CSV:**
```
Junior Developer, ENGINEERING CRAFT, Writing Code, Quality
Role model Rating: 1.2
Weights: 50%
```

This means:
- At Junior level, a "role model" junior scores 1.2 on Code Quality
- Code Quality is 50% of the Writing Code category
- Writing Code is 45% of Engineering Craft
- Engineering Craft is 70% of Junior Developer evaluation

---

## 🎯 How to Use the Framework

### For Individual Assessment

**Step 1: Identify Current Level**
Look up the IC's current career level in the CSV (Junior, Confirmed, Senior, etc.)

**Step 2: Review Role Model Ratings**
For each criterion at that level, note the "role model" rating. This is what "good" looks like.

**Step 3: Gather Evidence**
Collect specific examples of the IC's behaviors and outcomes:
- Code reviews and technical artifacts
- Peer feedback and collaboration patterns
- Project outcomes and impact
- Observable behaviors in meetings, discussions, etc.

**Step 4: Assess Against Criteria**
For each criterion, ask:
- Does the IC consistently demonstrate behaviors at or above the role model rating?
- Are there patterns of strength or areas needing development?
- What specific examples support this assessment?

**Step 5: Look at the Pattern**
- Where are the strengths?
- Where are development opportunities?
- Does the overall pattern align with the level, or are they performing above/below?

### For Promotion Evaluation

**To evaluate promotion readiness, assess:**

1. **Consistency at Current Level**
   - Performing at role model level across most criteria?
   - Any significant gaps at current level?

2. **Demonstration of Next Level**
   - Already showing behaviors from the next level?
   - In which areas specifically?
   - How consistently?

3. **Readiness Timing**
   - How long have they demonstrated next-level behaviors?
   - Minimum 3-6 months of consistent demonstration
   - Multiple projects/contexts showing the pattern

**Rule of Thumb:**
Someone is ready for promotion when they're already performing at that level consistently, not when they have potential to perform at that level.

---

## 📖 Reading the CSV File

### Column Structure

| Column | What It Contains |
|--------|------------------|
| **key** | Unique identifier (LevelSection combo) |
| **Order** | Sorting order (0-82) |
| **Level** | Career level (Junior Developer, etc.) |
| **Section** | Main pillar (ENGINEERING CRAFT, SOFT SKILLS, LEADERSHIP) |
| **Subsection** | Category within section (Writing Code, Testing, etc.) |
| **Criteria** | Specific criterion (Quality, Documentation, etc.) |
| **Role model Rating** | Benchmark rating for this level |
| **Weights** | Percentage importance |
| **Description** | What good looks like at this level |

### Example Row Interpretation

```csv
Junior Developer, ENGINEERING CRAFT, Writing Code, Quality, 1.2, 50%, 
"Your code has always followed correct convention, requiring only minor improvements.
You've made trade-offs knowingly."
```

**Translation:**
- **Level:** Junior Developer
- **What:** Code Quality (within Writing Code, within Engineering Craft)
- **Benchmark:** 1.2 (Basic competency with some support)
- **Importance:** 50% of Writing Code criteria
- **Expectation:** Code follows conventions, makes reasonable trade-offs, needs minor improvements

---

## 🔍 Practical Examples

### Example 1: Assessing a Junior Developer on Testing

**From CSV:**
- **Testing** → **Testing your code**
- Role Model Rating: 2.0
- Weight: 70% of Testing
- Description: "You consistently write solid unit tests, sometimes with help from more senior engineers."

**Manager's Assessment:**
1. **Observe:** Does the IC write tests for their code?
2. **Check:** Are the tests covering edge cases and happy paths?
3. **Ask:** Do they need prompting, or do they do it proactively?
4. **Review:** Do they seek help when needed?

**Evidence Collected:**
- ✅ Last 5 PRs all included tests
- ✅ Tests covered main functionality
- ⚠️ Missed some edge cases, but corrected after code review
- ✅ Asked senior engineer for help with async testing

**Conclusion:** Performing at 1.8-2.0 range—solid performance for Junior level.

---

### Example 2: Evaluating Senior → Staff Promotion

**Key Question:** Is this Senior already performing like a Staff developer?

**Check the Staff level criteria:**
1. **Engineering Craft:** 
   - Staff rating ~3.0-3.4 range
   - Influence across multiple teams
   - Deep domain expertise

2. **Soft Skills:**
   - Staff rating ~2.8-3.3 range
   - Bridge communication across teams
   - Drive initiatives beyond own team

3. **Leadership:**
   - Staff rating ~1.6-2.7 range
   - Active mentoring of senior engineers
   - Stakeholder management at higher levels

**Evidence to Collect:**
- Are they already leading cross-team initiatives?
- Do other teams seek their technical guidance?
- Have they mentored multiple engineers to higher levels?
- Do they demonstrate business acumen in technical decisions?

**Decision Framework:**
- If consistently demonstrating Staff behaviors for 6+ months → Ready
- If showing potential but not yet consistent → Create development plan
- If performing at Senior level well → Continue at Senior, no urgency

---

## 🚨 Common Mistakes to Avoid

### ❌ Treating Numbers as Absolute
**Wrong:** "You need to hit exactly 2.5 in every criterion."  
**Right:** "The pattern shows strengths in X and opportunities in Y. Let's focus on Y for next quarter."

### ❌ Comparing ICs to Each Other
**Wrong:** "Sarah is at 3.0 on this, and you're at 2.5."  
**Right:** "For Senior level, we're looking for 2.5-3.0. You're solidly in that range."

### ❌ Expecting Perfection
**Wrong:** "You need to be perfect across all criteria before promotion."  
**Right:** "You're strong in most areas. Let's work on these 2-3 specific development areas."

### ❌ Ignoring Context
**Wrong:** "The framework says 2.0, so you're exactly there."  
**Right:** "Given the complexity of the projects you've tackled, you're performing above the 2.0 benchmark."

### ❌ Using Framework as a Weapon
**Wrong:** "You're only at 1.5 here, which is below standard."  
**Right:** "This area is a development opportunity. Here's what I'd like to see, and here's how I can support you."

---

## ✅ Framework Best Practices

### 1. **Use It as a Conversation Tool**
The framework should enable dialogue, not replace it. Use it to:
- Create shared language
- Make expectations explicit
- Identify development opportunities
- Track progress over time

### 2. **Collect Evidence Continuously**
Don't wait for review time. Throughout the year:
- Note specific examples of behaviors
- Save artifacts (code, docs, presentations)
- Collect peer feedback regularly
- Document impact and outcomes

### 3. **Focus on Patterns, Not Perfection**
- Look at overall trends, not single instances
- Consider multiple data points over time
- Weight recent performance more heavily
- Allow for bad days/projects

### 4. **Be Transparent**
- Share the framework with your ICs
- Discuss where they are and why
- Explain what "next level" looks like
- Make criteria visible and accessible

### 5. **Calibrate with Peers**
- Discuss assessments with fellow managers
- Ensure consistency across teams
- Reality-check your interpretations
- Learn from others' examples

---

## 🔄 Framework Updates & Evolution

This framework is a living document. You should:

### Regularly Review
- Does this still reflect our organizational needs?
- Are weights appropriate for our context?
- Do descriptions match our actual expectations?

### Gather Feedback
- From ICs: Is this clear and helpful?
- From managers: Is this practical and usable?
- From leadership: Does this align with strategy?

### Adapt as Needed
- Update examples to reflect current work
- Adjust weights if priorities shift
- Add new criteria if roles evolve
- Archive outdated content

---

## 📚 Additional Resources

### For Deeper Understanding
- Review [`CRITERIA_RUBRICS/`](../CRITERIA_RUBRICS/) for detailed criterion explanations
- Read [`CAREER_LEVEL_GUIDES/`](../CAREER_LEVEL_GUIDES/) for level-specific guidance
- Study case studies in [`CASE_STUDIES/`](../CASE_STUDIES/)

### For Practical Use
- Templates in [`TOOLS_TEMPLATES/`](../TOOLS_TEMPLATES/)
- Common scenarios in [`FAQS_BY_SCENARIO/`](../FAQS_BY_SCENARIO/)
- Practical guides in [`PRACTICAL_GUIDES/`](../PRACTICAL_GUIDES/)

---

## 🎯 Quick Reference

### The Framework in One Page

**3 Pillars:**
1. Engineering Craft (40-70%) - Technical ability
2. Soft Skills (25-40%) - Collaboration & communication
3. Leadership (5-20%) - Influence & impact

**Rating Scale:**
- 0.0-1.0: Developing (Junior)
- 1.0-2.0: Competent (Confirmed)
- 2.0-3.0: Proficient (Senior)
- 3.0-3.5: Expert (Staff/Senior Staff)
- 3.5-4.0: Authority (Principal)

**Key Principles:**
- Evidence-based assessment
- Focus on patterns, not perfection
- Transparency builds trust
- Promotion = already performing at next level
- Continuous feedback > annual reviews

---

**Next:** Read [`02_Career_Levels_Guide.md`](02_Career_Levels_Guide.md) for an overview of all 7 career levels.
