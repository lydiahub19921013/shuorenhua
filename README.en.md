# Say It Plainly | Lydia communication assistant

[简体中文](README.md) · [Download v0.9.0](https://github.com/lydiahub19921013/shuorenhua/releases/latest) · [Report a problem](https://github.com/lydiahub19921013/shuorenhua/issues)

Say It Plainly helps turn a long or ambiguous message into a short action list, surface the detail that most needs clarification, and draft a reply based on what you actually mean. **AI-generated drafts are for your review; the app does not send them for you.**

## Current release

- **v0.9.0 is a feature-validation build**, not a claim of a finished general release.
- Requires an **Apple Silicon Mac running macOS 13 or later**.
- The app interface and complete usage guide are currently in Chinese.
- This repository distributes the app package and documentation; the application source code is not published here.

## How it works

1. Copy a message and press `Control + Option + R`. In apps that support standard text selections, you can also use the macOS Services menu.
2. Choose a scenario and review what the other person is asking, up to three concrete actions, and the most important missing detail.
3. Describe your intended reply in your own words. The app drafts a response and checks for added time, quantity, scope, responsibility, price, or guarantees.
4. Review the result. When the original text field is identified, the draft is placed there for you to inspect; you decide whether to send it.

The four current scenarios cover management requests, customer conversations, colleague handoffs, and personal conversations. They change how the message is interpreted, not the underlying rule that you review the draft.

## Privacy and model-use boundaries

- The app does not scan the clipboard in the background. You start each analysis yourself.
- When you request a generated analysis or reply, the selected message, your stated intent, and recent local examples used for tone may be sent to the configured model.
- The app can learn from replies you actually place back into the original field. It stores at most eight recent examples on this Mac; you can clear them in Settings.
- In this validation build, Developer Settings can store a test DeepSeek key in macOS Keychain. Without a test key, a clearly labeled preview is available. The planned service-gateway setup is not presented as an already-shipped capability.
- Fixed quick replies such as “Got it” follow a separate path: they do not call the AI model. They are sent only when the original field can be identified; otherwise they are copied.

## Install

1. Download the ZIP from [GitHub Releases](https://github.com/lydiahub19921013/shuorenhua/releases/latest) and extract it.
2. Move `说人话.app` into **Applications**.
3. If macOS asks you to confirm the app, Control-click it in Finder and choose **Open**.

For detailed screenshots and Chinese UI labels, see the [Chinese installation guide](安装与使用说明.txt). The v0.9.0 release includes a SHA-256 manifest; its digest was checked against the published ZIP asset on 2026-09-28.

## Feedback

Use [GitHub Issues](https://github.com/lydiahub19921013/shuorenhua/issues) for a reproducible bug report or feature suggestion. Do not post private conversations, personal data, API keys, or other credentials in an issue.
