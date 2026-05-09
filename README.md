# 🤖 ChatNext — AI Chatbot powered by Gemini

<div align="center">

![Next.js](https://img.shields.io/badge/Next.js-16-black?style=for-the-badge\&logo=next.js)
![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge\&logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=for-the-badge\&logo=typescript)
![Gemini](https://img.shields.io/badge/Google-Gemini-orange?style=for-the-badge\&logo=google)
![Vercel](https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge\&logo=vercel)
![Assistant UI](https://img.shields.io/badge/UI-Assistant_UI-purple?style=for-the-badge)

### 🚀 Modern AI Chatbot built using Next.js, Assistant UI, Vercel AI SDK, and Google Gemini API.

</div>

---

# 📌 Overview

**ChatGPT Next** is a modern AI chatbot application inspired by ChatGPT UI experiences.

This project provides:

✅ Real-time AI conversations
✅ Streaming responses
✅ Modern responsive UI
✅ Gemini AI integration
✅ Scalable architecture
✅ Production-ready deployment
✅ Assistant UI integration
✅ Vercel deployment support

The project is designed with modern frontend and AI engineering practices using the latest ecosystem tools.

---

# ✨ Features

## 💬 AI Chat Interface

* Interactive conversational UI
* Real-time message streaming
* ChatGPT-like experience
* Smooth assistant response rendering

## ⚡ Gemini AI Integration

* Integrated with Google Gemini API
* Fast response generation
* AI streaming support
* Easily swappable AI providers

## 🎨 Modern UI/UX

* Clean dark interface
* Responsive design
* Minimalist AI application styling
* Optimized user experience

## 🧠 AI SDK Integration

* Built using Vercel AI SDK
* Streaming architecture
* Tool-ready architecture
* Future extensibility support

## 🚀 Deployment Ready

* Optimized for Vercel deployment
* Environment variable support
* GitHub integration
* Production deployment workflow

---

# 🛠️ Tech Stack

| Technology           | Purpose                          |
| -------------------- | -------------------------------- |
| ⚛️ React 19          | Frontend framework               |
| ▲ Next.js 16         | Full-stack React framework       |
| 🟦 TypeScript        | Type safety                      |
| 🤖 Google Gemini API | AI model provider                |
| 🧠 Vercel AI SDK     | AI streaming & model integration |
| 🎛️ Assistant UI     | AI chat interface                |
| 🎨 Tailwind CSS      | Styling                          |
| 🧩 Radix UI          | Accessible UI components         |
| ☁️ Vercel            | Deployment platform              |
| 📦 npm               | Package manager                  |

---

# 📂 Project Structure

```bash
Chatgpt_Next/
│
├── app/
│   ├── api/
│   │   └── chat/
│   │       └── route.ts
│   ├── components/
│   ├── assistant.tsx
│   ├── layout.tsx
│   ├── page.tsx
│   └── globals.css
│
├── lib/
├── public/
├── .env.example
├── package.json
├── tsconfig.json
└── README.md
```

---

# ⚙️ Installation & Setup

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/your-repository-name.git
```

---

## 2️⃣ Navigate into Project

```bash
cd your-repository-name
```

---

## 3️⃣ Install Dependencies

```bash
npm install
```

---

# 🔑 Environment Variables

Create a `.env.local` file in the root directory.

```env
GOOGLE_GENERATIVE_AI_API_KEY=YOUR_GEMINI_API_KEY
```

---

# 🤖 Get Gemini API Key

You can generate your Gemini API key from:

👉 [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)

---

# ▶️ Run Development Server

```bash
npm run dev
```

Open:

```bash
http://localhost:3000
```

---

# ☁️ Deploy on Vercel

## 🚀 One-Click Deployment

1. Push project to GitHub
2. Import repository in Vercel
3. Add environment variable:

```env
GOOGLE_GENERATIVE_AI_API_KEY=YOUR_KEY
```

4. Deploy

---

# 🧠 API Route Example

```ts
import { google } from "@ai-sdk/google";
import { frontendTools } from "@assistant-ui/react-ai-sdk";
import { convertToModelMessages, streamText } from "ai";

export const maxDuration = 30;

export async function POST(req: Request) {
  const { messages, system, tools } = await req.json();

  const result = streamText({
    model: google("gemini-2.5-flash"),
    system,
    messages: await convertToModelMessages(messages),
    tools: frontendTools(tools),
  });

  return result.toUIMessageStreamResponse();
}
```

---

# 📦 Scripts

| Command            | Description              |
| ------------------ | ------------------------ |
| `npm run dev`      | Start development server |
| `npm run build`    | Create production build  |
| `npm run start`    | Run production server    |
| `npm run lint`     | Run lint checks          |
| `npm run lint:fix` | Fix lint issues          |
| `npm run format`   | Format project           |

---

# 🧩 Dependencies Used

## Core Dependencies

* `next`
* `react`
* `typescript`
* `ai`
* `@ai-sdk/google`
* `@assistant-ui/react`
* `@assistant-ui/react-ai-sdk`

## UI Libraries

* `radix-ui`
* `lucide-react`
* `tailwindcss`
* `clsx`
* `tailwind-merge`

---

# 🛡️ Security Best Practices

✅ Keep `.env.local` private
✅ Never expose API keys publicly
✅ Use server-side API routes
✅ Store secrets in Vercel Environment Variables
✅ Do not use `NEXT_PUBLIC_` for secret keys

---


# 🚀 Future Improvements

* [ ] Authentication system
* [ ] Chat history persistence
* [ ] Database integration
* [ ] Multi-model support
* [ ] Image generation
* [ ] File upload support
* [ ] Voice assistant support
* [ ] AI agents/tools support
* [ ] Markdown rendering improvements
* [ ] Mobile optimization

---

# 🤝 Contributing

Contributions are welcome!

## Steps to Contribute

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature-name
```

3. Commit your changes

```bash
git commit -m "Added new feature"
```

4. Push to your branch

```bash
git push origin feature-name
```

5. Open a Pull Request

---

# 🧪 Production Engineering Notes

This project follows modern AI application architecture:

```text
Frontend (Assistant UI)
        ↓
Next.js API Route
        ↓
Vercel AI SDK
        ↓
Google Gemini API
```

The architecture is scalable and production-ready for modern AI applications.

---


# 👨‍💻 Developer

### Built with ❤️ by Surya Prakash Gupta

* 💼 AI Engineer
* ⚛️ Full Stack Developer
* 🤖 AI Application Developer
  
---

# 📜 License

This project is licensed under the MIT License.

---

# ⭐ Support

If you like this project:

⭐ Star the repository
🍴 Fork the project
🧠 Contribute new features
🚀 Share with developers

---

<div align="center">

## 🚀 Happy Coding!

Built using modern AI engineering stack with ❤️

</div>
