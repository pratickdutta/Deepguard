# 🛡️ DeepGuard: Let's See Who's Faking It

[![Next.js](https://img.shields.io/badge/Next.js-15-black?style=flat&logo=next.js)](https://nextjs.org/)
[![Firebase](https://img.shields.io/badge/Firebase-11-orange?style=flat&logo=firebase)](https://firebase.google.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3-38B2AC?style=flat&logo=tailwind-css)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Expose the Fake. Protect the Truth.** DeepGuard is a powerful, AI-driven media verification platform designed to detect deepfakes, synthetic images, and manipulated content in real-time.

---

## 🌟 Key Features

- **High-Accuracy Detection**: Leverages advanced ML models via Replicate API.
- **Multiple AI Models**: Support for specialized detection models:
  - `bcmi/fake-image-detection`: General purpose synthetic image detection.
  - `wzhouwzhou/deepfake-detection`: Specialized in facial manipulation detection.
- **Real-Time Analysis**: Instant scanning of images and URLs with detailed confidence scores.
- **Secure Authentication**: Integrated with Firebase Auth for personalized scan history and profile management.
- **Interactive UI**: Built with modern components (Radix UI, Vaul, Embla) for a premium user experience.
- **History Tracking**: Keeps a logged history of your scans for future reference.
- **Mobile Responsive**: Fully optimized for desktop, tablet, and mobile devices.

## 🛠️ Tech Stack

### Frontend
- **Framework**: [Next.js 15](https://nextjs.org/) (App Router, Client Components)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) with [Shadcn/UI](https://ui.shadcn.com/)
- **Icons**: [Lucide React](https://lucide.dev/)
- **State Management**: React Context API
- **Animations**: Tailwind Animate, Vaul (Drawers)

### Backend
- **Server**: [Node.js](https://nodejs.org/) & [Express](https://expressjs.com/)
- **AI Inference**: [Replicate API](https://replicate.com/)
- **Database/Auth**: [Firebase](https://firebase.google.com/) (Auth, Firestore)

---

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- pnpm / npm / yarn
- Firebase Project
- Replicate API Key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/pratickdutta/Deepguard.git
   cd Deepguard
   ```

2. **Install Frontend Dependencies**
   ```bash
   pnpm install
   ```

3. **Set Up Environment Variables**
   Create a `.env.local` in the root and add your Firebase configurations.

4. **Install Backend Dependencies**
   ```bash
   cd backend
   npm install
   ```
   Create a `.env` file in the `backend` folder and add your `REPLICATE_API_TOKEN`.

---

## 💻 Development

You can run both the frontend and backend simultaneously:

### Run Frontend
```bash
pnpm run dev
```

### Run Backend
```bash
cd backend
npm run dev
```

The application will be available at `http://localhost:3000`.

---

## 📡 API Reference

DeepGuard exposes a robust backend API for media detection:

- `POST /detect`: Analyze a `mediaUrl` for synthetic manipulation.
- `GET /models`: List available AI detection models.
- `GET /history`: Fetch authenticated user scan history.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

<p align="center">Made with ❤️ for a safer digital world.</p>
