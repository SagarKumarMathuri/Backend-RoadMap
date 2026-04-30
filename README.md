# Lucide React Setup Guide

A complete guide to using **Lucide React** icons in modern React projects.

---

## 🚀 What is Lucide React?

**Lucide React** is a beautiful and lightweight open-source icon library for React applications.

It provides:

* Clean SVG icons
* Fully customizable size and color
* Tree-shakable imports
* Great for React + Next.js + Vite projects

---

## 📦 Installation

Using npm:

```bash
npm install lucide-react
```

Using yarn:

```bash
yarn add lucide-react
```

Using pnpm:

```bash
pnpm add lucide-react
```

---

## 📁 Project Structure

```bash
src/
 ├── App.jsx
 ├── components/
 │    └── Navbar.jsx
 └── main.jsx
```

---

## 🧠 Basic Usage

```jsx
import { Home } from "lucide-react";

function App() {
  return (
    <div>
      <Home />
    </div>
  );
}

export default App;
```

---

## 🎨 Customize Icons

```jsx
import { User } from "lucide-react";

function App() {
  return (
    <User size={40} color="blue" strokeWidth={1.5} />
  );
}
```

### Props

| Prop        | Description      |
| ----------- | ---------------- |
| size        | Icon size        |
| color       | Icon color       |
| strokeWidth | Border thickness |

---

## 🔥 Multiple Icons Example

```jsx
import { Home, User, Settings, Search } from "lucide-react";

function App() {
  return (
    <div>
      <Home />
      <User />
      <Settings />
      <Search />
    </div>
  );
}
```

---

## 🌙 Navbar Example

```jsx
import { Home, User, Menu } from "lucide-react";

function Navbar() {
  return (
    <nav>
      <Home />
      <User />
      <Menu />
    </nav>
  );
}

export default Navbar;
```

---

## ⚡ Tailwind CSS Example

```jsx
import { Moon } from "lucide-react";

function DarkModeBtn() {
  return (
    <button className="p-2 bg-black text-white rounded">
      <Moon className="w-5 h-5" />
    </button>
  );
}
```

---

## 💼 Real Project Use Cases

* Sidebar menus
* Dashboard icons
* Profile buttons
* Search bars
* Dark mode toggle
* Notifications
* Settings page

---

## 📌 Best Practices

✅ Import only required icons

```jsx
import { Home } from "lucide-react";
```

❌ Avoid importing all icons

```jsx
import * as Icons from "lucide-react";
```

---

## 🌐 Popular Icons

* Home
* User
* Search
* Bell
* Settings
* Moon
* Sun
* Menu
* Trash
* Edit

---

## 🛠 Example Dashboard Card

```jsx
import { Users } from "lucide-react";

function Card() {
  return (
    <div>
      <Users />
      <h2>Total Users</h2>
      <p>1,250</p>
    </div>
  );
}
```

---

## 📚 Official Website

https://lucide.dev

---

## 🤝 Contributing

Pull requests are welcome.

---

## 📄 License

MIT License

---

## ⭐ Support

If you found this useful, give the repository a star ⭐
