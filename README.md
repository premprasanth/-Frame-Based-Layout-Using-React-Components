# React Lab Exercise 7: Frame-Based Layout Using React Components 
## Name: PREM PRASANTH J
## Roll no: 2305001028
## Department: CSE

## AIM
### To develop a simple frame-based webpage layout using React components, consisting of a Header, Sidebar, Content area, and Footer.

## PROGRAM
### i) Header.jsx
```py
function Header() {
return (
<header className="header">
<h1>Student Management System</h1>
</header>
);
}
export default Header;
```
### ii) Sidebar.jsx
```py
function Sidebar() {
return (
<aside className="sidebar">
<h3>Menu</h3>
<ul>
<li>Home</li>
<li>Students</li>
<li>Courses</li>
<li>Contact</li>
</ul>
</aside>
);
}
export default Sidebar;
```
### iii) Content.jsx
```py
function Content() {
return (
<main className="content">
<h2>Welcome to Student Management System</h2>
<p>
This is the main content area of the React application.
</p>
<p>
React components can be arranged together to create
different webpage layouts.
</p>
</main>
);
}
export default Content;
```
### iv) Footer.jsx
```py
function Footer() {
return (
<footer className="footer">
<p>© 2026 Student Management System</p>
</footer>
);
}export default Footer;
```
### v) App.jsx
```py
import Header from "./components/Header";
import Sidebar from "./components/Sidebar";
import Content from "./components/Content";
import Footer from "./components/Footer";
import "./App.css";
function App() {
return (
<div className="app">
<Header />
<div className="main">
<Sidebar />
<Content />
</div>
<Footer />
</div>
);
}
export default App;
vi) App.css
* {
box-sizing: border-box;
}
body {
margin: 0;
font-family: Arial, sans-serif;
}
.app {
min-height: 100vh;
display: flex;
flex-direction: column;
}
.header {
background-color: #1976d2;
color: white;
padding: 20px;
text-align: center;
}
.main {
display: flex;
flex: 1;
min-height: 400px;
}
.sidebar {
width: 220px;
flex-shrink: 0;
background-color: #eeeeee;
padding: 20px;
}
.sidebar ul {
list-style: none;
padding: 0;
}
.sidebar li {
padding: 12px;
margin-bottom: 5px;
cursor: pointer;
}
.sidebar li:hover {
background-color: #d0d0d0;
}
.content {
flex: 1;
padding: 30px;
}
.content h2 {
color: #1976d2;
}
.footer {
background-color: #333333;
color: white;
text-align: center;
padding: 15px;
}
@media (max-width: 600px) {
.main {
flex-direction: column;
}
.sidebar {
width: 100%;
}
.content {
padding: 20px;
}
}
```
## OUTPUT
<img width="1125" height="653" alt="image" src="https://github.com/user-attachments/assets/4ca37265-623f-4b0e-8fb8-f328b67993e7" />

## RESULT
### Thus, a frame-based webpage layout was successfully created using React components and CSS Flexbox. The application contains separate Header, Sidebar, Content, and Footer components arranged into a complete webpage layout.
