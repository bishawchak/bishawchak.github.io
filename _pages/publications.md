---
layout: page
title: Publications
permalink: /publications/
nav: true
nav_order: 3
---

<style>
/* 🔹 Publication Card */
.publication-card {
  background-color: var(--card-bg, #f9f9f9);
  color: var(--text-color, #000);
  border: 1px solid var(--border-color, #ccc);
  border-radius: 0;
  padding: 1.2rem;
  margin-bottom: 1.5rem;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  transition: background-color 0.3s, color 0.3s, border-color 0.3s;
}

/* 🔹 Dark Theme Support */
[data-theme="dark"] .publication-card {
  --card-bg: #1e1e1e;
  --text-color: #e5e5e5;
  --border-color: #333;
}

/* 🔹 Buttons (rectangular + adaptive theme) */
.pub-buttons {
  margin-top: 0.8rem;
}
.pub-buttons button,
.pub-buttons a {
  display: inline-block;
  margin-right: 0.5rem;
  padding: 0.4rem 0.9rem;
  border-radius: 0; /* 🔳 Rectangular */
  font-size: 0.85rem;
  text-decoration: none;
  font-weight: 500;
  border: 1px solid;
  cursor: pointer;
  background: transparent;
  transition: all 0.25s ease;
}

/* 🌞 Light Mode Buttons */
[data-theme="light"] .pub-buttons button,
[data-theme="light"] .pub-buttons a {
  color: #222;
  border-color: #222;
}
[data-theme="light"] .pub-buttons button:hover,
[data-theme="light"] .pub-buttons a:hover {
   color: var(--global-theme-color);
  border-bottom: 1px solid var(--global-theme-color);
}

/* 🌙 Dark Mode Buttons */
[data-theme="dark"] .pub-buttons button,
[data-theme="dark"] .pub-buttons a {
  color: #fff;
  border-color: #fff;
}
[data-theme="dark"] .pub-buttons button:hover,
[data-theme="dark"] .pub-buttons a:hover {
   color: var(--global-theme-color);
  border-bottom: 1px solid var(--global-theme-color);
}

/* 🔹 Text sections */
.pub-title {
  font-size: 1.1rem;
  font-weight: 600;
}
.pub-title a {
  color: inherit;
  text-decoration: none;
  transition: color 0.3s, border-bottom 0.3s;
}
.pub-title a:hover {
  color: var(--global-theme-color);
  text-decoration: none;
  border-bottom: 1px solid var(--global-theme-color);
}

<div class="experience">
.pub-authors {
  margin-top: 0.4rem;
  font-size: 0.9rem;
  opacity: 0.85;
}
.pub-venue {
  font-style: italic;
  margin-top: 0.3rem;
  font-size: 0.85rem;
  color: var(--text-color);
  opacity: 0.75;
}

/* 🔹 Abstract & Bib (hidden by default) */
.pub-abstract, .pub-bib {
  display: none;
  margin-top: 0.8rem;
  font-size: 0.9rem;
  line-height: 1.5;
  border-left: 3px solid var(--border-color);
  padding-left: 0.6rem;
  opacity: 0.9;
  animation: fadeIn 0.3s ease-in-out;
  text-align: justify;
}

/* 🔹 Fade-in Animation */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(-4px); }
  to { opacity: 1; transform: translateY(0); }
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function() {
  // Toggle Abstract & Bib (auto-close the other)
  document.querySelectorAll(".publication-card").forEach(card => {
    const absBtn = card.querySelector(".pub-btn-abs");
    const bibBtn = card.querySelector(".pub-btn-bib");
    const abs = card.querySelector(".pub-abstract");
    const bib = card.querySelector(".pub-bib");

    absBtn.addEventListener("click", () => {
      const isOpen = abs.style.display === "block";
      abs.style.display = isOpen ? "none" : "block";
      bib.style.display = "none"; // auto close bib
    });

    bibBtn.addEventListener("click", () => {
      const isOpen = bib.style.display === "block";
      bib.style.display = isOpen ? "none" : "block";
      abs.style.display = "none"; // auto close abstract
    });
  });
});
</script>

<!-- 🔹 Publication 1 -->
<div class="publication-card">
  <div class="pub-title">
  <a href="https://github.com/bishawchak/PriBan">
    PriBan: A Benchmark Dataset and Modeling Framework for Privacy Preservation in Bengali Texts</a>
  </div>
  <div class="pub-authors">
    Authors: Md Anowarul Faruk Shishir, Bishaw Kirti Chakma, Indrajit Gupta
  </div>
  <div class="pub-venue">
    <a href="https://iccit.org.bd/2025/home/">
    <em>Submitted to ICCIT 2025 (Accepted)</em>
    </a>
  </div>

  <div class="pub-buttons">
    <button class="pub-btn-abs">Abstract</button>
    <button class="pub-btn-bib">BIB</button>
    <a href="#" class="pub-btn-doi">DOI</a>
    <a href="https://github.com/bishawchak/PriBan/blob/main/PriBan.pdf" class="pub-btn-pdf">PDF</a>
  </div>

  <div class="pub-abstract">
    Due to the widespread interaction with Large Language Models (LLMs), concerns regarding the leakage of private information have grown significantly. Although there have been some significant works taken place in English to preserve the privacy of the sensitive text, low-resource language like Bangla remain largely unexplored. To address this issue, we employed two human-rewritten approaches: (i) deleting sensitive expressions and (ii) obscuring sensitive details by abstracting them, both of which have achieved notable success in English. At first, we developed a corpus, named PriBan, through translation, crowd-sourcing and the utilization of Large Language Model (LLMs). Being the first work on Bangla, we achieved a satisfactory level of privacy preservation. We also demonstrated strong results in maintaining a natural tone in the generated text. Through automated evaluation metrics, we found that our approach preserved privacy with an average accuracy of 91.43% for obscure rewrite method and 94.75% for delete rewrite method. We believe this work sets the foundation for privacy-preserving text generation in Bangla and can be further extended to other low-resource languages in future research.
  </div>

  <div class="pub-bib">
    @inproceedings{chakma2025priban,<br>
    &nbsp;&nbsp;title={PriBan: A Benchmark Dataset and Modeling Framework for Privacy Preservation in Bengali Texts},<br>
    &nbsp;&nbsp;author={Md Anowarul Faruk Shishir and Bishaw Kirti Chakma and Indrajit Gupta},<br>
    &nbsp;&nbsp;booktitle={International Conference on Computer and Information Technology (ICCIT)},<br>
    &nbsp;&nbsp;year={2025},<br>
    &nbsp;&nbsp;note={Under Review}<br>
    }
  </div>
</div>

<!-- 🔹 Publication 2
<div class="publication-card">
  <div class="pub-title">
  <a href="https://github.com/bishawchak/Undergrad_Thesis/tree/main">
    Detection of LLM (Large Language Model) Generated Text Using Long Short Term Memory</a>
  </div>
  <div class="pub-authors">
    Authors: Bishaw Kirti Chakma<br>
    Undergraduate Thesis
  </div>
  <div class="pub-venue">
    Supervisor: Dr. Md. Foisal Hossain
  </div>

  <div class="pub-buttons">
    <button class="pub-btn-abs">Abstract</button>
    <button class="pub-btn-bib">BIB</button>
    <a href="#" class="pub-btn-doi">DOI</a>
    <a href="https://github.com/bishawchak/Undergrad_Thesis/blob/main/Thesis_Final_Report_LSTM.pdf" class="pub-btn-pdf">PDF</a>
  </div>

  <div class="pub-abstract">
    The rapid growth of Large Language Models (LLMs) has created new hurdles in detecting artificially generated text. Concerns about the possible misuse of created content, including spam, harmful activities, and misinformation, have grown as LLMs, like GPT-3, continue to develop. The urgent need for reliable techniques to recognise LLM-generated text and separate it from content created by humans is discussed in this paper. We examine current methods and suggest better ones that make use of machine learning algorithms and linguistic, semantic, and contextual aspects. Our goal is to reduce the risks related with the spread of LLM-generated material by improving the effectiveness and accuracy of detection systems and promoting a safer online environment. We also go over possible responses and ethical issues to weigh the advantages of LLMs against the need to avoid misuse. The suggested remedies have wide-ranging effects in a number of fields, such as content control, cybersecurity, and the appropriate use of LLMs in a variety of applications.
  </div>

  <div class="pub-bib">
    @thesis{chakma2024llm,<br>
    &nbsp;&nbsp;title={Detection of LLM (Large Language Model) Generated Text Using Long Short Term Memory},<br>
    &nbsp;&nbsp;author={Bishaw Kirti Chakma},<br>
    &nbsp;&nbsp;school={Khulna University of Engineering & Technology},<br>
    &nbsp;&nbsp;year={2024},<br>
    &nbsp;&nbsp;supervisor={Dr. Md. Foisal Hossain}<br>
    }
  </div>
</div> -->
