# Debugging & Monitoring

**Criterion:** Ability to find and fix bugs, diagnose production issues, and build observable systems through monitoring and logging.

Great debugging and monitoring capabilities are the difference between systems that are painful to operate and systems that hum quietly. Observable systems are understandable systems. You should know about problems before customers do.

---

## 📋 Quick Summary

| Level | Expectation | Impact |
|-------|-------------|--------|
| **Developing (0.0-1.0)** | Debugging with guidance; struggles to find root causes | Production mysteries; long MTTR |
| **Competent (1.0-2.0)** | Finds most bugs; adequate monitoring in code | Most issues resolved; some struggle |
| **Proficient (2.0-3.0)** | Expert debugger; builds observable systems | Production issues resolved quickly |
| **Expert (3.0-3.5)** | Exceptional diagnostics; mentors on monitoring | Org MTTR decreases; observability improves |
| **Authority (3.5-4.0)** | Org debugging/monitoring authority; sets standards | Prod reliability visible; issues proactive |

---

## 🎯 Definition

**Debugging & Monitoring** encompasses five interconnected capabilities:

### 1. **Root Cause Analysis**
Finding the real problem, not symptoms. Systematic investigation. Tracing from symptom to root cause. Understanding why problems happen, not just fixing them.

### 2. **Problem Diagnosis**
Systematic approach to finding issues. Using tools effectively (debuggers, logs, profilers). Forming hypotheses and testing them. Narrowing down problems efficiently.

### 3. **Observable Systems**
Building systems you can understand in production. Good logging. Meaningful metrics. Proper alerting. Systems that expose their behavior.

### 4. **Monitoring Strategy**
Knowing what to measure and why. Understanding business and technical health. Setting up alerts that matter. Building dashboards that tell you what you need to know.

### 5. **Production Confidence**
Comfort operating systems in production. Understanding behavior without deployments. Knowing what's normal. Detecting abnormal quickly. Proactive problem prevention.

---

## 📊 Detailed Level Descriptions

### 🟦 Developing (0.0 - 1.0)

**Core Behaviors:**
- Frustrated by bugs; doesn't know where to start
- Lacks debugging technique
- Limited monitoring; can't understand production
- Asks for help to find bugs
- Log output is overwhelming or unhelpful
- Debugger use is limited

**What You'd See:**
- "I don't know where to start debugging this"
- Doesn't know what to monitor
- Overwhelmed by production logs
- Can't narrow down problems
- Asks "is it this or that?" guessing
- Limited use of debugging tools

**What Success Looks Like:**
- Learn debugging techniques
- Understand debugging tools
- Add meaningful logging
- Learn what to monitor
- Start narrowing down problems systematically

**Development Focus:**
- Learn debugging techniques
- Build debugging skills
- Understand how to read logs
- Learn what to monitor
- Develop systematic approach

---

### 🟩 Competent (1.0 - 2.0)

**Core Behaviors:**
- Finds most bugs systematically
- Uses debugger effectively
- Adds monitoring to own code
- Can usually narrow down problems
- Learning root cause analysis
- Log output makes sense sometimes

**What You'd See:**
- Can find bugs without too much help
- Uses debugger to step through code
- Adds logging when needed
- Understands some metrics
- Narrows down issues reasonably well
- Still needs help on complex issues

**Specific Examples:**
- Used debugger to trace through function; found null pointer
- Added logging to understand production behavior
- Looked at metrics to understand performance issue
- Narrowed down bug to specific service

**What Success Looks Like:**
- Systematically debug issues
- Good debugging technique
- Meaningful logging in code
- Understanding of metrics
- Root cause finding emerging

**Development Focus:**
- Deeper debugging skills
- Build monitoring thinking
- Create observable code
- Learn monitoring strategy
- Mentor others on debugging

---

### 🟧 Proficient (2.0 - 3.0)

**Core Behaviors:**
- Expert at finding root causes
- Systematic debugging approach
- Builds highly observable systems
- Others learn from their debugging
- Monitoring catches issues early
- Can diagnose complex production issues
- Logs and metrics tell story

**What You'd See:**
- Asked to debug complex problems
- Code has excellent logging
- Monitoring catches issues proactively
- Can diagnose production issues quickly
- Mentors others on debugging
- Builds observable systems

**Specific Examples:**
- "Based on these logs, the issue is in [component]. Here's proof."
- Added detailed logging that helped diagnose issue
- Created metrics that caught performance regression
- Taught team about effective monitoring
- Reduced MTTR for team dramatically

**Evidence:**
- Can diagnose issues others struggle with
- Code has great logging and monitoring
- Production issues resolved quickly
- Others ask them debugging questions
- Observability improvements from them
- Metrics catch problems early

**What Success Looks Like:**
- Recognized for debugging skills
- Others learn from their approach
- Monitoring initiatives from them
- Production reliability improves

**Development Focus:**
- Mentor others on observability
- Lead monitoring improvements
- Build debugging culture
- Teach systematic approaches
- Move toward architecture/operations

---

### 🟨 Expert (3.0 - 3.5)

**Core Behaviors:**
- Exceptional problem diagnosis
- Can find bugs others can't find
- Builds monitoring systems for others
- Mentors on monitoring strategy
- Production issues are solvable because of their monitoring
- Proactively prevents problems
- Drives observability improvements

**What You'd See:**
- Asked for complex debugging challenges
- Can find subtle bugs quickly
- Monitoring systems are exemplary
- Mentors team on monitoring
- Proactively identifies issues
- Production reliability from their work
- Others emulate their approach

**Specific Examples:**
- Found memory leak others missed by understanding allocation patterns
- Created monitoring that predicted capacity issue 3 weeks early
- Mentored team on effective logging practices
- Reduced MTTR org-wide through monitoring improvements
- Identified subtle race condition through log analysis

**Evidence:**
- Asked to debug complex issues
- Mentors others on debugging
- Monitoring systems are excellent
- MTTR reduced
- Production reliability improved
- Others ask for debugging advice

**What Success Looks Like:**
- Set debugging/monitoring standards
- Multiple people mentored
- Monitoring culture improved
- Org MTTR decreased
- Could move to operations/architecture

**Development Focus:**
- Scale observability across organization
- Mentor more people
- Lead monitoring initiatives
- Influence org approach
- Could move to operations leadership

---

### 🟥 Authority (3.5 - 4.0+)

**Core Behaviors:**
- Org's debugging/monitoring authority
- Sets observability standards
- Others emulate their monitoring
- Visible improvement in MTTR
- Production reliability improved
- Monitoring culture reflects their influence
- Org observability transformed

**What You'd See:**
- Org debugging standards from them
- Others model their monitoring approach
- MTTR decreased org-wide
- Production reliability visible
- Monitoring practices reflect their approach
- Multiple teams improved
- Org proactively detects issues

**Specific Examples:**
- "This is how we approach observability at our scale"
- Org adopted their logging/monitoring patterns
- MTTR improved 50% from their initiatives
- Production incidents decreased measurably
- "We debug this way because..."

**Evidence:**
- Org recognizes as authority
- Standards and practices from them
- MTTR improved
- Fewer production issues
- Multiple teams influenced
- Culture changed

---

## 🎯 Debugging Methodology

### Systematic Debugging Approach

**The Five-Step Method:**

1. **Understand the Symptom**
   - What's the actual problem?
   - When did it start?
   - How often does it happen?
   - Who/what is affected?

2. **Gather Evidence**
   - Look at logs
   - Check metrics
   - Examine error traces
   - Review recent changes

3. **Form Hypothesis**
   - What could cause this?
   - What's most likely?
   - What assumptions might be wrong?
   - How would you test it?

4. **Test Hypothesis**
   - Design test to confirm/deny
   - Use debugger, logs, or test
   - Look for confirming evidence
   - Discard if evidence says no

5. **Find Root Cause**
   - Why did this happen?
   - Is this the real cause or symptom?
   - What else could be wrong?
   - Is there a deeper issue?

### Common Debugging Techniques

| Technique | When to Use | Effectiveness |
|-----------|------------|---|
| Logging | Always available | High if good logs |
| Debugger | During development | Very high if code available |
| Profiler | Performance issues | Essential for perf debugging |
| Metrics | Production issues | High for system-level problems |
| Tracing | Complex interactions | Essential for distributed systems |
| Binary search | Narrow down issues | Very effective for location finding |

---

## 📊 Observable System Framework

### The Observability Pyramid

```
           Traces
          /     \
         /       \
        /         \
    Metrics   Logs
     \       /
      \     /
       \   /
      Business Outcomes
```

**Understanding Each Layer:**

- **Business Outcomes**: Is the system meeting its purpose?
- **Metrics**: System health (latency, errors, throughput)
- **Logs**: Detailed event records
- **Traces**: Request paths through system

### What to Monitor

**Technical Metrics:**
- Latency (p50, p95, p99)
- Error rate and types
- Throughput (requests/sec)
- Resource usage (CPU, memory, disk, network)
- Saturation (how full are resources?)

**Business Metrics:**
- User activity
- Feature usage
- Revenue/value impact
- Conversion rates
- User satisfaction

**Reliability Metrics:**
- Uptime/availability
- MTTR (mean time to repair)
- MTTD (mean time to detect)
- Error budget usage

### Effective Alerting

**Good Alerts:**
- ✅ Fire for real problems only
- ✅ Are actionable (you can do something)
- ✅ Include context (what's wrong?)
- ✅ Include runbook (what do I do?)

**Bad Alerts:**
- ❌ Alert fatigue (cry wolf)
- ❌ Unclear what's wrong
- ❌ Can't do anything about it
- ❌ Fire for non-issues

---

## ❓ Assessment Questions

**For Developing → Competent:**
- Walk me through how you'd debug [issue]. Where would you start?
- What would you look at to understand [system] behavior?
- How would you use the debugger to find this bug?
- What logging would help debug this?

**For Proficient → Expert:**
- Walk me through how you'd approach monitoring [system]. What would you measure?
- Tell me about a time you diagnosed a complex production issue. How did you do it?
- How would you make this system more observable?
- What monitoring alerts would you set for [critical system]?

**For Expert → Authority:**
- How should we approach observability org-wide?
- What monitoring investments would have biggest impact?
- How do we build debugging/monitoring culture?
- What's your approach to MTTR reduction?

---

## 👀 Evidence to Look For

### At Proficient Level (2.0-3.0)
- ✅ Finds bugs quickly and systematically
- ✅ Code has good logging and monitoring
- ✅ Can diagnose production issues effectively
- ✅ Monitoring catches problems early
- ✅ Others learn debugging techniques from them
- ✅ Production issues resolved quickly

### At Expert Level (3.0-3.5)
- ✅ Asked to investigate complex issues
- ✅ Mentors others on debugging
- ✅ Monitoring systems are excellent
- ✅ MTTR reduced due to their work
- ✅ Others ask for debugging advice
- ✅ Proactively identifies issues before customers

### At Authority Level (3.5-4.0)
- ✅ Org's observability improved
- ✅ Others follow their patterns
- ✅ Production issues quickly diagnosed
- ✅ MTTR decreased org-wide
- ✅ Debugging culture changed
- ✅ Fewer production issues due to monitoring

### Negative Indicators (Any Level)
- ❌ Can't find bugs without help
- ❌ Code has no logging
- ❌ Production "mysteries" happen often
- ❌ MTTR is very high
- ❌ Alerts go off constantly but mean nothing
- ❌ Can't understand what's happening in prod
- ❌ Logs are noise (too much/unclear)
- ❌ No monitoring strategy
- ❌ Production issues are surprises
- ❌ Defensive about production problems

---

## 🔗 Related Skills & Competencies

**Directly Connected:**
- **Technical Understanding** (Engineering Craft) - Understanding systems helps debug them
- **Writing Code** (Engineering Craft) - Observable code is easier to debug
- **Software Architecture** (Engineering Craft) - Debuggable systems are architecturally sound
- **Testing** (Engineering Craft) - Tests prevent bugs that need debugging

**Indirectly Connected:**
- **Initiative** (Soft Skills) - Proactively improving observability
- **Communication** (Soft Skills) - Explaining debugging findings
- **Team Leadership** (Leadership) - Building debugging culture
- **Developing Others** (Leadership) - Teaching debugging techniques

---

## 🎯 Development Goals & Progression Paths

### Competent → Proficient
**Goal:** "Master debugging; build observable systems"

**Specific Actions:**
- [ ] Debug [complex issue]; document approach and findings
- [ ] Add comprehensive logging to [critical system]
- [ ] Create monitoring/dashboards for [system]
- [ ] Teach debugging workshop to team
- [ ] Reduce MTTR for [system] by 50%
- [ ] Mentor one person on debugging
- [ ] Create debugging guide for [common issue type]

**Timeline:** 6-12 months

---

### Proficient → Expert
**Goal:** "Mentor widely; improve org observability; identify patterns"

**Specific Actions:**
- [ ] Mentor 2+ people on monitoring/debugging
- [ ] Audit observability of [critical systems]
- [ ] Identify observability gaps org-wide
- [ ] Create monitoring patterns adopted by team
- [ ] Reduce org MTTR by 25%+
- [ ] Teach monitoring workshop or write guide
- [ ] Build monitoring/dashboarding tool

**Timeline:** 12-24 months

---

### Expert → Authority
**Goal:** "Shape org's observability approach; scale impact"

**Specific Actions:**
- [ ] Define org's observability standards
- [ ] Lead org-wide observability improvement
- [ ] Mentor leaders on monitoring/debugging
- [ ] Create observability guidelines org-wide
- [ ] Implement observability platform
- [ ] Measure and improve org MTTR
- [ ] External visibility: conference or article

**Timeline:** 2-3+ years

---

## � Detailed Development Guidance

### Building Logging Practices

**Good Logging Principles:**

1. **Contextual**: Logs include context (user, request ID, timestamp)
2. **Leveled**: Different verbosity levels (ERROR, WARN, INFO, DEBUG)
3. **Searchable**: Easy to search and filter
4. **Performance-aware**: Logging doesn't bog down system
5. **Structured**: Machine-readable format (JSON, not free text)

**Good Logging Example:**

```javascript
// ❌ Bad: Not enough context
console.log("Error occurred");

// ✅ Good: Structured, contextual
logger.error({
  timestamp: new Date().toISOString(),
  userId: request.userId,
  requestId: request.id,
  error: "Payment processing failed",
  reason: error.message,
  retryable: true,
  context: { orderId, amount }
});
```

### Building Monitoring Practices

**Metrics-Driven Debugging:**

1. **Define what matters**: Business and technical health
2. **Collect the data**: Instrument code to emit metrics
3. **Store effectively**: Time-series database
4. **Visualize clearly**: Dashboards showing what you need
5. **Alert appropriately**: Only for real problems

### Creating Effective Dashboards

**Dashboard Design:**

1. **Tell a story**: Dashboards should answer questions
2. **Red/yellow/green**: Easy to scan status
3. **Drill-down capability**: Click to see details
4. **Context**: Thresholds, recent changes
5. **Actionable**: When you see something, you know what to do

---

## 💡 Key Principles

### 1. **Good Debugging Saves Days**
Investing in debugging skills and tools saves enormous amounts of time. A person who debugs in minutes vs. days is a huge multiplier.

### 2. **Observable Systems are Understandable Systems**
Systems that expose their behavior are systems you can understand and trust. Invest in observability.

### 3. **Prevention is Better Than Debugging**
Catching problems before they're bugs (through monitoring) is better than debugging them. Proactive > reactive.

### 4. **Logs are Data**
Structure logs as machine-readable data. Free-text logs are harder to search and analyze. Make logs queryable.

### 5. **You Should Know Before Customers**
Good monitoring means you know about problems before customers report them. This is success.

### 6. **MTTR Matters More Than MTTF**
You can't prevent all failures, but you can minimize time to fix. Great observability enables fast fixes.

---

## 🎯 Red Flags & Warnings

- ⚠️ **Production issues are surprises** — Monitoring missing
- ⚠️ **MTTR is very high** — Debugging/observability weak
- ⚠️ **Logs are useless noise** — Too much, or not searchable
- ⚠️ **Alert fatigue** — Too many alerts, low signal
- ⚠️ **No metrics for critical systems** — Blind spot
- ⚠️ **Debugging is guessing** — No systematic approach
- ⚠️ **Can't find root causes** — Shallow debugging
- ⚠️ **Logs disappear quickly** — Can't investigate later
- ⚠️ **No correlation between errors** — Hard to debug
- ⚠️ **Production is mystery** — Observability failing

---

## 🏆 Observable System Checklist

A truly observable system has:
- ✅ Comprehensive logging at key points
- ✅ Meaningful metrics for business and technical health
- ✅ Alerts for real problems (not noise)
- ✅ Easy correlation between logs, metrics, traces
- ✅ Good dashboards for common questions
- ✅ Quick MTTR when issues arise
- ✅ Structured, searchable logs
- ✅ Context in all logs (user, request, trace ID)
- ✅ Monitoring that catches problems early
- ✅ Debugging that finds root causes

---

**Remember:** Good monitoring is preventative. You should know about problems before customers do. Good debugging saves days. Invest in both.
