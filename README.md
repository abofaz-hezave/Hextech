# Hextech AI Shopping Assistant

## FE
"Facilitate a chatbot with the capability of rendering React components"

## BE
"Integrating the online shopping database with chatgpt"

## 1. Core Problem Statement
**Shoppers in online retail lack personalized assistance, leading to decision fatigue and abandoned carts.**
- In physical stores, assistants help refine choices based on preferences and context.
- Online stores often fail to replicate this experience.

---

## 2. Solution: AI-Powered Virtual Store Assistant
An AI chatbot that interacts with users to **understand their needs**, **ask relevant follow-up questions**, and **suggest products** tailored to their occasion, preferences, and constraints.

---

## 3. Features Breakdown

### Core Features
1. **Conversational Interface:**
   - Chatbot that mimics natural conversations.
   - Supports follow-ups for clarifications.

2. **Product Recommendation Engine:**
   - Matches user preferences to products using tags (occasion, color, size, budget, etc.).
   - Ranks products based on relevance.

3. **Personalization Features:**
   - Tracks preferences during the session (size, colors, budget).
   - Suggests complementary items (e.g., shoes for a wedding outfit).

4. **Image Suggestions:**
   - Displays product images alongside text suggestions.
   - Enables visual browsing.

5. **Flexible Queries:**
   - Understands broad requests like:  
     *"I need something formal for a winter wedding."*
   - Handles specific prompts like:  
     *"Show me white dresses under $100."*

---

## 4. User Flow

1. **User Input Stage:**
   - User describes their need (e.g., “I’m attending a summer wedding.”).
   - AI asks clarifying questions about size, style, and preferences.

2. **AI Processing Stage:**
   - Understands the query and matches filters in DynamoDB.
   - Refines results based on follow-ups (e.g., “Do you prefer dresses or suits?”).

3. **Output Stage:**
   - Displays top suggestions with images, prices, and quick filters.
   - Allows the user to browse or ask for alternatives.

4. **Final Actions:**
   - Adds selections to a virtual shopping cart.
   - Provides a summary with links for checkout.

---

## 5. MVP Scope for Hackathon

### Must-Have Features for Day 1 Demo:
- **Conversational AI:** Chatbot flow powered by **Amazon Bedrock**.
- **Product Matching:** DynamoDB filters based on AI-extracted attributes.
- **Dynamic Queries:** User can refine searches during the session.
- **Product Display:** Frontend shows names, prices, and images.
- **Fallbacks:** Handles unknown inputs gracefully (e.g., “Sorry, I didn’t get that—could you clarify?”).

### Nice-to-Have Features (Stretch Goals):
- **Voice Input:** Use **Amazon Lex** for voice interactions.
- **Session Memory:** Store preferences during the session for better recommendations.
- **Multi-Language Support:** Translate queries for international users.
- **Personalization Memory:** Save preferences tied to user accounts for future sessions.

---

## 6. Competitive Edge
- **Context-Aware AI:** Unlike traditional filters, it understands vague prompts and asks clarifying questions.
- **Multi-Category Search:** Finds outfits and accessories in one query instead of browsing categories.
- **Speed:** Real-time suggestions in a fast, lightweight design.

---

## 7. Target Audience
1. **Busy Shoppers** who need quick and reliable suggestions.
2. **Fashion Enthusiasts** looking for inspiration and style tips.
3. **Occasion-Based Shoppers** preparing for events like weddings, interviews, or vacations.