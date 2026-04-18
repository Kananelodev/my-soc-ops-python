🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# 🎯 Soc Ops

## Break the Ice, Get 5 in a Row

**Soc Ops** is a social bingo game designed to get people mingling at in-person events. Find people who match the questions, mark them off, and be the first to get 5 in a row—all while making genuine connections.

Perfect for **mixers, conferences, team retreats, and networking events**.

---

## ✨ Why Soc Ops?

| 🎮 | **Instant Fun** |
|----|----|
| Get people talking in seconds, not hours. No awkward small talk required. |

| 🤝 | **Genuine Connections** |
|----|----|
| Questions reveal shared interests: "speaks more than 2 languages," "has a hidden talent," "loves spicy food." Real conversations happen naturally. |

| ⚡ | **Quick to Play** |
|----|----|
| 5–10 minutes per round. Perfect for event intervals or as an icebreaker. |

| 🎯 | **Mobile-First** |
|----|----|
| Works on any device. Tap squares, mark them, and celebrate wins together. |

---

## 🚀 How It Works

1. **Join a game** → Everyone gets a unique 5×5 bingo board
2. **Mingle** → Find people who match the questions on your board
3. **Mark & Win** → Get 5 in a row (horizontally, vertically, or diagonally) to win
4. **Celebrate** → First to bingo wins! (And everyone makes new friends along the way)

---

## 💻 Tech Stack

Built with **Python 3.13+** for speed and reliability:

- **FastAPI** — Modern, fast web framework
- **HTMX** — Interactive experiences without writing JavaScript
- **Pydantic** — Type-safe data validation
- **Jinja2** — Template rendering

---

## 📚 Getting Started

### For Event Organizers

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-repo/soc-ops.git
   cd soc-ops
   ```

2. **Install dependencies**
   ```bash
   uv sync
   ```

3. **Run the server**
   ```bash
   soc-ops
   ```

4. **Open in your browser**
   ```
   http://localhost:8000
   ```

5. **Share the link** with your event attendees!

### For Developers & Workshop Learners

This is also a **GitHub Copilot learning lab** designed to teach modern Python development practices:

| Part | Topic |
|------|-------|
| [**00**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview) | Overview & Checklist |
| [**01**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=01-setup) | Setup & Context Engineering |
| [**02**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=02-design) | Design-First Frontend |
| [**03**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=03-quiz-master) | Custom Quiz Master |
| [**04**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=04-multi-agent) | Multi-Agent Development |

📝 **Offline reading:** Lab guides are also in the [`workshop/`](workshop/) folder.

---

## 🎲 Sample Questions

Our default bingo board includes real questions that spark conversations:

✨ *"speaks more than 2 languages"*  
🎭 *"has a hidden talent"*  
🌏 *"has lived in another country"*  
🍜 *"loves spicy food"*  
🎵 *"plays an instrument"*  
🐕 *"has a pet"*  
📚 *"has read a book this month"*  
✌️ *"can juggle"*  

...and 16 more!

---

## 🛠️ Customization

Want to customize the questions for your event? Edit [`app/data.py`](app/data.py):

```python
QUESTIONS: Final[list[str]] = [
    "your custom question here",
    "another great icebreaker",
    # ... 24 total questions
]
```

---

## 📊 Features

- ✅ **Real-time gameplay** with HTMX
- ✅ **Session-based** — Each player gets their own board
- ✅ **Automatic win detection** — Diagonal, row, and column bingo
- ✅ **Responsive design** — Works on phones, tablets, desktops
- ✅ **No external dependencies** — Pure Python & lightweight JavaScript

---

## 🧪 Development

### Run Tests
```bash
uv run pytest
```

### Lint & Format
```bash
uv run ruff check .
```

### Project Structure
```
soc-ops/
├── app/
│   ├── main.py           # FastAPI app & routes
│   ├── game_logic.py     # Bingo game rules
│   ├── game_service.py   # Game session management
│   ├── models.py         # Data models
│   ├── data.py           # Questions & constants
│   ├── static/           # CSS, assets
│   └── templates/        # Jinja2 templates
├── tests/                # Pytest test suite
├── workshop/             # Lab guides
└── pyproject.toml        # Dependencies & config
```

---

## 🤝 Contributing

Have a great question for the bingo board? Found a bug? **We'd love your help!**

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

## 🎉 Ready to Break the Ice?

**[Get started now →](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview)**

Or jump straight to running it locally:
```bash
git clone https://github.com/your-repo/soc-ops.git
cd soc-ops
uv sync
soc-ops
```

**Happy mingling! 🎊**
