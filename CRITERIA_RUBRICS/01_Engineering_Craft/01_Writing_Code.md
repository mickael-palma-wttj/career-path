# Writing Code

**Criterion:** The ability to write clean, maintainable, efficient code that follows standards and best practices.

---

## 📋 Quick Summary

| Level | Expectation |
|-------|-------------|
| **Developing (0.0-1.0)** | Writing code with guidance; needs review for quality issues |
| **Competent (1.0-2.0)** | Writing working code reliably; minor quality issues caught in review |
| **Proficient (2.0-3.0)** | Writing clean, maintainable code consistently; sets good examples |
| **Expert (3.0-3.5)** | Code exemplifies best practices; mentors others on code quality |
| **Authority (3.5-4.0)** | Defines coding standards; influences org-wide code quality practices |

---

## 🎯 Definition

**Writing Code** means producing well-crafted source code that is:
- **Readable** - Easy for others (and yourself) to understand
- **Maintainable** - Can be modified with low risk of bugs
- **Efficient** - Performs well within system constraints
- **Consistent** - Follows agreed-upon standards and patterns
- **Testable** - Designed to be easily tested

This criterion evaluates both the technical quality of code and the care taken in producing it. It's not about raw speed or output volume, but about code that compounds in value over time through clarity and correctness.

---

## 📊 Level-by-Level Breakdown

### Level 0.0-1.0: Developing
**What You See:**
- Code works but often has quality issues
- Needs significant review feedback to meet standards
- Doesn't consider long-term maintainability
- May have variable naming, organization issues
- Quick-and-dirty solutions are default approach

**Typical Statements:**
- "I got it working!"
- "It works on my machine"
- "We can clean it up later"
- "I didn't know we had a standard for that"

**Manager's Focus:**
- Teach coding standards and patterns
- Model reviewing code for readability, not just correctness
- Provide specific feedback on quality issues
- Set clear expectations for code standards
- Pair on code to demonstrate good practices

---

### Level 1.0-2.0: Competent
**What You See:**
- Code generally works and meets basic quality standards
- Mostly follows coding conventions once explained
- Some refactoring needed, but generally maintainable
- Shows growing awareness of code quality
- Improving with feedback on style/standards

**Typical Statements:**
- "Should I follow the naming convention in X file?"
- "I tried to make it readable"
- "Is this the way we usually do it?"
- "What would you change in this code?"

**Manager's Focus:**
- Point to examples of great code in your codebase
- Give feedback on patterns and organization
- Start conversations about design choices
- Encourage thinking about future maintainability
- Gradually increase expectations

---

### Level 2.0-3.0: Proficient
**What You See:**
- Code is clean and well-organized by default
- Follows standards naturally, not by checklist
- Good variable naming, consistent structure
- Considers maintainability in design choices
- Code exemplifies how it "should" be written
- Teammates point to their code as example

**Typical Statements:**
- "I refactored that because..."
- "Following the pattern we used in X"
- "I named this to be clear about its purpose"
- "What would make this easier for the next person?"

**Manager's Focus:**
- Celebrate and highlight their code as example
- Ask them to review others' code
- Use their PRs as teaching material
- Challenge them to teach standards to juniors
- Move toward architecture-level thinking

---

### Level 3.0-3.5: Expert
**What You See:**
- Code is exceptionally clean and well-organized
- Demonstrates deep knowledge of patterns and best practices
- Makes sophisticated design choices
- Mentors others on code quality
- Identifies and fixes quality issues across codebase
- Others ask their advice on "how should this be structured?"

**Typical Statements:**
- "Let me show you a better way to structure this"
- "This pattern would make future changes easier"
- "I'd refactor this part to..."
- "Here's what concerns me about this design"

**Manager's Focus:**
- Use them to set coding standards
- Have them lead code quality initiatives
- Ask them to establish patterns/conventions
- Use their code as training material
- Involve in architecture decisions

---

### Level 3.5-4.0: Authority
**What You See:**
- Defines how code is written in the organization
- Influences org-wide code quality standards
- Creates tools, guidelines, or systems for better code
- Drives adoption of best practices
- Others reference their code as gold standard
- Visible impact on entire codebase quality

**Typical Statements:**
- "We should establish this as a team standard"
- "Let me create a guide for this pattern"
- "I've built tooling to help with this"
- "Here's how we should approach this at scale"

**Manager's Focus:**
- Leverage expertise for org-wide improvements
- Support leading code quality initiatives
- Challenge with architecture-level problems
- Amplify their standards-setting work
- Consider for technical leadership roles

---

## 🔍 How It Manifests in Work

### Code Structure & Organization
| Level | Appearance |
|-------|-----------|
| Developing | Functions are long; unclear organization; mixed concerns |
| Competent | Generally organized; mostly follows patterns with guidance |
| Proficient | Well-organized; clear structure; easy to navigate |
| Expert | Exceptionally organized; reusable patterns; elegant solutions |
| Authority | Defines organization and structure for the team |

### Naming & Clarity
| Level | Appearance |
|-------|-----------|
| Developing | Ambiguous names ("x", "temp", "thing1"); unclear intent |
| Competent | Generally clear names; some missing context |
| Proficient | Clear, intentional names; self-documenting code |
| Expert | Names reveal design intent; sophisticated naming patterns |
| Authority | Names set standard for org; educates others on naming |

### Efficiency & Optimization
| Level | Appearance |
|-------|-----------|
| Developing | Often inefficient; multiple passes when one would work |
| Competent | Generally efficient; occasional optimization opportunities |
| Proficient | Balanced efficiency and readability; good trade-offs |
| Expert | Optimal solutions that remain readable and maintainable |
| Authority | Defines efficiency expectations and optimization patterns |

### Consistency & Standards
| Level | Appearance |
|-------|-----------|
| Developing | Inconsistent with codebase; different style each file |
| Competent | Mostly follows standards; occasional misses |
| Proficient | Consistently follows all standards; second nature |
| Expert | Sets and refines standards; shows others how/why |
| Authority | Defines standards; ensures org-wide adoption |

---

## ❓ Assessment Questions

**For yourself (when reviewing code):**
- Is the purpose of this code immediately clear?
- Could I modify this without confusion?
- Does this follow our patterns and standards?
- Is there unnecessary complexity or wasted effort?
- Would a new team member understand this?
- Does this show care and intentionality?

**For conversation:**
- Walk me through the structure of this code. Why did you organize it this way?
- What standards were you following here?
- How would you approach maintaining this code 6 months from now?
- What part of this code are you most proud of? Why?
- If you saw this pattern elsewhere, would you refactor it?

**For feedback:**
- What would you change about this code if you wrote it today?
- How does this compare to [reference code]?
- What would make this easier for someone else to modify?

---

## 👀 Evidence to Look For

### At Proficient Level (2.0-3.0)
✅ Code reviews rarely mention quality/style issues  
✅ Teammates use their code as reference  
✅ PR feedback focuses on logic, not formatting  
✅ They refactor code proactively  
✅ New patterns emerge from their code  
✅ Others ask "how did you structure this?"  

### At Expert Level (3.0-3.5)
✅ Actively mentors others on code quality  
✅ Identifies and fixes quality issues across codebase  
✅ Establishes new patterns that others adopt  
✅ Code is discussed in team meetings as example  
✅ Others ask for code review specifically from them  
✅ Advocates for quality improvements  

### At Authority Level (3.5-4.0)
✅ Drives org-wide code quality standards  
✅ Creates tooling or guides adopted by org  
✅ Influences hiring and training decisions  
✅ Others reference their approach company-wide  
✅ Visible improvement in codebase across org  
✅ Thought leader in code quality  

---

## ⚠️ Common Misconceptions

### Misconception 1: "Lots of Code = Good Writing"
**Reality:** High output doesn't mean high quality. A person writing clean code carefully is often more valuable than someone churning out quantity.

### Misconception 2: "Code That Works = Good Code"
**Reality:** Code that works but is unreadable will cause problems later. Maintainability matters as much as correctness.

### Misconception 3: "Good Code is Obvious"
**Reality:** Writing clean, maintainable code takes practice and intention. It's a skill that improves over time.

### Misconception 4: "Code Quality is Just Style"
**Reality:** Code quality includes structure, efficiency, testability, and long-term maintainability—not just formatting.

### Misconception 5: "If Code Quality Doesn't Affect Today's Sprint, It Doesn't Matter"
**Reality:** Technical debt compounds. Today's sloppy code is tomorrow's time sink.

---

## 🔗 Related Skills

- **Testing** - Good code is testable code
- **Technical Understanding** - Understanding systems allows better code design
- **Software Architecture** - Code structure follows larger design patterns
- **Debugging & Monitoring** - Clear code is easier to debug
- **Communication** - Code clarity is a form of communication
- **Initiative** - Proactively improving code quality

---

## 🎓 Coaching Strategies

### For Developing Level (0.0-1.0)
1. **Teach Standards** - Provide clear coding conventions and examples
2. **Pair Programming** - Show how you write and refactor code
3. **Review Feedback** - Give specific, actionable feedback on every PR
4. **Model Behavior** - Write clean code they can learn from
5. **Celebrate Improvement** - Notice and praise when they apply feedback

**Conversation Starter:**
"I notice your code usually works well. Let's focus on making it even more maintainable. Here's what I suggest..."

### For Competent Level (1.0-2.0)
1. **Show Examples** - Point to great code in your codebase
2. **Ask Why** - Challenge design choices: "Why did you choose this approach?"
3. **Gradual Standards** - Introduce more sophisticated patterns
4. **Peer Review** - Have them learn from senior code reviews
5. **Refactoring Practice** - Give exercises in improving existing code

**Conversation Starter:**
"Your code is solid. I'd like to help you take it to the next level. Look at how X handled a similar problem..."

### For Proficient Level (2.0-3.0)
1. **Leadership Opportunities** - Ask them to review others' code
2. **Pattern Creation** - Invite them to establish conventions
3. **Teaching Role** - Have them mentor on code quality
4. **Architecture Thinking** - Move toward system-level design
5. **Recognition** - Highlight their code as exemplary

**Conversation Starter:**
"Your code is exemplary. I'd like you to help establish how we approach [pattern] as a team..."

### For Expert & Authority Levels (3.0+)
1. **Org-Wide Impact** - Involve in code quality initiatives
2. **Standards Setting** - Lead adoption of new practices
3. **Tool Creation** - Invest in tooling for code quality
4. **Thought Leadership** - Share approaches with broader org
5. **Strategic Challenges** - Give them high-stakes architectural problems

**Conversation Starter:**
"Your approach to code quality is exceptional. How can we scale this across the team/org?"

---

## 📝 Real Examples

### Scenario: Variable Naming

**Developing Level:**
```javascript
const x = data.map(d => {
  const t = d.v * 1.1;
  return t;
});
```
*Issue: Unclear what x, d, t, v represent. Next person has to decode.*

**Competent Level:**
```javascript
const adjustedValues = data.map(datum => {
  const adjustedValue = datum.value * 1.1;
  return adjustedValue;
});
```
*Better: Clear names, but slightly verbose.*

**Proficient Level:**
```javascript
const adjustedValues = data.map(datum => datum.value * 1.1);
```
*Good: Clear intent with clean, concise code.*

**Expert Level:**
```javascript
const increaseByPercentage = (value, percentage) => value * (1 + percentage / 100);
const adjustedValues = data.map(datum => increaseByPercentage(datum.value, 10));
```
*Excellent: Reusable, clear intent, easier to test and modify.*

---

### Scenario: Function Organization

**Developing:**
```javascript
function processData(data) {
  // 200+ lines of mixed concerns
  // data validation, transformation, API calls, error handling all mixed together
}
```
*Problem: Impossible to understand or modify safely.*

**Competent:**
```javascript
function processData(data) {
  validateData(data);
  const transformed = transformData(data);
  return sendToAPI(transformed);
}
```
*Better: Separated concerns, but each function might still be too complex.*

**Proficient:**
```javascript
const validateData = (data) => { /* ... */ };
const transformData = (data) => { /* ... */ };
const sendToAPI = (data) => { /* ... */ };
const processData = (data) => 
  pipe(validateData, transformData, sendToAPI)(data);
```
*Good: Clear separation, reusable, composable.*

**Expert:**
```javascript
// Created a general data processing pipeline pattern
class DataPipeline {
  addValidator(validator) { /* ... */ }
  addTransformer(transformer) { /* ... */ }
  addExporter(exporter) { /* ... */ }
  async process(data) { /* ... */ }
}

// Now used across multiple services
```
*Excellent: Created reusable pattern that others adopt.*

---

## 🎯 Development Goals by Level

**If currently at Competent, goal is Proficient:**
- "Reduce code review comments about style/organization by 50%"
- "Have one of my PRs used as teaching example by month 3"
- "Propose and implement one team coding standard"

**If currently at Proficient, goal is Expert:**
- "Mentor one junior on code quality practices"
- "Lead refactoring of legacy code section"
- "Establish naming conventions for our APIs"

**If currently at Expert, goal is Authority:**
- "Create tool or guide adopted org-wide"
- "Reduce technical debt in key system by X%"
- "Lead organization-wide code quality initiative"

---

**Remember:** Writing code is a craft. Great writers of code show care and intentionality in every line. The best code is a joy to read and modify months later.
