
# 🤖 ResumeBot: AI-Powered Resume & Career Coach

ResumeBot is a fine-tuned Falcon-1B large language model (LLM) built using QLoRA and Hugging Face's `transformers`, `peft`, and `trl` libraries. It provides smart, structured, and context-aware responses to resume building and career-related queries — acting as your personal AI career coach.

---

## 🔍 Problem Statement

Job seekers and freshers often struggle with:
- Resume formatting and optimization
- Writing summaries and bullet points
- Knowing what skills or projects to include
- Preparing for technical roles in a competitive market

---

## 🧠 Solution

ResumeBot is trained on 400+ real-world instructions covering:
- Resume tips for freshers and juniors
- Bullet point rewrites
- Summary suggestions
- Skill recommendations by role
- ATS optimization best practices

---

## 🚀 Model & Training

- **Base Model**: `tiiuae/falcon-rw-1b`
- **Fine-Tuning Method**: QLoRA via Hugging Face `peft`
- **Frameworks**: Transformers, Datasets, TRL (SFTTrainer)
- **Training Time**: ~5 mins on Google Colab Free (T4 GPU)
- **Final Loss**: `0.41` (very low — great learning)

---

## 📊 Dataset Format (Alpaca-style)

```json
{
  "instruction": "Suggest 3 skills for a beginner data scientist.",
  "input": "",
  "output": "Include tools like Python, SQL, and Tableau. Example: 'Built a predictive model improving accuracy by 20%.'"
}
```

---

## 🧪 Sample Output

**Prompt:**
```
### Instruction:
Suggest 3 skills to include in a resume for a beginner data scientist.
### Response:
```

**Generated:**
```
Include tools like Python, SQL, and Tableau. Example: ‘Built a predictive model, improving accuracy by 20%.’ Add certifications.
```

---

## 🧰 How to Run

### 1. Clone this repo
```bash
git clone https://github.com/your-username/ResumeBot-AI.git
cd ResumeBot-AI
```

### 2. Setup environment
```bash
pip install -q transformers datasets peft trl bitsandbytes gradio accelerate
```

### 3. Run the Gradio app
```bash
python app.py
```

---

## 🌐 Deploy Online

You can deploy this as a Hugging Face Space or host the model via the Transformers Hub after merging LoRA weights.

---

## 🙌 Credits

Built by [Aryan](https://www.linkedin.com/in/your-link), an AI/ML Engineer passionate about LLMs, GenAI, and building real-world tools.

---

## 📜 License

MIT License
