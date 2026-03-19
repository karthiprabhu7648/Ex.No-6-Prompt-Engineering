Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

Aim: 

Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools.

Explanation:

Develop a python code that integrates multiple AI tool by interacting with their APIs.
Compare outputs from different APIs.
Analyze the response and the Output.

The aim is to understand how to request help from AI tools for tasks like writing Python code, integrating with APIs, comparing outputs, and generating actionable insights.


Result:
CODE FOR POSITIVE REVIEW

```python
from nltk.sentiment import SentimentIntensityAnalyzer
import nltk
nltk.download('vader_lexicon')
generated_text = "This smartphone offers outstanding battery life and an intelligent AI camera that captures stunning photos."
print("Generated Review:\n")
print(generated_text)
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)
print("\nSentiment Analysis:")
print(sentiment)
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")
```
OUTPUT:

<img width="1005" height="168" alt="Screenshot 2026-03-19 at 12 08 32 AM" src="https://github.com/user-attachments/assets/63133e67-fda8-439e-af3e-b9b578f5d6b8" />

CODE FOR NEGATIVE REVIEW:
```python
from nltk.sentiment import SentimentIntensityAnalyzer
import nltk
nltk.download('vader_lexicon')
generated_text = "This smartphone offers worst battery life and an intelligent AI camera that captures pathetic photos."
print("Generated Review:\n")
print(generated_text)
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)
print("\nSentiment Analysis:")
print(sentiment)
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")

```

OUTPUT:

<img width="1005" height="168" alt="Screenshot 2026-03-19 at 12 11 15 AM" src="https://github.com/user-attachments/assets/2aeb8192-d687-4116-ba69-405de59e852e" />
