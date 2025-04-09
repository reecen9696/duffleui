# RampX Wrapped

A year-in-review experience for RampX users, showcasing their on-chain activity in an engaging, interactive presentation.

---

## 🚀 Getting Started

1. **Install dependencies:**
```bash
npm install --legacy-peer-deps
```

2. **Run development server:**
```bash
npm run start
```

3. **Build the project:**
```bash
npm run build
```

---

## 🧠 Project Structure

```
rampx-wrapped/
├── app/                  # Next.js App Router
├── components/           # React components
│   ├── slides/           # Individual slide components
│   └── ui/               # Reusable UI components
├── config/               # Configuration files
│   └── slides.ts         # Slide configuration and ordering
├── context/              # React context providers
├── hooks/                # Custom React hooks
├── lib/                  # Utility functions and API
├── public/               # Static assets
└── styles/               # Tailwind + global styles
```

---

## 🧩 Adding a New Slide

1. **Create your component:**  
   In `components/slides/`, follow the existing slide structure.

2. **Add to the enum:**  
   Update `SlideType` in `config/slides.ts`.

3. **Register in config:**  
   Add a new entry to `slidesConfig` in `config/slides.ts`.

4. **Provide data:**  
   Update `WrappedData` in `lib/api.ts` to include your new data.

---

## 🎨 Styling & Animation

- **TailwindCSS** is used for styling (config in `tailwind.config.ts`)
- **Framer Motion** handles animations

---

## 🔌 Data Source

- Located in `lib/api.ts`
- Mock data is used for development
- Replace with real API in production