# kami-paper

[中文](../README.md) · [Live Demo](https://kami-paper.abnerzhao.com/)

A tiny static Markdown typesetting tool that turns resumes, long-form notes, or one-pagers into an A4 document layout inspired by [Kami](https://github.com/tw93/kami).

It is designed for people who want polished documents without setting up a document toolchain.

![Kami Paper demo](../assets/demo.png)

## Features

- Live Markdown editing and preview
- Kami-inspired warm paper layout
- Resume-friendly metrics, timelines, and project blocks
- Local PDF export in the browser
- No build step, no backend, no account required

## Usage

Open `index.html` in a browser, or serve the directory with any static file server.

```bash
python3 -m http.server 4174
```

Then visit:

```text
http://127.0.0.1:4174
```

## Markdown Format

Start with a name and contact line:

```markdown
# Your Name
AI / Agent Engineer · Shanghai · GitHub @name · email@example.com
```

Use `## 核心数字` for metric cards:

```markdown
## 核心数字
- 8 年｜Engineering experience
- 40%｜Build time reduced
- 12 个｜Projects shipped
- 30+ 人｜Cross-team collaboration
```

Use `###` headings for experience or project blocks:

```markdown
### Project Name｜Product Area · Tech Area｜Role
- Role summary
- Key actions
- Measurable impact
```

## Credits

The document visual style is inspired by [tw93/kami](https://github.com/tw93/kami).

PDF export uses local copies of:

- [html2canvas](https://github.com/niklasvh/html2canvas)
- [jsPDF](https://github.com/parallax/jsPDF)

## License

MIT
