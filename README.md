# PL-300 Practice Studio

An interactive practice exam tool for the Microsoft PL-300 (Power BI Data Analyst Associate) certification, built as a single-page web app with no build tools, no dependencies to install, and no backend.

**Live demo:** [add your GitHub Pages link here]

## The problem

While preparing for the PL-300 exam, I wanted a free practice tool organized around Microsoft's actual exam domain weightings, with explanations that teach rather than just grade. I could not find one that fit, so I built it.

## What it does

- **30 scenario-style questions** mapped to the four official PL-300 exam domains: Prepare the Data, Model the Data, Visualize and Analyze, and Manage and Secure
- **Domain-weighted question bank** that deliberately goes heavier on Model the Data, because DAX and data modeling carry the hardest scenario questions on the real exam
- **DAX Focus mode** for targeted study sessions on modeling concepts like CALCULATE filter behavior, context transition, iterators, and time intelligence
- **Instant feedback with full explanations** covering why the correct answer is right and why each distractor is wrong
- **Per-domain score diagnostic** at the end of every session, highlighting the weakest domain so the next study block has a clear target

The diagnostic is the feature I care about most: it turns a quiz into a measurement tool. After each session, the results screen tells you exactly where to focus, which is the same think-measure-adjust loop I use in analytics work.

## How it is built

- Single-file React application, written with AI-assisted development using Claude
- Question bank stored as a plain data structure, fully separated from app logic, so the bank can grow without touching any component code
- Runs entirely in the browser from one `index.html` using React via CDN, which means it deploys to GitHub Pages with a single file upload
- Styling follows my personal document design system: deep forest green and gold, Georgia body text, Arial headings, and Courier New for DAX code blocks

## Running it

Open the live demo link above, or download `index.html` and open it in any modern browser. No installation required.

## What I learned

- Translating the PL-300 exam blueprint into a structured dataset forced me to understand the domain weightings and question styles at a deeper level than passive studying
- Separating data from presentation logic mirrors the same principle behind star schema design in Power BI: keep the facts in one place and let everything else reference them
- AI-assisted development works best when you scope the architecture first and review each piece, the same way I review dashboard requirements before building

## About me

I am Jordan Foltz, an entry-level data analyst working with Power BI, Power Apps, SQL, Tableau, and Python. 

- LinkedIn: [linkedin.com/in/jordan-foltz](https://www.linkedin.com/in/jordan-foltz)
- Email: jordy3338@gmail.com
