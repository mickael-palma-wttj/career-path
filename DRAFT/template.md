# Advocating for testing

The **Advocating for Testing** criterion measures a junior developer's ability to promote good testing practices, share the value of testing with teammates, and contribute to building a positive testing culture.

This progression shows the journey from understanding testing's importance personally to beginning to influence others and advocate for better testing practices within the team.

**Progression Scale**:

0.0 → 1.0 → 2.5 → 3.6 → 4.0

**Weight**:

0-50% of Testing competency

<aside>
🧭

You understand the value of testing and begin to share that enthusiasm with others, contributing to discussions about testing practices and helping create a positive testing culture.

</aside>

## **🫆 Key characteristics**

- Demonstrates enthusiasm for testing and its benefits
- Shares testing knowledge and experiences with teammates
- Speaks up when testing practices could be improved
- Helps other junior developers understand testing importance
- Contributes to positive team discussions about testing

## **📚 Specific behaviors & examples**

### **✅  What good looks like**

- Shares success stories when tests catch bugs
- Offers to help teammates with testing challenges
- Suggests testing improvements during retrospectives
- Demonstrates testing benefits through examples
- Encourages good testing practices in code reviews
- Shows excitement about learning new testing techniques

### Examples

- **Sharing testing success stories**
    
    ```jsx
    // During team standup or retrospective:
    
    "Yesterday I was refactoring the user validation function, and my tests 
    caught a bug where empty strings weren't being handled correctly. 
    Without the tests, this would have made it to production and caused 
    user registration failures. It really showed me how valuable having 
    good test coverage is!"
    
    // The test that caught the bug:
    describe('validateUserInput', () => {
      test('should reject empty username', () => {
        const result = validateUserInput({ username: '', email: 'test@example.com' });
        expect(result.isValid).toBe(false);
        expect(result.errors).toContain('Username is required');
      });
      
      test('should reject whitespace-only username', () => {
        const result = validateUserInput({ username: '   ', email: 'test@example.com' });
        expect(result.isValid).toBe(false);
        expect(result.errors).toContain('Username is required');
      });
    });
    ```
    
- **Offering help to teammates**
    
    ```jsx
    // In team chat or during pair programming:
    
    "Hey @teammate, I saw you're working on the payment processing feature. 
    I recently learned how to test async functions with mocks - would you 
    like me to show you how I approached testing the email service? 
    It might help with testing the payment API calls."
    
    // Example of sharing knowledge:
    describe('Payment Processing', () => {
      test('should process payment and send confirmation email', async () => {
        // Mock the external payment service
        const mockPaymentService = jest.fn().mockResolvedValue({
          success: true,
          transactionId: 'txn_123'
        });
        
        // Mock the email service
        const mockEmailService = jest.fn().mockResolvedValue(true);
        
        const result = await processPayment({
          amount: 100,
          paymentMethod: 'card',
          userEmail: 'user@example.com'
        });
        
        expect(mockPaymentService).toHaveBeenCalledWith({
          amount: 100,
          method: 'card'
        });
        expect(mockEmailService).toHaveBeenCalledWith({
          to: 'user@example.com',
          template: 'payment_confirmation',
          data: { transactionId: 'txn_123' }
        });
      });
    });
    ```
    
- **Contributing to testing discussions**
    
    ```markdown
    // During retrospective or team meeting:
    
    "I've noticed that when we have good tests, I feel much more confident 
    making changes to the code. Maybe we could set aside some time each sprint 
    to add tests to older code that doesn't have coverage? 
    
    I'd be happy to volunteer for that - I think it would help everyone feel 
    more confident about refactoring and would prevent bugs from reaching production."
    
    // Follow-up suggestion:
    "What if we made it a team practice to celebrate when someone's tests 
    catch a bug? It would help reinforce how valuable testing is."
    ```
    

## **⚙️ Development actions**

1. **Build Testing Enthusiasm**
    - Celebrate when your tests catch bugs or prevent issues
    - Share positive testing experiences with the team
    - Learn about testing benefits beyond bug prevention (documentation, confidence, etc.)
2. **Share Knowledge Proactively**
    - Offer to help teammates with testing challenges
    - Share useful testing techniques you've learned
    - Create or contribute to team testing documentation
3. **Contribute to Team Culture**
    - Speak up in retrospectives about testing improvements
    - Suggest testing-related team practices or rituals
    - Encourage testing discussions during code reviews
4. **Lead by Example**
    - Consistently demonstrate good testing practices
    - Show enthusiasm for writing and maintaining tests
    - Make testing visible and valued in your daily work

## **🏆 Success metrics**

- Teammates seek your input on testing questions
- You regularly contribute testing ideas to team discussions
- Others adopt testing practices you've shared or suggested
- Team testing culture improves partly through your contributions
- You're seen as someone who values and promotes good testing

## **❓ Assessing readiness for promotion**

### **Current level validation**

- Do they actively promote testing practices within the team?
- Do they share testing knowledge and help others?
- Do they contribute positively to testing culture discussions?

### **Next level readiness questions**

1. **Influence and Communication**
    - "Tell me about a time when you helped a teammate improve their testing practices."
    - "How do you explain the value of testing to someone who's skeptical?"
    - "What testing practices have you advocated for with your team?"
2. **Knowledge Sharing**
    - "What testing techniques or tools have you introduced to your teammates?"
    - "How do you stay updated on testing best practices to share with others?"
    - "Describe a time when you taught someone else about testing."
3. **Cultural Impact**
    - "How have you contributed to improving your team's testing culture?"
    - "What changes would you advocate for in your team's testing practices?"
    - "How do you handle resistance when advocating for better testing?"

### **Evidence to look for**

- Actively shares testing knowledge and experiences
- Contributes valuable ideas to improve team testing practices
- Helps create a positive, collaborative testing culture
- Demonstrates genuine enthusiasm for testing that influences others
- Shows growth in ability to articulate testing benefits

## **🚀 Next steps toward intermediate level**

To progress beyond junior level testing advocacy:

- **Cross-team influence**: Share testing practices beyond immediate team
- **Training and mentoring**: Formally teach testing to other developers
- **Process improvement**: Lead initiatives to improve testing workflows
- **Tool evaluation**: Research and advocate for new testing tools
- **Community engagement**: Participate in broader testing communities

## **💡 Practical ways to advocate for testing**

1. **Share success stories**
    - "My tests caught this bug before it went live"
    - "Refactoring was easy because I had good test coverage"
    - "Tests helped me understand this complex code"
2. **Make testing visible**
    - Celebrate test coverage improvements in team updates
    - Share interesting testing challenges and solutions
    - Highlight how tests serve as documentation
3. **Offer practical help**
    - "I can help you write tests for that feature"
    - "Let me show you this testing technique I learned"
    - "Want to pair on writing some tests together?"
4. **Suggest improvements**
    - "Could we add a 'testing time' estimate to our stories?"
    - "What if we shared testing tips in our team wiki?"
    - "Maybe we could do a testing lunch-and-learn session?"

## **⚠️ Common pitfalls to avoid**

- **Being preachy**: Advocate through example and enthusiasm, not lectures
- **Overwhelming others**: Start small and build gradually
- **Ignoring constraints**: Consider time and resource limitations when advocating
- **One-size-fits-all**: Recognize that different situations may need different approaches
- **Giving up easily**: Persistence is key, but know when to adjust your approach

## **🌟 Building testing advocacy skills**

1. **Understand the "why"**
    - Learn about business impact of bugs
    - Understand how testing improves developer productivity
    - Know the long-term benefits of maintainable test suites
2. **Develop communication skills**
    - Practice explaining testing concepts clearly
    - Learn to tailor your message to different audiences
    - Focus on benefits rather than just techniques
3. **Stay curious and learning**
    - Keep up with testing trends and best practices
    - Try new testing approaches and share your experiences
    - Learn from other teams' testing successes
4. **Be patient and persistent**
    - Culture change takes time
    - Celebrate small wins and incremental improvements
    - Stay positive even when facing resistance
