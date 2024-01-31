# Code Llama 70B Instruct Streamlit App Demo

This [Streamlit](https://streamlit.io/) application serves as an interface to the Code Llama 70B Instruct model, providing a user-friendly platform for interacting with the model in a chat-like format. The app is designed to assist users by answering questions related to Python or executing tasks requested of the model.

## Features

- Interactive chat interface for querying the Code Llama 70B Instruct model.
- Customizable parameters for model responses.
- Session history to keep track of the conversation.
- Responsive layout suitable for various screen sizes.

## Installation

To run this application on your local machine, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone [your-repository-link]
   cd [repository-name]
   ```

2. **Install the required packages:**

   Ensure that you have Python installed on your system. Then, install the required packages using the following command:

   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the API token:**

   The app requires a valid [Replicate](https://replicate.com/) API token to interact with the Code Llama 70B Instruct model. Add your API token to the .streamlit/secrets.toml file as follows:

   ```toml
   # .streamlit/secrets.toml
   REPLICATE_API_TOKEN = "your_replicate_token"
   ```

4. **Run the app:**

   Start the Streamlit server by executing:

   ```bash
   streamlit run streamlit_app.py
   ```

   The app should now be running on your local server (usually <http://localhost:8501>).

## Usage

After launching the app, you can interact with it as follows:

- Enter your Python-related queries or tasks into the chat input box.
- Customize the model behavior using the Customize expander, where you can adjust the max tokens to return and the system prompt.
- View the model's responses in a chat-like format, with the history of the conversation maintained within the session.
