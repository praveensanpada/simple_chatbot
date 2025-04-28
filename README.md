# simple_chatbot


<h1>👋 Hi, I'm Praveen!</h1>

<h3>|| Data Scientist | Full Stack Developer | Machine Learning Engineer ||</h3>

<p>I’m a passionate and multi-skilled professional from India with expertise across a wide range of technologies, including:</p>

<ul>
  <li><strong>Programming & Scripting:</strong> Java, Python, PHP</li>
  <li><strong>Frontend & App Development:</strong> React, React Native, MEAN & MERN Stack</li>
  <li><strong>Backend Frameworks:</strong> Spring Boot, Node.js</li>
  <li><strong>Database Systems:</strong> MySQL, MongoDB</li>
  <li><strong>Cloud & Security:</strong> Google Cloud Platform (GCP), Cyber Security</li>
  <li><strong>Machine Learning & AI:</strong> Applied ML solutions, model training, and deployment</li>
</ul>

<hr>

<h2>🚀 About Me</h2>
<p>
I’m a <strong>Full Stack Web & App Developer</strong>, a <strong>Machine Learning Engineer</strong>, and a <strong>Cybersecurity Enthusiast</strong>, focused on building robust, scalable, and intelligent solutions.
</p>
<p>
My goal is to become a successful expert in the IT industry by channeling my technical knowledge and creative energy toward continuous growth — both personal and organizational.
</p>

<hr>

<h2>📌 Explore More</h2>
<ul>
  <li>🔗 <a href="https://praveensanpada.github.io/praveensanpada/" target="_blank">Portfolio Website</a></li>
  <li>🔗 <a href="https://linktr.ee/praveen.sanpada" target="_blank">Linktree</a></li>
  <li>🔗 <a href="https://github.com/praveensanpada" target="_blank">GitHub Profile</a></li>
  <li>🔗 <a href="https://praveensanpada.github.io/praveen.sanpada/" target="_blank">Web Profile</a></li>
</ul>

<hr>

<h2>💡 Let's Collaborate!</h2>
<p>
I'm always open to working on exciting projects in <strong>web development</strong>, <strong>data science</strong>, <strong>app development</strong>, or <strong>cloud-based systems</strong>.
</p>
<p>
If you’re interested in collaboration or want to connect, feel free to reach out!
</p>






                     ┌────────────────────────────┐
                     │       User (Web UI)        │
                     └────────────┬───────────────┘
                                  ↓
                        [Flask Chat Form Input]
                                  ↓
                   ┌──────── Grammar Correction ────────┐
                   │ Model: prithivida grammar corrector│
                   └────────────────────────────────────┘
                                  ↓
                  ┌────── Intent Detection Layer ───────┐
                  │ Model: all-MiniLM-L6-v2 (semantic)  │
                  └─────────────────────────────────────┘
                                  ↓
         ┌────────────────── Retrieval Flow ─────────────┐
         │ IF intent is known → fetch MongoDB using ID   │
         │ ELSE → Search FAISS corpus for semantic match │
         │ ELSE → Generate via Local LLM (DialoGPT, T5)  │
         └───────────────────────────────────────────────┘
                                  ↓
                           Response Formatting
                                  ↓
                         Display on Flask Template



llm_flask_chatbot/
├── app.py                          # Flask entrypoint
├── templates/
│   └── chat.html                   # Frontend
├── utils/
│   ├── grammar_corrector.py       # Grammar correction
│   ├── intent_classifier.py       # Semantic intent detection
│   ├── mongo_query.py             # Query MongoDB by ID
│   ├── vector_search.py           # FAISS retrieval
│   ├── response_engine.py         # Final answer logic
│   └── llm_fallback.py            # GPT2/DialoGPT generation
├── config/
│   ├── intents.json               # Mapped intent types
│   └── mongo_keys.json            # Map Mongo field names
├── faiss_index/
│   ├── index.faiss                # FAISS vector index
│   └── corpus.json                # Documents used to create index
├── requirements.txt
├── README.md


