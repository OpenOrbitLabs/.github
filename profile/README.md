<picture><source media="(prefers-color-scheme: dark)" srcset="./assets/banner-dark.svg" /><source media="(prefers-color-scheme: light)" srcset="./assets/banner-light.svg" /><img src="./assets/banner-dark.svg" width="100%" alt="OpenOrbit: Small, open-source tools for developers and creators." /></picture>

OpenOrbit makes small, focused, open-source tools that take repetitive work off your plate. Each one runs locally, does one job well and is MIT licensed.

<br />

<picture><source media="(prefers-color-scheme: dark)" srcset="./assets/title-projects-dark.svg" /><source media="(prefers-color-scheme: light)" srcset="./assets/title-projects-light.svg" /><img src="./assets/title-projects-dark.svg" width="880" alt="Featured projects" /></picture>

<p>
  <a href="https://github.com/OpenOrbitLabs/Vedit"><picture><source media="(prefers-color-scheme: dark)" srcset="./assets/project-vedit-dark.svg" /><source media="(prefers-color-scheme: light)" srcset="./assets/project-vedit-light.svg" /><img src="./assets/project-vedit-dark.svg" width="49%" alt="Vedit" /></picture></a>
  <a href="https://github.com/OpenOrbitLabs/CommitGen"><picture><source media="(prefers-color-scheme: dark)" srcset="./assets/project-commitgen-dark.svg" /><source media="(prefers-color-scheme: light)" srcset="./assets/project-commitgen-light.svg" /><img src="./assets/project-commitgen-dark.svg" width="49%" alt="CommitGen" /></picture></a>
</p>

| | What it does | Built with |
|---|---|---|
| **[Vedit](https://github.com/OpenOrbitLabs/Vedit)** | Turns raw talking-head footage into a finished video: cuts pauses, filler words and bad takes, adds animated captions, reframes for Shorts, TikTok and Reels, balances audio and makes thumbnails. Runs as a CLI or a Claude Code skill. | Python, FFmpeg, Whisper |
| **[CommitGen](https://github.com/OpenOrbitLabs/CommitGen)** | Writes commit messages from your staged diff. Runs on a local model through Ollama by default, works with any OpenAI-compatible API, and masks secrets before anything is sent. | Go |

### Try them

```bash
# Vedit: raw recording in, platform-ready video out (needs FFmpeg)
git clone https://github.com/OpenOrbitLabs/Vedit.git && cd Vedit && pip install -e ".[all]"
vedit auto raw.mp4 --preset youtube --formats 9:16 --thumbs
```

```bash
# CommitGen: AI commit message for what you staged (needs Go 1.22+)
go install github.com/onetwothird/CommitGen@latest
git add . && CommitGen
```

### Contributing

Bug reports, ideas and pull requests are welcome. Open an issue on the project's repo, or read its `CONTRIBUTING.md` before sending a change.
