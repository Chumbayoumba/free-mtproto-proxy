# 🔓 Free MTProto Proxy — Stable, Daily Updated

> Free public MTProto proxy for Telegram. Server in NL, fake-TLS, no logs.
> Works in regions where Telegram is throttled or blocked.

[![Update](https://img.shields.io/badge/last%20update-auto-brightgreen)](./all_proxies.txt)
[![Uptime](https://img.shields.io/badge/uptime-99%25-blue)](https://vnespiska.uk)
[![Channel](https://img.shields.io/badge/Telegram-@vnespiska-26A5E4)](https://t.me/vnespiska)

## ⚡ Quick start

Tap on your phone — Telegram will offer to add the proxy automatically:

`tg://proxy?server=free.vnespiska.org&port=9443&secret=ee5b1977cd65b2b90aeea9a53a8d1120867461736b666c6f772e65676f722d6465762e7275`

Or copy parameters manually:

| Field | Value |
|---|---|
| Server | `free.vnespiska.org` |
| Port | `9443` |
| Secret | `ee5b1977cd65b2b90aeea9a53a8d1120867461736b666c6f772e65676f722d6465762e7275` |
| Type | MTProto (fake-TLS) |

## 📋 What's inside

- [`all_proxies.txt`](./all_proxies.txt) — primary proxy in standard TG format
- [`README.md`](./README.md) — this file

## 🌍 Why MTProto over VPN

| Feature | MTProto | VPN |
|---|---|---|
| Affects | Telegram only | All traffic |
| Speed | 90–100% native | 50–80% native |
| DPI evasion | fake-TLS (looks like HTTPS) | obvious |
| Setup | 1 tap | install app |
| Cost | Free | Often paid |

## 🛠 Run your own (5 min on any VPS)

```bash
git clone https://github.com/TelegramMessenger/MTProxy
cd MTProxy && make
cd objs/bin
curl -s https://core.telegram.org/getProxySecret -o proxy-secret
curl -s https://core.telegram.org/getProxyConfig -o proxy-multi.conf
SECRET=$(head -c 16 /dev/urandom | xxd -ps)
./mtproto-proxy -u nobody -p 8888 -H 443 -S $SECRET \
  --aes-pwd proxy-secret proxy-multi.conf -M 1
```

## 🆘 Backup proxies

If port 9443 is blocked at your ISP, ~10 backup proxies on different
servers and ports, auto-validated every 30 minutes:

→ https://vnespiska.uk

## 📡 Sponsor channel

This proxy has a sponsor channel attached: [@vnespiska](https://t.me/vnespiska).
That's how MTProto works in Telegram — proxy owners can pin a single
channel to appear in users' chat list. You can ignore it; you can't
unsubscribe without removing the proxy. The channel posts proxy updates,
new servers, and bypass tips. No spam.

## ❓ FAQ

**Is it safe?** The proxy sees only encrypted Telegram traffic, same
as any router on the path. It cannot decrypt messages — that's done by
Telegram's servers using your client's keys.

**Will logs be kept?** No logs are stored on this proxy. We can't
guarantee 100% (no third-party can — by definition), so for highly
sensitive workflows, run your own with the snippet above.

**Why is it free?** Because the sponsor channel mechanism organically
grows the channel. The marginal cost of additional users is near zero
on a $5/mo VPS.

**Will it die?** It's been running since 2025. If it ever does,
[vnespiska.uk](https://vnespiska.uk) always has 5–10 fresh validated
backups.

## 🤝 Want to share?

Star this repo, share the proxy link, or post it on your channel —
that's how the network grows.

## 📝 License

Public proxy. Use at your own discretion. The list is provided as-is
with no warranty.

## 🔗 Links

- Site: https://vnespiska.uk
- Channel: https://t.me/vnespiska
- Bot: https://t.me/vnespiskabot
- Official MTProxy: https://github.com/TelegramMessenger/MTProxy
