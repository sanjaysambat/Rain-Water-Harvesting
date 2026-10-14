<!-- AquaVest — Smart Rainwater Harvesting Solution -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:063B5C,45:087E8B,100:45D6B5&height=240&section=header&text=AquaVest&fontSize=82&fontColor=FFFFFF&fontAlignY=38&desc=SMART%20RAINWATER%20HARVESTING%20SOLUTION&descSize=16&descAlignY=60&animation=fadeIn" width="100%" alt="AquaVest — Smart Rainwater Harvesting Solution" />

### 💧 Every Drop Counts. Every Roof Has Potential.

An intelligent water-conservation platform that helps estimate rainwater harvesting potential, plan storage capacity, explore savings, and make more informed decisions for a water-secure future.

<p>
  <a href="https://github.com/"><strong>🌧️ Explore the Project</strong></a>
  &nbsp; · &nbsp;
  <a href="#-getting-started">Quick Start</a>
  &nbsp; · &nbsp;
  <a href="#-how-aquavest-works">How It Works</a>
</p>

<img src="https://img.shields.io/badge/Focus-Water%20Sustainability-087E8B?style=for-the-badge&labelColor=063B5C" alt="Water Sustainability" />
<img src="https://img.shields.io/badge/Framework-Next.js%2015-111827?style=for-the-badge&logo=next.js" alt="Next.js 15" />
<img src="https://img.shields.io/badge/AI-Google%20Genkit-4285F4?style=for-the-badge&logo=google" alt="Google Genkit" />

</div>

---

## 🌊 About AquaVest

Fresh water is precious, yet a significant amount of rainwater can flow away unused. **AquaVest** brings rainfall estimation, storage planning, sustainability insights, and financial analysis together in one web application.

Designed with an accessible interface and AI-assisted guidance, AquaVest helps users understand how much water their roof could collect and what a rainwater harvesting system might mean for their home or building.

> **Our vision:** turn rainfall into a practical resource through informed planning and responsible water use.

## ✨ Features at a glance

<table>
<tr>
<td width="50%" valign="top">

### 🌧️ Rainwater Potential Calculator
Estimate harvestable water from roof area and rainfall inputs using a runoff coefficient.

</td>
<td width="50%" valign="top">

### 🛢️ Smart Tank Sizing
Explore AI-assisted storage recommendations based on estimated collection potential and user inputs.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📈 Cost–Benefit Insights
Visualize estimated savings and explore the potential financial value of harvesting rainwater.

</td>
<td width="50%" valign="top">

### 📡 IoT-Style Simulation
View simulated rainfall sensor readings and visualize changing conditions without requiring physical sensors.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📄 PDF Reports
Generate a report of harvesting estimates and analysis for review and planning.

</td>
<td width="50%" valign="top">

### 🌐 Three Languages
Use the available English, Hindi, and Tamil localization resources.

</td>
</tr>
</table>

### 🌱 Designed for everyday use

- 📱 Responsive interface for desktop, tablet, and mobile
- 🌓 Dark and light theme support
- 🔐 Firebase Authentication for account access
- 📊 Interactive charts and results dashboards
- 🤖 Google Genkit integration for AI-assisted recommendations

---

## 💦 How AquaVest works

<div align="center">

| Step | What happens |
|:---:|---|
| **01 · INPUT** | Enter roof area, rainfall, and relevant details |
| **02 · CALCULATE** | Estimate potential water collection |
| **03 · PLAN** | Review storage sizing and conservation suggestions |
| **04 · COMPARE** | Explore cost–benefit estimates and visualizations |
| **05 · REPORT** | Generate a report to support planning |

</div>

### 🧮 The calculation behind the estimate

A simplified harvesting estimate is:

\[
\text{Harvestable Water (litres)} =
\text{Rainfall (mm)} \times \text{Roof Area (m²)} \times C
\]

Here, \(C\) is the runoff coefficient. The project uses **0.85** as a planning assumption in its stated formula. Actual collection depends on roof material, first-flush diversion, leakage, filtration, and other losses, so results should be treated as estimates rather than guarantees.

---

## 🛠️ Technology stack

<div align="center">

<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js" />
<img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
<br/>
<img src="https://img.shields.io/badge/Google_Genkit-4285F4?style=for-the-badge&logo=google&logoColor=white" alt="Google Genkit" />
<img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=111827" alt="Firebase" />
<img src="https://img.shields.io/badge/Shadcn%2Fui-111827?style=for-the-badge" alt="shadcn/ui" />

</div>

| Layer | Tools |
|---|---|
| Frontend | Next.js 15, React 18, TypeScript |
| Styling & UI | Tailwind CSS, shadcn/ui, Radix UI |
| AI | Google Genkit and Google AI models |
| Backend services | Next.js API routes, Firebase |
| Authentication | Firebase Authentication |
| State & context | React Context |
| Localization | JSON locale files for English, Hindi, and Tamil |

---

## 🗂️ Project structure

```text
AquaVest/
├── src/
│   ├── ai/
│   │   ├── genkit.ts
│   │   └── dev.ts
│   ├── app/
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   ├── admin/
│   │   ├── login/
│   │   ├── signup/
│   │   ├── forgot-password/
│   │   ├── settings/
│   │   ├── report/
│   │   └── iot-connect/
│   ├── components/
│   │   ├── aquavest/
│   │   ├── ui/
│   │   └── layout/
│   ├── contexts/
│   ├── hooks/
│   ├── lib/
│   └── locales/
│       ├── en.json
│       ├── hi.json
│       └── ta.json
├── docs/
│   └── blueprint.md
├── apphosting.yaml
└── package.json
```

---

## 🚀 Getting started

### Prerequisites

- Node.js 18 or newer
- npm
- Google AI / Genkit API credentials for AI features
- Firebase project credentials for Firebase-backed features

### 1. Get the source code

```bash
git clone <your-repository-url>
cd "rain water harvesting"
```

Replace `<your-repository-url>` with your actual repository URL. If the project is already on your computer, open a terminal in its root folder instead.

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create `.env.local` in the project root and add the values for your own Firebase and AI projects:

```env
NEXT_PUBLIC_FIREBASE_API_KEY=your_firebase_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_firebase_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_firebase_app_id

GENKIT_API_KEY=your_genkit_api_key
NEXT_PUBLIC_GOOGLE_AI_API_KEY=your_google_ai_api_key
```

Use only the environment variables required by the codebase. Never commit `.env.local` or real API keys to GitHub. Keep server-side secrets out of variables prefixed with `NEXT_PUBLIC_`, because those may be exposed to the browser.

### 4. Start the development server

```bash
npm run dev
```

If the project uses the Genkit development workflow, open a **second terminal** in the project root:

```bash
npm run genkit:watch
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### 5. Check the project

```bash
npm run lint
npm run typecheck
npm run build
```

Run only scripts that are defined in your `package.json`. If a script is missing, check the available scripts before running it.

---

## 📦 Useful commands

| Command | Purpose |
|---|---|
| `npm run dev` | Start the Next.js development server |
| `npm run genkit:dev` | Start the Genkit development workflow |
| `npm run genkit:watch` | Restart Genkit when files change |
| `npm run build` | Build the production application |
| `npm start` | Start the production server after building |
| `npm run lint` | Check code style and lint rules |
| `npm run typecheck` | Check TypeScript types, if configured |

---

## 🌏 Sustainability meets smart technology

AquaVest brings together digital planning and water conservation to help people ask useful questions:

- How much rainwater could this roof collect?
- What storage capacity should be considered?
- What might the estimated savings look like?
- How can rainfall and collection data be understood more clearly?

**Important:** AI recommendations, simulated sensor readings, and financial projections should be validated against local rainfall records, site conditions, current costs, and applicable regulations before making real-world construction or investment decisions.

---

## 🧭 Roadmap

- [ ] Connect to reliable local rainfall datasets
- [ ] Expand tank-sizing logic with demand and seasonal variation
- [ ] Integrate physical IoT sensors where available
- [ ] Add maintenance reminders and system-health insights
- [ ] Improve community-level water conservation analytics
- [ ] Explore mobile experiences and water-utility integrations
- [ ] Expand evaluation of AI recommendations and report accuracy

---

## 🐛 Troubleshooting

<details>
<summary><strong>“next is not recognized”</strong></summary>

Run `npm install` from the project root, then retry `npm run dev`.
</details>

<details>
<summary><strong>Port 3000 is already in use</strong></summary>

Try another port:

```bash
npm run dev -- -p 3001
```
</details>

<details>
<summary><strong>Firebase or AI API key errors</strong></summary>

Check that `.env.local` is in the project root, the variable names match the code, and the credentials are valid. Restart the development server after changing environment variables.
</details>

<details>
<summary><strong>Genkit command is missing</strong></summary>

Check `package.json` for the exact script name and confirm the project's dependencies are installed.
</details>

---

## 🤝 Contributing

Contributions, suggestions, and issue reports are welcome.

1. Create a feature branch: `git checkout -b feature/amazing-feature`
2. Commit your changes: `git commit -m "Add amazing feature"`
3. Push your branch: `git push origin feature/amazing-feature`
4. Open a pull request with a description of the changes.

Please do not include credentials, private user data, or unsupported claims about system accuracy.

---

## 👨‍💻 Author

<div align="center">

### **SANJAY S**

*Building technology for a more sustainable future.*

<img src="https://img.shields.io/badge/Project-AquaVest-087E8B?style=for-the-badge&logo=dropbox&logoColor=white" alt="AquaVest Project" />
<img src="https://img.shields.io/badge/Theme-Water%20%26%20Sustainability-45D6B5?style=for-the-badge&logo=leaflet&logoColor=063B5C" alt="Water and Sustainability" />

</div>

---

## 📄 License

Add the project's chosen license and corresponding `LICENSE` file before distributing the project. No specific license was provided in the supplied project description.

<div align="center">

### 🌧️ Save Rain. Store Water. Sustain Tomorrow.

*Every drop collected is a step toward a water-secure future.*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:45D6B5,50:087E8B,100:063B5C&height=120&section=footer" width="100%" alt="AquaVest water-inspired footer" />

</div>
