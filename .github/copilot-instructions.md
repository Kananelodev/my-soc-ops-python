## Development Checklist
- [ ] Lint: `uv run ruff check .`
- [ ] Test: `uv run pytest`
- [ ] Install: `uv sync`

## Code Style
Python 3.13+, Ruff (line-length 88, E F I N W), type hints, frozen Pydantic models.

## Architecture
FastAPI + HTMX, session-based games, components in templates/components/, logic in game_logic.py/data.py.

## Conventions
5x5 bingo board with center free space, questions from data.py, Jinja2 templates.

See workshop/ for guides.