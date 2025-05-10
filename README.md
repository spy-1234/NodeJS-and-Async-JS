# 🚀 30 Days of Full Stack Development Challenge

## 📅 Day 1 – Asynchronous JavaScript & Node.js Basics

### 🔍 Topics Covered

- ✅ Synchronous vs Asynchronous File Reading using `fs`
  - `fs.readFileSync()` vs `fs.readFile()`
- 🔄 Callback Hell Explained
  - Converted nested callbacks into Promise chains
- 🌐 Promises & Async/Await
  - `.then()` chaining
  - Cleaner structure using `async/await`
- 🛠️ Utility Functions Created
  - `delay(ms)` – Promisified timeout
  - `promisifiedFetch(url)` – Clean API calls
  - `readFilePromisified(path)` – Async file reading
  - Bonus: Manual Promise wrapping using `fs.readFile`

### 📁 Code Snippets

```js
// Promisified setTimeout
function delay(ms) {
  return new Promise(resolve => setTimeout(resolve, ms));
}

// Promisified file read
const fs = require('fs').promises;

async function readFilePromisified(path, encoding = 'utf8') {
  return fs.readFile(path, encoding);
}
