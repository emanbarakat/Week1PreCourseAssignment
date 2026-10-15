# LLM Text Summarizer

A small Node.js learning project that summarizes a paragraph into one concise sentence using the OpenAI API.

The project focuses on writing a safer and more structured LLM API call rather than just sending a prompt.

## What It Demonstrates

- OpenAI API integration
- environment-based API key handling
- input-length validation
- request timeout handling
- basic API error handling
- explicit prompt constraints
- prompt-injection-aware document framing

## Run Locally

Install dependencies:

```bash
npm install
```

Create a local `.env` file:

```text
OPENAI_API_KEY=your-key-here
```

Run:

```bash
npm start
```

## Example Task

The script asks the model to:

- summarize the supplied text
- return exactly one sentence
- stay within 25 words
- avoid adding new facts

## Project Structure

```text
llm-text-summarizer/
├── app.js
├── package.json
├── .env.example
├── .gitignore
└── README.md
```

## Notes

- The sample input is intentionally short.
- The input is limited to 2,000 characters.
- The API request is aborted after 20 seconds.
- This is a learning/portfolio example, not a production service.

## Author

**Eman Barakat**
