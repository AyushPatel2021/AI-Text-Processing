# AI Text Summarizer App

An intelligent web application that leverages the power of Artificial Intelligence to automatically summarize long texts into concise, digestible content. Built with Node.js and the Hugging Face Inference API.

## 🚀 Features

-   **AI-Powered Summarization**: Uses the state-of-the-art `facebook/bart-large-cnn` model to generate accurate summaries.
-   **Simple Interface**: Clean and user-friendly design for easy text input and result viewing.
-   **Real-time Feedback**: Visual loading indicators while the AI is processing your text.
-   **Input Validation**: Ensures text is within the optimal length (200 - 100,000 characters) for best results.
-   **Secure**: API keys are handled securely on the backend, keeping your credentials safe.

## 🛠️ Tech Stack

-   **Frontend**: HTML5, CSS3, Vanilla JavaScript
-   **Backend**: Node.js, Express.js
-   **API**: Hugging Face Inference API
-   **HTTP Client**: Axios

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
-   [Node.js](https://nodejs.org/) (v14 or higher)
-   [npm](https://www.npmjs.com/) (usually comes with Node.js)

You will also need a **Hugging Face Access Token**:
1.  Sign up or log in at [Hugging Face](https://huggingface.co/).
2.  Go to **Settings** > **Access Tokens**.
3.  Create a new token with `read` permissions.

## ⚙️ Installation & Setup

1.  **Clone the repository** (if you haven't already):
    ```bash
    git clone <repository-url>
    cd AI-Text-Processing
    ```

2.  **Install Dependencies**:
    ```bash
    npm install
    ```

3.  **Configure Environment Variables**:
    Create a file named `.env` in the root directory of the project. Add your Hugging Face Access Token to it:
    ```env
    ACCESS_TOKEN=hf_your_access_token_here
    ```
    > **Note**: The `.env` file is ignored by git to protect your secrets.

## ▶️ Usage

1.  **Start the Server**:
    ```bash
    npm start
    ```
    You should see the message: `Server running at http://localhost:3000/`

2.  **Open the App**:
    Open your web browser and navigate to [http://localhost:3000](http://localhost:3000).

3.  **Summarize Text**:
    -   Paste the text you want to summarize into the input box.
    -   Ensure the text is between 200 and 100,000 characters.
    -   Click the **Summarize** button.
    -   Wait a moment for the AI to process, and your summary will appear in the box below!

## 📂 Project Structure

```
AI-Text-Processing/
├── public/              # Static frontend files
│   ├── index.html       # Main HTML page
│   ├── script.js        # Frontend logic
│   └── stylesheet.css   # Styling
├── .env                 # Environment variables (not committed)
├── .gitignore           # Git ignore rules
├── index.js             # Express server entry point
├── summarize.js         # Hugging Face API integration logic
├── package.json         # Project dependencies and scripts
└── README.md            # Project documentation
```

## 🤝 Contributing

Feel free to fork this project and submit pull requests. You can also open issues for bugs or feature suggestions.