# 👋 Hi, I'm Mohamed Aymane Badia!
<p align="left">
  <img src="https://img.shields.io/badge/Status-Looking%20for%20a%20PFE%20internship-brightgreen?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Specialty-AI%20%26%20Data%20Science-blue?style=for-the-badge" />
</p>

🎓 **5th-year (final-year) AI & Data Science engineering student** — EMSI Marrakech

💼 **PFA internship at Lama Healthcare (USA)** — front-end lead + document extraction with LoRA fine-tuning

🤖 Passionate about **Machine Learning**, **Deep Learning**, **NLP** and **OCR**

💻 Full-Stack: **Next.js, React, TypeScript, Flask**

---

## 💼 Experience

### PFA Internship — Front-end & AI · Lama Healthcare (Practice One), USA · July – September 2026
*Rebuild of a SaaS credentialing platform for US healthcare providers, in a team of three (HIPAA scope).*
<p>
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/>
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black"/>
  <img src="https://img.shields.io/badge/PEFT-LoRA-blueviolet?style=flat-square"/>
</p>

- **Front-end lead:** design system and reusable components; dashboard, provider files, credentialing workflow, alerts, audit log and a public document-upload page.
- **Document extraction:** compared vision-language models, then fine-tuned **Qwen3-1.7B with LoRA** on a T4 GPU — **100% valid JSON (60/60)** and **87% correct fields (124/143)** on the public CORD dataset, 3.3 GB peak VRAM.
- **Data security:** contributed to role-based access control, data masking and access traceability — 6/6 roles validated by access tests.

---

## 🚀 Featured Projects

### 🧾 [Invoice Intelligence AI — OCR + fine-tuned LLM](https://github.com/BADIAMOHAMEDAYMANE/Invoice-Intelligence-ai)
*Photo or PDF of an invoice → OCR → fine-tuned small LLM → structured JSON → arithmetic repair → validation → Streamlit demo.*
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Hugging%20Face-Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black"/>
  <img src="https://img.shields.io/badge/Qwen2.5--0.5B-LoRA-blueviolet?style=flat-square"/>
  <img src="https://img.shields.io/badge/Tesseract-OCR-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/Field%20accuracy-0.99-brightgreen?style=flat-square"/>
</p>

- **OCR:** Tesseract (eng + fra) for images, PyMuPDF for PDFs.
- **LLM fine-tuning:** Qwen2.5-0.5B-Instruct fine-tuned with LoRA (r = 16, α = 32, 8.8M trainable parameters out of 503M).
- **Reliability:** arithmetic repair layer and Pydantic schema validation on the model output.
- **Results (synthetic test set, n = 40):** field accuracy **0.99** vs 0.54 for the base model and 0.53 for a regex baseline. Generalisation to real receipts is still limited and documented in the repo.
- **Tools:** Transformers, PEFT, PyTorch, pytesseract, PyMuPDF, Pydantic, pytest, Streamlit.

---

### 🧠 [CIFAR-10 CNN Classifier](https://github.com/BADIAMOHAMEDAYMANE/Animal-Classification)
*Convolutional Neural Network trained on GPU with PyTorch, deployed as a robust Streamlit app.*
<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/CUDA-GPU%20T4-76B900?style=flat-square&logo=nvidia&logoColor=white"/>
  <img src="https://img.shields.io/badge/Accuracy-~78%25-brightgreen?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dataset-CIFAR--10-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <a href="https://animal-classification-2gd59hwka4ppwvsjsnp7cp.streamlit.app/">
    <img src="https://img.shields.io/badge/Streamlit-Live%20Demo-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
  </a>
</p>

- **Deep Learning:** 3-block CNN (Conv2D → BatchNorm → ReLU → MaxPool), Dropout, ~500k parameters — **~78% test accuracy**.
- **Training:** Adam optimizer, StepLR scheduler, Tesla T4 GPU (Google Colab / Kaggle), `pin_memory`, `.to(device)`.
- **Robust demo:** a MobileNetV2 pre-filter rejects out-of-domain images; low-confidence or high-entropy predictions are reported as UNKNOWN.
- **Deployment:** Streamlit app ([🔗 Try it live](https://animal-classification-2gd59hwka4ppwvsjsnp7cp.streamlit.app/)) and Docker / docker compose.
- **Tools:** PyTorch, torchvision, Streamlit, Docker, Matplotlib, NumPy.

---

### 📰 [News Classification — BiLSTM vs TF-IDF baseline](https://github.com/BADIAMOHAMEDAYMANE/News-Classification-Project)
*Classifying news articles (headline + description) into 42 imbalanced categories, comparing a BiLSTM with a TF-IDF + linear SVM baseline.*
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white"/>
  <img src="https://img.shields.io/badge/NLTK-NLP-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dataset-209k%20articles-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Top--3%20accuracy-83.3%25-brightgreen?style=flat-square"/>
</p>

- **Data:** News Category Dataset — 209,527 articles, 42 imbalanced categories.
- **NLP preprocessing:** cleaning (URLs, mentions, digits, punctuation), NLTK stopwords, Keras tokenizer (15k vocabulary), padding.
- **Models:** Embedding (128) → Bidirectional LSTM (64) → Dense layers → Softmax, with softened class weights and EarlyStopping; baseline TF-IDF (1-2 grams) + LinearSVC.
- **Results (41,889 test articles):** TF-IDF + LinearSVC **63.5% top-1 / 83.3% top-3** (macro F1 0.50); BiLSTM 55.4% / 74.3% (macro F1 0.41).
- **Finding:** fully balanced class weights dropped POLITICS recall to 6% (36.7% accuracy); softening them restored it to 70%.
- **Tools:** TensorFlow/Keras, NLTK, Scikit-learn, Pandas, Matplotlib, Seaborn.

---

### 📡 [TrendRadar — Reddit Trend Detection](https://github.com/BADIAMOHAMEDAYMANE/TrendRadar-Project)
*Streamlit application that collects Reddit posts and detects emerging topics with NLP and Machine Learning.*
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/spaCy-09A3D5?style=flat-square&logo=spacy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white"/>
  <img src="https://img.shields.io/badge/KMeans-Clustering-blueviolet?style=flat-square"/>
</p>

- **Data:** Reddit posts collected through Reddit's public JSON endpoints (retries, streaming, Parquet cache).
- **NLP:** bilingual cleaning (FR/EN) with spaCy and NLTK, language detection, TF-IDF vectorization.
- **ML:** KMeans topic clustering, Random Forest trained on the clusters, sliding-window burst detection and virality prediction (gradient boosting).
- **Visualization:** interactive Plotly charts, hashtag treemap, word cloud.
- **Tools:** Streamlit, Pandas, Scikit-learn, spaCy, NLTK, Plotly, WordCloud.

---

### 🚦 [Smart Traffic Lights — Reinforcement Learning](https://github.com/BADIAMOHAMEDAYMANE/Road_Traffic_Management)
*Traffic-light control at an intersection with tabular Q-learning implemented from scratch.*
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/Q--learning-Reinforcement%20Learning-blueviolet?style=flat-square"/>
</p>

- **MDP:** state = (N-S queue, E-W queue, light phase) → 32 states; actions = keep / switch; reward = −(total queue).
- **Training:** ε-greedy exploration (ε 1.0 → 0.01), γ = 0.95, α = 0.1, Poisson car arrivals, 1,000 episodes.
- **Results (simulation):** average queue **−16.5%** vs a greedy policy and **−32.4%** vs fixed-time lights.
- **Tools:** Python, NumPy, Pandas, Streamlit.

---

### 🖼️ [Image Captioning — CNN vs Attention vs Transformer](https://github.com/BADIAMOHAMEDAYMANE/Image-Captioning)
*From-scratch image captioning system in PyTorch, comparing three decoder architectures on the same pipeline.*
<p>
  <img src="https://img.shields.io/badge/Status-Work%20in%20progress-yellow?style=flat-square"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/ResNet50-CNN%20Encoder-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/Attention-Bahdanau-blueviolet?style=flat-square"/>
  <img src="https://img.shields.io/badge/Transformer-Decoder-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dataset-Flickr8k-orange?style=flat-square"/>
</p>

- **Computer Vision:** frozen ResNet50 encoder (transfer learning), global + 7×7 region features.
- **Decoders implemented:** LSTM baseline, Bahdanau soft attention, Transformer decoder (self- and cross-attention).
- **NLP:** custom vocabulary pipeline, teacher forcing, greedy and beam search decoding.
- **Evaluation pipeline:** BLEU-1..4, model comparison table, attention heatmaps in a Streamlit demo.
- **Status:** pipeline verified end-to-end; full training on Flickr8k and BLEU results not published yet.

---

## 🛠️ Software Engineering Projects

| Project | Stack | Repository |
|---|---|---|
| 🚗 Car rental management | ASP.NET Core MVC (.NET 8), C#, EF Core (Code First), MySQL, N-Tier architecture, role-based access, PDF invoices (QuestPDF) | [Project-dotNet](https://github.com/BADIAMOHAMEDAYMANE/Project-dotNet) |
| 👔 Costume management REST API | Laravel 9, PHP, MySQL, JWT authentication, controller → service → repository layers | [backend-costume](https://github.com/BADIAMOHAMEDAYMANE/backend-costume) |
| ✈️ Real-time flight tracker & AI travel assistant | React (Vite), AviationStack API (search, filters, pagination), Flask REST API, Google Gemini API | [Flight-Management](https://github.com/BADIAMOHAMEDAYMANE/Flight-Management) |
| 📝 QCM generator | Java 21, JavaFX, MVC + DAO (JDBC, MySQL), Maven | [javafx-project](https://github.com/BADIAMOHAMEDAYMANE/javafx-project) |

---

## 🧠 Technical Skills
### 👨‍💻 Languages & Web
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![TypeScript](https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Java](https://img.shields.io/badge/java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![C#](https://img.shields.io/badge/c%23-239120?style=for-the-badge)
![PHP](https://img.shields.io/badge/php-777BB4?style=for-the-badge&logo=php&logoColor=white)
![Next.js](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Tailwind CSS](https://img.shields.io/badge/tailwind%20css-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Laravel](https://img.shields.io/badge/laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)

### 📊 Artificial Intelligence & Data
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![spaCy](https://img.shields.io/badge/spaCy-09A3D5?style=for-the-badge&logo=spacy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Plotly](https://img.shields.io/badge/plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)

### 🗄️ Databases
![PostgreSQL](https://img.shields.io/badge/postgresql-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### ⚙️ Professional Tools
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

---

## 📈 GitHub Activity
<p align="center">
  <img src="https://img.shields.io/badge/GitHub%20Profile-BADIAMOHAMEDAYMANE-181717?style=for-the-badge&logo=github&logoColor=white" />
  <br><br>
  <a href="https://github.com/BADIAMOHAMEDAYMANE?tab=repositories">
    <img src="https://img.shields.io/badge/View%20my%20repositories-%E2%86%92-blue?style=for-the-badge&logo=github" />
  </a>
</p>

---

## 🎯 My Goals
- 🏗️ Build **Deep Learning**, **NLP** and **OCR** models for real industry use cases.
- 🛠️ Deploy and monitor models in production (**MLOps**).
- 🔍 Land a final-year internship (**PFE**) in **Data Science** or **Artificial Intelligence**.

---

## 📫 Get in Touch
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohamed-aymane-badia-40a9712a1/)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://aymane-portfolio-lime.vercel.app)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:badiamohamedaymane@gmail.com)

---

<p align="center">
  <i>"Making sense of data, one commit at a time."</i>
</p>
