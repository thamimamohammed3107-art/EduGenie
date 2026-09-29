from flask import Flask, render_template, request
import google.generativeai as genai
import os
from dotenv import load_dotenv

load_dotenv()

app = Flask(__name__)

genai.configure(api_key=os.getenv("GEMINI_API_KEY"))

model = genai.GenerativeModel("gemini-1.5-flash")

@app.route("/", methods=["GET", "POST"])
def home():
    response_text = ""

    if request.method == "POST":
        user_prompt = request.form["prompt"]

        try:
            response = model.generate_content(
                f"""
                You are EduGenie, an AI learning assistant.
                Explain concepts clearly for students.

                User Query:
                {user_prompt}
                """
            )

            response_text = response.text

        except Exception as e:
            response_text = f"Error: {str(e)}"

    return render_template("index.html", response=response_text)

if __name__ == "__main__":
    app.run(debug=True)
