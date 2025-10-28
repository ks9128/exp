# Web Exercises — Experiments

This file lists the experiments with copy-paste-ready code and concise, practical steps. Click an experiment link to jump to it.

- [Exp 1 — Aim: Identify and apply the appropriate HTML tags to develop a webpage](#exp-1)
- [Exp 2 — Aim: To identify and apply the appropriate CSS tags in order to format the data on a webpage](#exp-2)
- [Exp 4 — Aim: To construct a frontend application using React (Simple To-Do List App) using Vite](#exp-4)
- [Exp 5 — Aim: To construct a backend using node.js/express](#exp-5)
- [Exp 6 — Aim: To use javascript to develop interactive webpages (Simple Unit Converter)](#exp-6)
- [Exp 7 — Aim: To design and simulate the environment for dynamic routing using Cisco Packet Tracer](#exp-7)
- [Exp 8 — Aim: To design and simulate VLAN /WLAN on switch/router using Cisco Packet Tracer](#exp-8)

---

<a id="exp-1"></a>

## Exp 1 — Aim: Identify and apply the appropriate HTML tags to develop a webpage

Save the following as `profile.html` and open it in your browser.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <title>My Profile — Arjun Sharma</title>
  </head>
  <body>
    <header>
      <h1>Welcome to My Profile</h1>
      <p>Hello! I am Arjun Sharma, a passionate Computer Science student.</p>
    </header>

    <main>
      <section aria-labelledby="about-heading">
        <h2 id="about-heading">About Me</h2>
        <p><strong>Name:</strong> Arjun Sharma</p>
        <p><strong>DOB:</strong> 06/02/2000</p>
        <p>
          <strong>LinkedIn:</strong>
          <a
            href="https://www.linkedin.com/in/arjunsharma-cs"
            target="_blank"
            rel="noopener noreferrer"
            >Visit My Profile</a
          >
        </p>
      </section>

      <section aria-labelledby="qual-heading">
        <h2 id="qual-heading">Qualification</h2>
        <p>Pursuing B.Tech in Computer Science from Zenith University</p>
        <p>The Global School — 12th Grade</p>
        <p>City Public Academy — 10th Grade</p>
      </section>

      <section aria-labelledby="leisure-heading">
        <h2 id="leisure-heading">Leisure Activities</h2>
        <ol type="A">
          <li>Competitive Programming in Python</li>
          <li>Reading books on Artificial Intelligence</li>
          <li>Developing personal projects in C++</li>
        </ol>
      </section>

      <section aria-labelledby="future-heading">
        <h2 id="future-heading">Future Plans</h2>
        <ul>
          <li>Interested in pursuing M.Tech in Data Science</li>
          <li>Aspiring for a PhD in Robotics and Computer Vision</li>
          <li>
            Aiming to become a Lead Software Architect at a top-tier tech firm
          </li>
        </ul>
      </section>
    </main>

    <footer>
      <p>&copy; 2025 Arjun Sharma. All rights reserved.</p>
    </footer>
  </body>
</html>
```

---

<a id="exp-2"></a>

## Exp 2 — Aim: To identify and apply the appropriate CSS tags in order to format the data on a webpage

Save as `profile-styled.html` and open in a browser.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <title>My Profile — Arjun Sharma</title>
    <style>
      :root {
        --accent: #cc0000;
        --bg: #f0f0f5;
        --text: #222;
      }
      * {
        box-sizing: border-box;
      }
      body {
        font-family: Inter, Arial, sans-serif;
        margin: 0;
        padding: 0;
        background: var(--bg);
        color: var(--text);
      }
      header {
        background: var(--accent);
        color: #fff;
        padding: 28px 16px;
        text-align: center;
      }
      main {
        max-width: 900px;
        margin: 20px auto;
        padding: 0 16px;
      }
      section {
        background: #fff;
        border: 2px solid var(--accent);
        padding: 16px;
        margin-bottom: 18px;
        border-radius: 8px;
      }
      a {
        color: var(--accent);
        text-decoration: none;
      }
      a:hover {
        text-decoration: underline;
      }
      ol,
      ul {
        padding-left: 1.2rem;
      }
      footer {
        text-align: center;
        padding: 12px;
        background: var(--accent);
        color: #fff;
        margin-top: 20px;
      }
      @media (max-width: 560px) {
        header {
          padding: 18px;
        }
        section {
          padding: 12px;
        }
      }
    </style>
  </head>
  <body>
    <header>
      <h1>Welcome to My Profile</h1>
    </header>

    <main>
      <section>
        <h2>About Me</h2>
        <p><strong>Name:</strong> Arjun Sharma</p>
        <p><strong>DOB:</strong> 11/12/2004</p>
        <p>
          <strong>LinkedIn:</strong>
          <a
            href="https://www.linkedin.com/in/arjunsharma-cs"
            target="_blank"
            rel="noopener noreferrer"
            >Visit My Profile</a
          >
        </p>
      </section>

      <section>
        <h2>Qualification</h2>
        <p>Pursuing B.Tech in Computer Science from Zenith University</p>
        <p>The Global School — 12th Grade</p>
        <p>City Public Academy — 10th Grade</p>
      </section>

      <section>
        <h2>Leisure Activities</h2>
        <ol type="A">
          <li>Competitive Programming in Python</li>
          <li>Reading books on Artificial Intelligence</li>
          <li>Developing personal projects in C++</li>
        </ol>
      </section>

      <section>
        <h2>Future Plans</h2>
        <ul>
          <li>Interested in pursuing M.Tech in Data Science</li>
          <li>Ambitious for a PhD in Robotics and Computer Vision</li>
          <li>
            Aiming for a position as a Lead Software Architect at a top-tier
            tech firm
          </li>
        </ul>
      </section>
    </main>

    <footer>&copy; 2025 Arjun Sharma. All rights reserved.</footer>
  </body>
</html>
```

---

<a id="exp-4"></a>

## Exp 4 — Aim: To construct a frontend application using React (Simple To-Do List App) using Vite

Use Vite (fast and simple). From your chosen project folder open a terminal (PowerShell) and run:

```powershell
npm create vite@latest todo-app -- --template react
cd todo-app
npm install
npm run dev
```

Open `src/App.jsx` and replace its contents with the code below (copy-paste-ready).

`src/App.jsx`:

```jsx
import { useState } from "react";

export default function App() {
  const [tasks, setTasks] = useState([]);
  const [newTask, setNewTask] = useState("");

  const addTask = () => {
    if (newTask.trim() === "") return;
    setTasks((prev) => [...prev, { text: newTask.trim(), completed: false }]);
    setNewTask("");
  };

  const toggleTask = (index) => {
    setTasks((prev) =>
      prev.map((t, i) => (i === index ? { ...t, completed: !t.completed } : t))
    );
  };

  const deleteTask = (index) => {
    setTasks((prev) => prev.filter((_, i) => i !== index));
  };

  return (
    <div style={styles.container}>
      <h1 style={styles.heading}>Simple Todo App</h1>
      <div style={styles.inputContainer}>
        <input
          type="text"
          value={newTask}
          placeholder="Enter a new task..."
          onChange={(e) => setNewTask(e.target.value)}
          style={styles.input}
          onKeyDown={(e) => e.key === "Enter" && addTask()}
        />
        <button onClick={addTask} style={styles.addButton}>
          Add
        </button>
      </div>

      <ul style={styles.list}>
        {tasks.map((task, index) => (
          <li key={index} style={styles.listItem}>
            <span
              onClick={() => toggleTask(index)}
              style={{
                textDecoration: task.completed ? "line-through" : "none",
                cursor: "pointer",
              }}
            >
              {task.text}
            </span>
            <button
              onClick={() => deleteTask(index)}
              style={styles.deleteButton}
              aria-label={`Delete ${task.text}`}
            >
              ✖
            </button>
          </li>
        ))}
      </ul>
    </div>
  );
}

const styles = {
  container: {
    textAlign: "center",
    marginTop: 50,
    fontFamily: "Arial, sans-serif",
  },
  heading: { color: "#333" },
  inputContainer: { marginBottom: 20 },
  input: { padding: 10, width: 240, marginRight: 10 },
  addButton: {
    padding: "10px 20px",
    backgroundColor: "green",
    color: "white",
    border: "none",
    cursor: "pointer",
  },
  list: { listStyle: "none", padding: 0 },
  listItem: {
    display: "flex",
    justifyContent: "center",
    alignItems: "center",
    margin: "8px 0",
    gap: 8,
  },
  deleteButton: {
    marginLeft: 8,
    backgroundColor: "red",
    color: "white",
    border: "none",
    cursor: "pointer",
    padding: "4px 8px",
  },
};
```

Notes:

- Vite serves the app on a development server (usually `http://localhost:5173`).
- Paste code into `src/App.jsx` (Vite React template uses `.jsx`).

---

<a id="exp-5"></a>

## Exp 5 — Aim: To construct a backend using node.js/express

Simple steps (assumes you already opened the project folder in VS Code):

1. Open a terminal in the project folder.
2. Initialize and install dependencies:

```powershell
npm init -y
npm install express morgan cors dotenv
```

3. Create a file named `server.js` and paste the code below.

`server.js`:

```js
require("dotenv").config();
const express = require("express");
const morgan = require("morgan");
const cors = require("cors");
const app = express();

app.use(express.json());
app.use(morgan("dev"));
app.use(cors());

app.get("/", (req, res) => {
  res.json({ message: "Hello, Node.js backend!" });
});

const PORT = process.env.PORT || 4000;
app.listen(PORT, () => {
  console.log(`Server running on http://localhost:${PORT}`);
});
```

4. Start the server:

```powershell
node server.js
```

Open `http://localhost:4000/` in a browser to verify.

---

<a id="exp-6"></a>

## Exp 6 — Aim: To use javascript to develop interactive webpages (Simple Unit Converter)

Save as `unit-converter.html` and open in your browser.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Simple Unit Converter</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        padding: 20px;
      }
      label,
      select,
      input {
        margin: 10px 0;
        display: block;
      }
      #result {
        font-size: 20px;
        margin-top: 20px;
      }
    </style>
  </head>
  <body>
    <h2>Simple Length Unit Converter</h2>
    <label for="inputValue">Value:</label>
    <input id="inputValue" type="number" placeholder="Enter value" />
    <label for="fromUnit">From:</label>
    <select id="fromUnit">
      <option value="meters">Meters</option>
      <option value="kilometers">Kilometers</option>
      <option value="miles">Miles</option>
      <option value="feet">Feet</option>
    </select>
    <label for="toUnit">To:</label>
    <select id="toUnit">
      <option value="meters">Meters</option>
      <option value="kilometers">Kilometers</option>
      <option value="miles">Miles</option>
      <option value="feet">Feet</option>
    </select>
    <button onclick="convert()">Convert</button>
    <div id="result">Result: -</div>

    <script>
      const rates = {
        meters: 1,
        kilometers: 1000,
        miles: 1609.34,
        feet: 0.3048,
      };
      function convert() {
        const input = parseFloat(document.getElementById("inputValue").value);
        if (isNaN(input)) {
          document.getElementById("result").innerText =
            "Result: Please enter a valid number";
          return;
        }
        const fromUnit = document.getElementById("fromUnit").value;
        const toUnit = document.getElementById("toUnit").value;
        const valueInMeters = input * rates[fromUnit];
        const convertedValue = valueInMeters / rates[toUnit];
        document.getElementById(
          "result"
        ).innerText = `Result: ${convertedValue.toFixed(4)} ${toUnit}`;
      }
    </script>
  </body>
</html>
```

---

## Quick commands (PowerShell)

- Create a Vite React app:

```powershell
npm create vite@latest todo-app -- --template react
cd todo-app
npm install
npm run dev
```

- Initialize Node backend and run server (in project folder):

```powershell
npm init -y
npm install express morgan cors dotenv
node server.js
```

---

If you'd like, I can now create the individual files directly in this workspace (`profile.html`, `profile-styled.html`, `unit-converter.html`, and `server.js`) and/or add localStorage to the Vite todo app. Which would you like next?

---

## Exp 7 — Aim: To design and simulate the environment for dynamic routing using Cisco Packet Tracer

<a id="exp-7"></a>

Files provided: `exp7_dynamic_routing.pkt` (Packet Tracer file).

Quick use: download `exp7_dynamic_routing.pkt`, open it in Cisco Packet Tracer and run the simulation or use the router CLI to test connectivity.

---

## Exp 8 — Aim: To design and simulate VLAN /WLAN on switch/router using Cisco Packet Tracer

<a id="exp-8"></a>

Files provided: `exp8_vlan_wlan.pkt` (Packet Tracer file).

Quick use: download `exp8_vlan_wlan.pkt`, open it in Cisco Packet Tracer and run the simulation or verify VLAN/WLAN behavior with the client devices.
