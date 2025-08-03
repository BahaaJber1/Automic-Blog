# The Atomic Blog

A performant and interactive React blog app that demonstrates atomic state management using context and custom hooks. Users can add, search, and clear posts, toggle a fake dark mode, and import posts from a large archive. This project is designed to showcase advanced React patterns, including context providers, memoization, and optimization techniques.


<img width="1914" height="902" alt="image" src="https://github.com/user-attachments/assets/174d9a96-64db-4347-b22f-17518d5b87a4" />

<img width="1919" height="911" alt="image" src="https://github.com/user-attachments/assets/1a8adf9f-de2e-4711-9672-b366ef26e6fe" />

<img width="1919" height="904" alt="image" src="https://github.com/user-attachments/assets/b81a75f6-0a02-49cb-9dde-c696d8220a9d" />

<img width="1916" height="901" alt="image" src="https://github.com/user-attachments/assets/1ef0b55b-0d4a-47c3-a1aa-3e7b436cb33c" />

<img width="1917" height="905" alt="image" src="https://github.com/user-attachments/assets/1c848243-d78d-4698-b5ed-5d3339fe2286" />

<img width="1916" height="902" alt="image" src="https://github.com/user-attachments/assets/03909a6b-571f-4b3e-96f0-9efed114221f" />


---

## Features

- **Add Posts:** Create new posts with a title and body.
- **Search Posts:** Filter posts in real time using a search input.
- **Clear Posts:** Remove all posts with a single click.
- **Archive:** Browse and import from a massive archive of randomly generated posts.
- **Fake Dark Mode:** Toggle a dark mode for the UI.
- **Performance Optimizations:** Uses memoization and lazy initialization for large data sets.
- **Atomic State Management:** All post-related state and actions are managed via context and custom hooks.

---

## Technologies Used

- React (functional components, hooks)
- Context API for global state management
- Custom hooks for encapsulating logic
- Memoization (`React.memo`)
- [@faker-js/faker](https://github.com/faker-js/faker) for generating random post data
- Vite for fast development

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- [npm](https://www.npmjs.com/)

### Installation

1. Clone this repository or download the source code.
2. Navigate to the project directory:

   ```bash
   cd 12 automic-blog
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

### Running the App

Start the development server:

```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) (or the port shown in your terminal) in your browser.

---

## Project Structure

- `src/App.js` – Main application component and UI logic.
- `src/PostContext.js` – Context provider and custom hook for managing posts and actions.
- `src/Test.js` – (Optional) Component for testing context and state.
- `src/index.css` – App styles.

---

## Customization

- **Archive Size:** Change the number of archive posts in the `Archive` component.
- **Post Generation:** Edit the `createRandomPost` function to customize random post content.
- **Styling:** Update styles in `src/index.css` or add your own CSS modules.
- **Dark Mode:** The fake dark mode toggles a CSS class on the root element; you can expand this for a real dark mode.

---

## How It Works

- The app uses a context provider (`PostProvider`) to manage all post-related state and actions.
- Components consume context via the `usePosts` custom hook.
- The archive uses lazy initialization to efficiently generate a large number of posts only once.
- Memoization (`React.memo`) is used for the main content to avoid unnecessary re-renders.
- The fake dark mode toggles a CSS class on the root HTML element.

---

## License

This project is for educational purposes only.

---
