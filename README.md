# Billions-network-Verified-Agent-test
# 💠 Verified Agent Identity — Easy Setup Guide

### Step-by-Step Guide (Beginner Friendly)

This guide shows how to set up your **Verified Agent Identity** using GitHub Codespaces.

---

## 📌 What You Need To Do

We will:
1. Create a GitHub repo  
2. Open Codespaces  
3. Run commands step-by-step  
4. Verify your identity  

---

## 🧱 Step 1 — Create Repository

1. Go to https://github.com  
2. Click **New Repository**  
3. Name it:
   ```
   verified-agent-identity
   ```
4. Enable:
   ✅ Add README file  
5. Click **Create Repository**

---

## 💻 Step 2 — Open Codespaces

1. Open your repo  
2. Click **Code (green button)**  
3. Click **Codespaces tab**  
4. Click **Create codespace on main**

> ⏳ Wait for terminal to load

---

## ⚙️ Step 3 — Run Commands

Now in terminal, run these **one by one**

---

### Clone Official Repo
```
git clone https://github.com/BillionsNetwork/verified-agent-identity
```

---

### Enter Folder
```
cd verified-agent-identity
```

---

### Install Packages
```
npm install shell-quote @iden3/js-iden3-auth @0xpolygonid/js-sdk ethers uuid cross-fetch
```

---

### Go to Scripts
```
cd scripts
```

---

### Create Identity
```
node createNewEthereumIdentity.js
```

👉 Save your output (wallet + DID)

---

### Link Identity
```
node manualLinkHumanToAgent.js --challenge '{"name":"YourName","description":"Your Agent"}'
```

---

### Install Skill
```
npx clawhub@latest install verified-agent-identity
```

---

### Add Skill
```
npx skills add BillionsNetwork/verified-agent-identity
```

👉 Type `y` and press Enter

---

### Check Private Key ⚠️
```
cat ~/.openclaw/billions/kms.json
```

❗ Keep this safe. Do NOT share.

---

## ✅ Step 4 — Verify

Check here:

https://attestations-explorer.billions.network/

Paste your wallet or DID.

---

## ⚡ All Commands (Quick Copy)

```
git clone https://github.com/BillionsNetwork/verified-agent-identity
cd verified-agent-identity
npm install shell-quote @iden3/js-iden3-auth @0xpolygonid/js-sdk ethers uuid cross-fetch
cd scripts
node createNewEthereumIdentity.js
node manualLinkHumanToAgent.js --challenge '{"name":"YourName","description":"Your Agent"}'
npx clawhub@latest install verified-agent-identity
npx skills add BillionsNetwork/verified-agent-identity
cat ~/.openclaw/billions/kms.json
```

---

## ❗ Important Notes

- Always run commands in order  
- Wait for each step to finish  
- Save your wallet + DID  
- Never share private key  

---

## 🔗 Useful Links

- Official: https://billions.network/verified-agent-identity-skill-openclaw  
- GitHub Repo: https://github.com/BillionsNetwork/verified-agent-identity  
- Explorer: https://attestations-explorer.billions.network/  

---

## ✍️ Made by

Kbin
