```markdown
# Swarm Node Manager

## Requirements
| Component   | Specification |
|-------------|---------------|
| CPU         | AMD64 or ARM  |
| RAM         | 25GB          |

## Ngrok Installation

### AMD64 Machines
```bash
wget https://bin.equinox.io/c/bNyj1mQVY4c/ngrok-v3-stable-linux-amd64.tgz
tar -xvzf ngrok-v3-stable-linux-amd64.tgz
sudo mv ngrok /usr/local/bin/
```

### arm Machines
```bash
wget https://bin.equinox.io/c/bNyj1mQVY4c/ngrok-v3-stable-linux-arm.tgz
tar -xvzf ngrok-v3-stable-linux-arm.tgz
sudo mv ngrok /usr/local/bin/
```


### 2. Configure Ngrok
1. Visit [ngrok.com](https://ngrok.com)
2. Sign up using your email
3. Go to `Your Authtoken` section
4. Click "Show Authtoken" and copy the command
5. On your VPS terminal, paste the authtoken command:
```bash
ngrok config add-authtoken YOUR_TOKEN_HERE
```
6. Start Ngrok tunnel:
```bash
ngrok http 3000
```
7. Use the generated Ngrok URL (e.g., `https://abc123.ngrok.io`) to:
   - Access the Gynsyn page
   - Authorize with your Google account

### 3. Create Swarm Manager Script  
We will create a file named `swarm.sh` and paste the script into it.  

1️⃣ Open another terminal 

2️⃣ Type the following command to create and open a new file:  
```bash  
nano swarm.sh  
```  

3️⃣ Copy and paste the contents of the Swarm Node Manager script into the file.  

4️⃣ After pasting, save the file:  
- Press `CTRL + X` to exit  
- Press `Y` to confirm saving changes  
- Press `Enter` to finalize  

🔑 Make the script executable:  
```bash  
chmod +x swarm.sh  
```  

▶️ Run the script:  
```bash  
./swarm.sh  
```  
You will see a menu with options to install, remove, or exit.  

---

## 🛠️ Troubleshooting  
🔹 **"Permission Denied" Error**  
If you get a "Permission denied" error when trying to run `swarm.sh`:  
```bash  
chmod +x swarm.sh  
./swarm.sh  
```  

🔹 **Installation Issues (Python, Node.js, Yarn)**  
If you see "unable to locate package":  
```bash  
sudo apt update && sudo apt upgrade -y  
```  
Then retry running the script.  

🔹 **Exiting the Script**  
Press `CTRL + C` or select "Exit" from the menu.  

---

## ⚠️ Important Notes  
- Does NOT remove essential software (Docker/Python/Node.js)  
- Only deletes Swarm-specific files during removal  
- Store your [HuggingFace Token](https://huggingface.co/settings/tokens) securely  

---

## 🎯 What's Next?  
Check your Swarm session:  
```bash  
screen -r swarm  
```  
If you see `"Hello, [Your Node Name]"`, your node is active!  

✅ **Enjoy running your Swarm Node effortlessly!**  

📌 **Follow for updates:** [@Ceejay1746756](https://twitter.com/Ceejay1746756)  
```

