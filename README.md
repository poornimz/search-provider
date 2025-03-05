
This project benchmarks multiple AI-powered search providers—Tavily, Perplexity API, Google Search (Gemini Grounding), and Exa—using LangSmith for evaluation with an LLM as a judge. The goal is determining which search provider generates the most accurate, well-grounded, and reliable responses.

How It Works

1. Search Query Execution

The same query is sent to multiple search providers:

Tavily: AI-powered search API.

Perplexity API: Uses Llama 3.1 Sonar for search and citation-based answers.

Google Search (Gemini Grounding): Google’s AI-integrated search.

Exa: AI-driven retrieval-augmented search.

2. Response Collection

Each provider returns a response containing:

Generated output (answer to the query)

Sources used (if available)

Grounding information (to check if the response is factual)

3. LLM as a Judge

An LLM evaluates all responses against a predefined ground truth answer.

The evaluation considers:

Accuracy: How close the response is to the correct answer.

Completeness: Whether all necessary details are covered.

Citations: If sources are provided and credible.

4. Evaluation with LangSmith

LangSmith logs and tracks all queries, responses, and evaluations.

Performance metrics are generated to identify the best-performing search provider.
