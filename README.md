# ISB-Body-language-and-EMO-Scoring 🎥🧠

An open-source evaluation tool for ISB students to self-assess their public speaking videos based on transparent and explainable metrics—body language, facial expression, voice modulation, and content quality.

Built as a response to the **opaque and unmodifiable uSpeek system**, this tool lets students **test, understand, and improve** their performance before final submissions.
 
---

## 🔍 Why this exists

At ISB (Indian School of Business, https://www.isb.edu/en.html), students are asked to upload videos on the uSpeek platform for scoring. Unfortunately, the system is closed, opaque, and lacks real-time feedback—making it hard for students to iterate and improve. This tool provides a **transparent, replicable, and research-driven** alternative.

By making this open-source, we aim to:

- Allow students to experiment and understand the scoring breakdown.
- Provide meaningful feedback on *how to improve*.
- Empower users with a practical, AI-powered scoring framework using LLMs, CV, and audio analysis.

---

## 🚀 Quick Start

Click below to **run the tool directly on Google Colab**. You don't need to install anything locally.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alpha-AI-LTD/ISB-Body-language-and-EMO-Scoring/blob/main/Bodylanguage_EMO_Detection_Scoring_With_Flags_v2.ipynb)

---

## 🔧 What it Does

After uploading a video, the tool:

1. **Extracts and analyzes audio** using Groq Whisper API:
   - Transcribes the content
   - Calculates pitch & volume variation
   - Scores speech modulation

2. **Processes the video using MediaPipe**:
   - Identifies posture, hand gestures, and facial expressions
   - Detects smiling frequency and engagement level

3. **Assesses transcript quality using an LLM**:
   - Evaluates filler/pet words
   - Scores content clarity, relevance, and impact

4. **Generates an AI-based feedback report** simulating uSpeek's criteria:
   - Each section is scored out of 5
   - Final score includes actionable recommendations
   - Final score is also avaiable in ranges

Caution:
- The results may not be 100% accurate. We have tried to replicate how uSpeek works. Seemingly uSpeek lacks at a lot of places which this tool covers but our object is to mimic uSpeek results as close as possible.
- There can be an error margin for positive scores of +/- 0.2 (For now). In case you are consistenly facing issues with the scoring that is bad score are getting worse or something on these lines, simply connect with us on Linkedin (https://www.linkedin.com/company/alphaaico/) or send us a mail with the proofs, video and some ways in which we can maybe fix this further.
- Again, the tool is an approximation similar to uSpeek. Please do not expect similar results but it will be somewhat near. The good scores you get here will ensure you get better scores on uSpeek.
---

## 📦 Requirements

This Colab notebook automatically installs all dependencies, including:

- `mediapipe`
- `librosa`
- `opencv-python`
- `ffmpeg-python`
- `openai-whisper`
- `langchain-groq`

> **Important**: You will need a **free Groq API key** from [https://console.groq.com/keys](https://console.groq.com/keys) to run the notebook.

---

## 📝 Output

The tool will generate:

- A detailed report (`evaluation_report.txt`)
- Section-wise breakdown (body language, facial expression, speech quality, content)
- Actionable recommendations for improvement

---

## 📬 Support & Feedback

For queries or suggestions, reach out to [info@alphaai.biz](mailto:info@alphaai.biz).

---

## 🤝 Credits

Developed by the team at [Alpha AI](https://www.alphaai.biz). We believe that **transparency and empowerment** should be at the heart of every assessment tool.

---

## 🙌 Spread the Word

If this helps you or your peers, do share it within the ISB community. Let’s push for open, fair, and student-centric evaluation methods.

