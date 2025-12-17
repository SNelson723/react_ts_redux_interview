# React Technical Interview: Task Manager

**Tech Stack:** React 18 + Vite + TypeScript + Redux Toolkit + Axios + Tailwind CSS  
**Time:** 60 minutes

---

## Setup (2 minutes)

1. Clone the repository (starts with empty React + Vite + TypeScript app)
2. `npm install @reduxjs/toolkit react-redux axios`
3. `npm run dev`

**API Details** (provided during interview):

- Endpoint URL
- Authorization token

**API Response Structure:**

```ts
// GET /api/tasks
{
  data: Task[],
  total: number
}

// Task shape:
interface Task {
  id: string;
  title: string;
  description?: string;
  completed: boolean;
  createdAt: string;
}

// POST/PUT body
{
  title: string;
  description?: string;
  completed: boolean;
}

// DELETE body
{
  id: number
}
```

### Requirements

1. Redux store (`@reduxjs/toolkit`) with typed hooks (`useAppSelector`, `useAppDispatch`)
2. `tasksSlice` for state management (loading, error, tasks)
3. CRUD operations via Axios thunks
4. Client-side search/filter

### Bonus

- Explicit typing
- Responsive Tailwind UI
- Error handling + loading states
- Clean architecture

### Submission

**Live coding exercise** - evaluated in real-time.  
Follow-up questions upon completion.
