# Discord Backup Bot

A Python-based Discord tool that clones ("backs up") a server's structure — including categories, channels, and roles. This script uses `discord.py` and is intended for educational or personal backup purposes.

⚠️ **Note:** The included code is currently written as a *selfbot* (`self_bot=True` and `bot=False`), which violates Discord's Terms of Service. Running selfbots can result in account termination. Use responsibly and at your own risk.

---

## 🚀 Features

* Clone an entire server's **categories**, **text channels**, and **voice channels**.
* Recreate all **roles** (except `@everyone`).
* Automatically creates a new server named `backup-<original server name>`.
* Simple command: `copyserver`

---

## 📦 Requirements

* Python 3.8+
* `discord.py`
* `colorama`

Install dependencies:

```bash
pip install discord.py colorama requests
```

---

## 📁 Usage

Run the script:

```bash
python main.py
```

You will be prompted to enter:

* **TOKEN** – your Discord token
* **PREFIX** – your preferred command prefix

Inside any server, type:

```bash
<prefix>copyserver
```

This will:

1. Create a new server with the name `backup-<current server>`
2. Remove all auto-created channels
3. Recreate all categories, channels, and roles from the original server

---

## 🧩 Example

If your prefix is `!`, run:

```
!copyserver
```

---

## ⚠️ Disclaimer

This project is for **educational purposes only**.
Using selfbots or account automation **violates Discord's Terms of Service**.
I am **not responsible** for any misuse, banned accounts, or damages.

---

## 📄 License

MIT License — feel free to modify and use as needed.
