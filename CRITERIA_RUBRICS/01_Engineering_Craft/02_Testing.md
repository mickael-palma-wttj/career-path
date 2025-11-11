# Testing

**Criterion:** The ability to design and write effective tests that verify code correctness, catch regressions, and instill confidence in deployments.

---

## 📋 Quick Summary

| Level | Expectation |
|-------|-------------|
| **Developing (0.0-1.0)** | Writing basic tests with guidance; inconsistent coverage |
| **Competent (1.0-2.0)** | Writing tests that pass; adequate coverage for most code |
| **Proficient (2.0-3.0)** | Writing comprehensive, well-designed tests; owns test quality |
| **Expert (3.0-3.5)** | Tests exemplify best practices; mentors on testing strategy |
| **Authority (3.5-4.0)** | Sets org testing standards; influences testing culture |

---

## 🎯 Definition

**Testing** means designing and implementing test suites that:
- **Verify Correctness** - Tests confirm code behaves as intended
- **Catch Regressions** - Tests prevent broken code from deploying
- **Document Behavior** - Tests serve as executable documentation
- **Enable Refactoring** - Good tests allow safe code changes
- **Scale Well** - Tests run fast and remain maintainable

This criterion evaluates both the technical skill of writing tests and the judgment about *what* to test and *how much* testing is appropriate.

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

**Manager's Focus:**
- Establish that testing is non-negotiable
- Teach testing patterns and frameworks
- Show why tests matter (demo a regression catch)
- Review test quality as carefully as code quality
- Help them understand "good" tests

---

### Level 1.0-2.0: Competent
**What You See:**
- Tests are written as part of their routine
- Most tests are reliable; occasional flakiness
- Coverage is reasonable but has gaps
- Tests mostly verify behavior, but some over-specify
- Learning testing best practices through feedback
- Tests pass but don't inspire confidence

**Typical Statements:**
- "I wrote tests for this"
- "Why didn't the test catch that bug?"
- "What's a good test coverage target?"
- "Should I test this edge case?"

**Manager's Focus:**
- Model good test design
- Point out gaps in test strategy
- Discuss test coverage goals
- Celebrate when tests catch bugs
- Gradually increase expectations

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

**Manager's Focus:**
- Use their tests as examples to others
- Ask them to review test quality
- Have them establish testing patterns
- Move toward testing strategy thinking
- Challenge to reduce flakiness across codebase

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

**Manager's Focus:**
- Use them to set testing standards
- Have them lead testing improvements
- Ask them to mentor on testing practices
- Involve in testing tool/framework decisions
- Use their tests as training material

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

**Manager's Focus:**
- Leverage expertise for org-wide improvements
- Support leading testing initiatives
- Involve in hiring/training on testing
- Challenge with complex testing problems
- Amplify their influence on testing culture

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
