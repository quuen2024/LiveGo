
STREAMIX42


![GitHub Pages](https://img.shields.io/github/deployments/nexoscreator/html5-custom-video-player/github-pages.svg?style=flat-square&color=cyan)
![GitHub Release](https://img.shields.io/github/v/release/nexoscreator/html5-custom-video-player.svg?style=flat-square&color=cyan)
![GitHub License](https://img.shields.io/github/license/nexoscreator/html5-custom-video-player.svg?style=flat-square&color=cyan)
![GitHub Code](https://img.shields.io/github/languages/code-size/nexoscreator/html5-custom-video-player.svg?style=flat-square&color=cyan)
---
# IPTVTools

A set of scripts that help to better IPTV experience.

[![CI](https://github.com/huxuan/iptvtools/actions/workflows/ci.yml/badge.svg)](https://github.com/huxuan/iptvtools/actions/workflows/ci.yml)
[![CommitLint](https://github.com/huxuan/iptvtools/actions/workflows/commitlint.yml/badge.svg)](https://github.com/huxuan/iptvtools/actions/workflows/commitlint.yml)
[![DevContainer](https://github.com/huxuan/iptvtools/actions/workflows/devcontainer.yml/badge.svg)](https://github.com/huxuan/iptvtools/actions/workflows/devcontainer.yml)
[![Release](https://github.com/huxuan/iptvtools/actions/workflows/release.yml/badge.svg)](https://github.com/huxuan/iptvtools/actions/workflows/release.yml)
[![Renovate](https://github.com/huxuan/iptvtools/actions/workflows/renovate.yml/badge.svg)](https://github.com/huxuan/iptvtools/actions/workflows/renovate.yml)
[![Semantic Release](https://github.com/huxuan/iptvtools/actions/workflows/semantic-release.yml/badge.svg)](https://github.com/huxuan/iptvtools/actions/workflows/semantic-release.yml)
[![Coverage](https://img.shields.io/endpoint?url=https://huxuan.github.io/iptvtools/_static/badges/coverage.json)](https://huxuan.github.io/iptvtools/reports/coverage)
[![Release](https://img.shields.io/github/v/release/huxuan/iptvtools)](https://github.com/huxuan/iptvtools/releases)
[![PyPI](https://img.shields.io/pypi/v/iptvtools)](https://pypi.org/project/iptvtools/)
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/iptvtools)](https://pypi.org/project/iptvtools/)
[![GitHub](https://img.shields.io/github/license/huxuan/iptvtools)](https://github.com/huxuan/iptvtools/blob/main/LICENSE)

[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)
[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
[![Copier](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/copier-org/copier/master/img/badge/badge-grayscale-inverted-border-orange.json)](https://github.com/copier-org/copier)
[![Serious Scaffold Python](https://img.shields.io/endpoint?url=https://serious-scaffold.github.io/ss-python/_static/badges/logo.json)](https://serious-scaffold.github.io/ss-python)
[![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/huxuan/iptvtools)

> [!IMPORTANT]
> _IPTVTools_ is in the **Beta** phase.
> Changes and potential instability should be anticipated.
> Any feedback, comments, suggestions and contributions are welcome!
## Features

Scripts currently provided:

- iptvtools-cli filter
  - Merge from different resources.
  - Check the tcp/udp connectivity.
  - Filter by custom criteria, e.g. resolution.
  - Match with templates and EPG.
  - Format the url with UDPxy if provided.
  - Unify channels' titles.

Features planned on the road:

- [ ] Scan certain ip and port range to find new channels.
- [ ] Establish a lightweight database for routine maintenance.

Besides, all scripts should be lightweight and able to keep running regularly after proper configuration.

Last but not least, any ideas, comments and suggestions are welcome!

## Prerequisites

To filter by stream information, e.g., resolution/height, [ffmpeg](https://www.ffmpeg.org/) (or [ffprobe](https://www.ffmpeg.org/ffprobe.html) more precisely) is needed, please install according to the [documentation](https://www.ffmpeg.org/download.html).

## Installation

It is recommended to manage iptvtools via [pipx](https://github.com/pypa/pipx):

```shell
pipx install iptvtools
```

## Usage

Please refer to the [documentation](https://iptvtools.readthedocs.io/) while some useful information in [wiki](https://github.com/huxuan/iptvtools/wiki).
## 📜 License

MIT License, for more details, see the [LICENSE](https://github.com/huxuan/iptvtools/blob/main/LICENSE) file.


pdm-managed pre-commit Checked with mypy Ruff Conventional Commits Pydantic v2 Copier Serious Scaffold Python Open in Dev Containers

## 🎥 Custom HTML5 Video Player

![image](https://raw.githubusercontent.com/quuen2024/logo/refs/heads/queen/drift.jpg)

> A **lightweight, customizable, and feature-rich** video player built using plain JavaScript and CSS. Includes essential video controls such as **play/pause, volume adjustment, speed control, fullscreen mode, theater mode, mini-player, and more**.

---

## ✨ Features

- **Responsive Design**: Works seamlessly on desktop & mobile devices.
- **Supports Multiple Video Formats**: (MP4, WebM, Ogg, etc.)
- **Keyboard Shortcuts**: for easy navigation.
- **Custom Controls**: Play/Pause, Volume, Speed Control, Fullscreen, Mini Player, Theater Mode.
- **Loading Indicator**: for better UX.
- **Touch & Click Support**: for mobile devices.
- **Customizable**: Easily modify styles & functionality.

---

## 📥 Installation

1. **Include the Video Player in HTML**

   Use the following HTML to include the video player in your page:

   ```html
   <div
     class="nex-video-player"
     data-src="path/to/your/video.mp4"
     data-title="Video Title"
   ></div>
   ```

   > **Note:** Replace `"path/to/your/video.mp4"` with your actual video file URL and update the `"Video Title"`.

2. **Link CSS Styles**

   Include the necessary CSS to style the video player and controls.

   ```html
   <link
     rel="stylesheet"
     href="https://raw.githubusercontent.com/quuen2024/LiveGo/refs/heads/queen/video-player.css"
	 [
  "https://raw.githubusercontent.com/quuen2024/LiveGo/refs/heads/queen/newslive.m3u8",
  "https://raw.githubusercontent.com/quuen2024/LiveGo/refs/heads/queen/newssport.m3u8",
   ]
   />
   ```

3. **Link the JavaScript**

   Add the JavaScript code cdn link provided below to the functionality of the video player.

   ```html
   <script
     src="https://raw.githubusercontent.com/quuen2024/LiveGo/refs/heads/queen/video-player.js"
     defer
   ></script>
   ```

---

## 🎯 Keyboard Shortcuts

This custom video player supports the following keyboard shortcuts to enhance your video playback experience:

| Shortcut Key      | Action              | Description                              |
| ----------------- | ------------------- | ---------------------------------------- |
| `F`               | Fullscreen Toggle   | Enter or exit fullscreen mode.           |
| `→` (Right Arrow) | Forward             | Skip the video forward.                  |
| `←` (Left Arrow)  | Backward            | Rewind the video.                        |
| `T`               | Toggle Theater Mode | Switch between normal and theater modes. |
| `I`               | Mini Player Mode    | Activate or deactivate mini player view. |
| `M`               | Mute/Unmute         | Mute or unmute the video.                |
| `+`               | Increase Speed      | Increase playback speed.                 |
| `-`               | Decrease Speed      | Decrease playback speed.                 |

---

## 🎨 Customization

You can customize the **CSS styles** and **JavaScript functionality** according to your needs.

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/quuen2024/LiveGo.git
   cd html5-custom-video-player
   ```

2. **Customize CSS:**
   Edit the `video-player.css` file to change the styles.

3. **Customize JavaScript:**
   Customize the player controls by modifying `video-player.js`. You can update controls, navigation, or error handling as needed.

---

## 🔗 Useful Links

[![Web Demo](https://img.shields.io/badge/Web-Demo-blue?style=for-the-badge&logo=google-chrome)](https://nexoscreator.github.io/html5-custom-video-player)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Repo-green?style=for-the-badge&logo=github)](https://github.com/nexoscreator/html5-custom-video-player)
[![YouTube Video](https://img.shields.io/badge/YouTube-Video-red?style=for-the-badge&logo=youtube)](https://youtu.be/rMnDe0iEGRs?si=B2viVesOhHYusbBG)

---

## 🤝 Contributing

We ❤️ contributions! Follow these steps to contribute:

1. 🍴 **Fork** the repository
2. 🌿 **Create** a new branch (`git checkout -b feature/AmazingFeature`)
3. 💾 **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. 🚀 **Push** to the branch (`git push origin feature/AmazingFeature`)
5. 🔃 **Open a Pull Request**

📖 _See our [Contribution Guidelines](CONTRIBUTING.md) for more details._

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 📬 Contact & Community

💬 Join us on **Discord**: [Click Here](https://github.com/quuen2024/LiveGo)  
🐦 **Follow on Twitter**: [@nexoscreator](https://twitter.com/betok.id)  
📧 **Email**: [contact@nexoscreator.tech](mailto:contact@betok.id)

If you find this project helpful, please consider **starring ⭐ the repository** or **sponsoring 💖 on GitHub**!

<p align="center">
  Created with ❤️ by <a href="https://github.com/quuen2024/LiveGo">@quuen2024/LiveGo</a>
</p>
