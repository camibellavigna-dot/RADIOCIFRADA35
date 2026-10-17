:root {
  color-scheme: dark;
  --background: #0a1115;
  --panel: #122128;
  --border: #29424a;
  --text: #e8f1f2;
  --muted: #91a8ad;
  --green: #7de6b2;
  --blue: #45b4d5;
}

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  background: var(--background);
  color: var(--text);
  font-family: Arial, sans-serif;
}

.topbar {
  padding: 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  border-bottom: 1px solid var(--border);
}

.topbar h1 {
  margin: 0;
  color: var(--green);
  font-size: 22px;
}

.topbar p,
.eyebrow,
.section-title {
  color: var(--muted);
  font-size: 11px;
  letter-spacing: 2px;
}

#status {
  color: var(--green);
  font-size: 11px;
}

main {
  max-width: 900px;
  padding: 20px;
  margin: auto;
}

.panel {
  padding: 22px;
  margin-bottom: 18px;
  border: 1px solid var(--border);
  border-radius: 15px;
  background: var(--panel);
}

.panel h2 {
  margin-top: 0;
}

.spectrum-box {
  padding: 12px;
  border: 1px solid var(--border);
  border-radius: 10px;
  background: #071013;
}

.section-title {
  display: flex;
  justify-content: space-between;
  gap: 8px;
}

canvas {
  display: block;
  width: 100%;
  height: 160px;
}

label {
  display: block;
  margin-top: 15px;
  color: var(--muted);
}

input {
  width: 100%;
  padding: 12px;
  margin-top: 7px;
  border: 1px solid var(--border);
  border-radius: 8px;
  background: #091317;
  color: white;
}

button {
  padding: 12px 15px;
  margin: 12px 5px 0 0;
  border: 1px solid var(--border);
  border-radius: 8px;
  background: #203840;
  color: white;
  font-weight: bold;
  cursor: pointer;
}

button:hover {
  border-color: var(--green);
}

button:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}

#uploadSong,
#loginForm button {
  background: var(--green);
  color: #092017;
}

audio {
  width: 100%;
  margin-top: 10px;
}

.note,
footer {
  color: var(--muted);
  font-size: 12px;
  line-height: 1.6;
}

footer {
  padding: 20px;
  text-align: center;
}

hr {
  border: 0;
  border-top: 1px solid var(--border);
  margin-top: 22px;
}

[hidden] {
  display: none !important;
}

@media (max-width: 600px) {
  .topbar {
    align-items: flex-start;
  }

  .panel {
    padding: 16px;
  }

  .topbar h1 {
    font-size: 18px;
  }
}
