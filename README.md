# 🌟 OvarlayComp

**OvarlayComp** is a smooth, animated overlay component built with **React**, **Tailwind CSS**, and **GSAP**. It provides a plug-and-play solution for modals, popups, or fullscreen animated overlays in your app.

## ✨ Features

- ⚡ GSAP-powered animations
- 🎨 Styled with Tailwind CSS
- ⚛️ Easy integration with any React project
- 🧩 Simple and flexible usage
- 🧘‍♂️ Clean exit and enter transitions

## 🚀 Installation

Using **npm**:

```bash
npm install ovarlaycomp
````

Using **bun**:

```bash
bun add ovarlaycomp
```

Or with **yarn**:

```bash
yarn add ovarlaycomp
```

## 🧑‍💻 Usage

```jsx
import { OvarlayComp } from "ovarlaycomp";

function App() {
  const [isOpen, setIsOpen] = useState(false);

  return (
    <>
      <button onClick={() => setIsOpen(true)} className="btn">
        Open Overlay
      </button>

      <OvarlayComp isOpen={isOpen} onClose={() => setIsOpen(false)}>
        <div className="p-6 bg-white rounded-xl shadow-xl text-center">
          <h1 className="text-2xl font-bold mb-4">Hello 👋</h1>
          <p>This is an animated overlay using GSAP + Tailwind!</p>
          <button onClick={() => setIsOpen(false)} className="mt-4 btn">
            Close
          </button>
        </div>
      </OvarlayComp>
    </>
  );
}
```

## ⚙️ Props

| Prop       | Type        | Required | Description                            |
| ---------- | ----------- | -------- | -------------------------------------- |
| `isOpen`   | `boolean`   | ✅        | Toggle to show/hide the overlay        |
| `onClose`  | `function`  | ✅        | Callback fired when overlay closes     |
| `children` | `ReactNode` | ✅        | The content to show inside the overlay |

## 🧪 Tech Stack

* **React**
* **Tailwind CSS**
* **GSAP (GreenSock Animation Platform)**

## 🧩 Example Use Cases

* Modals
* Lightboxes
* Onboarding Screens
* Fullscreen Notices

## 📜 License

MIT © 2025

---

> Built for developers who love clean UI and smooth motion.



