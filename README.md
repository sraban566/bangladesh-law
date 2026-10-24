# Bangladesh Law 🇧🇩 — Digital Legal Assistant Knowledge Base

**📦 GitHub**: https://github.com/sraban566/bangladesh-law

বাংলাদেশের আইন নিয়ে তৈরি একটি **AI-রেডি নলেজ বেস** — Claude, ChatGPT, Kimi সহ যেকোনো AI প্ল্যাটফর্মে লোড করলেই সেটি একজন **ডিজিটাল আইন সহকারী** হিসেবে কাজ করবে।

An AI-ready knowledge base of Bangladeshi law. Load it into Claude, ChatGPT, Kimi, or any AI platform — and it becomes a **digital legal assistant** that can explain your rights, guide victims, and check business compliance in plain Bangla or English.

> ⚠️ **দাবিত্যাগ / Disclaimer**: এই রিপোজিটরি ও এ থেকে তৈরি যেকোনো AI সহকারী **আইনজীবী নয়**। এটি শুধুমাত্র সাধারণ তথ্য ও পদ্ধতি জানায় — আইনি পরামর্শ নয়। নির্দিষ্ট মামলার জন্য সর্বদা লাইসেন্সপ্রাপ্ত অ্যাডভোকেটের পরামর্শ নিন এবং অফিসিয়াল সূত্র (https://bdlaws.minlaw.gov.bd) যাচাই করুন।

## 🤖 AI প্ল্যাটফর্মে ইনস্টল করুন

| প্ল্যাটফর্ম | গাইড | সময় |
|---|---|---|
| **Claude** (Projects / Claude Code / Skill) | [install/claude.md](install/claude.md) | ~৫ মিনিট |
| **ChatGPT** (Custom GPT / Instructions) | [install/chatgpt.md](install/chatgpt.md) | ~৫ মিনিট |
| **Kimi** (সেশন / Skill / Plugin) | [install/kimi.md](install/kimi.md) | ~৫ মিনিট |

AI-কে কীভাবে আচরণ করতে হবে তা লেখা আছে [`SKILL.md`](SKILL.md) ও [`AGENTS.md`](AGENTS.md)-এ — এই দুটো ফাইলই "ডিজিটাল আইনজীবী" ব্যবহারকে নিরাপদ, সঠিক ও সহায়ক করে তোলে।

### এক লাইনে শুরু (যেকোনো AI-তে)

```
https://github.com/sraban566/bangladesh-law — এই repo-র SKILL.md অনুসরণ করে
বাংলাদেশের আইন বিষয়ে ডিজিটাল আইন সহকারী হিসেবে কাজ করো।
```

এই মেসেজটা + repo-র ফাইলগুলো যেকোনো AI চ্যাটে দিলেই ডিজিটাল আইন সহকারী চালু।

## 🆘 ভুক্তভোগী? এখান থেকে শুরু করুন

| পরিস্থিতি | গাইড |
|---|---|
| ঠকানো হয়েছে / প্রতারণার শিকার | [guides/victims/what-to-do-if-cheated.md](guides/victims/what-to-do-if-cheated.md) |
| FIR বা GD করতে চান | [guides/victims/how-to-file-fir-gd.md](guides/victims/how-to-file-fir-gd.md) |
| ফ্রি আইনি সাহায্য ও হেল্পলাইন (999, 109, 16430…) | [guides/victims/legal-aid-helplines.md](guides/victims/legal-aid-helplines.md) |

## 🏢 ব্যবসায়ী? আপনার ব্যবসা legal কিনা চেক করুন

| প্রয়োজন | গাইড |
|---|---|
| ব্যবসার legality চেকলিস্ট (ট্রেড লাইসেন্স, TIN, VAT, শ্রম আইন) | [guides/business/business-legality-checklist.md](guides/business/business-legality-checklist.md) |
| কোম্পানি রেজিস্ট্রেশন (RJSC) ধাপে ধাপে | [guides/business/company-registration.md](guides/business/company-registration.md) |
| দলিল/কোম্পানি যাচাই — জালিয়াতি থেকে বাঁচুন | [guides/business/verify-deed-and-company.md](guides/business/verify-deed-and-company.md) |

## 📂 পূর্ণ কাঠামো

```
bangladesh-law/
├── SKILL.md               # AI-এর জন্য মূল নির্দেশনা (digital lawyer persona)
├── AGENTS.md              # AI agent-দের জন্য সংক্ষিপ্ত নিয়ম
├── install/               # Claude / ChatGPT / Kimi install গাইড
├── guides/
│   ├── victims/           # ভুক্তভোগীদের জন্য ধাপে ধাপে গাইড
│   └── business/          # ব্যবসার legality চেকলিস্ট ও যাচাই
├── constitution/          # সংবিধান, সংশোধনী, মৌলিক অধিকার
├── codes/                 # Penal Code, CrPC, CPC, Evidence Act (ধারাভিত্তিক)
├── acts/                  # শ্রম, পারিবারিক, সাইবার, ভূমি, নারী-শিশু আইন
├── judgments/             # ১০টা landmark রায় (facts, issues, ratio সহ)
├── resources/             # অফিসিয়াল সূত্র, আদালতের কাঠামো
└── data/laws-index.json   # মেশিন-রিডেবল আইনের ইনডেক্স
```

## 📖 বিস্তারিত আইনি নোট

| Document | Description |
|----------|-------------|
| [Penal Code, 1860](codes/penal-code-1860.md) | খুন, চুরি, প্রতারণা, মানহানি — ধারাভিত্তিক |
| [CrPC, 1898](codes/crpc-1898.md) | FIR থেকে আপিল — arrest, remand, bail, s. 561A |
| [CPC, 1908](codes/cpc-1908.md) | মামলা দায়ের থেকে ডিক্রি জারী |
| [Evidence Act, 1872](codes/evidence-act-1872.md) | স্বীকারোক্তি, সাক্ষ্য, জেরা |
| [Labour Act, 2006](acts/labour/labour-act-2006.md) | নিয়োগপত্র, ছুটি, ওভারটাইম, ম্যাটার্নিটি |
| [Fundamental Rights](constitution/fundamental-rights.md) | Article 26–47A ম্যাপ |
| [Landmark Judgments](judgments/README.md) | 8th/5th/7th/13th/16th Amendment, PIL, Masdar Hossain |

## 📜 অফিসিয়াল সূত্র

- **Laws of Bangladesh**: https://bdlaws.minlaw.gov.bd
- **Supreme Court**: https://supremecourt.gov.bd | **RJSC**: https://rjsc.gov.bd | **NBR**: https://nbr.gov.bd

## 🤝 Contributing

ভুল পেলে, নতুন আইন/সংশোধনী যোগ করতে চাইলে — [CONTRIBUTING.md](CONTRIBUTING.md) পড়ে PR দিন। প্রতিটা এন্ট্রি অবশ্যই অফিসিয়াল সূত্রসহ।

## 📄 License

[CC0 1.0](LICENSE) — বাংলাদেশের আইন জনস্বার্থে উন্মুক্ত; এই repo-র সামারি ও গাইড পাবলিক ডোমেইনে।
