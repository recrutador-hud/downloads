<div align="center">

# Changelog / Historico de Versoes

All notable changes to Recrutador HUD are documented here.\
Todas as mudancas importantes do Recrutador HUD estao documentadas aqui.

</div>

---

## 1.0.2-alpha — 2026-04-05

### EN - Audio Quality Fix & Version Display

#### Bug Fixes
- **Windows audio clicking fixed** — Eliminated clicking and noise artifacts during audio capture on Windows. The issue was caused by stateless resampling that created discontinuities at audio chunk boundaries.
- **Version label now shows pre-release tag** — The version displayed in the UI now correctly shows the full version including pre-release suffixes (e.g., "v1.0.2-alpha" instead of "v1.0.2").

---

### PT - Correcao de Qualidade de Audio & Exibicao de Versao

#### Correcoes
- **Cliques no audio do Windows corrigidos** — Eliminados cliques e ruidos durante a captura de audio no Windows. O problema era causado por reamostragem sem estado que criava descontinuidades nas bordas dos blocos de audio.
- **Versao agora mostra tag de pre-release** — A versao exibida na interface agora mostra corretamente a versao completa incluindo sufixos de pre-release (ex: "v1.0.2-alpha" ao inves de "v1.0.2").

---

## 1.0.1-alpha — 2026-04-03

### EN - Version Display & CI Improvements

#### What's New
- **Version label in UI** — The current app version is now visible in the HUD status bar and Smart Sidecar header. Clicking it opens the release notes for that version on GitHub.

#### Improvements
- **Updated CI pipeline** — Upgraded GitHub Actions to v5 (Node.js 24) to eliminate deprecation warnings

---

### PT - Versao Visivel & Melhorias no CI

#### Novidades
- **Versao visivel na interface** — A versao atual do app agora aparece na barra de status do HUD e no cabecalho do Smart Sidecar. Clicar nela abre as notas da versao no GitHub.

#### Melhorias
- **Pipeline de CI atualizado** — GitHub Actions atualizadas para v5 (Node.js 24) para eliminar avisos de depreciacao

---

## 1.0.0-alpha — 2026-04-03

### EN - First Alpha Release

This is the first public alpha of **Recrutador HUD** — the real-time interview assistant desktop companion.

#### Highlights

- **Real-time audio capture** — Captures both microphone and system audio simultaneously using platform-native APIs (CoreAudio on macOS, WASAPI on Windows, PulseAudio on Linux)
- **Live transcription** — Streams audio to Deepgram for real-time speech-to-text, relayed to the backend via SignalR
- **Smart Sidecar** — Floating overlay window displaying AI-powered interventions, coverage insights, and prompt suggestions during live interviews
- **Seamless deep linking** — Click a link in the web app and the HUD launches directly into your session
- **Crash recovery** — Automatically detects and recovers interrupted sessions on restart
- **Offline resilience** — Transcript segments are buffered locally and replayed when connectivity is restored
- **Auto-updates** — The app silently checks for updates in the background and applies them on next launch — no manual downloads needed
- **Bilingual interface** — Full English and Portuguese (PT-BR) support with runtime language switching

#### Known Limitations

- macOS requires Screen Recording and Microphone permissions (prompted on first launch)
- System audio loopback on macOS uses ProcessTap (requires macOS 14.2+)
- No code signing yet — macOS users may need to right-click > Open on first launch

---

### PT - Primeiro Alpha

Este e o primeiro alpha publico do **Recrutador HUD** — o assistente de entrevistas em tempo real para desktop.

#### Destaques

- **Captura de audio em tempo real** — Captura microfone e audio do sistema simultaneamente usando APIs nativas da plataforma (CoreAudio no macOS, WASAPI no Windows, PulseAudio no Linux)
- **Transcricao ao vivo** — Transmite audio para o Deepgram para transcricao em tempo real, retransmitida ao backend via SignalR
- **Smart Sidecar** — Janela flutuante exibindo intervencoes com IA, insights de cobertura e sugestoes de prompts durante entrevistas ao vivo
- **Deep linking** — Clique em um link no app web e o HUD abre diretamente na sua sessao
- **Recuperacao de falhas** — Detecta e recupera automaticamente sessoes interrompidas ao reiniciar
- **Resiliencia offline** — Segmentos de transcricao sao armazenados localmente e reenviados quando a conectividade e restaurada
- **Atualizacoes automaticas** — O app verifica atualizacoes silenciosamente em segundo plano e as aplica na proxima abertura — sem downloads manuais
- **Interface bilingue** — Suporte completo em Ingles e Portugues (PT-BR) com troca de idioma em tempo de execucao

#### Limitacoes Conhecidas

- macOS requer permissoes de Gravacao de Tela e Microfone (solicitadas na primeira abertura)
- Captura de audio do sistema no macOS usa ProcessTap (requer macOS 14.2+)
- Sem assinatura de codigo ainda — usuarios macOS podem precisar clicar com botao direito > Abrir na primeira execucao
