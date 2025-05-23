## Name:Archana
## Reg no:212222240011
## React Router DOM Project
This is a simple React application demonstrating routing using React Router DOM (v6). It includes basic navigation between Home, About, and Contact pages using the <BrowserRouter>.

## 📁 Project Structure
my-app/ ├── public/ │ └── index.html ├── src/ │ ├── components/ │ │ ├── Home.js │ │ ├── About.js │ │ ├── Contact.js │ │ └── Navbar.js │ ├── App.js │ └── index.js ├── package.json └── README.md

## Getting Started
Install dependencies
npm install
## Start the development server
npm start
This will start the app on http://localhost:3000.

## 📦 Dependencies
->React

->React DOM

->React Router DOM

## 🔗 Navigation
Implemented using react-router-dom@6:

/ – Home page

/about – About page

/contact – Contact page

🧱 Key Features
Single Page Application (SPA)

Route-based code separation

Reusable Navbar component

Clean and responsive UI

## 🛠️ Scripts
npm start       # Runs the app in development mode

npm run build   # Builds the app for production

## program:
## index.jsx
```
import React from 'react';
import ReactDOM from 'react-dom/client';
import App from './App';
import { BrowserRouter } from 'react-router-dom';

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <BrowserRouter>
    <App />
  </BrowserRouter>
);

```

app.jsx
```
import React from 'react';
import { Routes, Route, Link } from 'react-router-dom';
import Home from './home';
import About from './about';
import Contact from './contact';
import './App.css';

function App() {
  return (
    <div>
      <nav className="navbar">
        <Link to="/">Home</Link>
        <Link to="/about">About</Link>
        <Link to="/contact">Contact</Link>
      </nav>

      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/about" element={<About />} />
        <Route path="/contact" element={<Contact />} />
      </Routes>
    </div>
  );
}

export default App;
```
contact.jsx
```
import React from 'react';

function Contact() {
  return <h2>This is the Contact Page</h2>;
}

export default Contact;
```
about.jsx
```
import React from 'react';

function About() {
  return <h2>About Us</h2>;
}

export default About;
```
home.jsx
```import React from 'react';

function Home() {
  return <h2>This is the Home Page</h2>;
}

export default Home;
```
## output:
![image](https://github.com/user-attachments/assets/2aa91e83-2254-42f3-b920-90df05aa89c2)
![image](https://github.com/user-attachments/assets/b6dffe81-e3bb-4d79-b414-5dfdfc9154be)
![image](https://github.com/user-attachments/assets/86ff0fcd-186d-459f-b75d-6ada20849b22)


