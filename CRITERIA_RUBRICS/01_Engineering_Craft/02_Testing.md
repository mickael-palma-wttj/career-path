# Testing

**Criterion:** The ability to design and write effective tests that verify code correctness, catch regressions, and instill confidence in deployments.

---

## 📋 Quick Summary

| Level | Expectation |
|-------|-------------|
| **Developing (0.0-1.0)** | Writing basic tests with guidance; inconsistent coverage |
| **Competent (1.0-2.0)** | Writing tests that pass; adequate coverage for most code | Catches some bugs; team mostly confident |
| **Proficient (2.0-3.0)** | Writing comprehensive, well-designed tests; owns test quality | Strong confidence; catches real bugs; helps team |
| **Expert (3.0-3.5)** | Tests exemplify best practices; mentors on testing strategy | Trusted tester; shapes team approach; mentors others |
| **Authority (3.5-4.0)** | Sets org testing standards; influences testing culture | Org reliability improves; testing mindset spreads |

---

## 🎯 Definition

**Testing** encompasses five interconnected capabilities:

### 1. **Test Design Strategy**
Understanding what to test and why. Knowing the difference between unit, integration, and end-to-end tests. Making smart choices about test coverage that focus on behavior verification and catching real bugs.

### 2. **Test Implementation Skill**
Writing tests that are clear, reliable, and maintainable. Using testing frameworks and patterns effectively. Creating tests that fail for the right reasons and pass when behavior is correct.

### 3. **Reliability & Maintainability**
Writing tests that don't fail randomly (eliminating flakiness). Designing tests that survive code refactors. Creating test code that's as clean as production code.

### 4. **Coverage Thinking**
Determining appropriate coverage targets. Avoiding both under-testing (missing critical paths) and over-testing (testing implementation details). Understanding that coverage % is a tool, not a goal.

### 5. **Testing Culture & Advocacy**
Promoting good testing practices. Helping others improve. Identifying gaps in testing strategy. Moving the organization toward better testing.

---

## 📊 Level-by-Level Breakdown

### Level 0.0-1.0: Developing
**What You See:**
- Tests written only with prompting
- High test flakiness; tests fail unpredictably
- Tests verify implementation details rather than behavior
- Coverage is inconsistent; important paths untested
- Doesn't understand trade-offs in testing strategy
- Tests often harder to understand than the code

**Typical Statements:**
- "Should I write a test for this?"
- "My test keeps failing randomly"
- "I just copied the pattern from another test"
- "All my tests are passing... well, mostly"

**Core Behaviors:**
- Writes tests reactively, not proactively
- Doesn't think about test strategy
- Treats tests as checkbox item, not quality tool
- Can't diagnose why tests fail
- Copies test patterns without understanding
- Tests verify implementation, not behavior

**What You'd See:**
- No tests on new code
- Tests fail randomly on CI
- Tests tightly coupled to implementation
- Tests don't actually verify much
- Resists writing tests
- Gets frustrated with flakiness

**What Success Looks Like:**
- Consistently write tests with code
- Tests pass reliably
- Understanding why tests exist
- Testing becomes routine
- Tests verify actual behavior

**Development Focus:**
- Establish habit of testing
- Understand test value
- Learn to write reliable tests
- Think about what to test
- Build testing fundamentals

---

### Level 1.0-2.0: Competent
**What You See:**
- Tests are written as part of their routine
- Most tests are reliable; occasional flakiness
- Coverage is reasonable but has gaps
- Tests mostly verify behavior, but some over-specify
- Learning testing best practices through feedback
- Tests pass but don't inspire full confidence

**Typical Statements:**
- "I wrote tests for this"
- "Why didn't the test catch that bug?"
- "What's a good test coverage target?"
- "Should I test this edge case?"

**Core Behaviors:**
- Tests as routine part of work
- Basic test patterns understood
- Coverage thinking is developing
- Most tests are reliable
- Some flakiness still present
- Learning from feedback

**What You'd See:**
- Code comes with tests
- Tests mostly pass
- Coverage 60-75%
- Few but occasional flaky tests
- Testing patterns emerging
- Good faith effort on test quality

**Specific Examples:**
- New feature PR includes tests covering happy path and main edge cases
- Wrote 15 tests for data processing function (80% coverage achieved)
- Tests caught regression but missed similar edge case in different module

**What Success Looks Like:**
- 75%+ coverage consistently
- Reliable tests (no flakiness)
- Tests verify behavior
- Thoughtful about coverage
- Learning testing patterns

**Development Focus:**
- Increase coverage systematically
- Eliminate flakiness
- Understand test design patterns
- Think strategically about what to test
- Improve test code quality

---

### Level 2.0-3.0: Proficient
**What You See:**
- Tests are comprehensive and reliable
- Coverage is thoughtful; important paths covered
- Tests verify behavior, not implementation
- Test suite runs quickly and consistently
- Tests serve as documentation
- Others feel confident deploying code with these tests
- Proactively improves test quality

**Typical Statements:**
- "Let me add tests for the edge cases"
- "This test is too brittle; let me refactor it"
- "The coverage is good; shipping with confidence"
- "This test structure will make future changes easier"

**Core Behaviors:**
- Tests are comprehensive and reliable
- Design tests intentionally
- Cover critical paths thoughtfully
- Eliminate flakiness proactively
- Test code is clean and DRY
- Mentors others on testing

**What You'd See:**
- Coverage 80%+ consistently
- Zero flaky tests
- Tests verify actual behavior
- Test refactoring happens naturally
- Tests serve as documentation
- Team trusts their tests
- Proactively improves test infrastructure

**Specific Examples:**
- Feature has 85% coverage; tests cover main flows, edge cases, error scenarios
- "I noticed tests were timing-dependent; refactored to use controlled timing"
- Helped junior improve test design; taught about parametrized tests
- Test caught critical edge case in production-like scenario

**Evidence:**
- Coverage consistently 80%+
- No flaky test complaints
- Other engineers reference their tests
- Bugs are caught by tests
- Team confidence in deployments
- Tests help with refactoring

**What Success Looks Like:**
- Recognized for test quality
- Mentoring others
- Test quality standards improving
- Initiatives to improve test infrastructure
- Tests consistently catch bugs

**Development Focus:**
- Mentor others on testing
- Improve test speed/efficiency
- Establish testing patterns for team
- Strategic coverage thinking
- Leadership on testing improvements

---

### Level 3.0-3.5: Expert
**What You See:**
- Tests are exemplary; others study their test code
- Comprehensive coverage with smart test design
- Tests are fast, reliable, and maintainable
- Mentors others on testing practices
- Identifies gaps in org's testing approach
- Advocates for test quality improvements
- Balances coverage and test maintenance costs

**Typical Statements:**
- "Let me show you how I'd approach testing this"
- "This test is too slow; here's how to speed it up"
- "Our testing strategy should be..."
- "I've found a pattern that makes tests more maintainable"

**Core Behaviors:**
- Tests are exemplary and used as reference
- Deep understanding of testing patterns
- Mentors others on testing strategy
- Proactively improves test infrastructure
- Identifies testing gaps across codebase
- Advocates for time on test improvements

**What You'd See:**
- Tests used as examples for others
- Mentoring juniors on testing
- Identified and fixed flaky tests across codebase
- Implemented testing patterns adopted team-wide
- Reduced test execution time significantly
- Coverage thoughtfully targeted 85-90%+
- Test code is exemplary

**Specific Examples:**
- "I created a test factory pattern that the team now uses"
- Mentored 2+ engineers on testing; they improved significantly
- Identified slow tests; refactored to run 10x faster
- Created testing guide that shaped team approach
- Helped team reduce production issues from untested scenarios

**Evidence:**
- Others ask for testing advice
- Test patterns and strategies reference theirs
- Proactively improves testing across codebase
- Mentors on testing practices
- Org testing quality visibly improves
- Fast, reliable, comprehensive tests

**What Success Looks Like:**
- Set testing standards for team
- Multiple people mentored
- Testing initiatives led by them
- Org-wide testing improvements
- Could transition to testing leadership

**Development Focus:**
- Scale impact across organization
- Lead testing improvements
- Mentor more people
- Shape org testing culture
- Could move to architecture/leadership

---

### Level 3.5-4.0: Authority
**What You See:**
- Defines how organization approaches testing
- Org-wide improvements in test quality and coverage
- Created testing tools, patterns, or guidelines adopted widely
- Others reference their test strategies
- Visible reduction in production bugs
- Testing culture reflects their influence
- Makes strategic testing decisions

**Typical Statements:**
- "We should establish this as our testing standard"
- "Here's how we should think about testing at scale"
- "Let me create a guide for this test pattern"
- "Our testing practices have improved because..."

**Core Behaviors:**
- Authority on testing approach
- Org testing quality shaped by them
- Creates patterns adopted widely
- Mentors leaders on testing
- Strategic testing decisions from them
- Visible org improvements

**What You'd See:**
- Org testing standards from them
- Testing tools/frameworks reflect their input
- Others model their approach
- Production issues decrease
- Org coverage standards from them
- Testing culture reflects their thinking
- Multiple teams improved by their guidance

**Specific Examples:**
- Created testing strategy adopted across engineering
- Testing framework migration driven by them
- Org coverage improved 30% based on their initiatives
- Multiple leaders learned testing approach from them
- Engineering hires assessed on their testing standards

**Evidence:**
- Org recognizes as testing authority
- Org testing quality improving
- Strategies and standards from them adopted
- Multiple teams influenced
- Production quality improvements
- Testing culture changes visible

---

## 📊 Testing Strategy Framework

### Understanding Test Types

**Unit Tests:** Test single functions/classes in isolation
- Speed: Very fast
- Isolation: Complete (usually mocked dependencies)
- Use Case: Verify logic, edge cases
- Coverage Goal: 70-90% of most code
- Examples: Pure functions, calculations, string processing

**Integration Tests:** Test multiple components working together
- Speed: Moderate (seconds, not milliseconds)
- Isolation: Some real dependencies
- Use Case: Verify components work together
- Coverage Goal: 20-40% of critical paths
- Examples: API endpoints, database queries, service interactions

**End-to-End Tests:** Test full user workflows
- Speed: Slow (minutes for suite)
- Isolation: None; real dependencies
- Use Case: Verify complete workflows work
- Coverage Goal: 5-10% of most critical flows only
- Examples: Login flow, payment workflow, key user scenarios

### Coverage Strategy Matrix

| Scenario | Unit | Integration | E2E | Total |
|----------|------|-------------|-----|-------|
| Core business logic | 70-90% | 10-20% | 5% | ~100% |
| API endpoints | 50-60% | 40-50% | 10% | ~100% |
| UI workflows | 30-40% | 20-30% | 30-40% | ~100% |
| Infrastructure | 30-50% | 30-50% | 0% | ~60-80% |

---

## ❓ Assessment Questions

**For yourself (when reviewing tests):**
- Do these tests verify behavior or implementation details?
- If I changed the code (but kept behavior same), would tests still pass?
- What would happen if this code had a bug? Would these tests catch it?
- Are the tests fast? Do they have external dependencies?
- Would someone new understand what these tests verify?
- Does coverage align with business criticality?
- Are these tests reliable or do they have timing/ordering issues?
- Am I testing too many things in one test?

**For conversation (Developing → Competent):**
- Walk me through your testing approach for this feature. Why did you test it this way?
- What scenarios did you consider testing? Any you decided not to test?
- If I introduced a subtle bug here, would your tests catch it?
- This test is flaky (fails randomly). How would you debug it?

**For conversation (Proficient → Expert):**
- How would you improve the test strategy for this system?
- This code has low coverage. How would you decide what to test?
- Tell me about a time you mentored someone on testing. How did it go?
- What's your philosophy on test maintenance? How do you keep tests from becoming burden?

**For conversation (Expert → Authority):**
- How should we think about testing strategy at org level?
- What testing improvements would have biggest impact?
- How would you build testing culture across engineering?
- What's your approach to testing in systems with high churn?

---

## 👀 Evidence to Look For

### At Proficient Level (2.0-3.0)
✅ Coverage is 75-85% and thoughtful
✅ Tests are reliable; no flakiness complaints
✅ New code comes with comprehensive tests
✅ Tests catch bugs when deployed
✅ Team feels confident with their test suite
✅ Test refactoring happens without breaking code
✅ Tests serve as documentation

### At Expert Level (3.0-3.5)
✅ Tests are used as reference by others
✅ Proactively fixes flaky tests across codebase
✅ Mentors others on testing patterns
✅ Owns testing improvement initiatives
✅ Tests are remarkably fast and reliable
✅ Others ask them for testing advice
✅ Team testing practices improved because of them

### At Authority Level (3.5-4.0)
✅ Org testing quality has improved
✅ Coverage standards set and adopted
✅ Testing tools or frameworks reflect their input
✅ Others reference their testing approach
✅ Testing culture reflects their leadership
✅ Production issues from untested code decrease
✅ Multiple teams model their testing

### Negative Indicators (Any Level)
❌ Tests failing randomly (flakiness)
❌ Tests tightly coupled to implementation
❌ Over-specifying tests (brittle)
❌ Skipping tests on urgent work
❌ Not writing tests at all
❌ Tests don't actually verify anything
❌ Coverage % without substance
❌ Tests taking as long as development
❌ No strategy; just following patterns
❌ Defending poor test quality

---

## 🔗 Related Skills & Competencies

**Directly Connected:**
- **Writing Code** (Engineering Craft) - Tests are code; quality matters
- **Technical Understanding** (Engineering Craft) - Understanding system informs test design
- **Debugging & Monitoring** (Engineering Craft) - Tests prevent bugs that need debugging
- **Software Architecture** (Engineering Craft) - Testability influences design

**Indirectly Connected:**
- **Communication** (Soft Skills) - Tests communicate behavior; clear tests teach
- **Initiative** (Soft Skills) - Proactively improving test quality
- **Objectivity** (Soft Skills) - Test data and feedback drive decisions
- **Team Leadership** (Leadership) - Models testing practices for team

---

## 🎯 Development Goals & Progression Paths

### Developing → Competent
**Goal:** "Make testing routine and understand what good tests look like"

**Specific Actions:**
- [ ] Write tests for every new feature you build
- [ ] Study 3 good test examples in codebase; understand why they're good
- [ ] Fix one flaky test in codebase; document what made it flaky
- [ ] Learn your testing framework thoroughly (read docs)
- [ ] Pair with [Expert person] on writing tests
- [ ] Get to 70% coverage on your code
- [ ] Stop copying test patterns; write from understanding

**Timeline:** 3-6 months

**Key Milestones:**
- Month 1: Testing every feature is routine
- Month 2-3: Tests mostly pass reliably
- Month 3-6: Coverage 70%+, tests verify behavior

---

### Competent → Proficient
**Goal:** "Master test design; own test quality; help others"

**Specific Actions:**
- [ ] Increase coverage to 85% with thoughtful tests
- [ ] Eliminate all flaky tests in your code
- [ ] Have one feature with exemplary tests; explain why
- [ ] Refactor tests to be more maintainable; document changes
- [ ] Mentor one person on testing; help improve their tests
- [ ] Lead discussion on "what should we test?"
- [ ] Create testing documentation for [new feature area]

**Timeline:** 6-12 months

**Key Milestones:**
- Month 1-2: 80%+ coverage consistently
- Month 3-6: Zero flakiness; tests serve documentation
- Month 6-12: Mentoring others; setting patterns

---

### Proficient → Expert
**Goal:** "Mentor widely; improve team testing; identify gaps"

**Specific Actions:**
- [ ] Mentor 2+ people on advanced testing topics
- [ ] Identify one testing gap in codebase; propose solution
- [ ] Improve test execution time by 25%+
- [ ] Create testing pattern adopted by team
- [ ] Lead initiative to fix flaky tests across codebase
- [ ] Contribute to testing tool/framework evaluation
- [ ] Teach class or write guide on testing

**Timeline:** 12-24 months

**Key Milestones:**
- Month 1-6: Recognized for test quality and mentoring
- Month 6-12: Leading improvements; mentoring multiple people
- Month 12-24: Testing culture influenced by you

---

### Expert → Authority
**Goal:** "Shape org's testing approach; scale impact"

**Specific Actions:**
- [ ] Define org testing standards and get adoption
- [ ] Lead testing improvement initiative
- [ ] Mentor leaders on testing strategy
- [ ] Contribute to testing tool/framework selection org-wide
- [ ] Measure and improve org testing quality
- [ ] Create testing guide adopted across org
- [ ] External visibility: conference talk or article on testing

**Timeline:** 2-3+ years

**Key Milestones:**
- Year 1: Org testing quality improving
- Year 2: Standards and tools reflect your input
- Year 2-3: Multiple teams modeling your approach

---

## 📚 Detailed Development Guidance

### Eliminating Flaky Tests

**What Makes Tests Flaky:**
- Timing dependencies (tests pass 90% of time, fail 10% randomly)
- External service dependencies (API might be slow)
- Shared state (test execution order matters)
- Randomness (tests with random data or timing)
- Resource limits (running out of memory at random times)

**How to Find Flaky Tests:**
1. Run tests 10+ times; see which fail inconsistently
2. Check CI logs for failures on otherwise passing code
3. Ask team: "Which tests fail randomly?"
4. Run tests in different orders
5. Run tests with different system load

**How to Fix Flaky Tests:**
```javascript
// ❌ Flaky: Timing-dependent
test('message appears quickly', (done) => {
  setTimeout(() => {
    expect(getMessage()).toBe('hello');
    done();
  }, 100); // Fails on slow machines
});

// ✅ Reliable: Controlled timing
jest.useFakeTimers();
test('message appears after timeout', () => {
  const callback = jest.fn();
  setTimeout(callback, 100);
  jest.advanceTimersByTime(100);
  expect(callback).toHaveBeenCalled();
});

// ❌ Flaky: External dependency
test('fetches user data', async () => {
  const user = await fetchUserFromAPI(); // Real network call
  expect(user.name).toBe('John');
});

// ✅ Reliable: Mocked dependency
test('fetches user data', async () => {
  jest.spyOn(api, 'getUser').mockResolvedValue({ name: 'John' });
  const user = await fetchUserFromAPI();
  expect(user.name).toBe('John');
});
```

**Key Principles:**
- Control time (use fake timers)
- Mock external services
- Avoid ordering dependencies
- Isolate test state
- Use deterministic data

### Building Test Design Skills

**Good Test Design Checklist:**

1. **Tests verify behavior, not implementation**
   - ❌ Wrong: `test('x variable assigned', ...)`
   - ✅ Right: `test('function returns correct value', ...)`

2. **Tests are independent**
   - ❌ Wrong: Test depends on order of execution
   - ✅ Right: Each test is completely independent

3. **Tests are clear about intent**
   - ❌ Wrong: Test name doesn't explain what it tests
   - ✅ Right: `test('rejects expired tokens with 401 error')`

4. **Tests fail for right reason**
   - ❌ Wrong: Test passes even with broken code
   - ✅ Right: Test fails only when behavior changes

5. **Tests are maintainable**
   - ❌ Wrong: Duplicated test setup across 50 tests
   - ✅ Right: DRY test code with shared utilities

6. **Tests run fast**
   - ❌ Wrong: Tests hit real database (5 seconds)
   - ✅ Right: Tests with mocks (50 milliseconds)

### Strategic Coverage Thinking

**The Coverage Pyramid:**
```
         ▲
        /|\
       / | \  E2E Tests (5%)
      /  |  \
     /   |   \
    /____|____\ Integration (20%)
   /     |     \
  / Unit Tests  \  (75%)
 /_______|_______\
```

**Coverage by Business Criticality:**

| Code Type | Why | Coverage Target |
|-----------|-----|-----------------|
| Core business logic | Most bugs here; highest impact | 80-95% |
| Payment/security | Failures very costly | 90-100% |
| UI components | Testing slower than value | 30-50% |
| Infrastructure | Harder to test; lower ROI | 40-60% |
| Configuration | Low ROI on testing | 0-30% |

**Coverage Questions:**
1. What fails if this code breaks?
2. How much would that failure cost?
3. How likely is the bug?
4. How hard would testing be?
5. Should we test it?

### Mentoring Others on Testing

**How to Help Someone Improve Their Testing:**

1. **Start with mindset** - "Tests should make you sleep well before production"
2. **Show examples** - Review good tests together; explain why they're good
3. **Test together** - Write tests as pair; narrate your thinking
4. **Review process** - Review test quality as carefully as code
5. **Ask questions** - "What scenarios would break this?" "Is this flaky?"
6. **Celebrate** - When their test catches a bug, celebrate loudly!

**Coaching Language:**
- "Great instinct to test this. Let me show you how to make it even better..."
- "Your test is close. What behavior are we really verifying here?"
- "This test is brittle. How would you make it more robust?"
- "Love that you caught this edge case. How would you test it?"

---

## 💡 Key Principles

### 1. **Tests Are First-Class Code**
Tests are not second-class. Test code quality matters as much as production code. Invest in clean, maintainable tests.

### 2. **Test Reliability is Non-Negotiable**
One flaky test ruins trust in the entire suite. Flaky tests should be fixed immediately, not ignored. Reliability first.

### 3. **Test Intent Over Coverage %**
90% coverage of bad tests doesn't help. 70% coverage of good tests is better. Coverage % is a guide, not a goal.

### 4. **Tests Enable Confidence**
Great tests let you deploy with confidence. If you're nervous before deploy, your tests aren't good enough. Tests should enable speed and safety.

### 5. **Good Tests Document Behavior**
Tests are executable documentation. Someone should understand system behavior by reading tests. Clear intent means clear behavior.

### 6. **Testing Scales Exponentially**
Investing in good testing patterns early pays dividends. Bad test practices compound. Establish good patterns early.

---

## 🎯 Red Flags & Warnings

⚠️ **Test flakiness increasing** — Tests unreliable; architecture issue
⚠️ **Coverage declining** — Less testing; quality declining
⚠️ **Tests taking longer than code** — Inefficient tests or over-testing
⚠️ **Skipping tests on urgent work** — Slowing down next sprint
⚠️ **Tests not catching bugs** — Not testing right things
⚠️ **Difficulty adding tests to legacy code** — Architecture problem
⚠️ **Tests too tightly coupled to implementation** — Will break on refactors
⚠️ **No test code review** — Test quality not owned
⚠️ **Testing only after bugs found** — Wrong philosophy
⚠️ **Testing culture disconnected from quality** — Not connecting dots

---

**Remember:** Great tests are like great code—they're an investment that pays dividends. Good tests let you sleep at night before deployments.

---

## 🔍 How It Manifests in Work

### Coverage
| Level | Appearance |
|-------|-----------|
| Developing | < 50% coverage; major gaps in critical paths |
| Competent | 60-75% coverage; some gaps but main paths covered |
| Proficient | 75-90% coverage; thoughtful about what matters |
| Expert | 85-95% coverage; smart about edge cases |
| Authority | Org standard 80%+; coverage is thoughtfully targeted |

### Test Reliability
| Level | Appearance |
|-------|-----------|
| Developing | Frequent random failures; "flaky tests" |
| Competent | Mostly reliable; occasional timing/ordering issues |
| Proficient | Consistently reliable; fails only when code changes |
| Expert | Consistently 100% reliable; no flakiness |
| Authority | Org-wide reliability standards; fixes flaky tests |

### Test Design Quality
| Level | Appearance |
|-------|-----------|
| Developing | Tests are brittle; fail on refactors; over-specified |
| Competent | Tests are mostly behavior-focused; some brittleness |
| Proficient | Tests verify behavior; refactor-safe; clear intent |
| Expert | Tests are elegant; document behavior beautifully |
| Authority | Tests define how org thinks about verification |

### Test Documentation
| Level | Appearance |
|-------|-----------|
| Developing | Tests are unclear; hard to understand purpose |
| Competent | Tests are mostly clear; occasional confusion |
| Proficient | Tests serve as documentation of behavior |
| Expert | Tests are exemplary documentation |
| Authority | Tests educate others about system behavior |

---

## ❓ Assessment Questions

**For yourself (when reviewing tests):**
- Do these tests verify behavior or implementation details?
- If I changed the code (but kept behavior same), would tests still pass?
- What would happen if this code had a bug? Would these tests catch it?
- Are the tests fast? Do they have external dependencies?
- Would someone new understand what these tests verify?
- Does coverage align with business criticality?

**For conversation:**
- Walk me through your testing strategy for this feature. Why did you test it this way?
- If I introduced a subtle bug here, would your tests catch it?
- What test scenarios concern you for this code?
- How much of this code is covered by tests? What's not covered and why?
- If this test fails in production, what would you do?

**For feedback:**
- This test is passing but doesn't feel like it's testing the right thing. What are you trying to verify?
- Your test coverage is good. What's your confidence level in this code?
- This test is timing-dependent. How would you make it reliable?

---

## 👀 Evidence to Look For

### At Proficient Level (2.0-3.0)
✅ Coverage is 75%+ and thoughtful  
✅ Tests are reliable; no flakiness complaints  
✅ New code comes with comprehensive tests  
✅ Tests catch bugs when deployed  
✅ Team feels confident with their test suite  
✅ Code that breaks tests broke actual functionality  

### At Expert Level (3.0-3.5)
✅ Tests are used as reference by others  
✅ Proactively fixes flaky tests across codebase  
✅ Mentors others on testing patterns  
✅ Owns testing improvement initiatives  
✅ Tests are remarkably fast and reliable  
✅ Others ask them for testing advice  

### At Authority Level (3.5-4.0)
✅ Org testing quality has improved  
✅ Coverage standards set and adopted  
✅ Testing tools or frameworks reflect their input  
✅ Others reference their testing approach  
✅ Testing culture reflects their leadership  
✅ Production issues from untested code decrease  

---

## ⚠️ Common Misconceptions

### Misconception 1: "High Coverage = Good Testing"
**Reality:** 90% coverage of bad tests doesn't help. Test quality and coverage intent matter more than raw numbers.

### Misconception 2: "If Tests Pass, Code is Correct"
**Reality:** Bad tests pass! Tests must verify actual behavior, not just run without errors.

### Misconception 3: "Testing is Slower than Not Testing"
**Reality:** Testing takes time upfront but saves time on debugging, rework, and production issues.

### Misconception 4: "Unit Tests are the Only Tests That Matter"
**Reality:** Unit, integration, and end-to-end tests all serve purposes. Strategy matters.

### Misconception 5: "We Test the Implementation"
**Reality:** Great tests verify behavior. They're decoupled from implementation details.

---

## 🔗 Related Skills

- **Writing Code** - Tests are code; quality matters
- **Technical Understanding** - Understand system to design good tests
- **Debugging & Monitoring** - Tests prevent bugs that need debugging
- **Communication** - Tests communicate behavior
- **Initiative** - Proactively improving test quality and coverage

---

## 🎓 Coaching Strategies

### For Developing Level (0.0-1.0)
1. **Establish Expectation** - Testing is non-negotiable
2. **Teach Testing Patterns** - Show common patterns in your codebase
3. **Pair Testing** - Write tests together to show strategy
4. **Review Rigorously** - Review test quality as carefully as code quality
5. **Celebrate Catches** - When their test catches a bug, celebrate!

**Conversation Starter:**
"Great work on writing tests. Let me show you how to make them even more effective..."

### For Competent Level (1.0-2.0)
1. **Show Examples** - Point to excellent tests in codebase
2. **Discuss Strategy** - Talk about what deserves tests
3. **Improve Reliability** - Help eliminate flakiness
4. **Edge Cases** - Discuss important scenarios to test
5. **Coverage Thinking** - Move beyond just coverage %

**Conversation Starter:**
"Your test coverage is good. I want to help you write tests that really catch bugs..."

### For Proficient Level (2.0-3.0)
1. **Leadership** - Have them review test quality across team
2. **Patterns** - Ask them to establish testing conventions
3. **Teaching** - Mentor juniors on testing
4. **Strategy** - Discuss org-wide testing approach
5. **Recognition** - Highlight their test quality

**Conversation Starter:**
"Your tests are exemplary. I'd like you to help the team raise our testing standards..."

### For Expert & Authority Levels (3.0+)
1. **Org Impact** - Lead testing improvements
2. **Tools & Frameworks** - Invest in testing infrastructure
3. **Culture** - Shape how org thinks about testing
4. **Strategic** - Involve in complex testing challenges
5. **Thought Leadership** - Share approaches with peers

**Conversation Starter:**
"Your testing approach is exceptional. How can we scale this across the organization?"

---

## 📝 Real Examples

### Scenario: What to Test

**Developing:**
```javascript
// Tests every line but doesn't verify actual behavior
test('function returns a number', () => {
  expect(typeof calculateDiscount(100, 0.1)).toBe('number');
});

test('discount variable gets assigned', () => {
  // Tests implementation detail
  expect(calculateDiscount.toString()).toContain('const discount =');
});
```
*Problem: Tests don't verify actual behavior. Would pass with broken code.*

**Competent:**
```javascript
test('calculateDiscount applies discount correctly', () => {
  expect(calculateDiscount(100, 0.1)).toBe(90);
});

test('calculateDiscount handles edge cases', () => {
  expect(calculateDiscount(0, 0.5)).toBe(0);
  expect(calculateDiscount(100, 0)).toBe(100);
});
```
*Better: Verifies behavior, but still missing some edge cases.*

**Proficient:**
```javascript
describe('calculateDiscount', () => {
  it('applies discount percentage correctly', () => {
    expect(calculateDiscount(100, 0.1)).toBe(90);
    expect(calculateDiscount(200, 0.25)).toBe(150);
  });

  it('handles edge cases gracefully', () => {
    expect(calculateDiscount(0, 0.5)).toBe(0);
    expect(calculateDiscount(100, 0)).toBe(100);
    expect(calculateDiscount(100, 1)).toBe(0);
  });

  it('rejects invalid inputs', () => {
    expect(() => calculateDiscount(-100, 0.1)).toThrow();
    expect(() => calculateDiscount(100, 1.5)).toThrow();
  });
});
```
*Good: Comprehensive, verifies behavior, catches likely bugs.*

**Expert:**
```javascript
describe('calculateDiscount', () => {
  const testCases = [
    { price: 100, discount: 0.1, expected: 90 },
    { price: 200, discount: 0.25, expected: 150 },
    { price: 0, discount: 0.5, expected: 0 },
  ];
  
  testCases.forEach(({ price, discount, expected }) => {
    it(`correctly calculates discount for $${price} with ${discount * 100}%`, () => {
      expect(calculateDiscount(price, discount)).toBe(expected);
    });
  });

  it('rejects invalid inputs with descriptive errors', () => {
    expect(() => calculateDiscount(-100, 0.1))
      .toThrow('Price must be non-negative');
    expect(() => calculateDiscount(100, 1.5))
      .toThrow('Discount must be between 0 and 1');
  });
});
```
*Excellent: DRY, parametrized, clear test intent, good error messages.*

---

### Scenario: Flaky vs. Reliable Tests

**Flaky:**
```javascript
test('response comes back quickly', (done) => {
  setTimeout(() => {
    expect(true).toBe(true);
    done();
  }, 100); // Arbitrary delay; fails on slow machine
});

test('data arrives in correct order', async () => {
  // Depends on execution order or timing
  const results = await fetchData();
  expect(results[0].id).toBe(1); // Might not be in order!
});
```
*Problem: Tests fail unpredictably based on timing or system state.*

**Reliable:**
```javascript
jest.useFakeTimers();

test('response is processed after timeout', () => {
  const callback = jest.fn();
  scheduleCallback(callback, 100);
  jest.advanceTimersByTime(100);
  expect(callback).toHaveBeenCalled();
});

test('data items have expected properties', async () => {
  const results = await fetchData();
  results.forEach(item => {
    expect(item).toHaveProperty('id');
    expect(typeof item.id).toBe('number');
  });
});
```
*Good: Tests control timing; don't depend on order; verify properties not sequence.*

---

## 🎯 Development Goals by Level

**If currently at Competent, goal is Proficient:**
- "Increase test coverage from 70% to 85% with thoughtful tests"
- "Eliminate flaky tests in my features"
- "Have zero tests that test implementation details"

**If currently at Proficient, goal is Expert:**
- "Mentor 2 juniors on testing best practices"
- "Reduce flakiness across entire codebase by 50%"
- "Establish testing standards that team adopts"

**If currently at Expert, goal is Authority:**
- "Lead testing improvement initiative org-wide"
- "Create testing tool adopted by multiple teams"
- "Measurably improve org's production quality through testing"

---

**Remember:** Great tests are like great code—they're an investment that pays dividends. Good tests let you sleep at night before deployments.
