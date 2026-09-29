# TaskFlow - Task Management Web App

A responsive task management app (vanilla HTML, CSS, JavaScript).

## Run
Open `index.html` in a browser, or serve the folder: `python3 -m http.server 8000`.

Demo login: demo@taskflow.app / demo123

## Structure
- `index.html` - page shell
- `css/styles.css` - theme tokens (light/dark), layout, components
- `js/app.js` - views, routing, validation, event handling, and the `api` object

## Connect a backend
All CRUD goes through the `api` object in `js/app.js` (list, create, update, remove).
Replace each method with a fetch() call, e.g. `fetch('/api/tasks', {method:'POST', ...})`.
Auth is currently browser-only (localStorage, plain-text passwords) - replace with JWT/sessions and hashed passwords.
