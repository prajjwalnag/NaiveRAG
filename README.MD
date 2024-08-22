# AI-Powered Query Answering System

This project is an AI-powered query answering system that retrieves relevant information from a PostgreSQL database, integrates it into the context of a user's query, and generates a response using OpenAI's GPT-3.5-turbo model. The project also includes a Gradio web interface for easy interaction.

![Interface Screenshot](/Capture.PNG)

## Features

- **Information Retrieval**: Retrieves relevant text chunks from a PostgreSQL database based on the user's query.
- **Contextual Response Generation**: Uses the retrieved information to create a context-rich prompt and generates a response using OpenAI's GPT-3.5-turbo model.
- **User-Friendly Interface**: A simple and intuitive Gradio web interface.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7 or higher installed on your machine.
- A PostgreSQL database set up with the `pgvector` extension enabled.
- OpenAI API key (you can sign up for access [here](https://beta.openai.com/signup/)).
- The following Python packages installed:
  - `openai`
  - `psycopg2`
  - `gradio`

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/ai-query-answering-system.git
    cd ai-query-answering-system
    ```

2. Install the required Python packages:

    ```bash
    pip install openai psycopg2 gradio
    ```

3. Set up your PostgreSQL database and ensure it contains a table named `vectordatabase` with the appropriate schema for storing text chunks and embeddings.

4. Set your OpenAI API key in the environment:

    ```bash
    export OPENAI_API_KEY="your_openai_api_key"
    ```

    Or include it directly in the script where indicated.

## Usage

1. **Run the Gradio Interface:**

    To launch the Gradio interface, run the following command:

    ```bash
    python your_script_name.py
    ```

2. **Interact with the System:**

    - Open the provided URL in your web browser.
    - Enter your query into the text box.
    - The system will retrieve relevant information, generate a contextual response, and display it in the interface.

## Customization

### Database Connection

Update the PostgreSQL connection details in the script according to your database configuration.

## Contributing

If you'd like to contribute to this project, please fork the repository and use a feature branch. Pull requests are warmly welcome.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Contact

If you have any questions or feedback, feel free to contact me at your.email@example.com.
