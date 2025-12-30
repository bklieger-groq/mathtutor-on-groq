<h2 align="center">
 <br>
Voice-Enabled AI Math Tutor That Calculates and Renders Live Problems and Instruction with LaTeX in Seconds!
 <br>
</h2>

<p align="center">
 <a href="#Overview">Overview</a> •
 <a href="#Features">Features</a> •
  <a href="#Interfaces">Interfaces</a> •
 <a href="#Quickstart">Quickstart</a> •
 <a href="#Credits">Credits</a>
</p>

<br>


https://github.com/user-attachments/assets/24abe05a-ee6f-49d8-bdfc-13214b8d3d54


## Overview

Math Tutor on Groq is an AI-powered voice chatbot that leverages 8090's xRx framework, Whisper and Llama 3.3 70b on Groq, and TTS on Elevenlabs to respond in conversation with the student with live LaTeX and Markdown-formatted equations and notes specifically tailored to the student's requests. Groq's speed makes providing a complex response near instantaneous, enabling a seamless experience.

The speed also enables algebra and calculus problems to first be solved via an internal math engine, then providing the solution as context to the AI, increasing accuracy of the response.

## Quickstart

> [!IMPORTANT]
> To use Math Tutor, you can use a hosted version at [coming soon](/#).
> Alternatively, you can run Math Tutor locally using the quickstart instructions.

1. **Clone the Repository**
   ```bash
   git clone --recursive https://github.com/bklieger-groq/mathtutor-on-groq.git
   ```
   *The recursive flag ensures the xRx library is downloaded as well.*

2. **Create File for Environment Variables**
   ```bash
   cp env-example.txt .env
   ```

3. **Configure API Keys**
   - Add your Groq API key to `.env`:
     ```
     LLM_API_KEY="your_groq_api_key_here"
     GROQ_STT_API_KEY="your_groq_api_key_here"
     ```

   - Configure TTS settings with your preferred provider (e.g., ElevenLabs)
   ```
   ELEVENLABS_API_KEY="your_elevenlabs_api_key"
   ```
   *You can obtain a Groq API key from the [Groq console](https://console.groq.com/keys)*

4. **Run the Application**
   ```bash
   docker-compose up --build
   ```

Your application will be available at [localhost:3000](http://localhost:3000/).


## Changelog

See [CHANGELOG.md](CHANGELOG.md) to see the latest changes and versions. Major versions are archived.

## Credits

This app was developed by Benjamin Klieger at [Groq](https://groq.com) and uses the xRx framework created by 8090 Solutions: [Github Repository](https://github.com/8090-inc/xrx-core).
