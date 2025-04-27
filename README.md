
# 🌍 Bookmark & Hotel Finder App

A modern travel assistant web application built with **React**, **TypeScript**, **React Router**, and **Context API**, designed to help users discover and save interesting locations and accommodations with ease. Featuring an interactive map and real-time hotel search.

---

## ✨ Key Features

- 🗺️ Bookmark real-world locations using reverse geolocation
- 🧭 Browse and highlight bookmarked cities on a map
- 📍 Country flags and geodata rendered with `react-country-flag`
- 🔄 Live search for hotels with date and guest filtering
- 🏨 View hotels by location using coordinates and `searchParams`
- 🧠 Global state management via `useReducer` + `Context API`
- 🔐 Simple authentication system using `useReducer`
- 📦 JSON Server used as a mock backend

---




## 📸 Preview
 

[![Video Preview](https://img.youtube.com/vi/VIDEO_ID/maxresdefault.jpg)](src/video/TravelBook_V1.mp4)

![Rick and Morty App Screenshot](https://i.postimg.cc/qB3MjYyf/Screenshot-280.png)


![Rick and Morty App Screenshot](https://i.postimg.cc/C57vG0Cy/Screenshot-286.png)

![Rick and Morty App Screenshot](https://i.postimg.cc/RFYMdrvY/Screenshot-22233.png)




---

## 🧰 Tech Stack

| Technology       | Description                               |
|------------------|-------------------------------------------|
| **React**        | UI library with modern Hooks architecture |
| **TypeScript**   | Static typing and type safety             |
| **React Router** | SPA routing and query param management    |
| **Context API**  | Global state without prop drilling        |
| **Axios**        | HTTP client for data fetching             |
| **React Icons**  | Beautiful icon pack for UI elements       |
| **React Date Range** | Date picker with calendar integration  |
| **Toast**        | For error and success feedback            |
| **JSON Server**  | Local mock API server                     |

---

## 🏗️ Architecture & Best Practices

### ✅ Functional Components & Hooks
All components are functional and use modern hooks like `useState`, `useEffect`, `useRef`, `useContext`, `useReducer`.

### ✅ Custom Hooks
- `useOutsideClick` – closes dropdowns when clicking outside
- `useUrlLocation` – extracts latitude/longitude from query params
- `useFetch` – custom data fetching hook

### ✅ Separation of Logic and UI
Logic (like booking, searching, or fetching data) is handled inside context or hooks, while UI remains declarative and clean.

### ✅ Global State Management
Used `useReducer` for managing bookmark, hotel, and auth states inside their respective `ContextProvider` files.

---

## 📁 Folder Structure

```bash
src/
├── components/
│   ├── Bookmark/
│   ├── Hotels/
│   ├── Header/
│   ├── Layout/
│   ├── Loader/
│   └── Map/
├── context/
│   ├── BookmarkListContext.tsx
│   ├── HotelsProvider.tsx
│   └── AuthProvider.tsx
├── hooks/
│   ├── useOutsideClick.ts
│   ├── useUrlLocation.ts
│   └── useFetch.ts
├── App.tsx
├── main.tsx
└── index.css
```

---

## 🚀 Getting Started

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/bookmark-hotel-finder.git
cd bookmark-hotel-finder

# 2. Install dependencies
npm install

# 3. Start the JSON server
npx json-server --watch db.json --port 5000

# 4. Run the app
npm run dev
```

Visit: [http://localhost:5173](http://localhost:5173)

---

## 📜 License

MIT License. Feel free to use and modify for your own projects.

> Built with ❤️ by Kasra using React + TypeScript + Context API
