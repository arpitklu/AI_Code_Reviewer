# AI Code Reviewer

![AI Code Reviewer Banner]([https://raw.githubusercontent.com/yourusername/yourrepo/main/assets/banner.png](https://www.google.com/url?sa=i&url=https%3A%2F%2Ftypoapp.io%2Fblog%2Fai-in-the-code-review-process&psig=AOvVaw10mVqhyXj-4J6n5uRFQZ_I&ust=1753726348287000&source=images&cd=vfe&opi=89978449&ved=0CBUQjRxqFwoTCPDW-vPR3Y4DFQAAAAAdAAAAABAV))

## Overview

**AI Code Reviewer** is a backend service that leverages Google's Gemini AI to review code snippets provided by users. It analyzes your code, suggests corrections, and recommends optimized solutions for better performance and readability.

![AI Reviewing Code Example](https://raw.githubusercontent.com/yourusername/yourrepo/main/assets/review_example.png)

## Features

- **Automated Code Review:** Get instant feedback and suggestions for your code.
- **Code Correction:** Receive corrected versions of your code.
- **Optimization Suggestions:** Improve your code with AI-powered recommendations.
- **REST API:** Simple endpoints to interact with the AI reviewer.

## Getting Started

### Prerequisites

- Node.js (v16+)
- npm
- Google Gemini API Key

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/ai-code-reviewer.git
    cd ai-code-reviewer/BackEnd
    ```

2. Install dependencies:
    ```sh
    npm install
    ```

3. Create a `.env` file in the `BackEnd` directory and add your Gemini API key:
    ```
    GOOGLE_GEMINI_KEY=your_api_key_here
    ```

### Running the Server

```sh
node server.js
```

The server will start at [http://localhost:3000](http://localhost:3000).

## API Usage

### Review Code

Send a GET request to `/ai/get-response` with your code as the `prompt` query parameter.

**Example:**

```sh
curl "http://localhost:3000/ai/get-response?prompt=your_code_here"
```

**Response:**
- AI-reviewed code
- Corrections and optimizations

## Project Structure

```
BackEnd/
  ├── src/
  │   ├── app.js
  │   ├── controllers/
  │   │   └── ai.controller.js
  │   ├── routes/
  │   │   └── ai.routes.js
  │   └── services/
  │       └── ai.service.js
  ├── server.js
  ├── package.json
  └── .env
```

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change. 

## License

This project is licensed under the ISC License.

---

*Powered by [Google Gemini AI](https://ai.google.com/).*
