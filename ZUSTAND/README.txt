# What is Zustand?

Zustand is a lightweight state management library for React that helps manage and share state across components without prop drilling.

It uses hooks and provides a simple way to create a global store.

## Key Features

- Lightweight and fast
- Minimal boilerplate
- No Provider required
- Uses React hooks
- Supports TypeScript
- Easy to learn compared to Redux

# Installation

## npm install zustand

# Example

import { create } from "zustand";

const useStore = create((set) => ({
  count: 0,
  increment: () =>
    set((state) => ({
      count: state.count + 1,
    })),
}));


# Using the store:

function Counter() {
  const count = useStore((state) => state.count);
  const increment = useStore((state) => state.increment);

  return (
    <div>
      <h1>{count}</h1>
      <button onClick={increment}>Increment</button>
    </div>
  );
}

# Why Use Zustand?

## Without Zustand:

App
 ├── Parent
 │    └── Child
 │         └── GrandChild


 You may need to pass props through multiple components (prop drilling).

# With Zustand:

Global Store
     ↑
Any Component can access state directly

