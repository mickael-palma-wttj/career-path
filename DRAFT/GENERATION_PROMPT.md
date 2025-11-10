# IC Evaluation Rubric Generation Prompt

Use this prompt with Claude or another AI to generate detailed rubric documents for specific career levels and criteria.

---

## Template Prompt

```
You are an expert in creating career development rubrics and technical evaluation frameworks. 
I need you to create a detailed rubric document for the following:

**Career Level**: [INSERT_LEVEL]
**Criteria**: [INSERT_CRITERIA]
**Subsection (if applicable)**: [INSERT_SUBSECTION]
**Weight**: [INSERT_WEIGHT]%

The document should follow this exact structure:

# [Criteria Name]

[1-2 sentence description of what this criterion measures and its importance]

[Context about the progression and what it represents in the career journey]

**Progression Scale**:

[List the progression ratings from the raw_weights.csv for this level and all previous levels]

**Weight**:

[Weight]% of [Section] competency

<aside>
🧭

[A brief, inspiring description (2-3 sentences) of what being good at this means]

</aside>

## **🫆 Key characteristics**

[5-7 bullet points describing the essential traits and behaviors for this level]

## **📚 Specific behaviors & examples**

### **✅ What good looks like**

[5-7 bullet points with descriptive examples]

### Examples

[3-5 concrete, detailed examples with:
- Context/scenario
- What the person does/says
- If relevant, code samples or artifacts
- How it demonstrates the criterion
Format as nested bullets with code blocks where appropriate]

## **⚙️ Development actions**

[4-6 themed tracks for how to develop this skill, each with 3-4 sub-points]

## **🏆 Success metrics**

[5-7 observable metrics that indicate someone is succeeding at this criterion]

## **❓ Assessing readiness for promotion**

### **Current level validation**

[3-4 key questions to determine if someone is currently meeting this criterion]

### **Next level readiness questions**

[3-4 themes, each with 2-3 specific interview/assessment questions to evaluate readiness for the next level]

### **Evidence to look for**

[5-7 bullet points describing what evidence should be collected]

## **🚀 Next steps toward [next level]**

[3-5 specific growth areas and capabilities needed to progress]

## **💡 Practical ways to [demonstrate this criterion]**

[4-5 practical, actionable approaches with 2-3 examples each]

## **⚠️ Common pitfalls to avoid**

[5-7 bullet points with brief explanations of what NOT to do]

## **🌟 Building [skill name] skills**

[4-5 development areas, each with 2-3 actionable steps]
```

---

## How to Use This Prompt

### Step 1: Gather Information from CSV
From the `IC_evaluation_grid_template - raw_weights.csv`, find:
- The **Level** (e.g., "Junior Developer", "Senior Developer", "Principal Developer")
- The **Criteria** (e.g., "Writing Code", "Communication", "Testing")
- The **Subsection** if it exists (e.g., "Quality", "Testing your code")
- The **Weight** percentage
- The **Description** from the CSV
- The **Role Model Rating** for progression context

### Step 2: Fill in the Template
Replace the bracketed placeholders:
- `[INSERT_LEVEL]` → e.g., "Junior Developer"
- `[INSERT_CRITERIA]` → e.g., "Advocating for Testing"
- `[INSERT_SUBSECTION]` → e.g., "Testing" (or omit if top-level)
- `[INSERT_WEIGHT]` → e.g., "50"

### Step 3: Provide Context to the AI
Include additional details like:
- The role model rating for this level and adjacent levels
- What the previous level looked like (for comparison)
- Specific technologies or examples relevant to your organization
- Any organizational context (team size, product type, etc.)

### Example Complete Request

```
You are an expert in creating career development rubrics. Create a detailed rubric document for:

**Career Level**: Senior Developer
**Criteria**: Technical Understanding & Prioritisation
**Subsection**: Understanding Code
**Weight**: 55%

Context from our evaluation grid:
- Junior Developer rating: 1.4
- Confirmed Developer rating: 2.2
- Senior Developer rating: 2.2
- Staff Developer rating: 3.4

Description from our template:
"You understand a good amount of the team's domain, and can gain sufficient context 
to work productively within that." (Confirmed Developer)

For Senior: "You understand your team's domain at a high level, including the breadth 
of services, how they interact, and data flows between systems. You understand adjacent 
domains as they affect your team."

Our organization:
- Backend-focused engineering team
- Microservices architecture with 15+ services
- Python and Go primary languages
- Team of 8-12 engineers

Please follow the rubric structure provided in the template prompt above.
```

---

## Tips for Best Results

1. **Be specific about your organization**
   - Company size, industry, technology stack
   - Team structure and size
   - Products or services

2. **Include the progression context**
   - What was expected at the previous level?
   - What comes next at the higher level?

3. **Provide real examples if possible**
   - Specific project types
   - Common challenges in your domain
   - Tools and technologies you use

4. **Customize the tone**
   - Adjust formality level based on your culture
   - Modify emojis/formatting if needed
   - Add organizational-specific language

5. **Iterate**
   - Use the generated rubric as a starting point
   - Refine with your team's feedback
   - Adjust examples to match real scenarios

---

## Customization Ideas

### Different Formats
- Adjust emoji usage (e.g., remove if too informal)
- Change section headings to match your style
- Modify the aside/callout box styling

### Additional Sections You Could Add
- **Common mistakes** that hold people back
- **Related skills** that support this criterion
- **Timeline** - expected time to progress to next level
- **External resources** - books, courses, communities
- **Tools & templates** - specific artifacts to use
- **Peer feedback guide** - how to give feedback on this criterion

### Organizational Variations
- Add **business context** - why this matters to company goals
- Include **customer/stakeholder impact** - how this affects others
- Add **compliance or regulatory context** if relevant
- Include **team-specific expectations** or variations
