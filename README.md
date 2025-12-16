Tech Stack
Frontend
React (Vite)
TypeScript
Tailwind CSS
React Query (Server‑state management)
React Hook Form + Zod
Socket.io Client
Features
- User authentication (Login & Register)
- Create, update, delete tasks
- Assign tasks to other users
- Real-time task updates (status, priority, assignee)
- Instant in-app notifications on task assignment
- Personal dashboard views:
  - Tasks assigned to me
  - Tasks created by me
  - Overdue tasks
- Filter tasks by status and priority
- Sort tasks by due date
- Skeleton loaders for smooth loading states
- Fully responsive, mobile-first UI
  Application Pages
- `/login` – User login
- `/register` – User registration
- `/dashboard` – User dashboard
- `/tasks` – Task list with filters & sorting
   Real-Time Functionality
- Socket.io listens for task update and assignment events
- UI updates instantly without page reload
- React Query cache invalidation ensures data consistency
   Project Structure
src/
├── api/ # API client & request handlers
├── components/ # Reusable UI components
├── hooks/ # Custom React Query hooks
├── pages/ # Route-level pages
├── socket/ # Socket.io client setup
├── App.tsx
└── main.tsx
Environment Variables
Create a .env file in the root directory:
VITE_API_URL=https://<your-backend-url>.onrender.com
Styling & UX
Tailwind CSS used for clean and consistent UI
Mobile-first responsive design
Skeleton loaders for improved user experience
Simple, intuitive task management interface
Build for Production
npm run build
Notes & Assumptions
Authentication handled via HttpOnly cookies from backend
No sensitive data stored on the frontend
Role-based access control not required as per assignment scope
Conclusion
This frontend application fully satisfies all UI, UX, and real-time requirements of the assignment and integrates seamlessly with the backend services.
https://<your‑frontend‑url>.vercel.app
Author: <pravallika akurathi>
