# YakGPT

A simple, locally running ChatGPT UI that makes your text generation faster and chatting even more engaging!

## Features

- **GPT 3.5 & GPT 4** via OpenAI API
- **Speech-to-Text** via Azure & OpenAI Whisper
- **Text-to-Speech** via Azure & Eleven Labs
- Run locally on browser – no need to install any applications
- Faster than the official UI – connect directly to the API
- Easy mic integration – no more typing!
- Use your own API key – ensure your data privacy and security
- Data submitted via the API is not used for training and stored for 30 days only
- All state stored locally in localStorage – no analytics or external service calls
- Access on https://yakgpt.vercel.app or run locally!

> Note that GPT-4 API access is needed to use it. GPT 3.5 is enabled for all users.

## Screenshots

| Mobile                                                                                                           | Voice Mode                                                                                                       | Light Theme                                                                                                      | Dark Theme                                                                                                       |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| ![image](https://user-images.githubusercontent.com/129409586/229259007-ec4e0a27-cb5e-42fb-91b1-8e4efde99689.png) | ![image](https://user-images.githubusercontent.com/129409586/229259076-b29fe1e6-78a6-47c5-a330-fa34845a0e5f.png) | ![image](https://user-images.githubusercontent.com/129409586/229259145-0dd24f32-ea01-47f5-beab-68b80bfb1bb9.png) | ![image](https://user-images.githubusercontent.com/129409586/229259112-6e7223f8-d92d-49a7-9551-50276bf32089.png) |

## 🚀 Getting Started

Visit [YakGPT](https://yakgpt.vercel.app) to try it out without installing, or follow these steps to run it locally:

### Prerequisites

You'll need the following tools installed on your computer to run YakGPT locally.

- [Git](https://git-scm.com/)
- [Yarn](https://yarnpkg.com/) (or npm or pnpm)
- Any modern web browser like Google Chrome, Mozilla Firefox, or Microsoft Edge

### Installation

1. Clone the repository:

```
$ git clone https://github.com/yakGPT/YakGPT.git
```

2. Install dependencies, build the bundle and run the server

```
$ yarn
$ yarn build
$ yarn start
```

Then navigate to http://localhost:3000

Congratulations! 🎉 You are now running YakGPT locally on your machine.

## 🔑 API Key Configuration

To utilize YakGPT, you'll need to acquire an API key for OpenAI. The app should prompt you to insert you key.

### Add to .env.local(⚠️ Local use only)

If you want the keys to persist across app builds, you can add it to the .env.local.

```
$ echo "NEXT_PUBLIC_OPENAI_API_KEY=<your-open-ai-key-here>" > .env.local
$ echo "NEXT_PUBLIC_11LABS_API_KEY=<your-eleven-labs-key-here>" >> .env.local
```

## 🐳 Docker

```
$ docker build -t w3gpt
$ docker run -it -p 3000:80 w3gpt:latest
```

---

To build the Docker image yourself (such as if you're on arm64), run:

```
$ docker build -t yakgpt:latest .
$ docker run -it -p 3000:3000 yakgpt:latest
```

## 🎤 Microphone Integration

YakGPT makes chatting a breeze with its microphone integration! Activate your microphone using your browser's permissions, and YakGPT will automatically convert your speech into text.

You can also toggle the mic integration as needed by clicking on the microphone icon in the app.

Remember to use a supported web browser and ensure your microphone is functioning properly.

## 🛡️ Data Privacy and Security

YakGPT ensures your data privacy and security by letting you use your own API key. Your conversation with YakGPT takes place directly between your browser and OpenAI's GPT-3 API, with no intermediary servers.

## 📃 License

This project is licensed under the MIT License - see the [`LICENSE`](LICENSE) file for details

## 🙌 Acknowledgments

- [OpenAI](https://openai.com/) for building such amazing models and making them cheap as chips.
- [Mantine UI](https://ui.mantine.dev/) just an all-around amazing UI library.

Got feedback, questions or ideas? Feel free to submit an issue!
