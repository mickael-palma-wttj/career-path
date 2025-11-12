# Writing Code

**Criterion:** The ability to write clean, maintainable, efficient code that follows standards and best practices. Code that compounds in value over time through clarity, correctness, and care.

Writing code is a craft. It's not just about making things work—it's about making things work in ways that others (including future you) can understand, modify, and build upon. The best code is a joy to read months or years later because it was written with intention and care.

---

## 📋 Quick Summary

| Level | Expectation | Impact |
|-------|-------------|--------|
| **Developing (0.0-1.0)** | Writing code with guidance; needs review for quality issues | Code works but hard to maintain; creates technical debt |
| **Competent (1.0-2.0)** | Writing working code reliably; minor quality issues caught in review | Code is generally good; some maintenance friction |
| **Proficient (2.0-3.0)** | Writing clean, maintainable code consistently; sets good examples | Code is exemplary; others learn from it; joy to modify |
| **Expert (3.0-3.5)** | Code exemplifies best practices; mentors others on code quality | Code is best-in-class; shapes how team thinks about quality |
| **Authority (3.5-4.0)** | Defines coding standards; influences org-wide code quality practices | Org code quality reflects their standards; competitive advantage |

---

## 🎯 Definition

**Writing Code** encompasses five interconnected capabilities:

### 1. **Code Structure & Organization**
Organizing code logically so it's easy to understand and navigate. Breaking complex problems into manageable pieces. Grouping related functionality together. Making the codebase easy to traverse.

### 2. **Clarity & Naming**
Writing code that's self-explanatory. Choosing names that reveal intent. Writing comments when logic is non-obvious. Making purpose obvious to reader. Code as communication, not just instruction.

### 3. **Maintainability**
Writing code that's easy to modify safely. Avoiding tight coupling. Reducing side effects. Making changes localized. Enabling refactoring with confidence.

### 4. **Efficiency & Performance**
Writing code that performs well without being premature. Understanding performance implications of choices. Making good trade-offs between clarity and performance. Not leaving obvious optimization on the table.

### 5. **Standards & Consistency**
Following established patterns and conventions. Consistency across codebase. Using agreed-upon style. Making it feel cohesive, not like patchwork from different people.

---

## 📊 Detailed Level Descriptions

### 🟦 Developing (0.0 - 1.0)

**Core Behaviors:**
- Code works but quality issues visible
- Needs significant review feedback
- Doesn't consider long-term maintainability
- Variable naming unclear or inconsistent
- Functions often mix multiple concerns
- Quick-and-dirty approach default
- Doesn't follow established patterns
- Code feels temporary, not permanent

**What You'd See:**
- Long functions (50+ lines) doing multiple things
- Variable names like `x`, `temp`, `data1`, `result2`
- Inconsistent style between files
- Comments explaining "what" not "why"
- Repeated code patterns
- Code review feedback focuses on quality, not just correctness
- Others struggle to understand intent
- "We can clean this up later" attitude

**Specific Examples:**
- `const x = arr.map(a => { const t = a.v * 1.1; return { ...a, v: t }; });`
- 200-line function mixing validation, transformation, and API calls
- Variable names that don't explain purpose

**What Success Looks Like:**
- Follow style guide consistently
- Use clear, intentional names
- Break functions into logical pieces
- Consider how others will read code
- Apply feedback on structure and organization

**Development Focus:**
- Learn coding standards
- Build awareness of maintainability
- Develop naming discipline
- Practice breaking down complexity
- Study good code in codebase

---

### 🟩 Competent (1.0 - 2.0)

**Core Behaviors:**
- Code generally meets quality standards
- Mostly follows conventions (with guidance)
- Generally well-organized
- Shows growing quality awareness
- Some refactoring needed but maintainable
- Improving with feedback
- Learning design patterns
- Starting to think about readability

**What You'd See:**
- Code is generally understandable
- Names are mostly clear (with occasional ambiguity)
- Functions are reasonable length
- Some concerns separated
- Code reviews find minor style/organization issues
- Growing consistency with codebase
- Shows care in structure
- Asks "Is this the right way to do this?"

**Specific Examples:**
- `const adjustedValues = data.map(datum => datum.value * 1.1);`
- Functions 30-40 lines with mostly single purpose
- Names like `processUser`, `formatDate`, `calculateTotal`
- Follows most patterns after explanation

**What Success Looks Like:**
- Code review comments rarely about quality
- Others use your code as reference
- Show growing understanding of standards
- Make good naming choices
- Organize code logically

**Development Focus:**
- Deepen understanding of patterns
- Improve consistency automatically
- Move from following rules to understanding them
- Develop code "taste"
- Learn to refactor effectively

---

### 🟧 Proficient (2.0 - 3.0)

**Core Behaviors:**
- Code is clean and well-organized consistently
- Follows standards naturally, not by checklist
- Excellent naming that reveals intent
- Strong consideration for maintainability
- Code exemplifies how it "should" be written
- Others point to their code as reference
- Takes pride in craft
- Thinks about future readers

**What You'd See:**
- Code reviews almost never mention style/organization
- Teammates use code as teaching example
- Functions are well-named and focused
- Structure makes purpose obvious
- Intentional design choices
- Others ask "How would you structure this?"
- Code is refactored proactively
- New patterns emerge from their work
- Colleagues describe as "writes beautiful code"

**Specific Examples:**
- `const increaseByPercentage = (value, percentage) => value * (1 + percentage / 100);`
- `const adjustedValues = data.map(datum => increaseByPercentage(datum.value, 10));`
- Functions organized by purpose; clear data flow
- Consistent structure across similar functions
- Comments explain "why", not "what"

**Evidence:**
- Code reviews focus on logic/design, not style
- Others reference their code as good example
- Minimal refactoring needed after code review
- Self-refactors proactively for clarity
- New team members learn from their code
- Consistent high quality across all work

**What Success Looks Like:**
- Build reputation for code quality
- Help others improve their code
- Establish patterns for team
- Mentor others on code craft
- Lead code quality improvements

**Development Focus:**
- Mentor others on code quality
- Establish team patterns
- Move toward architecture thinking
- Help raise bar across team
- Could lead code quality initiatives

---

### 🟨 Expert (3.0 - 3.5)

**Core Behaviors:**
- Code is exceptionally clean and well-crafted
- Demonstrates deep pattern knowledge
- Makes sophisticated design choices
- Mentors others on code quality
- Identifies and fixes issues across codebase
- Others seek advice: "How should this be structured?"
- Creates reusable patterns
- Advocates for code quality

**What You'd See:**
- Code is discussed in team meetings as exemplary
- Others ask to review their code for structure
- Actively mentors team on code quality
- Identifies quality issues across codebase and proposes fixes
- Establishes new patterns others adopt
- Code quality initiatives led by them
- Others describe as "cares deeply about craft"
- New team members learn coding standards from them

**Specific Examples:**
- Recognizes repeated pattern, extracts reusable component
- Mentors junior: "Here's how I'd structure this..."
- Proposes architectural improvements for clarity
- Creates guide for common patterns
- Code reviews include teaching moment

**Evidence:**
- Actively mentors multiple people
- Identifies and fixes quality issues they didn't write
- Establishes patterns others adopt
- Code quality initiatives led by them
- Others seek advice on code structure
- Known as code quality advocate
- Reputation for excellence in craft

**What Success Looks Like:**
- Mentor multiple people on code quality
- Lead code quality initiatives
- Establish team patterns/standards
- Help org think about code craft
- Create lasting impact on code quality

**Development Focus:**
- Scale impact across team/org
- Lead code quality improvements
- Mentor leaders on code quality
- Could move to leadership roles

---

### 🟥 Authority (3.5 - 4.0+)

**Core Behaviors:**
- Defines how code is written in org
- Influences org-wide code quality standards
- Creates tools, guidelines adopted widely
- Drives adoption of best practices
- Others reference their code as gold standard
- Visible impact on codebase across org
- Sets tone for code quality
- Code quality is competitive advantage

**What You'd See:**
- Org cites them as code quality model
- Code quality initiatives reflect their approach
- Tools/guides they created are standard
- Others throughout org model their style
- Org-wide improvement in code quality
- Hiring considers their standards
- New team members learn from their code
- Codebase reflects their influence

**Specific Examples:**
- Created linting rules now org standard
- Developed coding guide everyone references
- Mentors team leads on code quality
- Org code quality measurably improved
- Others cite their approach when writing code

**Evidence:**
- Org-wide reputation for setting code quality
- Tools/standards created by them adopted org-wide
- Others model their approach
- Code quality improvements visible org-wide
- Multiple teams influenced by their work
- Hiring/training reflects their standards

---

## ❓ Assessment Questions

### For Any Level:
- **Walk me through this code structure.** Why did you organize it this way?
- **What standards or patterns are you following here?**
- **If you saw this code in a year, what would you change?**

### For Competent+ Levels:
- **What would make this code easier to maintain?**
- **How would you refactor this for clarity?**
- **Explain your naming choices here. Why these names?**

### For Proficient+ Levels:
- **What part of this code are you most proud of?** Why?
- **How would you teach someone your approach to structure?**
- **Tell me about code you've refactored for quality.**
- **How do you stay consistent with our patterns?**

### For Expert+ Levels:
- **Tell me about someone you've mentored on code quality.**
- **Describe how you approach establishing new patterns.**
- **How do you identify code quality issues across codebase?**
- **What makes code maintainable?** Give examples from your work.

---

## 👀 Evidence to Look For

### By Level

**Developing:**
- Makes effort to follow standards
- Takes feedback on code structure
- Shows willingness to improve
- Learns coding patterns

**Competent:**
- Generally clean, organized code
- Mostly consistent with codebase
- Code reviews find minor issues
- Learning and improving
- Uses clear naming usually

**Proficient:**
- Code is exemplary and consistent
- Code reviews focus on logic, not style
- Others use code as reference
- Self-refactors for clarity
- Helps others improve code
- Teaches coding standards

**Expert:**
- Actively mentors on code quality
- Identifies issues across codebase
- Establishes new patterns
- Code quality initiatives
- Others seek advice on structure
- Reputation for excellence

**Authority:**
- Org-wide code quality improved
- Standards/tools created by them
- Others model their approach
- Executive sees code quality impact
- Multiple teams influenced

### Negative Indicators (Any Level)
- ❌ Code is hard to understand
- ❌ Variable names are ambiguous
- ❌ Functions do too many things
- ❌ Repeated code patterns
- ❌ Inconsistent with codebase style
- ❌ Doesn't consider maintenance
- ❌ "We can clean this up later" mentality
- ❌ Doesn't follow established patterns
- ❌ Takes no pride in code craft
- ❌ Ignores feedback on code quality

---

## 🔗 Related Skills & Competencies

**Directly Connected:**
- **Testing** (Engineering Craft) - Good code is testable
- **Technical Understanding** (Engineering Craft) - Deep knowledge enables better design
- **Software Architecture** (Engineering Craft) - Code follows larger patterns
- **Debugging & Monitoring** (Engineering Craft) - Clean code is easier to debug
- **Communication** (Soft Skills) - Code is communication

**Indirectly Connected:**
- **Initiative** (Soft Skills) - Proactively improving code quality
- **Objectivity & Adaptability** (Soft Skills) - Learning from feedback on code
- **Empathy & Humility** (Soft Skills) - Writing for readers, not just yourself

---

## 🎯 Development Goals & Progression Paths

### Developing → Competent
**Goal:** "Learn standards and write consistent code"

**Specific Actions:**
- [ ] Learn coding standards; reference document when writing
- [ ] Use linter/formatter; fix issues it finds
- [ ] Choose clear names: would new person understand?
- [ ] Break functions into smaller pieces (target: 30-40 lines)
- [ ] Ask for code review feedback and apply it
- [ ] Study 3 examples of good code in codebase
- [ ] Refactor one piece for clarity; document why
- [ ] Consistency check: Does my code look like codebase?

**Timeline:** 3-6 months

---

### Competent → Proficient
**Goal:** "Write exemplary code naturally"

**Specific Actions:**
- [ ] Reduce code review comments about quality by 50%
- [ ] One of my PRs used as teaching example
- [ ] Proactively refactor code for clarity
- [ ] Establish one team coding convention
- [ ] Help junior improve code quality
- [ ] Study patterns; can explain why they're good
- [ ] Mentor 1-2 people on code structure
- [ ] Build reputation: "They write beautiful code"

**Timeline:** 6-12 months

---

### Proficient → Expert
**Goal:** "Mentor others; establish patterns"

**Specific Actions:**
- [ ] Mentor 2+ people on code quality practices
- [ ] Lead refactoring of legacy code section
- [ ] Establish naming conventions for your domain
- [ ] Create guide for common patterns
- [ ] Lead code quality discussion/initiative
- [ ] Identify and propose architectural improvements
- [ ] Get feedback: Are others modeling your code?
- [ ] Quarterly: How's codebase quality changing?

**Timeline:** 12-24 months

---

### Expert → Authority
**Goal:** "Shape org's code quality standards"

**Specific Actions:**
- [ ] Mentor team leads on code quality
- [ ] Create org-wide coding standards guide
- [ ] Develop tooling that improves code quality
- [ ] Lead org-wide code quality initiative
- [ ] Model code quality consistently
- [ ] Help hiring calibrate on code quality
- [ ] Share approach with peers/org
- [ ] Measure org-wide quality improvements

**Timeline:** 2-3+ years

---

## 📚 Detailed Development Guidance

### Improving Code Structure & Organization

**Principles:**
1. **One thing per function** - A function should do one thing well
2. **Single Responsibility** - A class/module should have one reason to change
3. **Cohesion** - Related code should be together
4. **Loose coupling** - Minimize dependencies between modules
5. **Easy to navigate** - Reader can find things easily

**How to Improve:**
- Break long functions into smaller pieces
- Extract repeated logic into reusable functions
- Group related functionality
- Make data flow obvious
- Separate concerns (logic, data access, formatting)

**Red Flags (Poor Organization):**
- ❌ Function longer than 50 lines
- ❌ Function does multiple unrelated things
- ❌ Deep nesting (3+ levels)
- ❌ Repeated code patterns
- ❌ Hard to find things

### Improving Naming

**Good Names Reveal Intent:**
- **Variables:** What does it contain? `user`, `emailAddress`, `isValid`
- **Functions:** What does it do? `calculateDiscount`, `validateEmail`, `formatDate`
- **Classes:** What is it? `UserRepository`, `EmailValidator`, `PaymentProcessor`

**Naming Principles:**
1. **Be specific** - Not `data`, but `userData`
2. **Use full words** - Not `usr`, but `user`
3. **Avoid numbers** - Not `data1`, `data2`, but `userData`, `systemData`
4. **Use pronounceable names** - Others need to discuss them
5. **Use searchable names** - Grep-able, not single letters
6. **Match domain** - Use business terms when appropriate

**Common Mistakes:**
- ❌ Single letter names (except i, j in loops)
- ❌ Names that hide purpose
- ❌ Names that are too short
- ❌ Names that don't match meaning
- ❌ Misleading names

### Improving Maintainability

**Code is Maintainable When:**
- Changes are localized (you know where to change)
- Side effects are minimal (change doesn't break other things)
- Dependencies are clear (you know what depends on what)
- Logic is obvious (you don't have to decode it)
- Tests give confidence (changing doesn't break things)

**How to Build It:**
1. **Minimize scope** - Variables and functions with small scope
2. **Reduce coupling** - Fewer dependencies between modules
3. **Use interfaces** - Hide implementation details
4. **Make dependencies explicit** - Parameter injection, not globals
5. **Enable testing** - Code designed to be testable

**Red Flags (Poor Maintainability):**
- ❌ Global state everywhere
- ❌ Tightly coupled components
- ❌ Hidden dependencies
- ❌ Complex logic hard to understand
- ❌ Changes break unrelated code

### Improving Efficiency & Performance

**Balance:**
- **Clarity** vs. **Performance** - usually clarity wins until profiling says otherwise
- **Generality** vs. **Specificity** - specific code usually faster
- **Simplicity** vs. **Optimization** - simple until bottleneck found

**Efficiency Principles:**
1. **Profile before optimizing** - Find actual bottlenecks
2. **Optimize at the right level** - Algorithm > data structure > micro-optimization
3. **Measure improvement** - Know if it actually helped
4. **Keep it readable** - Performance code can still be clear
5. **Document trade-offs** - Why you chose this approach

**Common Mistakes:**
- ❌ Premature optimization (optimizing before profiling)
- ❌ Sacrificing clarity for marginal gains
- ❌ Optimizing wrong part of code
- ❌ Not measuring actual impact
- ❌ Leaving obvious inefficiencies

### Following Standards & Consistency

**Standards Matter Because:**
- **Reduce friction** - No debate about style
- **Enable learning** - New people follow patterns
- **Make refactoring safer** - Consistent code is easier to change
- **Professional** - Shows care and discipline

**Building Consistency:**
1. **Use formatters/linters** - Automate style decisions
2. **Learn team patterns** - Study existing code
3. **Ask questions** - When uncertain about style
4. **Propose improvements** - If you see better approach
5. **Be consistent** - Apply same approach everywhere

---

## 💡 Key Principles

### 1. **Code is Read More Than Written**
You write code once. It's read dozens or hundreds of times by others and future-you. Optimize for readability, not speed of writing.

### 2. **Clarity is a Competitive Advantage**
Clear codebases are easier to maintain, extend, and debug. They attract good engineers. They move faster long-term.

### 3. **Technical Debt Compounds**
Sloppy code written today is debt you pay every time someone touches it. Small, frequent cleanups cost less than big rewrites.

### 4. **Good Code is Craft**
Writing good code takes intention and practice. It's not something that happens by accident. Treat it as craft worth mastering.

### 5. **Patterns Enable Scaling**
When everyone follows the same patterns, new people learn faster and code works together. Consistency enables scaling.

### 6. **Future You is Your Colleague**
Write code you'd want to see if you came back to it in 6 months. If you wouldn't want to maintain it, it's not done.

---

## 🎯 Red Flags & Warnings

⚠️ **Code is hard to understand** — Clarity missing
⚠️ **Long functions (50+ lines)** — Doing too much
⚠️ **Ambiguous variable names** — Purpose unclear
⚠️ **Repeated code patterns** — Needs refactoring
⚠️ **Inconsistent with codebase** — Not following standards
⚠️ **"We can clean this up later"** — Debt accumulating
⚠️ **Doesn't follow established patterns** — Inconsistent
⚠️ **Hard to test** — Poor maintainability
⚠️ **Ignores code review feedback** — Not growing
⚠️ **Takes no pride in craft** — Unsustainable

---

**Remember:** Writing code is a craft. Great code is not just functional—it's a joy to read and modify. Invest in improving your craft deliberately.

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
