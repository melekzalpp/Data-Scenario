🛍️ Product Recommendation System with OpenAI Embeddings
This project implements a content-based product recommendation system using OpenAI embeddings and cosine similarity. It aims to suggest similar products based on their textual descriptions, enabling smarter product discovery for users.

📌 Key Steps and Workflow

1. Data Loading
A sample dataset containing product information (such as Product ID, Product Name, and Description) is loaded using pandas.

2. Text Preprocessing
Basic preprocessing is applied to the product descriptions (e.g., lowercasing, removing unnecessary characters) to prepare them for embedding.

3. Generating Embeddings with OpenAI API
The cleaned product descriptions are passed through the OpenAI Embeddings API (e.g., text-embedding-ada-002) to generate high-dimensional vector representations that capture semantic meaning.

4. Calculating Similarity Scores
Cosine similarity is computed between the embedding vectors to determine how closely related each product is to the others.

5. Creating a Recommendation Function
A function is implemented to take a product name or ID as input and return the top N most similar products based on the similarity scores.

6. Displaying Results
The recommendations are returned in a pandas DataFrame, showing the similar products and their corresponding similarity scores.

🧠 Technologies Used
- Python
- Pandas & NumPy
- OpenAI API (text embeddings)
- Scikit-learn (cosine_similarity)
- dotenv (for API key management)

🔐 Environment Setup
API keys are securely loaded from a .env file using the python-dotenv library. Make sure to create your own .env file with the following structure:
- APIKEY=your_openai_api_key

💡 Use Case
This approach can be extended to e-commerce platforms, digital content recommendation, or any system where product/content similarity based on text is valuable.
