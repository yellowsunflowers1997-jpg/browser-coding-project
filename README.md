# 💻 Browser Coding Environment

A fully-featured browser-based coding playground for learning and experimenting with web development. Write HTML, CSS, and JavaScript, and see live results instantly.

## ✨ Features

- **Three Code Editors**: Separate sections for HTML, CSS, and JavaScript
- **Live Preview**: See your code execute in real-time with an embedded preview iframe
- **Console Output**: View console logs, errors, and warnings from your JavaScript code
- **Dark Mode**: Toggle between light and dark themes for comfortable coding
- **Auto-Save**: Your code is automatically saved to browser's local storage
- **Copy to Clipboard**: Quick copy buttons for each code section
- **Download HTML**: Export your complete code as a standalone HTML file
- **Tab-Based Interface**: Easy navigation between editors and preview
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Keyboard Shortcuts**: Press Ctrl/Cmd + Enter to run your code

## 🚀 Getting Started

1. Open `index.html` in your web browser
2. Start writing HTML, CSS, and JavaScript in the respective editors
3. Click "Run Code" or use Ctrl/Cmd + Enter to execute
4. View your results in the Preview tab
5. Check the Console Output for any messages or errors

## 📁 Project Structure

```
browser-coding-project/
├── index.html      # Main HTML file with the editor interface
├── styles.css      # Complete styling for the environment
├── script.js       # JavaScript functionality and interactivity
└── README.md       # Documentation (this file)
```

## 🎯 Suggested Use Cases

- **Learning**: Perfect for beginners to practice HTML, CSS, and JavaScript
- **Prototyping**: Quickly test ideas without setting up a development environment
- **Teaching**: Great tool for educators to demonstrate web concepts
- **Experimentation**: Play with web technologies and see results immediately
- **Code Snippets**: Test and refine code snippets before using them in projects

## 💡 Tips & Tricks

### Default Examples
- The environment comes with default HTML, CSS, and JavaScript examples
- Use the "Reset" button to restore these defaults anytime

### Saving Your Work
- Your code is automatically saved to browser local storage
- To backup your work, use the "Download HTML" button

### Console Debugging
- Use `console.log()` to print messages to the Console Output
- Use `console.error()` or `console.warn()` for different message types
- Errors will also appear in the console automatically

### JavaScript Tips
- You can manipulate the DOM just like in regular web pages
- Use `document.querySelector()` to select elements
- Add event listeners to create interactive experiences
- The sandboxed iframe prevents code from affecting the main page

## 🎨 Customization

### Changing Default Code
Edit the `defaultCode` object in `script.js` to change the default HTML, CSS, or JavaScript.

### Modifying Themes
Edit the CSS variables in `styles.css` (`:root` selector) to customize colors:
```css
:root {
    --primary-color: #667eea;
    --secondary-color: #764ba2;
    /* ... other variables ... */
}
```

## 🌐 Browser Compatibility

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Any modern browser with ES6 support

## 📝 Example Projects

Try these simple projects to get started:

### 1. Personal Card
```html
<div class="card">
  <img src="profile.jpg" alt="Profile">
  <h1>Your Name</h1>
  <p>Web Developer</p>
  <button>Contact Me</button>
</div>
```

### 2. Interactive Counter
```html
<div>
  <p>Count: <span id="count">0</span></p>
  <button id="increment">+</button>
  <button id="decrement">-</button>
</div>
```

```javascript
let count = 0;
const countDisplay = document.getElementById('count');

document.getElementById('increment').addEventListener('click', () => {
  count++;
  countDisplay.textContent = count;
});

document.getElementById('decrement').addEventListener('click', () => {
  count--;
  countDisplay.textContent = count;
});
```

### 3. Todo List
```html
<div class="todo-app">
  <input type="text" id="todoInput" placeholder="Add a task...">
  <button id="addBtn">Add</button>
  <ul id="todoList"></ul>
</div>
```

```javascript
const input = document.getElementById('todoInput');
const addBtn = document.getElementById('addBtn');
const list = document.getElementById('todoList');

addBtn.addEventListener('click', () => {
  if (input.value.trim()) {
    const li = document.createElement('li');
    li.textContent = input.value;
    list.appendChild(li);
    input.value = '';
  }
});
```

## 🔒 Security

- Code runs in a sandboxed iframe with limited permissions
- Scripts cannot access the parent page or its data
- External resources can be loaded but will be restricted by CORS policies

## 🐛 Troubleshooting

### Preview Not Showing
- Make sure your HTML is valid
- Check the console for any JavaScript errors
- Click the "Refresh" button in the Preview tab

### Code Not Saving
- Ensure your browser allows local storage
- Check if you're in private/incognito mode
- Try clearing browser cache

### Errors in Console
- Click "Clear" to clear old messages
- Re-read error messages carefully for hints
- Check for typos in HTML element names or CSS classes

## 📜 License

This project is free to use and modify for educational purposes.

## 🤝 Feedback

Found a bug or have a suggestion? Feel free to open an issue or contribute!

---

**Happy Coding!** 🎉

Start experimenting and building amazing web projects right in your browser!
