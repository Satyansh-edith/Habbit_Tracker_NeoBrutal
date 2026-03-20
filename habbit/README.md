# 🚀 Habbit Tracker - NeoBrutal Edition

> A powerful, AI-enhanced habit tracking application built with **Next.js 16**, **React 19**, and **MongoDB**. Track your daily habits, journal your progress, analyze your patterns with AI, and visualize your growth all in one place.

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-16-black?style=for-the-badge&logo=next.js" alt="Next.js 16">
  <img src="https://img.shields.io/badge/React-19-61dafb?style=for-the-badge&logo=react" alt="React 19">
  <img src="https://img.shields.io/badge/TypeScript-5-3178c6?style=for-the-badge&logo=typescript" alt="TypeScript 5">
  <img src="https://img.shields.io/badge/MongoDB-Connected-13aa52?style=for-the-badge&logo=mongodb" alt="MongoDB">
  <img src="https://img.shields.io/badge/Tailwind%20CSS-4-38b2ac?style=for-the-badge&logo=tailwindcss" alt="Tailwind CSS 4">
</p>

---

## ✨ Features

### 📊 Habit Tracking
- **Create & Manage Habits** - Add unlimited habits to track
- **Daily Logging** - Mark habits as complete or incomplete each day
- **Streak Calculation** - Automatic streak counting to keep you motivated
- **Progress Overview** - Visual dashboard showing all your habits and their status
- **Habit History** - View complete history of all your habit logs

### 🤖 AI-Powered Intelligence
- **Journal Analysis** - Use Groq AI to analyze your journal entries and get insights
- **Habit Suggestions** - Get personalized habit recommendations based on your patterns
- **Weekly Reflections** - AI generates meaningful reflections on your weekly progress
- **Smart Insights** - Pattern recognition to identify your habits and improvements

### 📝 Journal & Reflection
- **Daily Journaling** - Write and save daily journal entries
- **Journal History** - Browse all past entries
- **AI-Powered Analysis** - Get AI insights on your journal content
- **Weekly Summaries** - Automatic weekly reflection generation

### 💪 Motivation & Gamification
- **Hypeman Feature** - Get motivational messages when you complete habits
- **Streak Tracking** - Visual streak counter for each habit
- **Progress Metrics** - Track completion rates and trends
- **Achievement Display** - Celebrate your wins with the app

### 📈 Mood & Analytics
- **Mood Tracking** - Log your daily mood and emotions
- **Mood Trends** - Visualize mood patterns over time with interactive charts
- **Performance Analytics** - See correlations between habits and mood
- **Data Visualization** - Beautiful charts powered by Recharts

### 📸 Proof & Verification
- **Upload Proof** - Attach images/files as proof of habit completion
- **File Storage** - Secure file storage with Uploadthing
- **Verification System** - Verify habit completion with uploaded proof
- **Proof History** - Review all submitted proofs

### 🎯 Additional Features
- **Demo Mode** - Pre-seeded demo data for testing
- **Responsive Design** - Works on desktop, tablet, and mobile
- **NeoBrutal UI** - Bold, colorful 90s/Y2K inspired design
- **API Agents** - Auditor and enforcer agents for habit management
- **Vercel Ready** - Optimized for Vercel deployment

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Frontend** | React 19, Next.js 16, TypeScript 5 |
| **Styling** | Tailwind CSS 4, PostCSS |
| **Database** | MongoDB with Mongoose 9.3 |
| **AI/ML** | Groq SDK (Llama 3.3 70B), Google Generative AI |
| **File Upload** | Uploadthing 7.7 |
| **Visualization** | Recharts 3.8, Lucide React Icons |
| **Date Handling** | date-fns 4.1 |
| **Runtime** | Node.js, ES Modules |
| **Dev Tools** | ESLint 9, ts-node 10.9 |

---

## 📁 Project Structure

```
habbit/
├── app/                           # Next.js App Router
│   ├── api/                      # API Routes
│   │   ├── agents/               # AI agents (auditor, enforcer)
│   │   ├── ai/                   # AI endpoints
│   │   │   ├── analyze-journal/  # Journal analysis
│   │   │   ├── habit-suggestions/# AI suggestions
│   │   │   └── weekly-reflection/# Weekly summaries
│   │   ├── habits/               # Habit CRUD & verification
│   │   ├── habitlogs/            # Habit logging
│   │   ├── journal/              # Journal endpoints
│   │   ├── mood/                 # Mood tracking
│   │   ├── progress/             # Progress metrics
│   │   ├── streaks/              # Streak calculations
│   │   ├── upload/               # File uploads
│   │   └── uploadthing/          # Uploadthing integration
│   ├── dashboard/                # Dashboard page
│   ├── habits/                   # Habits management UI
│   ├── history/                  # Habit history view
│   ├── journal/                  # Journal pages
│   ├── mood/                     # Mood tracking UI
│   ├── test upload/              # Upload testing
│   ├── today/                    # Today's habits view
│   ├── layout.tsx                # Root layout
│   └── page.tsx                  # Home page
├── components/                    # Reusable React components
│   ├── AgentAlert.tsx            # Alert component
│   ├── AISuggestions.tsx         # AI suggestions display
│   ├── DemoModeButton.tsx        # Demo mode toggle
│   ├── Footer.tsx                # Footer
│   ├── HypemanBanner.tsx         # Motivation banner
│   ├── JournalAI.tsx             # Journal AI interface
│   ├── MoodChart.tsx             # Mood visualization
│   ├── Navbar.tsx                # Navigation bar
│   ├── ProofUploader.tsx         # File upload component
│   ├── Sidebar.tsx               # Sidebar navigation
│   └── WeeklyReflection.tsx      # Weekly summary display
├── models/                        # MongoDB schemas
│   ├── Habit.ts                  # Habit model
│   ├── HabitLog.ts               # Habit log model
│   ├── Journal.ts                # Journal model
│   └── User.ts                   # User model
├── lib/                           # Utility functions
│   ├── calculateStreak.ts        # Streak calculation logic
│   ├── getToday.ts               # Date utilities
│   ├── groq.ts                   # Groq AI integration
│   └── mongodb.ts                # MongoDB connection
├── hooks/                         # React hooks
│   └── useHypeman.ts             # Hypeman motivation hook
├── scripts/                       # Utility scripts
│   ├── seedDemoData.ts           # Demo data seeder
│   └── seedUser.ts               # User seeding
├── public/                        # Static assets
├── package.json                   # Dependencies & scripts
├── tsconfig.json                  # TypeScript config
├── next.config.ts                # Next.js config
├── eslint.config.mjs             # ESLint rules
├── postcss.config.mjs            # PostCSS plugins
└── tailwind.config.ts            # Tailwind configuration
```

---

## 🚀 Getting Started

### Prerequisites
- **Node.js** 16+ and **npm** or **yarn**
- **MongoDB** database (local or cloud via MongoDB Atlas)
- **API Keys** for:
  - Groq API (for AI analysis)
  - Google Generative AI (optional, for additional AI features)
  - Uploadthing (for file uploads)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Satyansh-edith/Habbit_Tracker_NeoBrutal.git
   cd Habbit_Tracker_NeoBrutal
   cd habbit
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env.local
   ```
   
   Fill in `.env.local` with your credentials:
   ```env
   # MongoDB
   MONGODB_URI=mongodb+srv://user:password@cluster.mongodb.net/habbit

   # Groq AI
   GROQ_API_KEY=your_groq_api_key

   # Google Generative AI
   GOOGLE_GENERATIVE_AI_KEY=your_google_ai_key

   # Uploadthing
   UPLOADTHING_SECRET=your_uploadthing_secret
   UPLOADTHING_APP_ID=your_uploadthing_app_id

   # Next.js
   NODE_ENV=development
   ```

4. **Run the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. **Open your browser**
   ```
   http://localhost:3000
   ```

---

## 📖 Usage Guide

### Creating a Habit
1. Navigate to **Habits** page
2. Click "Add New Habit"
3. Enter habit title and click create
4. Habit appears on dashboard and today's view

### Logging Habits
1. Go to **Today** page
2. Click ✓ to mark a habit as completed
3. Track your daily progress
4. View streaks to stay motivated

### Journaling
1. Navigate to **Journal** page
2. Write your daily thoughts and reflections
3. Click "Analyze with AI" to get insights
4. View past entries in **Journal History**

### Tracking Mood
1. Go to **Mood** page
2. Log your mood for the day
3. View **Trends** to see mood patterns
4. Correlate mood with habit completion

### Uploading Proof
1. Go to **Habits** → **Verify Proof**
2. Select a habit requiring verification
3. Upload screenshot/image as proof
4. AI verification agent reviews your submission

### Viewing Analytics
1. **Dashboard** - Overview of all habits and stats
2. **Progress** - Detailed progress metrics
3. **Streaks** - Current streaks for each habit
4. **History** - Complete habit log history

### Demo Mode
- Click the **Demo Mode** button to seed example data
- Test the app with pre-populated habits, logs, and journal entries
- Perfect for exploring features without starting from scratch

---

## 🔗 API Endpoints

### Habits
- `GET /api/habits` - Get all habits
- `POST /api/habits` - Create new habit
- `GET /api/habits/[id]` - Get specific habit
- `PUT /api/habits/[id]` - Update habit
- `DELETE /api/habits/[id]` - Delete habit

### Habit Logs
- `POST /api/habitlogs` - Log habit completion
- `GET /api/habitlogs` - Get all logged habits
- `DELETE /api/habitlogs` - Delete log entry

### Journal
- `POST /api/journal` - Create journal entry
- `GET /api/journal` - Get all entries
- `GET /api/journal/history` - Get journal history

### AI Features
- `POST /api/ai/analyze-journal` - Analyze journal with AI
- `POST /api/ai/habit-suggestions` - Get habit suggestions
- `POST /api/ai/weekly-reflection` - Generate weekly reflection

### Mood
- `POST /api/mood` - Log mood
- `GET /api/mood` - Get mood logs
- `GET /api/mood/trends` - Get mood trends

### Others
- `GET /api/streaks` - Get all streaks
- `GET /api/progress` - Get progress metrics
- `POST /api/habits/verify-proof` - Verify proof uploads
- `POST /api/uploadthing/route` - Handle file uploads

---

## 🎨 Design System

This app uses a **NeoBrutal design aesthetic** with:
- **Colors**: Bold neon pinks (#FF7AC6), purples (#8C6CFF), yellows (#FFD84D), and cyans (#6DD3FF)
- **Borders**: Thick black borders (4-8px) for a strong visual impact
- **Animations**: Smooth floating, spinning, and sliding animations
- **Typography**: Clean sans-serif with bold weights for impact
- **Layout**: Modern, spacious layouts with ample padding

---

## 📝 Scripts

```bash
# Development
npm run dev           # Start development server

# Production
npm run build         # Build for production
npm start             # Start production server

# Linting
npm run lint          # Run ESLint

# Database
npm run seed          # Seed demo data
npm run seed:user     # Seed user data
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📚 Deployment

### Deploy to Vercel (Recommended)
```bash
npm install -g vercel
vercel
```
The app is optimized for Vercel deployment per the "Initial commit - ready for Vercel deployment" message.

### Environment Variables on Vercel
Set all `.env.local` variables in Vercel's environment settings for your production deployment.

---

## 🐛 Troubleshooting

### MongoDB Connection Issues
- Ensure MongoDB URI in `.env.local` is correct
- Check MongoDB Atlas IP whitelist includes your IP
- Verify network connectivity

### AI Features Not Working
- Verify Groq API key is valid and has available credits
- Check Google Generative AI key if using that service
- Monitor API rate limits

### File Uploads Failing
- Ensure Uploadthing credentials are correct
- Check file size limits (default 4MB)
- Verify CORS settings

### Build Errors
```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install
npm run build
```

---

## 📄 License

This project is open source and available under the **MIT License**.

---

## 👨‍💻 Author

**Satyansh Edith**
- GitHub: [@Satyansh-edith](https://github.com/Satyansh-edith)
- Repository: [Habbit_Tracker_NeoBrutal](https://github.com/Satyansh-edith/Habbit_Tracker_NeoBrutal)

---

## 🌟 Acknowledgments

- **Groq** - Fast AI inference
- **Google Generative AI** - Advanced AI capabilities
- **MongoDB** - Robust database
- **Next.js** - Amazing React framework
- **Uploadthing** - Easy file handling
- **Vercel** - Deployment platform

---

## 💡 Future Enhancements

- [ ] Social sharing of streaks and achievements
- [ ] Habit reminders and notifications
- [ ] Advanced data export (CSV, PDF)
- [ ] Mobile app (React Native)
- [ ] Dark mode theme
- [ ] Habit templates/presets
- [ ] Leaderboards
- [ ] Community habits library
- [ ] Advanced analytics and reporting
- [ ] Integration with calendar apps

---

**Ready to build better habits? Start tracking today! 🚀**
