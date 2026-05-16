# 🇮🇳 BharatBoli AI — Vercel पर Deploy कैसे करें

## आपको क्या चाहिए
- GitHub account (free) → github.com
- Vercel account (free) → vercel.com  
- आपकी Anthropic API Key

---

## Step 1 — GitHub पर Code Upload करें

1. **github.com** पर जाएं → Login करें
2. ऊपर **"+"** button दबाएं → **"New repository"** चुनें
3. Name दें: `bharatboli` → **"Create repository"** दबाएं
4. अपने computer पर यह सारी files एक folder में रखें
5. GitHub की instructions follow करके files upload करें  
   (या GitHub Desktop app use करें — आसान है)

---

## Step 2 — Vercel पर Deploy करें

1. **vercel.com** पर जाएं → **"Sign Up"** → GitHub से login करें
2. **"Add New Project"** दबाएं
3. अपना `bharatboli` repository चुनें → **"Import"** दबाएं
4. Framework: **Vite** automatically detect होगा
5. ⚠️ **"Environment Variables"** section में जाएं:
   - Name: `ANTHROPIC_API_KEY`
   - Value: आपकी actual API key paste करें (जैसे `sk-ant-...`)
6. **"Deploy"** दबाएं — 2 मिनट में done!

---

## Step 3 — Link मिलेगा और Share करें!

Deploy होने के बाद Vercel आपको एक link देगा जैसे:
```
https://bharatboli.vercel.app
```

**यह link WhatsApp पर भेजें** — दोस्त mobile में खोलेंगे तो बिल्कुल app जैसा दिखेगा! 🎉

---

## ✅ Security — API Key Safe कैसे है?

पहले: Browser → सीधे Anthropic (❌ Key expose होती थी)  
अब:   Browser → आपका Vercel Server → Anthropic (✅ Key server पर छुपी है)

---

## 📱 WhatsApp में कैसे दिखेगा?

दोस्त link खोलेंगे तो:
- पूरी screen पर WhatsApp जैसा UI दिखेगा
- 10 भारतीय भाषाओं में chat कर सकेंगे
- बिल्कुल native app जैसा feel

---

## ❓ कोई problem हो तो

Vercel का "Logs" section देखें → वहाँ error details मिलेंगी।
API Key गलत हो तो Vercel Settings → Environment Variables में update करें।
