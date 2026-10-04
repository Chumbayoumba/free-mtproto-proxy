# 🔓 Free MTProto Proxy — Stable, Daily Updated

<!-- GIVEAWAY:START -->
<a href="https://t.me/vnespiskabot?start=gw_github"><img src="https://vnespiska.win/gw/img/giveaway-4x1.webp" alt="Giveaway: 3 × 90 days, 7 × 30 days of VPN, 30 × 20% discounts" width="100%"></a>

> 🎁 **Giveaway until 10 October, 20:00 MSK:** 3 × 90-day and 7 × 30-day VPN subscriptions, 30 × 20% discounts. Free to enter in Telegram: **[join →](https://t.me/vnespiskabot?start=gw_github)** · +1 ticket per invited friend
<!-- GIVEAWAY:END -->

> Free public MTProto proxy for Telegram. Server in NL, fake-TLS, no logs.
> Works in regions where Telegram is throttled or blocked.

[![WEB Proxy](https://img.shields.io/badge/NEW-WEB%20Proxy-7c3aed?logo=telegram)](https://vnespiska.win/webproxy/)
[![Update](https://img.shields.io/badge/last%20update-auto-brightgreen)](./all_proxies.txt)
[![Uptime](https://img.shields.io/badge/uptime-99%25-blue)](https://vnespiska.win)
[![Channel](https://img.shields.io/badge/Telegram-@vnespiska-26A5E4)](https://t.me/vnespiska)
[![Mirror](https://img.shields.io/badge/mirror%20(RU)-goida.win-success)](https://goida.win/)

## ⚡ Working proxies right now — checked from Russia

Tap **⚡ Connect** on a device with Telegram installed. The list is refreshed automatically every 2 hours and contains only proxies that connected from a Russian server.

<!-- UPDATED:START -->
> 🟢 **Обновлено: 04.10.2026 18:21 МСК** · рабочих прокси: **3** · каждый проверен подключением с российского сервера
<!-- UPDATED:END -->

> 🖥 **On a computer? Use our WEB proxy** (Telegram Desktop 7.1.1+): Telegram traffic looks like ordinary HTTPS, so it is harder to block. **[Connect in one click →](https://vnespiska.win/webproxy/)** · server `free.vnespiska.win` · secret `9fc8d7d1aeee614bd5fa3b760da44dd3` · type **WEB**


<!-- LIVE:START -->
| # | Сервер | Порт | Пинг из РФ | Подключить |
|---|--------|------|-----------|------------|
| 1 | `edge.turboass.live` | `443` | 🟢 79 мс | **[⚡ Подключить](https://t.me/proxy?server=edge.turboass.live&port=443&secret=ee51116f4018a2b3dfc9bda286c52afe9f656467652e747572626f6173732e6c697665)** |
| 2 | `host.white-dns.info` | `443` | 🟡 93 мс | **[⚡ Подключить](https://t.me/proxy?server=host.white-dns.info&port=443&secret=ee3e85aac6e7bcc0ba3847479bff8ef2a4)** |
| 3 | `193.39.15.115` | `443` | 🟢 58 мс | **[⚡ Подключить](https://t.me/proxy?server=193.39.15.115&port=443&secret=dd585256032fd8a78a0602ddd90f9c981f)** |
<!-- LIVE:END -->

> 📢 Free proxies live for hours, not weeks. **Fresh ones every hour in the Telegram channel [@vnespiska](https://t.me/+FhRJPseOXOszZGM6)** (~4 000 subscribers), or get one instantly from the bot **[@vnespiskabot](https://t.me/vnespiskabot?start=proxy_notify_gh_en)**.
>
> 🛑 Telegram doesn't work even with a proxy (mobile internet white lists in Russia)? → **[VPN in @vnespiskabot](https://t.me/vnespiskabot?start=promo_VNESPISKA_gh_en)**: Basic plan free forever, Premium 239 ₽ with promo code `VNESPISKA`.

## 🆕 WEB proxy for Telegram Desktop — free

Since August 2026 **Telegram Desktop 7.1.1+** supports a new proxy type, **WEB**: Telegram traffic travels over plain HTTPS/WebSocket like an ordinary website, which makes it much harder to detect and block. The proxy never sees your messages, it only relays already encrypted data.

👉 **[CONNECT THE WEB PROXY](https://vnespiska.win/webproxy/)** (the button opens Telegram Desktop)

| Field | Value |
|-------|-------|
| **Type** | `WEB` |
| **Server** | `free.vnespiska.win` |
| **Secret** | `9fc8d7d1aeee614bd5fa3b760da44dd3` |
| **Client** | Telegram Desktop 7.1.1+ (Windows, macOS, Linux) |

Link for Telegram Desktop (paste it into Saved Messages and click it there):

```
tg://webproxy?server=free.vnespiska.win&secret=9fc8d7d1aeee614bd5fa3b760da44dd3
```

> ⚠️ Do not open `t.me/webproxy?…` in a browser: t.me does not know this link type yet and shows an unrelated channel. Stable mobile apps do not support WEB proxies yet (only Telegram beta builds do), use the MTProto proxy above.

---

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

→ https://vnespiska.win
→ https://goida.win (mirror that opens without VPN in Russia)

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

**How do I check what's blocked at my ISP?** Run a free in-browser block
test (Cheburnet Connect): https://glushilok.net/proverka/ — it shows which
services are unreachable on your network and whether DPI/TSPU is present.

**Will it die?** It's been running since 2025. If it ever does,
[vnespiska.win](https://vnespiska.win) always has 5–10 fresh validated
backups.

## 🤝 Want to share?

Star this repo, share the proxy link, or post it on your channel —
that's how the network grows.

## 📝 License

Public proxy. Use at your own discretion. The list is provided as-is
with no warranty.

## 🔗 Links

- Mirror not blocked in Russia: https://goida.win — Telegram proxy + VPN, whitelist bypass (RU)
- Site (RU): https://glushilok.net — free Telegram proxy + VPN, block checker
- Check what's blocked for you: https://glushilok.net/proverka/
- Guides (VLESS, Hiddify, routers): https://glushilok.net/guides/
- Site: https://vnespiska.win
- Channel: https://t.me/vnespiska
- Bot: https://t.me/vnespiskabot
- Official MTProxy: https://github.com/TelegramMessenger/MTProxy
