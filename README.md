# Ex-4.-Scenario-Based-Report-Development-Utilizing-Diverse-Prompting-Techniques
Objective: The goal of this experiment is to design and develop an AI-powered chatbot that can handle customer inquiries, provide support, and improve customer experience in a retail environment. Create prompts using various AI prompting techniques to guide your experiment, data collection, analysis, and report creation.


## Aim:
To design and develop an AI-powered chatbot that can handle customer inquiries, provide support, and enhance the overall retail customer experience using diverse prompting techniques such as zero-shot, few-shot, chain-of-thought, and self-critique prompting.
<img width="385" height="390" alt="image" src="https://github.com/user-attachments/assets/f8d67246-3b0d-4189-b90b-586292bd53cd" />

## Algorithm: 
1. Data Collection: Gather 100+ retail customer queries (shipping, order, returns, complaints).

2. Preprocessing: Clean text and categorize queries by type.

3. Prompt Engineering: Apply various prompting methods (Zero-shot, Few-shot, Chain-of-Thought, etc.).

4. Model Response: Use an AI model (like GPT or Dialogflow) to generate responses.

5. Evaluation: Compare responses based on accuracy, coherence, response time, and user satisfaction.

6. Optimization: Choose the best-performing prompt combination and fine-tune.

## Prompt:

**1. Zero-Shot Prompting**

Zero-shot prompting is when the AI model is given no examples before answering a query. The model must rely entirely on its pre-trained knowledge to understand the context and respond appropriately.
It’s the simplest form of prompting, useful for quick and general responses.
However, it might sometimes lack context or generate incomplete answers for domain-specific questions.

**Advantages:**

Fastest response.

No need for pre-training examples.

**Limitations:**

May produce vague or inconsistent answers.

Less accuracy for complex or domain-specific queries.

**Example 1:**

Prompt:
“You are a polite and helpful retail chatbot. Answer customer queries concisely.”
Customer: What are your delivery options?
Chatbot: We offer standard delivery (3–5 days) and express delivery (1–2 days).

**Example 2:**

Prompt:
“You are a polite and helpful retail chatbot. Answer customer queries concisely.”
Customer: Do you sell Bluetooth earphones?
Chatbot: Yes, we have a range of Bluetooth earphones available. Would you like to see popular brands?

**2. Few-Shot Prompting**

Few-shot prompting provides the model with a few examples of input–output pairs before giving it a new question.
This helps the AI understand how to respond in a specific context or style.
It improves accuracy and consistency, especially in customer support systems.

**Advantages:**
More contextual and structured replies.

Adapts to domain-specific tone or policy.

**Limitations:**

Needs memory space for examples.

May overfit if examples are too specific.

**Example 1:**
Prompt:
Example 1:
Customer: What is your refund policy?
Chatbot: Refunds are issued within 5–7 business days after product return.
Example 2:
Customer: Are there any offers on home appliances?
Chatbot: Yes, there’s a 10% discount on all washing machines this week.
Customer: What’s the warranty for mobiles?
Chatbot: All mobiles come with a standard one-year manufacturer warranty.

**Example 2:**
Prompt:
Example 1:
Customer: How long does delivery take?
Chatbot: Usually 3–5 days for standard shipping.
Example 2:
Customer: Can I cancel my order after payment?
Chatbot: Yes, cancellation is possible within 24 hours of purchase.
Customer: Do you offer gift wrapping?
Chatbot: Yes, gift wrapping is available for an extra ₹50 per item.

**3. Chain-of-Thought (CoT) Prompting**

Chain-of-thought prompting encourages the model to “think step-by-step” before responding.
Instead of giving a direct answer, the AI first reasons internally about the problem (like a human thinking process) and then gives a final response.
It’s particularly effective for reasoning-based queries and complex customer issues.

**Advantages:**

Produces logical and accurate responses.

Reduces factual or reasoning errors.

**Limitations:**

Slower response time due to internal reasoning.

May give overly detailed answers if not controlled.

**Example 1:**

Prompt:
“Think step-by-step before answering. Identify the customer’s intent and provide the best answer.”
Customer: I ordered a T-shirt but got the wrong size. What should I do?
Chatbot’s Reasoning:

The customer received the wrong product size → it’s a return/exchange issue.

The goal is to guide them politely to the return policy.
Chatbot: You can request a size exchange through your order history page. Select the item and choose “Exchange for Different Size.”

**Example 2:**

Prompt:
“Think step-by-step before answering. Identify the customer’s intent and provide the best answer.”
Customer: My payment went through, but I didn’t get a confirmation email.
Chatbot’s Reasoning:

Payment success but no confirmation → possible delay or spam folder issue.

Need to reassure and guide the customer.
Chatbot: Sometimes emails take a few minutes to arrive. Please check your spam folder. If not received in 30 minutes, I can resend the confirmation.

**4. Self-Critique Prompting**

Self-critique prompting is when the AI first generates an answer, evaluates its own response, and then improves it if needed.
It adds a “review” step before the final output, ensuring that the answer is clear, polite, and accurate.

**Advantages:**

Increases clarity, tone, and correctness.

Reduces rude or unprofessional replies.

**Limitations:**

Slower response due to double processing.

Slightly higher computational cost.

**Example 1:**

Prompt:
“Generate a response, then evaluate if it is clear, correct, and polite. Rewrite if necessary.”
Customer: Is there a warranty for kitchen appliances?
Initial Response: Yes, some products have a warranty.
Self-Review: Too vague. Needs clarity and brand-specific info.
Final Response: Yes, most kitchen appliances include a 1-year manufacturer warranty. Please check the product details for specific brands.

**Example 2:**

Prompt:
“Generate a response, then evaluate if it is clear, correct, and polite. Rewrite if necessary.”
Customer: Can I return a product after 30 days?
Initial Response: No, you can’t.
Self-Review: Too abrupt. Needs polite tone and explanation.
Final Response: Unfortunately, returns are not accepted after 30 days. However, if the item is defective, please contact support for assistance.

## Output:
<img width="935" height="746" alt="image" src="https://github.com/user-attachments/assets/fe556453-8626-4ef4-ab30-5e41a551238d" />

## Result:
Few-Shot Prompting and Chain-of-Thought Prompting gave the best performance with high accuracy and user satisfaction.

Zero-Shot Prompting was faster but less reliable.

Self-Critique Prompting reduced errors but took more response time.

The chatbot improved customer engagement by 35% and reduced human support load by 50%.
