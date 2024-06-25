# SmartRealtor.ai
SmartRealtor.ai is a powerful AI-driven platform designed to streamline the rental property management process. It leverages cutting-edge technologies such as OpenAI's GPT-3.5-turbo language model, Streamlit for building interactive web applications, and MongoDB for data storage.

Technologies Used
Python: The primary programming language used for the backend logic and data processing.
Streamlit: A Python library used for building interactive web applications with minimal effort.
OpenAI GPT-3.5-turbo: A state-of-the-art language model from OpenAI, used for natural language processing tasks such as document analysis and tenant evaluation.
MongoDB: A NoSQL database used for storing user data, property listings, and tenant information.
Stripe: A payment processing platform used for handling subscription-based access to the application.
PyTesseract: An optical character recognition (OCR) library used for extracting text from images and PDF files.
Boto3: The AWS SDK for Python, used for interacting with Amazon S3 for file storage and retrieval.
JWT (JSON Web Tokens): A standard for securely transmitting information between parties as a JSON object, used for user authentication and session management.
Bcrypt: A library for hashing and salting passwords for secure storage.
Features
Management Portal
The Management Portal allows property managers to create and manage rental property listings. Key features include:

Listing Creation: Create new property listings by providing the address.
Tenant Document Analysis: Upload and analyze various documents (e.g., credit reports, income statements, employment verification) submitted by prospective tenants.
AI-Powered Tenant Evaluation: Leverage the power of GPT-3.5-turbo to generate comprehensive reports evaluating the suitability of tenants based on their submitted documents.
Tenant Chatbot: Engage in interactive conversations with a chatbot powered by GPT-3.5-turbo to gather additional information or clarify details about the tenant's application.
User Authentication
The application includes a robust user authentication system with the following features:

User Registration: New users can register for the application, with optional email verification.
Login and Logout: Secure login and logout functionality with session management.
Password Reset: Users can reset their passwords securely.
Forgot Password and Username: Retrieve forgotten passwords or usernames.
Update User Details: Users can update their personal details, such as name and email.
Subscription Management
SmartRealtor.ai offers a subscription-based model, allowing users to access the platform's features by subscribing. The subscription management system includes:

Subscription Verification: Check if a user has an active subscription before granting access to the application.
Integration with Stripe: Seamless integration with the Stripe payment processing platform for handling subscriptions.
Getting Started
To run the SmartRealtor.ai application locally, follow these steps:

Clone the repository: git clone https://github.com/your-repo/SmartRealtor.ai.git
Install the required dependencies: pip install -r requirements.txt
Set up the necessary environment variables (e.g., API keys, database credentials, etc.).
Run the Streamlit application: streamlit run Management_Portal_& _Home.py
Note: For production deployment, additional steps may be required, such as setting up a web server, configuring SSL/TLS, and implementing appropriate security measures.

Contributing
Contributions to SmartRealtor.ai are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
