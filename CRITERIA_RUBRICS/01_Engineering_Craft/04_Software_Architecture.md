# Software Architecture

**Criterion:** Ability to design systems, make scalability decisions, and ensure long-term maintainability through thoughtful system design.

Architecture is about making choices today that enable tomorrow. Good architecture is invisible—it lets systems grow without constant rewrites. Great architects think 3-5 years ahead while staying grounded in present constraints.

---

## 📋 Quick Summary

| Level | Expectation | Impact |
|-------|-------------|--------|
| **Developing (0.0-1.0)** | Designs small features; needs guidance on larger systems | Limited scalability; technical debt accumulates |
| **Competent (1.0-2.0)** | Can design features; follows established patterns | Follows patterns; some forward thinking |
| **Proficient (2.0-3.0)** | Designs systems thoughtfully; considers future growth | Systems remain maintainable as they grow |
| **Expert (3.0-3.5)** | Exceptional architecture; mentors on design decisions | Org avoids re-architects; patterns adopted |
| **Authority (3.5-4.0)** | Org-wide architectural influence; sets design standards | Architecture enables rapid development |

---

## 🎯 Definition

**Software Architecture** encompasses five interconnected capabilities:

### 1. **System Design**
Structuring systems for scalability, maintainability, and future growth. Understanding how to break systems into components that can evolve independently. Designing boundaries and interfaces thoughtfully.

### 2. **Tradeoff Awareness**
Understanding the trade-offs in every architectural decision. No perfect solution exists—only solutions with different trade-offs. Making conscious choices about what you're optimizing for.

### 3. **Scalability Thinking**
Designing systems that can grow—in data volume, traffic, complexity, or team size. Anticipating growth patterns and planning for them. Understanding bottlenecks before they appear.

### 4. **Long-term Vision**
Considering how systems will need to evolve. Avoiding lock-in decisions that make future changes expensive. Building flexibility into systems where uncertainty exists.

### 5. **Design Communication**
Clearly explaining architectural choices, trade-offs, and reasoning. Getting alignment on architecture. Helping others understand why systems are designed certain ways.

**📖 Further Reading:** At Staff+ levels, architecture transcends technical decisions to include organizational and strategic thinking. *[The Staff Engineer's Path](../../BOOKS/The%20Staff%20Engineer's%20Path%20-%20Tanya%20Reilly.pdf)* explores how Staff engineers use architectural leadership to shape organizational direction.

---

## 📊 Detailed Level Descriptions

### 🟦 Developing (0.0 - 1.0)

**Core Behaviors:**
- Designs small features in isolation
- Doesn't consider larger system implications
- No tradeoff awareness
- Treats code as temporary
- Needs architecture guidance for anything beyond simple features
- Can't estimate scalability impacts
- Follows patterns without understanding

**What You'd See:**
- "I'll just build this feature"
- No consideration of how it integrates
- Designs that don't scale
- Code that needs rewriting soon
- Asks for guidance on architecture frequently
- Treats tech debt casually

**What Success Looks Like:**
- Learn architectural patterns
- Start thinking about systems holistically
- Understand tradeoffs
- Consider future implications
- Ask questions about architecture

**Development Focus:**
- Study system design
- Understand existing architecture
- Learn common patterns
- Think about scalability
- Build architectural thinking

---

### 🟩 Competent (1.0 - 2.0)

**Core Behaviors:**
- Designs within established patterns
- Follows architectural guidance from seniors
- Considers immediate scaling needs
- Some tradeoff awareness emerging
- Learning to think beyond current requirements
- Can implement recommended designs

**What You'd See:**
- "I'll follow the pattern from [similar system]"
- Designs that work for current needs
- Some forward thinking about growth
- Questions about tradeoffs
- Relies on established patterns
- Learning architectural thinking

**Specific Examples:**
- "Should I build this as a separate service?"
- "I designed this module to be independent so we can swap it out later"
- "What happens if we get 10x more traffic?"

**What Success Looks Like:**
- Designs that scale beyond immediate needs
- Conscious tradeoff thinking
- Can explain design choices
- Learning from architecture discussions

**Development Focus:**
- Deeper architectural thinking
- Understand tradeoffs better
- Lead design of features
- Contribute to architecture discussions
- Think about long-term implications

---

### 🟧 Proficient (2.0 - 3.0)

**Core Behaviors:**
- Designs thoughtful systems naturally
- Considers scalability and maintainability
- Makes good tradeoff decisions
- Anticipates future needs
- Others ask for design input
- Contributes meaningfully to architecture decisions
- Explains reasoning clearly

**What You'd See:**
- Asked for design input on new systems
- Designs remain relevant as systems grow
- Anticipates scaling challenges accurately
- Makes conscious tradeoff decisions
- Explains architectural thinking clearly
- Helps others understand architecture

**Specific Examples:**
- "For this volume, a relational database works. When we hit 1M queries/day, we'll need to reconsider. Here's what that path looks like."
- "I designed this module with these boundaries so we can shard it later if needed"
- "This design optimizes for query speed now, which means we trade some write performance"

**Evidence:**
- People ask them for design input
- Designs scale well over time
- Tradeoff decisions are conscious and communicated
- Architecture discussions include their input
- Systems they designed remain maintainable

**What Success Looks Like:**
- Recognized for good architectural decisions
- Systems they designed scale gracefully
- Mentoring others on design
- Leading architectural improvements

**Development Focus:**
- Mentor others on architecture
- Lead architectural improvements
- Improve org's architectural standards
- Think strategically about systems
- Consider organizational implications

---

### 🟨 Expert (3.0 - 3.5)

**Core Behaviors:**
- Exceptional architectural sense
- Anticipates future needs accurately
- Makes sophisticated design tradeoffs
- Mentors others on architecture
- Drives architectural improvements
- Recognizes architectural problems early
- Influences multiple systems

**What You'd See:**
- Sought for architectural decisions
- Systems they designed become exemplars
- They identify architectural problems before they hurt
- Mentoring others on design
- Proactively improves architecture
- Design decisions ripple across org

**Specific Examples:**
- "I see we're going to hit scaling limits here in 6 months. Here's how I'd restructure to handle it"
- Mentored junior on service-oriented design; they applied it successfully
- "This pattern we've been using won't scale to multiple teams. Let me propose a better approach"

**Evidence:**
- Sought out for architectural decisions
- Systems they designed become reference implementations
- Mentors on architecture effectively
- Org avoids painful re-architectures due to their guidance
- Design patterns they establish are adopted

**What Success Looks Like:**
- Architecture decisions reflect their input
- Others emulate their design approach
- Architectural improvements from their leadership
- Org recognizes as architectural authority

**Development Focus:**
- Scale impact across organization
- Mentor leaders on architecture
- Lead org-wide architectural strategy
- Shape how org thinks about design
- Could move to architecture/leadership

---

### 🟥 Authority (3.5 - 4.0+)

**Core Behaviors:**
- Org's architectural authority
- Sets architectural standards
- Influences org-wide design decisions
- Others follow their architectural approach
- Visible improvements in system architecture
- Architecture conversations include their voice
- Shapes how org thinks about design

**What You'd See:**
- Org architecture reflects their input
- Others reference their designs
- Org-wide architectural improvements
- New teams learn their approach
- Systems designed using their patterns
- Architecture discussions start with their principles
- Org avoids costly architectural mistakes due to their guidance

**Specific Examples:**
- Org adopted their service-oriented approach; improved deployment speed
- "This is how we do architecture at our scale"
- Multiple teams successfully applied their architectural patterns

**Evidence:**
- Org-wide architectural decisions from them
- Others model their approach
- Systems structured according to their principles
- Visible improvements in maintainability
- Reduced need for re-architectures

---

## 📊 Architectural Decision Matrix

Understanding how to navigate architectural choices:

| Dimension | Scalability | Simplicity | Flexibility | Immediate Cost |
|-----------|-----------|-----------|-----------|-----------|
| **Monolith** | Limited | High | Low | Low |
| **Microservices** | Excellent | Low | High | High |
| **Event-Driven** | Excellent | Medium | High | Medium |
| **Layered Monolith** | Medium | High | Medium | Low |

**How to Use:** Each architecture is right for different contexts. Better architects choose based on actual constraints, not trends.

---

## ❓ Assessment Questions

**For Developing → Competent:**
- Walk me through how you'd design [simple system]. What are your main considerations?
- Why might this design need to change as the system grows?
- What patterns have you seen in our codebase? When do we use each?

**For Proficient → Expert:**
- Walk me through how you'd design [complex system]. What are the key decisions?
- What scaling challenges do you anticipate? How would you address them?
- What tradeoffs are you making in this design? What would you optimize differently at 10x scale?
- How would this architecture handle [hypothetical future scenario]?

**For Expert → Authority:**
- How do you approach designing systems at org scale?
- What architectural improvements would have the biggest impact across engineering?
- How should we think about architecture for our scale and growth?
- How do you mentor others on architectural thinking?

---

## 👀 Evidence to Look For

### At Proficient Level (2.0-3.0)
✅ Asked for design input on new systems
✅ Designs scale gracefully over time
✅ Tradeoff decisions are conscious and explained
✅ Systems they designed remain maintainable
✅ Others feel confident with their architecture
✅ Anticipates scaling needs accurately

### At Expert Level (3.0-3.5)
✅ Sought out for architectural decisions
✅ Systems they designed become exemplars
✅ Mentors others on architecture effectively
✅ Identifies architectural problems early
✅ Proactively improves architecture
✅ Org avoids painful re-architectures

### At Authority Level (3.5-4.0)
✅ Org architecture reflects their input
✅ Others reference their designs
✅ Org-wide architectural improvements visible
✅ New teams learn their approach
✅ Systems structured using their patterns
✅ Architectural mistakes decrease org-wide

### Negative Indicators (Any Level)
❌ Designs without considering growth
❌ Over-engineers simple systems
❌ Can't explain tradeoff reasoning
❌ Copies patterns without understanding
❌ Resists changing architecture when needed
❌ Systems become bottlenecks later
❌ Doesn't consider maintainability
❌ No forward thinking about growth
❌ Makes architectural decisions in isolation
❌ Can't defend architectural choices

---

## 🔗 Related Skills & Competencies

**Directly Connected:**
- **Technical Understanding** (Engineering Craft) - Deep tech knowledge enables better architecture
- **Writing Code** (Engineering Craft) - Clean code follows good architecture
- **Stakeholder Management** (Leadership) - Selling and explaining architectural vision
- **Team Leadership** (Leadership) - Gaining alignment on architectural decisions

**Indirectly Connected:**
- **Communication** (Soft Skills) - Explaining complex architectural concepts
- **Business Acumen** (Soft Skills) - Understanding business drivers for architecture
- **Initiative** (Soft Skills) - Proactively improving architecture
- **Developing Others** (Leadership) - Teaching architectural thinking

---

## � Development Goals & Progression Paths

### Competent → Proficient
**Goal:** "Master architectural thinking; design systems that scale"

**Specific Actions:**
- [ ] Lead design of [new system]; present architectural decisions
- [ ] Document architecture of [existing major system]
- [ ] Evaluate [competing architectural approaches]; explain tradeoffs
- [ ] Anticipate growth for [system]; design scaling path
- [ ] Mentored one person on architectural thinking
- [ ] Study architectural patterns (microservices, event-driven, etc.)
- [ ] Design that anticipates 5x growth

**Timeline:** 6-12 months

---

### Proficient → Expert
**Goal:** "Mentor widely; improve org architecture; identify patterns"

**Specific Actions:**
- [ ] Mentor 2+ people on architectural thinking
- [ ] Improve architecture of [key system]; document improvements
- [ ] Identify architectural gap in org; propose solution
- [ ] Lead architectural evaluation for [major decision]
- [ ] Create architectural patterns adopted by team
- [ ] Anticipate and prevent architectural problems
- [ ] Teach architectural workshop or write guide

**Timeline:** 12-24 months

---

### Expert → Authority
**Goal:** "Shape org's architectural direction; scale impact"

**Specific Actions:**
- [ ] Define org's architectural standards and approach
- [ ] Lead org-wide architectural improvement initiative
- [ ] Mentor leaders on architectural thinking
- [ ] Contribute to org-wide architecture decisions
- [ ] Create architectural guidelines adopted org-wide
- [ ] Measure and improve org's architectural quality
- [ ] External visibility: conference talk or article on architecture

**Timeline:** 2-3+ years

---

## � Detailed Development Guidance

### Understanding Tradeoffs

**The Core Tradeoff Triangle:**
```
        Simplicity
            /\
           /  \
          /    \
         /      \
        /________\
    Scalability  Flexibility
```

Every system sits somewhere in this triangle. Move toward one corner and you move away from the others.

**Common Tradeoffs:**
- **Monolith vs. Microservices**: Simple (monolith) vs. scalable (microservices)
- **Relational vs. Document DB**: Consistency vs. flexibility
- **Synchronous vs. Asynchronous**: Simplicity vs. scalability
- **Caching vs. Direct Access**: Speed vs. consistency

**How to Navigate:**
1. Understand your constraints (scale, team, latency requirements)
2. Identify the most important tradeoff for your situation
3. Make conscious choice about what you're optimizing for
4. Be prepared to re-architect when constraints change

### Designing for Scale

**Scalability Patterns:**

1. **Database Scaling**: Single DB → Read replicas → Sharding → Distributed DB
2. **Compute Scaling**: Single server → Multiple servers → Horizontal scaling → Microservices
3. **Complexity Scaling**: Monolith → Modular monolith → Microservices → Event-driven
4. **Team Scaling**: Single team → Teams by feature → Teams by domain → Platform teams

**Design Decisions for Each Level:**

| Growth Stage | Database | Compute | Architecture | Teams |
|-------------|----------|---------|--------------|-------|
| 100s | Single instance | Single server | Monolith | 1-2 |
| 1000s | Read replicas | Load balancer | Modular monolith | 3-5 |
| 10Ks | Sharding | Auto-scaling | Microservices | 5-20 |
| 100Ks | Distributed DB | Service mesh | Event-driven | 20+ |

### Building Flexibility

**Anti-Patterns That Lock You In:**
- ❌ Hardcoding service URLs
- ❌ Tightly coupling components
- ❌ Single deployment for everything
- ❌ Shared databases between services
- ❌ Synchronous dependencies everywhere

**Patterns That Build Flexibility:**
- ✅ Configuration and discovery
- ✅ Loose coupling (interfaces, events)
- ✅ Independent deployability
- ✅ Data isolation
- ✅ Asynchronous communication where appropriate

### Communicating Architecture

**Architecture Communication Framework:**

1. **Problem**: What are we trying to solve?
2. **Constraints**: What limits our options?
3. **Options**: What are 2-3 possible approaches?
4. **Tradeoffs**: What does each approach trade off?
5. **Recommendation**: Which approach and why?
6. **Risks**: What could go wrong?
7. **Plan**: How do we build/migrate to this?

**Visualization Tips:**
- Draw components and their relationships
- Show data flow
- Highlight boundaries and interfaces
- Note scaling points
- Document tradeoff decisions

### Learning from Mistakes

**Common Architectural Mistakes:**

| Mistake | Why It Happens | Prevention |
|---------|---|---|
| Over-engineering | Anticipating needs that don't come | Design for current needs + clear paths to scale |
| Under-engineering | Ignoring growth | Estimate growth; design for it explicitly |
| Wrong tool choice | Fashion/trend | Choose based on actual constraints |
| Ignoring operations | Too focused on features | Involve ops in architecture decisions |
| Tight coupling | Expedient initially | Establish boundaries early |

---

## 💡 Key Principles

### 1. **Simplicity Scales Longer Than Complexity**
Simple systems take you further than complex ones. Complex systems become burdens quickly. Choose simplicity when it's sufficient.

### 2. **Architecture Enables or Prevents Growth**
Good architecture lets teams and systems grow independently. Bad architecture becomes the bottleneck to scaling.

### 3. **Design for Your Constraints**
The best architecture for your company is the one that fits your constraints (scale, team size, maturity). Not the one used by tech giants.

### 4. **Flexibility Costs**
Every bit of flexibility costs something (complexity, performance, development time). Only build flexibility where you'll use it.

### 5. **Re-architecture is Normal**
Systems outgrow their original design. Plan for re-architecture rather than trying to perfect the first design forever.

### 6. **Architecture Serves Business Goals**
Architecture isn't a technical exercise. It should enable or support business goals. If it doesn't, reconsider.

---

## 🎯 Red Flags & Warnings

⚠️ **Designing without constraints** — What are you actually optimizing for?
⚠️ **Over-engineering for imagined scale** — Build what you need now
⚠️ **Tight coupling increasing** — Hard to change later
⚠️ **Scaling decisions made in isolation** — Consider ops impact
⚠️ **No path to change architecture** — Lock-in happening
⚠️ **Architecture out of sync with reality** — Design drifting from implementation
⚠️ **Monolith growing without plan** — Eventual re-architecture pain
⚠️ **Microservices without operational support** — Too much complexity too early
⚠️ **Can't explain tradeoff reasoning** — Architecture unclear
⚠️ **Architecture decisions not documented** — Why is it this way?

---

**Remember:** Good architecture is about enabling change, not preventing it. Architecture decisions made today should let you change tomorrow.
