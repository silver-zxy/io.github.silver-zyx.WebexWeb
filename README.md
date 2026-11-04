# <img src="data/io.github.silver_zyx.WebexWeb.svg" alt="" width="30" align="top"> Webex Web

> *A working Linux client for Webex – because the official app is broken.*

Webex in its own window, with desktop Integration. Built with Electron.

> **This is an unofficial project. It is not made by, affiliated with, endorsed by, sponsored by, or connected to Cisco in any way.**
>
> "Webex" and the Webex logo are trademarks of Cisco Systems, Inc. This app only wraps the public web client (web.webex.com) in a window — it ships no Cisco code, assets, or branding, and the icon is an original mark, not Cisco's logo. If you want the official client, get it from Cisco.

## Install

    flatpak remote-add --if-not-exists webexweb \
      https://silver-zyx.github.io/io.github.silver_zyx.WebexWeb/index.flatpakrepo
    flatpak install webexweb io.github.silver_zyx.WebexWeb

## Build locally

    flatpak install -y flathub org.flatpak.Builder
    flatpak install -y flathub \
      org.freedesktop.Platform//25.08 \
      org.freedesktop.Sdk//25.08 \
      org.electronjs.Electron2.BaseApp//25.08

    flatpak run org.flatpak.Builder --user --install --force-clean \
      build-dir io.github.silver_zyx.WebexWeb.yaml

    flatpak run io.github.silver_zyx.WebexWeb

## License

MIT. See [LICENSE](LICENSE).
