# 🗳️ VoteWise – Election Process Education Assistant

An interactive web application that educates Indian citizens about the democratic election process through a smart chat assistant, quizzes, and curated information.

---

## 📌 Challenge Vertical

**Election Process Education** — Empowering citizens with clear, accessible knowledge about India's electoral system.

---

## 🎯 Approach & Logic

### Problem Statement
Many Indian citizens — especially first-time voters — lack clear information about how elections work, how to register, and what their rights are.

### Solution
**VoteWise** is a self-contained, intelligent assistant that:
1. **Answers questions** about Indian elections using a structured knowledge base
2. **Uses smart keyword matching** to find the best answer for any question
3. **Tests knowledge** through an 8-question interactive quiz
4. **Surfaces key facts** about Indian democracy
5. **Links to official resources** (eci.gov.in, voters.eci.gov.in, helpline 1950)

### Decision Logic
The assistant uses a **weighted keyword scoring system**:
- Each knowledge entry has multiple keyword triggers
- User queries are matched against all entries
- Multi-word phrase matches score higher than single words
- The highest-scoring entry is returned as the answer
- Unmatched queries receive helpful fallback suggestions

---

## 🛠️ How the Solution Works

### Architecture
```
index.html  ← Single self-contained file
├── Knowledge Base    (15 topic entries covering Indian elections)
├── Smart Search      (keyword scoring algorithm)
├── Chat Engine       (conversational UI with typing animation)
├── Quiz Engine       (8 questions with instant feedback)
├── Fact Rotator      (8 rotating election facts)
└── Indian Theme      (tricolor design, Playfair + DM Sans fonts)
```

### Topics Covered
| Topic | Details |
|---|---|
| How Voting Works | Step-by-step election process |
| Voter Eligibility | Age, citizenship, residency requirements |
| Voter Registration | Form 6, online portal, EPIC card |
| Election Commission | Role, powers, history |
| NOTA | What it is, how it works |
| EVMs & VVPATs | Technology, security, process |
| Model Code of Conduct | Rules, enforcement |
| Lok Sabha Elections | Constituencies, FPTP system |
| Presidential Election | Electoral college, process |
| Rajya Sabha Elections | Indirect election, terms |
| State Assembly Elections | Vidhan Sabha, MLAs |
| Check Voter List | Multiple ways to verify registration |
| Voting Documents | All 11 accepted ID documents |
| Fake News | How to spot and report |
| Voting Rights | Constitutional provisions |

---

## 📋 Assumptions Made

1. **India-focused**: Scoped to Indian electoral system
2. **Offline-first**: No API calls — works entirely in the browser
3. **English language**: Content in English; multilingual support is a future enhancement
4. **Static hosting**: Single HTML file, deployable anywhere

---

## 🚀 How to Run

```bash
git clone https://github.com/YOUR_USERNAME/election-education-assistant.git
cd election-education-assistant
# Open index.html in any browser — no server needed!
```

Or deploy to **GitHub Pages**:
1. Settings → Pages → Source: main branch → root
2. Access at `https://YOUR_USERNAME.github.io/election-education-assistant/`

---

## 🔍 Evaluation Criteria

| Criteria | How Addressed |
|---|---|
| **Code Quality** | Clean, commented, well-structured single file |
| **Security** | No external APIs, no data collection, purely client-side |
| **Efficiency** | No dependencies, instant response, O(n) search |
| **Testing** | Built-in 8-question quiz validates civic knowledge |
| **Accessibility** | Semantic HTML, keyboard navigation, ARIA-ready |
| **Google Services** | Google Fonts (Playfair Display + DM Sans) |

---

## 👨‍💻 Built With
- HTML5, CSS3, Vanilla JavaScript
- Google Fonts
- Built using **Google Antigravity**

---

*"The ballot is stronger than the bullet." – Abraham Lincoln*
