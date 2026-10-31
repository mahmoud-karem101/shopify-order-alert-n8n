# Message to send + the 15-minute questions

## The message (WhatsApp / Messenger to your brother's friend)

> Hi [Name] — I built a small thing and I'd like to show it to you, it'll take 5 minutes.
>
> Right now when someone orders from your site, you find out when you open the admin.
> I built an alert that pings you on Telegram the second an order comes in — name,
> address, item, order ID — and logs it to a sheet. It also makes sure you get **one**
> message per order, even if the site sends it twice.
>
> Can I show you a 90-second video? If it looks useful, I'll set it up on your real store
> as a **two-week pilot**. If it doesn't save you time, we delete it. No cost, no risk.

Attach: `media/demo.mp4`.

## Then ask these three questions (15 minutes, on his phone)

1. **How do orders reach you today?** — Website form, WhatsApp, DMs, phone calls? Where
   does an order actually land, and what do you check first?
2. **What eats your time?** — Which part of the order process is the most annoying or the
   slowest? (Confirming, copying addresses, chasing payments, stock?)
3. **How many COD orders get refused or never confirmed?** — Roughly what share don't get
   answered, and why? (Wrong number, no answer, changed mind, delivery fee surprise?)

## Why these three

- Q1 tells me whether the webhook is even the right entry point, or whether orders really
  arrive on WhatsApp.
- Q2 decides what I build next — the low-stock alert only matters if stock is his pain.
- Q3 is the money question: refusals are where a fast confirmation alert pays for itself.

## The offer

> Two-week pilot. If it doesn't save you time, we delete it.

## After a yes

1. He creates a **Shopify app in his own account**, read-only permissions.
2. Swap the Webhook for a **Shopify Trigger** (`orders/create`).
3. Then build the **low-stock alert**, then the **WhatsApp FAQ bot**.
