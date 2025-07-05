
# TaskFlow - Modern Task Management Application

A full-stack todo task management web application built with React, featuring social authentication, real-time collaboration, and a beautiful, responsive UI.

## 🚀 Features

### Core Functionality
- **Social Authentication**: Google OAuth integration with JWT-based session management
- **Task Management**: Full CRUD operations for tasks with status tracking
- **Real-time Updates**: Live collaboration features (WebSocket integration ready)
- **Task Sharing**: Share tasks with team members via email/username
- **Smart Filtering**: Filter tasks by status, priority, and due dates
- **Responsive Design**: Optimized for desktop and mobile devices

### User Experience
- **Modern UI/UX**: Clean, intuitive interface with smooth animations
- **Priority Management**: Color-coded priority levels (High, Medium, Low)
- **Status Tracking**: Visual status indicators (Todo, In Progress, Completed)
- **Search Functionality**: Quick task search and filtering
- **Toast Notifications**: Real-time feedback for user actions

## 🛠 Tech Stack

### Frontend
- **React 18** with TypeScript
- **Vite** for fast development and building
- **Tailwind CSS** for styling
- **Shadcn/UI** for component library
- **React Router** for navigation
- **React Query** for state management and API calls
- **Lucide React** for icons

### Backend Integration Ready
- **Supabase** integration for authentication, database, and real-time features
- **RESTful API** architecture
- **JWT** authentication
- **PostgreSQL** database support

## 🎨 Design System

### Color Palette
- Primary: Blue gradient (#3B82F6 to #1D4ED8)
- Secondary: Subtle grays and whites
- Status Colors: Green (completed), Blue (in-progress), Orange (todo)
- Priority Colors: Red (high), Yellow (medium), Green (low)

### Typography
- Font Family: Inter (system fonts fallback)
- Clear hierarchy with varied font weights
- Optimized for readability across devices

## 📁 Project Structure

```
src/
├── components/
│   ├── auth/
│   │   └── AuthModal.tsx          # Authentication modal
│   ├── tasks/
│   │   ├── TaskList.tsx           # Task list component
│   │   └── TaskForm.tsx           # Task creation/editing form
│   └── ui/                        # Shadcn/UI components
├── pages/
│   ├── Index.tsx                  # Landing page
│   ├── Dashboard.tsx              # Main dashboard
│   └── NotFound.tsx               # 404 page
├── hooks/
│   └── use-toast.ts               # Toast notification hook
├── lib/
│   └── utils.ts                   # Utility functions
└── App.tsx                        # Main app component
```

## 🔧 Setup Instructions

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd taskflow-app
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:8080`

### Environment Variables
For full functionality, you'll need to set up:
- `VITE_SUPABASE_URL` - Your Supabase project URL
- `VITE_SUPABASE_ANON_KEY` - Your Supabase anonymous key
- `VITE_GOOGLE_CLIENT_ID` - Google OAuth client ID

## 🚀 Deployment

### Frontend Deployment
- **Vercel**: Connect your GitHub repository for automatic deployments
- **Netlify**: Deploy via Git integration
- **Firebase Hosting**: Use Firebase CLI for deployment

### Backend Integration
- **Supabase**: Set up database, authentication, and real-time subscriptions
- **Database Schema**: User profiles, tasks, task sharing, and activity logs

## 📋 Assumptions & Decisions

1. **Authentication**: Google OAuth is the primary authentication method (GitHub and Facebook can be added)
2. **Database**: Tasks are stored with user relationships and sharing capabilities
3. **Real-time**: WebSocket integration ready for live collaboration
4. **Mobile-first**: Responsive design optimized for mobile devices
5. **Performance**: Lazy loading and optimized rendering for large task lists

## 🎯 Future Enhancements

- [ ] WebSocket integration for real-time updates
- [ ] Drag-and-drop task management
- [ ] File attachments for tasks
- [ ] Team workspaces and project organization
- [ ] Advanced filtering and sorting options
- [ ] Email notifications and reminders
- [ ] Offline support with sync capabilities
- [ ] Dark mode theme
- [ ] Analytics and productivity insights

## 🧪 Testing

```bash
# Run tests
npm run test

# Run tests with coverage
npm run test:coverage

# Run e2e tests
npm run test:e2e
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Shadcn/UI](https://ui.shadcn.com/) for the beautiful component library
- [Tailwind CSS](https://tailwindcss.com/) for the utility-first CSS framework
- [Lucide](https://lucide.dev/) for the icon library
- [Supabase](https://supabase.com/) for the backend infrastructure

---

**This project is a part of a hackathon run by https://www.katomaran.com**
