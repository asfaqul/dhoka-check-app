# ধোঁকা চেক (Dhoka Check)

A Bangla scam checker for Bangladeshi users. Paste a suspicious SMS, link, phone number, or screenshot, and get an instant verdict in Bangla: safe, suspicious, or shows scam signs.

> ⚠️ This is an automated aid, not a guarantee. When in doubt, contact the official organization directly.

## Screenshots

| Check screen | Result screen |
|---|---|
| ![Check screen](screenshots/check.png) | ![Result screen](screenshots/result.png) |

## What it does

- **Scam check:** paste text or upload a screenshot and get an AI-based verdict with red flags and safe next steps, all in Bangla.
- **Number lookup:** search a phone number to see how many users reported it.
- **Report scams:** submit a number or link with a category (bKash/Nagad, bank, job offer, lottery, loan app).
- **Shareable card:** share "I avoided a scam" without exposing private message content.
- **Family mode:** forward a suspicious message to a family member via WhatsApp.
- **Learn tab:** short tips for spotting common scams in Bangladesh.

## Tech stack

- [React / Vite, or whatever AI Studio generated]
- Google Gemini API for message analysis
- [Firebase / localStorage] for reports

## How to run locally

**Requirements:** Node.js 18 or newer.

1. Clone the repo:
   ```bash
   git clone https://github.com/asfaqul/dhoka-check.git
   cd dhoka-check
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a file named `.env.local` in the project root and add your Gemini API key:
   ```
   GEMINI_API_KEY=your_key_here
   ```
   Get a key from [Google AI Studio](https://aistudio.google.com/). **Never commit this file.**
4. Start the app:
   ```bash
   npm run dev
   ```
5. Open the local address shown in the terminal (usually `http://localhost:5173`).

## Privacy

Messages are sent to the Gemini API for analysis and are not stored unless the user chooses to report them.

## Roadmap

- [ ] Real-time SMS scanning (Android app)
- [ ] Family alerts
- [ ] Backend for the community scam-number database
- [ ] Verified-report system to prevent false accusations

## License

[All rights reserved]
