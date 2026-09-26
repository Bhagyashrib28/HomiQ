# HomiQ React Frontend

Frontend-only React + TypeScript + Vite implementation based on the uploaded HomiQ prototype screens.

## Included
- Premium HomiQ visual system: forest green, gold, off-white, rounded cards.
- React Router navigation.
- 19 major screens/routes from the HomiQ architecture.
- Reusable header, footer, property cards, AI widgets and form/dashboard components.
- Local prototype-derived image assets.
- Mock data only. No Django/Node backend, database, authentication service, payment gateway, AI API or real VR engine is connected.

## Run on Windows

```bash
npm install
npm run dev
```

Then open the Vite URL shown in the terminal, usually http://localhost:5173.

## Backend integration later

Replace mock data with API calls in a future `src/services/api.ts` layer. The intended backend architecture can use your planned Django/NestJS/FastAPI services without changing the main UI structure.

Structure 
homiq-frontend/
│
├── package.json
├── index.html
│
├── public/
│   └── images/
│
└── src/
    │
    ├── main.tsx
    ├── App.tsx
    ├── styles.css
    │
    ├── components/
    │   ├── Header.tsx
    │   ├── Footer.tsx
    │   ├── PropertyCard.tsx
    │   ├── Badge.tsx
    │   └── SectionTitle.tsx
    │
    └── pages/
        ├── Home.tsx
        ├── Properties.tsx
        ├── PropertyDetails.tsx
        ├── Login.tsx
        ├── Signup.tsx
        └── VirtualTour.tsx
