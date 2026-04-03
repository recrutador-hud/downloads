<div align="center">

# Recrutador HUD

**Your real-time interview intelligence companion**\
**Seu assistente de entrevistas em tempo real**

[![Latest Release](https://img.shields.io/github/v/release/recrutador-hud/downloads?label=latest&style=flat-square)](https://github.com/recrutador-hud/downloads/releases/latest)
[![macOS](https://img.shields.io/badge/macOS-14.2%2B_(Apple_Silicon)-000?style=flat-square&logo=apple&logoColor=white)](https://github.com/recrutador-hud/downloads/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%2B_(x64)-0078D4?style=flat-square&logo=windows&logoColor=white)](https://github.com/recrutador-hud/downloads/releases/latest)
[![Linux](https://img.shields.io/badge/Linux-x64-FCC624?style=flat-square&logo=linux&logoColor=black)](https://github.com/recrutador-hud/downloads/releases/latest)

</div>

---

## Download / Baixar

> Go to [**Releases**](https://github.com/recrutador-hud/downloads/releases/latest) and download the installer for your platform.\
> Va em [**Releases**](https://github.com/recrutador-hud/downloads/releases/latest) e baixe o instalador para sua plataforma.

| Platform / Plataforma | File / Arquivo | Notes / Observacoes |
|:----------------------|:---------------|:--------------------|
| **macOS** (Apple Silicon) | `RecrutadorHUD-*-osx-arm64-Setup.pkg` | Requires macOS 14.2+ / Requer macOS 14.2+ |
| **Windows** (x64) | `RecrutadorHUD-*-win-x64-Setup.exe` | Requires Windows 10+ / Requer Windows 10+ |
| **Linux** (x64) | `RecrutadorHUD-*-linux-x64-Setup.AppImage` | Requires PulseAudio / Requer PulseAudio |

After the first install, the app **updates itself automatically** — no need to come back here.\
Apos a primeira instalacao, o app **se atualiza automaticamente** — nao precisa voltar aqui.

---

## What is Recrutador HUD? / O que e o Recrutador HUD?

<details>
<summary><strong>English</strong></summary>

Recrutador HUD is a lightweight desktop companion for the [Recrutador](https://seurecrutador.com.br) recruitment intelligence platform. It runs alongside your video call and provides real-time assistance during interviews:

- **Audio capture** — Records microphone and system audio simultaneously using native platform APIs
- **Live transcription** — Streams audio to Deepgram for instant speech-to-text
- **Smart Sidecar** — A floating overlay with AI-powered suggestions, coverage tracking, and interview insights
- **Seamless launch** — Click a link in the Recrutador web app and the HUD opens directly into your session
- **Auto-updates** — Silently downloads updates in the background; applied on next launch
- **Crash recovery** — Automatically resumes interrupted sessions

The HUD is a **thin client** — all intelligence lives on the backend. No data is stored locally. Audio is transient and never persisted to disk.

</details>

<details>
<summary><strong>Portugues</strong></summary>

O Recrutador HUD e um aplicativo desktop leve que acompanha a plataforma de inteligencia em recrutamento [Recrutador](https://seurecrutador.com.br). Ele roda junto com sua videochamada e oferece assistencia em tempo real durante entrevistas:

- **Captura de audio** — Grava microfone e audio do sistema simultaneamente usando APIs nativas da plataforma
- **Transcricao ao vivo** — Transmite audio para o Deepgram para transcricao instantanea
- **Smart Sidecar** — Janela flutuante com sugestoes de IA, acompanhamento de cobertura e insights da entrevista
- **Abertura automatica** — Clique em um link no app web do Recrutador e o HUD abre direto na sua sessao
- **Atualizacoes automaticas** — Baixa atualizacoes silenciosamente em segundo plano; aplicadas na proxima abertura
- **Recuperacao de falhas** — Retoma automaticamente sessoes interrompidas

O HUD e um **cliente leve** — toda a inteligencia esta no backend. Nenhum dado e armazenado localmente. O audio e transitorio e nunca e salvo em disco.

</details>

---

## First Launch / Primeira Abertura

<details>
<summary><strong>macOS</strong></summary>

1. Download and open the `.pkg` installer
2. If macOS blocks the app ("unidentified developer"), go to **System Settings > Privacy & Security** and click **Open Anyway**
3. Grant **Microphone** and **Screen Recording** permissions when prompted — both are required for audio capture
4. The app registers the `recrutador://` protocol automatically — deep links from the web app will work immediately

</details>

<details>
<summary><strong>Windows</strong></summary>

1. Download and run the `Setup.exe` installer
2. The app installs to `%LocalAppData%\RecrutadorHUD` (no admin required)
3. The `recrutador://` deep link protocol is registered automatically
4. If Windows SmartScreen warns about an unrecognized app, click **More info > Run anyway**

</details>

<details>
<summary><strong>Linux</strong></summary>

1. Download the `.AppImage` file
2. Make it executable: `chmod +x RecrutadorHUD-*-linux-x64-Setup.AppImage`
3. Run it — PulseAudio must be available for audio capture
4. Register the `recrutador://` protocol manually if needed:
   ```
   xdg-mime default recrutador.desktop x-scheme-handler/recrutador
   ```

</details>

---

## Updates / Atualizacoes

The HUD checks for updates automatically in the background. When a new version is available, it downloads silently and applies on the next app launch. You don't need to do anything.

O HUD verifica atualizacoes automaticamente em segundo plano. Quando uma nova versao esta disponivel, ela e baixada silenciosamente e aplicada na proxima abertura do app. Voce nao precisa fazer nada.

---

## Changelog / Historico de Versoes

See [CHANGELOG.md](CHANGELOG.md) for the full release history in English and Portuguese.

Veja [CHANGELOG.md](CHANGELOG.md) para o historico completo de versoes em Ingles e Portugues.

---

<div align="center">

**[seurecrutador.com.br](https://seurecrutador.com.br)**

</div>
