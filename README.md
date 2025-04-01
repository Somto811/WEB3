# Swarm Node Manager

## 🚀 Quick Start Guide
This guide will help you install and run the **Swarm Node Manager** script step by step. No coding experience is required!

## 📌 What is this script for?
This script helps you:
- **Set up and install** all necessary dependencies for running a Swarm node.
- **Start a Swarm node** automatically.
- **Completely remove the Swarm setup** (without affecting important system software like Docker).

---

## ✍️ Step 1: Create the Script File
We will create a file named **swarm.sh** and paste the script into it.

1️⃣ Open a terminal (Command Line). If you are using a VPS, connect via SSH first.

2️⃣ Type the following command to create and open a new file:
```bash
nano swarm.sh
```

3️⃣ Copy and paste the contents of the **Swarm Node Manager** script into the file.

4️⃣ After pasting, save the file:
   - Press **CTRL + X** to exit.
   - Press **Y** to confirm saving changes.
   - Press **Enter** to finalize.

---

## 🔑 Step 2: Make the Script Executable
Now, we need to give the script permission to run:
```bash
chmod +x swarm.sh
```

---

## ▶️ Step 3: Run the Script
To start the script, simply run:
```bash
./swarm.sh
```
You will see a menu with options to **install, remove, or exit**.

---

## 🛠️ Troubleshooting
### 🔹 "Permission Denied" Error
If you get a "Permission denied" error when trying to run **swarm.sh**, fix it by running:
```bash
chmod +x swarm.sh
```
Then, try running it again:
```bash
./swarm.sh
```

### 🔹 Installation Issues (Python, Node.js, Yarn)
If you run into errors like **"unable to locate package"**, make sure your system is updated:
```bash
sudo apt update && sudo apt upgrade -y
```
Then, retry running the script.

### 🔹 Exiting the Script
At any time, you can exit by pressing **CTRL + C** or selecting "Exit" from the menu.

---

## 📌 Follow for Updates
Stay updated with more guides and improvements! Follow me on **Twitter (X):** [@Daddy_savy](https://twitter.com/Daddy_savy)

---

## ⚠️ Important Notes
- This script does **not** remove essential software like **Docker**, **Python**, or **Node.js** if they are already installed.
- If you remove the Swarm setup, it will only delete files **specific to Swarm**, keeping your system safe.
- Ensure your HuggingFace token is stored securely. You can get a token here: [HuggingFace Tokens](https://huggingface.co/settings/tokens).

---

## 🎯 What’s Next?
- Once installed, access your node at:
  ```bash
  http://<your-server-ip>:3000/
  ```
- Use the command below to check your Swarm screen session:
  ```bash
  screen -r swarm
  ```
- If you see **"Hello, [Your Node Name]"**, your Swarm node is running successfully!

✅ **Enjoy running your Swarm Node effortlessly!**

