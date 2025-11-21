# Personalized Real Estate Agent (HomeMatch)
### AIML STREAM — Udacity Nanodegree (Accenture Track)
#### Name: Sneha Chakrabartty
### Date: 21/11/25

This project demonstrates how Generative AI, Large Language Models (LLMs), vector databases, and Retrieval-Augmented Generation (RAG) can be combined to build a Personalized Real Estate Recommendation Assistant called HomeMatch.

The system simulates how modern real estate companies can leverage AI to provide tailored property recommendations based on user preferences. It is specifically aligned with the requirements of the Udacity AIML Final Project.

## What HomeMatch Does
HomeMatch transforms generic real estate listings into highly personalized narratives that resonate with a buyer’s unique lifestyle, preferences, and priorities.

This is achieved through these key components:

    **1. Synthetic Data Generation:**
    To begin, the system creates synthetic real estate listings using an LLM (OpenAI GPT-3.5-Turbo). A structured template is used to generate listings containing:
    - Neighborhood
    - Price
    - Number of bedrooms/bathrooms
    - House size
    - Property description
    - Neighborhood description
    These listings mimic realistic property data and act as the foundation for the semantic search pipeline.
    
    **2. Semantic Search Using Vector Database:**
    - Once synthetic listings are generated, they are:
    - Converted into embeddings using OpenAI Embeddings
    - Stored in a vector database (ChromaDB)
    This enables semantic similarity search, allowing the system to find the most relevant properties based on a buyer’s natural-language preferences.
    
    **3. Augmented Response Generation (RAG):**
    HomeMatch uses Retrieval-Augmented Generation to:
      - Retrieve the top-matching property listings
      - Feed them into the LLM along with the user’s preferences
      - Generate enhanced, context-aware responses
    RAG ensures that outputs are factual (grounded in retrieved listings) while still personalized.
    
    **4. Personalized Listing Description Generation:**
    After retrieving the best-matching listings:
      - The LLM rewrites each listing
      - It emphasizes features aligned with the buyer’s goals (e.g., quiet neighborhoods, spacious kitchens, backyard, transportation)
      - No factual information is altered — only the storytelling changes
      - A buyer persona is generated based on the preferences
    This creates output that feels uniquely tailored, improving user engagement.
     
     **5. Conversation Memory for Better Personalization:**
    This project uses Conversation Buffer Memory, enabling the model to:
      - Remember previous questions and answers
      - Maintain consistent buyer preferences across listings
      - Generate coherent, personalized descriptions
    Memory allows the system to understand context instead of treating each listing independently.
    Project Purpose
    You are a developer at Future Homes Realty, tasked with building an innovative application — HomeMatch — that transforms property listings into personalized narratives.
    The goal is to help buyers:
      - Feel understood
      - Find properties aligned with their lifestyle
      - Engage more deeply with real estate content
### **Core Components of HomeMatch**
   **Understanding Buyer Preferences:**
   Buyers will input their requirements and preferences, such as location, property type, budget, amenities, and lifestyle choices. The application uses LLMs to interpret these inputs in natural language, understanding nuanced requests beyond basic filters. 
   **Integrating with a Vector Database:**
   Connect "HomeMatch" with a vector database, where all available property listings are stored.
   Utilize vector embeddings to match properties with buyer preferences, focusing on aspects like neighborhood vibes, architectural styles, and proximity to specific amenities.
   **Personalized Listing Description Generation:**
   For each matched listing, use an LLM to rewrite the description in a way that highlights aspects most relevant to the buyer’s preferences.
Ensure personalization emphasizes characteristics appealing to the buyer without altering factual information about the property.
    **Listing Presentation:**
Output the personalized listing(s) as a text description of the listing.

## **Final Output**
The final system returns: 
Clean, formatted, personalized property descriptions
Buyer persona
Explanations of how preferences influenced the narrative
This gives users a convincing, human-like property recommendation experience.

## **Conclusion**
HomeMatch illustrates how AI can revolutionize real estate by combining:
LLM-powered generation
Semantic search
Vector databases
Contextual memory
Personalized narrative construction
It bridges advanced AI with practical industry applications—aligning perfectly with the Udacity AI/ML Nanodegree Final Project requirements.
