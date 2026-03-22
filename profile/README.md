<p align="center">
  <a href="https://smello.io">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/smelloscope/smello/main/docs/assets/logo-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/smelloscope/smello/main/docs/assets/logo.svg">
      <img alt="Smello" src="https://raw.githubusercontent.com/smelloscope/smello/main/docs/assets/logo.svg" width="120" height="120">
    </picture>
  </a>
</p>

<h3 align="center">Smello — HTTP request inspector for Python</h3>

<p align="center">
Inspect outgoing HTTP and gRPC requests from your Python code in a local dashboard.<br>
Like <a href="https://mailpit.axllent.org/">Mailpit</a>, but for HTTP requests.
</p>

<p align="center">
  <a href="https://smello.io">Website</a> · <a href="https://smello.io/getting-started/">Docs</a> · <a href="https://github.com/smelloscope/smello">GitHub</a>
</p>

```python
import smello
smello.init(server_url="http://localhost:5110")

# Outgoing requests now appear at localhost:5110
```

Captures traffic from **requests**, **httpx**, **gRPC** (Google Cloud libraries), and **boto3** (AWS). Redacts `Authorization` and `X-Api-Key` headers by default. Without a server URL, `init()` is a no-op — no patching, no threads.

<p align="center">
  <a href="https://github.com/smelloscope/smello">
    <img src="https://raw.githubusercontent.com/smelloscope/smello/main/docs/assets/screenshot.png" alt="Smello dashboard" width="720">
  </a>
</p>
