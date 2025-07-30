# Restaurant-1 W'FoodJS - Modern Next.js Frontend Restaurant Website (Design 1)

![project23](https://github.com/user-attachments/assets/77de8404-aeba-4f67-b5fe-0438e80bda73) ![Screenshot 2024-09-13 at 03 34 24](https://github.com/user-attachments/assets/1ef89f8a-e6f8-4bfa-9c95-453e35bbf4ee) ![Screenshot 2024-09-13 at 03 35 51](https://github.com/user-attachments/assets/9f3eb9e5-5dd7-46fd-9b23-aee505fa84d1) ![Screenshot 2024-09-13 at 03 34 55](https://github.com/user-attachments/assets/bd1df324-3ba9-45d9-a530-5ebce27cfe36) ![Screenshot 2024-09-13 at 03 35 12](https://github.com/user-attachments/assets/d6f0347c-3ec7-41d1-9d64-695ee0ddfd24) ![Screenshot 2024-09-13 at 03 35 33](https://github.com/user-attachments/assets/7bff98ba-b797-4c01-962e-ec0e2156bbd6)

---

## Project Summary

W'FoodJS is a modern, visually appealing static restaurant website built with Next.js 14, React.js, TailwindCSS, and a suite of supporting libraries. This project demonstrates how to build a responsive, animated, and interactive front-end application using a best-practices tech stack, suitable for learning, teaching, and real-world static site deployments.

- **Live-Demo:** [https://restaurant-js-arnob.vercel.app/](https://restaurant-js-arnob.vercel.app/)

> _Note: This project is implemented in JavaScript. A TypeScript version is also available at [RestaurantTS-NextJS](https://github.com/arnobt78/RestaurantTS-NextJS-Website)._

---

## Table of Contents

- [Project Summary](#project-summary)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Running the Project](#running-the-project)
- [API & Routing](#api--routing)
- [Component Walkthrough](#component-walkthrough)
- [Learning & Teaching Content](#learning--teaching-content)
- [Keywords](#keywords)
- [Deployment](#deployment)
- [References](#references)
- [Conclusion](#conclusion)

---

## Features

- Responsive design with TailwindCSS utility-first framework
- Modern UI/UX with smooth animations (Framer Motion & TailwindCSS Animate)
- Date selection and management (date-fns, React-Day-Picker)
- Interactive map via React-Leaflet
- Dynamic iconography with Lucide-React and React-Icons
- Scroll effects and responsive queries (React-Scroll, React-Responsive)
- Google Fonts optimization (next/font)
- Modular, reusable component architecture
- Easy setup and deployment via Vercel
- Clean, semantic codebase for learning and teaching

---

## Technology Stack

- **Framework:** [Next.js 14](https://nextjs.org/) (React-based SSR/SSG framework)
- **Language:** JavaScript (ES6+)
- **Styling:** [TailwindCSS](https://tailwindcss.com/), [tailwindcss-animate](https://github.com/joe-bell/tailwindcss-animate)
- **Animation:** [Framer Motion](https://www.framer.com/motion/)
- **Date Handling:** [date-fns](https://date-fns.org/), [React-Day-Picker](https://react-day-picker.js.org/)
- **Maps:** [React-Leaflet](https://react-leaflet.js.org/)
- **Icons:** [Lucide-React](https://lucide.dev/), [React-Icons](https://react-icons.github.io/react-icons/)
- **Responsive Utilities:** [React-Responsive](https://github.com/contra/react-responsive), [React-Scroll](https://www.npmjs.com/package/react-scroll)
- **Font Optimization:** [next/font](https://nextjs.org/docs/basic-features/font-optimization)
- **Deployment:** [Vercel](https://vercel.com/)

---

## Project Structure

> _Note: The actual file/folder names may differ slightly depending on your customization._

```
/
├── app/
│   ├── page.js            # Main homepage
│   └── ...                # Other Next.js App Directory files
├── components/            # Reusable React components
├── public/                # Static assets (images, icons)
├── styles/                # TailwindCSS, global styles
├── package.json           # Dependencies and scripts
├── tailwind.config.js     # TailwindCSS configuration
├── next.config.js         # Next.js configuration
└── README.md              # Project documentation
```

---

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/arnobt78/RestaurantJS--TailwindCSS-Fundamental-Project-5.git
   cd RestaurantJS--TailwindCSS-Fundamental-Project-5
   ```

2. **Install dependencies:**  
   Make sure you have [NodeJS](https://nodejs.org/en/) installed.  
   Then run:
   ```bash
   npm install
   # or
   yarn
   # or
   pnpm install
   # or
   bun install
   ```

   **Install specific packages (if not auto-installed):**
   ```bash
   npm i framer-motion date-fns react-leaflet lucide-react react-day-picker react-scroll react-icons react-responsive tailwindcss-animate
   ```

---

## Running the Project

Start the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to view the app.

You can start editing the main page by modifying `app/page.js`. The app supports hot reloading for rapid development.

---

## API & Routing

This project is a static front-end site and does not connect to a backend API by default.  
Next.js routing is file-based; each file in the `app/` directory corresponds to a route:

- `/` → `app/page.js` (Homepage)
- Additional pages/components can be added under `app/` or as dynamic segments.

If you wish to add an API or server-side logic, refer to the [Next.js API Routes documentation](https://nextjs.org/docs/pages/building-your-application/routing/api-routes).

---

## Component Walkthrough

- **Header & Navigation:** Responsive site header, mobile-friendly nav using Tailwind's utilities
- **Hero Section:** Eye-catching introduction with animations (Framer Motion)
- **Menu Display:** Showcases featured dishes or menu categories using card components
- **Reservation:** Date selection with React-Day-Picker and date-fns
- **Location/Map:** Interactive map using React-Leaflet for showing restaurant location
- **Contact Section:** Clean, accessible form for user inquiries
- **Footer:** Social links, copyright

All components are modular and reusable.  
Example (simplified):
```jsx
// components/Hero.jsx
import { motion } from "framer-motion";
export default function Hero() {
  return (
    <motion.section initial={{ opacity: 0 }} animate={{ opacity: 1 }}>
      <h1 className="text-4xl font-bold">Welcome to RestaurantJS</h1>
      <p className="mt-4">Experience modern dining with us!</p>
    </motion.section>
  );
}
```

---

## Learning & Teaching Content

This project is ideal for:

- Learning Next.js (App Router, SSR/SSG, routing)
- Mastering TailwindCSS for rapid UI prototyping
- Using animation libraries (Framer Motion, tailwindcss-animate)
- Integrating third-party React libraries (maps, icons, date pickers)
- Understanding component-driven design in React
- Practicing responsive web development

**Customization Tips:**

- Add new pages by creating files in `app/`
- Update menu and content in the corresponding components
- Modify Tailwind config for branding
- Deploy easily with Vercel for free

---

## Keywords

`Next.js`, `React`, `TailwindCSS`, `Framer Motion`, `Static Site`, `Restaurant Website`, `Frontend`, `Animation`, `Responsive Design`, `React Components`, `Learning Project`, `Map Integration`, `UI/UX`, `Vercel Deployment`, `JavaScript`

---

## Deployment

The easiest way to deploy is with [Vercel](https://vercel.com/):

- Push your project to GitHub
- Import the repository into Vercel
- Choose the default settings; Vercel will handle the build and deployment

For more details, see [Next.js deployment documentation](https://nextjs.org/docs/deployment).

---

## References

- [Next.js Documentation](https://nextjs.org/docs)  
- [Learn Next.js](https://nextjs.org/learn)  
- [TailwindCSS Documentation](https://tailwindcss.com/docs)  
- [Framer Motion Docs](https://www.framer.com/motion/)  
- [React-Leaflet Docs](https://react-leaflet.js.org/docs/)  
- [React-Day-Picker Docs](https://react-day-picker.js.org/)  
- [Vercel Docs](https://vercel.com/docs)

---

## Conclusion

This project is a showcase of modern static site development using the React and Next.js ecosystem, featuring powerful UI frameworks and libraries to deliver a delightful learning and user experience.

---

## Happy Coding! 🎉

Feel free to use this project repository and extend this project further!

If you have any questions or want to share your work, reach out via GitHub or my portfolio at [https://arnob-mahmud.vercel.app/](https://arnob-mahmud.vercel.app/).

**Enjoy building and learning!** 🚀

Thank you! 😊

---

