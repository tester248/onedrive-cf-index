<div align="center">
  <img src="./public/header.png" alt="TSQ Drive" />
  <h3>TSQ Drive</h3>
  <p><em>A public OneDrive directory listing, powered by Cloudflare and Next.js</em></p>

  <img src="https://img.shields.io/badge/OneDrive-2C68C3?style=flat&logo=microsoft-onedrive&logoColor=white" alt="OneDrive" />
  <img src="https://img.shields.io/badge/Cloudflare-f38020?style=flat&logo=Cloudflare&logoColor=white" alt="Cloudflare" />
  <img src="https://img.shields.io/badge/Next.js-black?style=flat&logo=next.js&logoColor=white" alt="Next.js" />
  <a href="https://github.com/lyc8503/onedrive-cf-index-ng/wiki"><img src="https://img.shields.io/badge/Documentation-black?style=flat&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAABmJLR0QA/wD/AP+gvaeTAAABeUlEQVRIie2VwUrDQBCGZ5ZubNmS0Ba9tF6CUqTHpg+g+AhCn8R30DfpM3jRezdHoZJroaBJQ2qgsIEdD7YSsCtJVBTxP87u/t/u7M4swDcLTQNSSseyLFbERCmlPc9LCgF83z/jnE9s294vvk+AJEmesiwbe553awQEQbCXZVnY7/ebjBXa/Ju01jCbzVIA6AwGA7WN1/KT4jg+6vV6TcYYpGlKq9UKiQgAAOr1OnU6HWNKGWPQarWa8/n8GADudwIQ0UJ89QjDEKMoOiEitRm7tm37gnNuPAUiAiJa+VjNNJmIYDgcPiAiAQD4vh9tT1NG5RJdQT8PkFKak/5ZgJTyUgjxPJ1Ob4josArAeMmWZYHrulftdhvX6/X5YrEwPtFKgG63C7ApxEajga7rVvH/BZf8D/hjACJSVRpabj1su+9OgBAiiOM41VqXNtdaw3K5TIUQQT7+rjqllKec84njOAdlAEmSPCqlxqPR6O5DQA70JZ/+t+sFAb2R22dSZ7wAAAAASUVORK5CYII=" alt="Documentation" /></a>
</div>

---

A free, serverless way to showcase, share, preview, and download files from **your OneDrive folder** — this is a personal deployment of [onedrive-cf-index-ng](https://github.com/lyc8503/onedrive-cf-index-ng), serving only the `TSQDrive` folder.

- 💸 Completely free to host (Cloudflare Pages)
- ⚡ Fast and responsive
- ⏱️ Deployable in ~15 minutes
- ⚒️ Highly customisable
- 🍌 Pretty (●'◡'●)

## Crediting the original authors

This project stands on the shoulders of others — full credit to the original authors:

- **[onedrive-cf-index-ng](https://github.com/lyc8503/onedrive-cf-index-ng)** by [@lyc8503](https://github.com/lyc8503) — the Cloudflare/Next.js rewrite this fork is based on.
- **[onedrive-vercel-index](https://github.com/spencerwooo/onedrive-vercel-index)** by [@spencerwooo](https://github.com/spencerwooo) — the original Vercel-based project it was forked from.
- All contributors of both projects — thank you. ❤️

## Quick start

🚀 [Getting started guide](https://github.com/lyc8503/onedrive-cf-index-ng/wiki/Getting-Started) (upstream wiki).

*If you find the upstream project useful, give it a star!* :3

## Features

- 👀 File preview — PDF, EPUB, markdown, code, plain text, images
- 📄 Office preview — docx, pptx, xlsx, ...
- 🎥 Video and audio playback (mp4, mp3, ... with subtitle support)
- 💠 List / Grid layouts, with pagination for large folders
- 🔒 Password-protected folders and files
- ⏬ Multi-file and folder download (zip)
- 🔎 Native search across the shared folder
- 🖼️ Direct raw-file serving / hosting
- 🌙 Full dark mode, style and site customisation
- 📚 OPDS catalog endpoint for ebook readers at `/api/opds?path=/`

> **Note:** This project focuses on showcasing and sharing files from OneDrive. If you run your own server, need WebDAV, or use other cloud providers, check out [alist](https://github.com/alist-org/alist).

## Configuration

All runtime settings are provided via **environment variables** on the Cloudflare Pages project (not in this repo):

| Variable | Purpose |
| --- | --- |
| `USER_PRINCIPLE_NAME` | The Microsoft account email used to authenticate the initial setup |
| `BASE_DIRECTORY` | The OneDrive-relative folder to expose (e.g. `Documents/TSQDrive`) |
| `OAUTH_CLIENT_ID` | Microsoft Graph OAuth client ID |
| `OAUTH_CLIENT_SECRET` | Obfuscated Microsoft Graph OAuth client secret |

## Documentation

- [Getting started](https://github.com/lyc8503/onedrive-cf-index-ng/wiki/Getting-Started)
- [Configurations](https://github.com/lyc8503/onedrive-cf-index-ng/wiki/Configurations)
- [Docker deployment](https://github.com/lyc8503/onedrive-cf-index-ng/wiki/Docker-Deployment)
- Feature docs: [protected folders](https://ovi.swo.moe/docs/features/protected-folders) · [multi-file download](https://ovi.swo.moe/docs/features/multi-file-folder-download) · [hosting files directly](https://ovi.swo.moe/docs/features/hosting-images-directly) · [search](https://ovi.swo.moe/docs/features/search-for-files-and-folders) · [subtitles](https://ovi.swo.moe/docs/features/load-video-subtitles)
- Upgrading an existing deployment? [Migration guide](https://ovi.swo.moe/docs/migration/updating-to-latest-version)

## License

[MIT](LICENSE)
