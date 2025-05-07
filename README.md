
# 🤖 n8n Auto-Quote Telegram Bot

This project is a fully self-hosted **automation built using n8n** that sends a motivational or inspirational quote automatically to a Telegram chat at scheduled intervals. It uses the **Telegram Bot API** and can optionally fetch quotes from a public API or a custom list.

No manual commands or replies are handled—this is a one-way bot that pushes quotes to Telegram on autopilot.

---

## 📌 Features

- 🧘 Sends a random or predefined quote automatically
- 🔁 Scheduled using Cron expressions in n8n
- 🔗 Connects with Telegram Bot API
- ⚙️ Fully local and self-hosted (no cloud dependencies)
- 📤 Easy to import and customize

---

## 🛠️ Tech Stack

- [n8n](https://n8n.io/) – for building and automating the workflow
- [Telegram Bot API](https://core.telegram.org/bots/api)
- (Optional) [Quote APIs](https://type.fit/api/quotes), or a static list in n8n

---

## 🚀 Getting Started

### 1. Clone this Repository

```bash
git clone https://github.com/yourusername/n8n-auto-quote-bot.git
cd n8n-auto-quote-bot
````

### 2. Install n8n Locally

Follow the n8n documentation for installing it locally without Docker. You can install **n8n** directly on your system via [Node.js](https://docs.n8n.io/getting-started/installation/).

For example, to install via npm:

```bash
# Install n8n globally
npm install n8n -g

# Start n8n locally
n8n
```

This will start your n8n instance on `http://localhost:5678`.

### 3. Create a Telegram Bot

1. Open Telegram
2. Search for `@BotFather`
3. Use `/newbot` and follow the prompts
4. Copy the **Bot Token**

### 4. Import the Workflow into n8n

1. Open your local n8n instance at `http://localhost:5678`
2. Click on the three-dot menu (⋮) in the workflow list
3. Select **Import from File**
4. Upload `quote-sender-workflow.json`

### 5. Set Credentials

Inside the n8n editor:

* Go to the **Telegram node**
* Create a new Telegram credential using your **Bot Token**
* (Optional) Set the Chat ID or use the chat where you want to send messages

---

## ⚙️ Configuration

* You can update the **Cron node** to control when quotes are sent (e.g., daily at 9 AM).
* The quotes can come from:

  * A fixed list inside a **Set node**
  * A public **Quote API**
* Customize the message format inside the **Telegram node**

---

## 🧪 Example Use Case

Send a random motivational quote every morning to:

* Personal Telegram account
* Friends/family group
* Study group, productivity or mental wellness chats

---

## 📁 Files Included

```bash
n8n-auto-quote-bot/
├── README.md                 # Project documentation
├── .env.example             # Example environment variables
└── quote-sender-workflow.json  # The actual n8n workflow
```

---


## 📄 License

This project is licensed under the MIT License.

---

## 🙌 Credits

* [n8n](https://n8n.io/)
* [Telegram Bot API](https://core.telegram.org/bots)

```

---

With this version, you can install and run **n8n locally** using **Node.js** without Docker. You can follow the installation process specific to your OS. Let me know if you'd like further adjustments or additions!
```
