# Debugging & Monitoring

**Criterion:** Ability to find and fix bugs, diagnose production issues, and build observable systems through monitoring and logging.

---

## 📋 Quick Summary

| Level | Expectation |
|-------|-------------|
| **Developing (0.0-1.0)** | Debugging with guidance; struggles to find root causes |
| **Competent (1.0-2.0)** | Finds most bugs; adequate monitoring in code |
| **Proficient (2.0-3.0)** | Expert debugger; builds observable systems |
| **Expert (3.0-3.5)** | Exceptional diagnostics; mentors on monitoring |
| **Authority (3.5-4.0)** | Org debugging/monitoring authority; sets standards |

---

## 🎯 Definition

**Debugging & Monitoring** means:
- **Root Cause Analysis** - Finding the real problem, not symptoms
- **Problem Diagnosis** - Systematic approach to finding issues
- **Observable Systems** - Building systems you can understand in production
- **Monitoring Strategy** - Knowing what to measure and alert on
- **Production Comfort** - Confidence in understanding system behavior

---

## 📊 Level-by-Level Breakdown

### Developing (0.0-1.0)
- Frustrated by bugs; doesn't know where to start
- Lacks debugging technique
- Limited monitoring; can't understand production
- Asks for help to find bugs
- Log output is overwhelming or unhelpful

### Competent (1.0-2.0)
- Finds most bugs systematically
- Uses debugger effectively
- Adds monitoring to own code
- Can usually narrow down problems
- Learning root cause analysis

### Proficient (2.0-3.0)
- Expert at finding root causes
- Systematic debugging approach
- Builds highly observable systems
- Others learn from their debugging
- Monitoring catches issues early
- Can diagnose complex production issues

### Expert (3.0-3.5)
- Exceptional problem diagnosis
- Can find bugs others can't
- Builds monitoring systems for others
- Mentors on monitoring strategy
- Production issues are solvable because of their monitoring

### Authority (3.5-4.0)
- Org's debugging/monitoring authority
- Sets observability standards
- Others emulate their monitoring approach
- Visible improvement in MTTR (mean time to repair)
- Production reliability improved

---

## ❓ Assessment Questions

- Walk me through how you'd debug [issue].
- What would you monitor for this system? Why?
- How would you know if something was wrong in production?
- What's your approach to finding root causes?
- Can you explain what this log output tells us?

---

## 👀 Evidence to Look For

**Proficient:**
✅ Finds bugs quickly and systematically  
✅ Code has good logging and monitoring  
✅ Can diagnose production issues effectively  
✅ Monitoring catches problems early  
✅ Others learn debugging techniques from them  

**Expert:**
✅ Asked to investigate complex issues  
✅ Mentors others on debugging  
✅ Monitoring systems are excellent  
✅ MTTR reduced due to their monitoring  

**Authority:**
✅ Org's monitoring and observability improved  
✅ Others follow their observability patterns  
✅ Production issues are quickly diagnosed  

---

## 🔗 Related Skills

- **Technical Understanding** - Understanding systems helps debug them
- **Writing Code** - Observable code is easier to debug
- **Initiative** - Proactively improving observability

---

## 🎓 Coaching Strategies

**Developing:** Teach systematic debugging; pair debugging sessions

**Competent:** Teach monitoring strategy; discuss what to observe

**Proficient:** Position as debugging expert; have them teach others

**Expert/Authority:** Support observability leadership; involve in monitoring decisions

---

## 📝 Real Examples

**Developing:** "I don't know why it's broken. Can you help me figure it out?"

**Competent:** "I added logging here so we can see what's happening. Let me check the logs."

**Proficient:** "Based on these metrics and logs, the issue is likely in [component]. Here's how I'd diagnose it further."

**Expert:** "Here's what I notice from the monitoring. This pattern suggests [root cause]. I'd verify with [test]."

**Authority:** "Our systems should be designed for observability. Here's how we approach monitoring at our scale."

---

## 🎯 Development Goals

**Competent → Proficient:** "Owner responsibility for monitoring [system]. Make it observable."

**Proficient → Expert:** "Become org expert on debugging [complex system]. Mentor team."

**Expert → Authority:** "Lead org's observability and monitoring strategy."

---

## 🏆 Observable System Checklist

A truly observable system has:
- ✅ Comprehensive logging at key points
- ✅ Meaningful metrics for business and technical health
- ✅ Alerts for real problems (not noise)
- ✅ Easy correlation between logs, metrics, traces
- ✅ Good dashboards for common questions
- ✅ Quick MTTR when issues arise

---

**Remember:** Good monitoring is preventative. You should know about problems before customers do.
