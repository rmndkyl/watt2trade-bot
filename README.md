# Watt2Trade Bot

**Versi:** 1.0.0 · **Harga:** Rp 100.000 (~$6) · **Kontak pembelian:** [@rmndkyl](https://t.me/rmndkyl)

Script otomasi Watt2Trade Bot untuk workflow LYID.

## Kebutuhan

| Item | Detail |
|---|---|
| Runtime | Node.js 18+ |
| Wallet | EVM / sesuai chain proyek (kamu sendiri) |
| Proxy | opsional (1 proxy per akun) |
| Captcha | tidak perlu |
| Akses | akun proyek yang kamu kelola sendiri |

## Pembayaran

E-Wallet: DANA / GoPay / ShopeePay · Bank: BCA / Seabank · Crypto: contact for wallet address.
Pembeli menghubungi [@rmndkyl](https://t.me/rmndkyl), kirim bukti transfer, lalu terima license key.

---

## Project Info
- **Project:** Watt2Trade ($WATTOIN)
- **Chain:** L1
- **Funding:** $1.55M (ParisBlock, Alphabot)
- **Total Rewards:** $4,000,000
- **Website:** https://www.watt2trade.com/
- **Dashboard:** https://rewards.watt2trade.com/

## Features
- Multi-wallet support (6 wallets)
- Proxy rotation
- Wallet signature auth (REST → JWT cookie)
- Task automation (social: like, retweet, follow, join)
- User info & points display
- Daily auto-run mode (--daily flag)
- Interactive CLI menu

## Requirements
- Node.js v18+
- npm install

## Usage
```bash
npm install
node index.js          # Interactive menu
node index.js --daily  # Daily auto-run
```

## Menu Options
1. Show User Info & Points (all wallets)
2. Complete Tasks (all wallets)
3. Run All (Info + Tasks)
4. Revalidate Token
5. Exit

## Auth Flow
1. POST /generate-nonce → get nonce + message
2. Sign message with ethers.js
3. POST /verify-signature → get refresh_token cookie
4. Use cookie for all authenticated requests

## Config
Edit `config.json` for delays, retry, proxy settings.

## ⚠️ Notes
- Social tasks (like/retweet/follow) may require actual Twitter/Telegram interaction first
- Bot calls /verify-task to claim points after social action completed
- Trading WXP points are NOT automatable (requires actual trades)

## Support
- Telegram: @layerairdrop
- Discord: discord.gg/ZK2NVkfSNn
- GitHub: github.com/layerairdrop

---
© Layer Airdrop ID (LYID)

## 💰 Harga

| Lisensi | Harga | Fitur |
|---------|-------|-------|
| **Single** | Rp 100.000 / ~$6 | 1 device, lifetime |
| **Bundle (3 bot)** | Rp 100.000 / ~$16 | Pilih 3 bot, hemat 20% |
| **Pro (semua bot)** | Rp 100.000 / ~$70 | Semua bot + update, hemat 30% |

**Cara beli:** Chat [@OG_LYID_bot](https://t.me/OG_LYID_bot) di Telegram → /buy

**Bayar pakai:**
- 🇮🇩 DANA / GoPay / ShopeePay / BCA / Seabank
- 🌐 Crypto (USDT/SOL/ETH)

## 🔧 Troubleshooting

| Masalah | Solusi |
|---------|--------|
| `Cannot find module` | Jalankan `npm install` di folder bot |
| `insufficient balance` | Pastikan wallet punya cukup token untuk gas |
| `429 Too Many Requests` | Tunggu 30-60 detik, bot auto-retry |
| Bot diam/tidak jalan | Cek `config.json` — pastikan API key valid |
| License invalid | Chat [@OG_LYID_bot](https://t.me/OG_LYID_bot) → /verify |

**Butuh bantuan?** Join [Discord](https://discord.gg/ZK2NVkfSNn) atau chat [@layerairdrop](https://t.me/layerairdrop)
