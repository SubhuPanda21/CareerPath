<div align="center">

<!-- Logo / Banner -->
<br/>

```
 ██████╗ █████╗ ██████╗ ███████╗███████╗██████╗ ██████╗  █████╗ ████████╗██╗  ██╗
██╔════╝██╔══██╗██╔══██╗██╔════╝██╔════╝██╔══██╗██╔══██╗██╔══██╗╚══██╔══╝██║  ██║ 
██║     ███████║██████╔╝█████╗  █████╗  ██████╔╝██████╔╝███████║   ██║   ███████║
██║     ██╔══██║██╔══██╗██╔══╝  ██╔══╝  ██╔══██╗██╔═══╝ ██╔══██║   ██║   ██╔══██║
╚██████╗██║  ██║██║  ██║███████╗███████╗██║  ██║██║     ██║  ██║   ██║   ██║  ██║
 ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝╚══════╝╚═╝  ╚═╝╚═╝     ╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝
```

### 🧭 Discover the career that was built for *you*  

<br/>

[![React](https://img.shields.io/badge/React-18.3-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.5-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Vite](https://img.shields.io/badge/Vite-5.4-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

<br/>

> **CareerPath** is a science-backed, interactive career assessment tool that helps you cut through the noise and find the career that genuinely fits your personality, skills, and ambitions — in under 5 minutes.

<br/>

---

</div>

## ✨ What is CareerPath?

Most people stumble into a career. **CareerPath** changes that.

Answer a carefully curated quiz about how you think, what you love, and where you want to go — and the app's weighted-scoring algorithm instantly surfaces your top career matches with a percentage fit score, curated learning resources, educational pathways, and a personalised action plan to get you there.

Whether you're a student, a career-switcher, or just curious — CareerPath gives you clarity.

---


## 🖼️ Screenshots

<div align="center">

| Home — Hero | Quiz in Progress | Your Results |
|:-----------:|:----------------:|:------------:|
| *(Gradient hero, CTA buttons)* | *(Progress bar, question cards)* | *(Career cards with % match)* |

</div>

---

## 🎯 Features

| Feature | Description |
|---------|-------------|
| 🧠 **Smart Quiz Engine** | Multi-category questions (personality, skills, interests, goals) with a weighted scoring algorithm |
| 📊 **Career Match Score** | Each result comes with a percentage match based on your unique profile |
| 💡 **Detailed Career Cards** | Expandable cards with key skills, educational pathways, recommended courses & communities |
| 🗺️ **Action Steps** | Personalised, step-by-step roadmap to start or advance your chosen career |
| 🌙 **Dark Mode** | Fully theme-aware UI — looks great day or night |
| 📱 **Fully Responsive** | Mobile-first design, works seamlessly on any screen size |
| ⚡ **Blazing Fast** | Vite-powered build — zero config, instant HMR |

---

## 🛠️ Tech Stack

```
careerpath/
├── ⚛️  React 18       — UI component library
├── 🔷  TypeScript     — Full static typing
├── 🎨  Tailwind CSS   — Utility-first styling
├── ⚡  Vite           — Lightning-fast bundler & dev server
├── 🔗  React Router   — Client-side routing
└── 🖼️  Lucide React   — Beautiful, consistent icons
```

---

## 📁 Project Structure

```
project/
├── src/
│   ├── components/
│   │   ├── home/          # Hero, HowItWorks, Testimonials, CallToAction
│   │   ├── quiz/          # QuizQuestion, ProgressBar, EmailCapture
│   │   └── results/       # CareerCard, ActionSteps
│   ├── context/
│   │   ├── QuizContext    # Quiz state, scoring algorithm, navigation
│   │   └── ThemeContext   # Dark/light mode management
│   ├── data/
│   │   ├── quizData.ts    # All quiz questions with weighted career affects
│   │   └── careerData.ts  # Full career database with skills, resources & job boards
│   ├── pages/
│   │   ├── Home.tsx       # Landing page
│   │   ├── Quiz.tsx       # Quiz flow
│   │   └── Results.tsx    # Career match results
│   └── App.tsx            # Root component & routing
├── tailwind.config.js
├── vite.config.ts
└── package.json
```

---

## ⚙️ Getting Started

### Prerequisites

- **Node.js** v18 or higher
- **npm** or **yarn**

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/careerpath.git

# 2. Navigate into the project
cd careerpath

# 3. Install dependencies
npm install

# 4. Start the development server
npm run dev
```

The app will be available at `http://localhost:5173` 🎉

### Build for Production

```bash
npm run build       # Compiles & bundles for production
npm run preview     # Preview the production build locally
```

---

## 🧠 How the Scoring Algorithm Works

The quiz is divided into **4 categories**: `personality`, `skills`, `interests`, and `goals`.

Each answer option carries a set of `affects` — a list of career IDs and weights. When you answer a question, the weights for your chosen option are accumulated into a score map:

```ts
// Each option in quizData.ts looks like:
{
  id: 0,
  text: "Analytically, breaking things down step by step",
  affects: [
    { careerId: "data-science",          weight: 10 },
    { careerId: "software-engineering",  weight: 8  },
    { careerId: "finance",               weight: 7  }
  ]
}
```

After all questions are answered, careers are **ranked by total accumulated score** and normalised into a percentage match. The top careers are then displayed with rich detail cards.

---

## 🗺️ Roadmap

- [x] Core quiz engine with weighted scoring
- [x] Career result cards with expandable detail
- [x] Dark mode support
- [x] Personalised action steps
- [ ] 🔜 User authentication & saved results
- [ ] 🔜 More career profiles (50+ careers)
- [ ] 🔜 Share your results on social media
- [ ] 🔜 AI-powered career chat advisor

---

## 🤝 Contributing

Contributions are welcome and appreciated! Here's how to get started:

```bash
# Fork the repo, then:
git checkout -b feature/your-feature-name
git commit -m "feat: add your amazing feature"
git push origin feature/your-feature-name
# Open a Pull Request 🚀
```

Please follow the existing code style and keep PRs focused and concise.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<div align="center">

Made with ❤️ and a lot of ☕ by **[Subhalaxmi Panda](https://github.com/SubhuPanda21)**

⭐ If this project helped you, give it a star — it means a lot!

</div>
