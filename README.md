# apnoai-task-2-rushikesh

## React Developer Profile Card

A premium, professional, and fully functional React Developer Profile Card built as part of the ApnoAI Web Development Internship Task 2. This project demonstrates React 18 fundamentals, including functional components, props, hooks (useState), and modern glassmorphism UI design.

---

## 📖 Project Description

This project transforms a starter HTML file into a polished React Developer Profile Card featuring:

- A reusable `ProfileCard` component that accepts dynamic props
- Glassmorphism design with dark navy/purple gradient aesthetics
- Dark/Light mode toggle using React state
- Interactive Like counter with heart animation
- Skill badges, social links, and circular profile avatar
- Fully responsive layout for mobile, tablet, and desktop
- No build step required — runs directly via CDN

The component is designed to be easily customizable: update the profile data or swap the avatar image without touching the component logic.

---

## ✨ Features

- **Reusable ProfileCard Component** — accepts 8 props: name, role, bio, skills, avatar, github, linkedin, twitter
- **Glassmorphism UI** — transparent card with backdrop blur, gradient borders, and glowing accents
- **Dark/Light Mode Toggle** — switch themes interactively using React `useState`
- **Like Counter** — interactive heart button with click animation and persistent counter
- **Skill Badges** — stylized tag chips displaying developer skills
- **Social Links** — clickable GitHub, LinkedIn, and Twitter icons
- **Responsive Design** — works beautifully on mobile, tablet, and desktop screens
- **React 18** — uses `ReactDOM.createRoot` and modern hooks
- **CDN-Only** — no npm, no build step, no Node.js required
- **Beginner-Friendly Comments** — every concept is explained inline

---

## 🛠️ Technologies Used

- **React 18** — JavaScript library for building user interfaces
- **Tailwind CSS** — utility-first CSS framework for rapid UI styling
- **Google Fonts** — Inter font for professional typography
- **ReactDOM.createRoot** — React 18 root rendering
- **useState Hook** — state management for theme and like counter
- **JSX** — XML-like syntax for defining UI components

---

## 🎯 React Concepts Learned

1. **Functional Components** — `function ProfileCard({ name, role, ... })` — a reusable component function that accepts inputs as props

2. **Props** — properties passed from parent to child component to customize rendering. In this project:
   - `name` — displays the developer's full name
   - `role` — shows the professional role/title
   - `bio` — renders the developer biography
   - `skills` — an array displayed as skill badges
   - `avatar` — URL for the profile picture
   - `github`, `linkedin`, `twitter` — social media profile URLs

3. **useState Hook** — React's built-in hook for adding state to functional components:
   - `useState(0)` initializes a state variable with a default value
   - `const [likeCount, setLikeCount] = useState(0)` creates a counter state and its updater function
   - `useState(true)` manages dark/light mode toggle state
   - State updates trigger automatic re-renders with new UI

4. **Theme Toggle** — `setIsDarkMode(prev => !prev)` flips the boolean state, which recalculates CSS styles based on the current theme

5. **Like Counter** — `setLikeCount(prev => prev + 1)` increments the count on each click without a page refresh

6. **Reusable Components** — `ProfileCard` can be instantiated multiple times with different props, making it suitable for dashboards, portfolios, or user dashboards

---

## ▶️ How to Run the Project

Since this project uses CDN-based React (no build step), you can run it in any modern browser:

1. **Save the file** — keep the code as `index.html`
2. **Open in browser** — double-click `index.html` or drag it into any browser window
3. **No installation required** — all dependencies are loaded from CDNs

### For development with live reload:

If you want to use a local development server, you can use the `serve` package:

```bash
npm install -g serve
serve -s .
```

Then open `http://localhost:5000` in your browser.

### Or with Python's built-in server:

```bash
python3 -m http.server
```

Then open `http://localhost:8000` in your browser.

---

## 📦 GitHub Repository

**Repository:** `apnoai-task-2-rushikesh`

The complete project is available on GitHub. To run from the repository:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/apnoai-task-2-rushikesh.git
   ```

2. Navigate to the project folder:
   ```bash
   cd apnoai-task-2-rushikesh
   ```

3. Open `index.html` in your browser, or use a local server as described above.

---

## 🚀 Vercel Deployment

This project deploys directly to Vercel with the following configuration:

1. **Keep `index.html` in the repository root** — do not move or rename it
2. **Framework Preset: Other** — select "Other" as the framework preset in Vercel
3. **No build command** — leave the Build Settings empty (blank)
4. **No output directory** — leave the Output Directory field empty
5. **Deploy** — push to GitHub and connect to Vercel, or drag-and-drop the `index.html` folder

### Vercel Dashboard Settings:

- **Framework Preset:** Other
- **Build Command:** (leave blank)
- **Output Directory:** (leave blank)
- **Root Directory:** `.` (root)

### Deployment Steps:

1. Create a new repository on GitHub with the code
2. Go to Vercel and click "Add New Project"
3. Import the GitHub repository
4. In the settings, set Framework Preset to "Other"
5. Ensure Build Command and Output Directory are empty
6. Click "Deploy"
7. Once deployed, visit your Vercel preview URL

The deployed page will load the CDN-based React and Tailwind CSS exactly as the local development version.

---

## 👤 Author

**Rushikesh Gaiwal**
- GitHub: [@rushi380](https://github.com/rushi380)
- Role: Blockchain & Web3 Developer

---

## 📝 Commit Message

```
feat: build interactive React profile card with props and state
```