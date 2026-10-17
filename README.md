# 🧠 Customer Feedback Summarizer

An AI-powered application built to automate customer feedback analysis using Python and the Gemini API. The project analyzes customer opinions, identifies sentiment, categorizes feedback, and generates concise summaries to help businesses understand customer needs more efficiently.

## 🎯 Problem Statement

Businesses receive hundreds of customer feedback messages every day. Manually reading each message, identifying customer sentiment, categorizing issues, and preparing summaries requires time and effort.

The Customer Feedback Summarizer aims to automate this process using Generative AI, making feedback easier to organize, understand, and analyze.

## ✨ Key Features

- 📂 **Feedback Input:** Process customer feedback from CSV files or Google Sheets.
- 😊 **Sentiment Analysis:** Identify feedback as Positive, Negative, or Neutral.
- 🏷️ **Feedback Categorization:** Classify feedback into categories such as Product, Delivery, Support, and other relevant issues.
- 🧠 **AI-Powered Summarization:** Generate concise summaries that capture the main point of customer feedback.
- 💬 **Prompt Engineering:** Use structured prompts to guide the AI model toward consistent, relevant responses.
- 📋 **Structured JSON Output:** Organize the AI-generated sentiment, category, and summary into separate fields.
- 🛡️ **Error Handling:** Handle failed API requests and invalid or unexpected responses.
- 📊 **Organized Results:** Store processed feedback and analysis in a structured format for easier review.

## 🛠️ Tech Stack

- **Programming Language:** Python
- **Generative AI:** Google Gemini API
- **Prompt Engineering:** Task-specific prompts for sentiment analysis, categorization, and summarization
- **Data Input:** CSV files / Google Sheets
- **Data Format:** JSON
- **Data Processing:** Python
- **Error Handling:** Exception handling and response validation

## 🔄 Project Workflow

1. **Input Feedback:** Read customer feedback from a CSV file or Google Sheets.
2. **Data Processing:** Use Python to read and prepare the feedback records.
3. **Prompt Construction:** Create instructions describing the sentiment, category, and summary required.
4. **AI Analysis:** Send the prompt and feedback to the Gemini API.
5. **Response Processing:** Receive the AI response and parse the structured JSON output.
6. **Validation:** Check that the expected fields are present and handle invalid responses.
7. **Output Storage:** Save the processed feedback, sentiment, category, and summary in a structured sheet.

## 💡 Example

**Input Feedback:**

"My product quality is excellent, but my order arrived three days late."

**Illustrative AI Output:**

```json
{
  "sentiment": "Mixed",
  "category": "Delivery",
  "summary": "The customer liked the product quality but reported a delivery delay."
}
```

The example illustrates the intended output structure. Actual classifications depend on the model response and the application's validation rules.

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/AbhishekPawar-1904/feedback-analyzer.git
cd feedback-analyzer
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate on Windows:

```powershell
.\venv\Scripts\Activate.ps1
```

### 3. Install Dependencies

Install the dependencies listed in `requirements.txt`:

```bash
pip install -r requirements.txt
```

### 4. Configure the Gemini API Key

Create a `.env` file in the project root:

```env
GEMINI_API_KEY=your-api-key-here
```

Keep your API key private and never upload the `.env` file to GitHub.

### 5. Run the Application

Run the Python entry point for your implementation. For example:

```bash
python main.py
```

Update this command to match the actual entry point in your project.

## 📈 Expected Benefits

- Reduces repetitive manual feedback analysis.
- Organizes customer opinions into meaningful categories.
- Helps identify recurring complaints and customer concerns.
- Produces concise summaries for quicker review.
- Demonstrates practical integration of Generative AI into a Python workflow.

## 🔮 Future Enhancements

- Add an interactive dashboard for feedback trends.
- Support batch processing of large feedback datasets.
- Add more robust validation and retry handling for API failures.
- Identify frequently reported issues across multiple feedback records.
- Measure classification quality using a manually labeled test dataset.

## 📄 License

Refer to the repository's `LICENSE` file for licensing terms.
