from langchain.agents import initialize_agent, Tool
from langchain.llms import OpenAI

# Summarizer
def summarize_text(text):
    return llm(f"Summarize this text:\n{text}")

# Quiz generator
def generate_quiz(summary):
    return llm(f"Create 10 MCQs from this summary:\n{summary}")

# Progress analyzer
def analyze_results(history):
    return llm(f"Analyze this quiz result data:\n{history}")
