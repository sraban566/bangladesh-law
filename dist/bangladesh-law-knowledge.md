# Bangladesh Law — Combined Knowledge Base



---

<!-- FILE: SKILL.md -->

---
name: bangladesh-law-assistant
description: Digital legal information assistant for Bangladesh law. Use when the user asks about Bangladeshi laws, legal rights, business legality/compliance, what to do when cheated or in legal trouble, company/deed verification, FIR/GD filing, or any question about the legal system of Bangladesh. NOT a lawyer — provides information, procedures, and referrals only.
---

# Bangladesh Digital Legal Assistant

You are a **digital legal information assistant** for the laws of Bangladesh. This skill's knowledge base contains the Constitution, major codes, acts by category, landmark judgments, practical guides for victims, and business-compliance checklists.

## Your role

- Help ordinary people — especially those who don't know the legal system — understand their **rights, options, and next steps**.
- Help small business owners check **whether their business/deed/activity is legal** and what registrations or licenses they need.
- Point victims to the **right forum, helpline, and procedure** (FIR, GD, legal aid, consumer protection).

## Hard rules (never break)

1. **You are NOT a lawyer.** Never present your answer as legal advice. Every substantive legal answer must end with a short recommendation to consult a licensed advocate for the specific case.
2. **Never invent laws, sections, case names, or citations.** If unsure, say so and direct the user to the official database: https://bdlaws.minlaw.gov.bd
3. **Emergencies first.** If someone is in immediate danger, lead with emergency numbers (999 police, 109 women/children, 1098 child helpline) before any explanation.
4. **Language**: reply in the user's language. If they write in Bangla or Banglish, reply in Bangla (simple, non-technical words; explain legal terms in brackets).
5. **No political commentary.** Summarize law factually and neutrally.
6. **Mark time-sensitive content.** Laws change — where relevant say "verify the current version at bdlaws.minlaw.gov.bd".

## Answer structure

For every legal question, answer in this order:

1. **সংক্ষিপ্ত উত্তর** — one or two sentences, plain language
2. **কোন আইন/ধারা** — the relevant act/section (cite from the knowledge base; never invent)
3. **আপনি কী করবেন** — concrete step-by-step action list (which office, which form, which helpline)
4. **সতর্কতা** — deadline/limitation risks, common traps
5. **দাবিত্যাগ** — "এটি সাধারণ তথ্য, আইনি পরামর্শ নয় — নির্দিষ্ট মামলার জন্য একজন আইনজীবীর সাথে কথা বলুন।"

## Knowledge base map

| Topic | Location |
|-------|----------|
| Constitution & fundamental rights | `constitution/` |
| Penal Code, CrPC, CPC, Evidence Act (section-wise) | `codes/` |
| Labour, family, cyber, land, women-children laws | `acts/` |
| Landmark judgments (facts/issues/ratio) | `judgments/` |
| Victim guides (cheated? FIR/GD? helplines) | `guides/victims/` |
| Business legality & compliance checklists | `guides/business/` |
| Official sources, court structure, legal aid | `resources/` |
| Machine-readable law index | `data/laws-index.json` |

## Common situations → where to look

- "আমাকে ঠকিয়েছে / প্রতারণা করেছে" → `guides/victims/what-to-do-if-cheated.md`
- "FIR/GD কীভাবে করব" → `guides/victims/how-to-file-fir-gd.md`
- "ফ্রি আইনি সাহায্য কোথায় পাব" → `guides/victims/legal-aid-helplines.md`
- "আমার ব্যবসা legal কিনা" → `guides/business/business-legality-checklist.md`
- "কোম্পানি রেজিস্ট্রেশন কীভাবে" → `guides/business/company-registration.md`
- "দলিল ঠিক আছে কিনা" → `guides/business/verify-deed-and-company.md`



---

<!-- FILE: AGENTS.md -->

# AGENTS.md — Bangladesh Law Knowledge Base

If you are an AI agent working with this repository, you are a **digital legal information assistant for Bangladesh law**. Read `SKILL.md` first — it defines your role, hard rules, and answer structure.

Key constraints:

1. Not legal advice — always refer to a licensed advocate.
2. Never invent laws, sections, or citations. Official source: https://bdlaws.minlaw.gov.bd
3. Emergencies first: 999 / 109 / 1098 / 16121 (consumer) / 16430 (legal aid).
4. Reply in the user's language (Bangla by default for Bangla/Banglish users).
5. When editing this repo: accuracy first, every entry links to an official source, neutral tone, no legal advice in content.



---

<!-- FILE: README.md -->

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



---

<!-- FILE: guides/victims/what-to-do-if-cheated.md -->

# আমাকে ঠকানো হয়েছে — এখন কী করব? / What to Do If You've Been Cheated

প্রতারণার শিকার হলে আতঙ্কিত হওয়া স্বাভাবিক। এই গাইড ধাপে ধাপে বলছে কী করবেন।

## ধাপ ০: নিরাপত্তা আগে

- জীবনের ঝুঁকি বা চলমান হুমকি থাকলে এখনই কল করুন: **999** (জাতীয় জরুরি সেবা)
- নারী/শিশু নির্যাতন হলে: **109** | শিশু সংক্রান্ত: **1098**

## ধাপ ১: প্রমাণ সংগ্রহ করুন (সবচেয়ে জরুরি)

যা যা জমা রাখুন:

- চুক্তিপত্র, রশিদ, মানি রিসিপ্ট, দলিল, চেক, ব্যাংক স্টেটমেন্ট
- SMS, WhatsApp/Messenger চ্যাট, ইমেইল, কল রেকর্ডের স্ক্রিনশট (স্ক্রিনশটে তারিখ দেখা যাক)
- প্রতারকের নাম, ঠিকানা, ফোন নম্বর, NID/ব্যবসার নাম (যতটুকু জানেন)
- সাক্ষীদের নাম ও ফোন

> ⚠️ মূল কাগজ কাউকে দিবেন না — ফটোকপি দিন, মূল নিজের কাছে রাখুন।

## ধাপ ২: প্রথমে সাধারণ ডায়েরি (GD) — ঐচ্ছিক কিন্তু কার্যকর

নিকটস্থ থানায় গিয়ে **GD** করুন (নিরাপত্তা/প্রমাণের জন্য)। GD-র কপি সঙ্গে নিন। বিস্তারিত: [how-to-file-fir-gd.md](how-to-file-fir-gd.md)

## ধাপ ৩: কোন ধরনের প্রতারণা — সেই অনুযায়ী আইনি পথ

| পরিস্থিতি | প্রযোজ্য আইন (সাধারণত) | কোথায় যাবেন |
|---|---|---|
| টাকা ধার দিয়ে ফেরত দিচ্ছে না | দেওয়ানি মামলা (CPC 1908); Artha Rin Ain (ব্যাংক/আর্থিক প্রতিষ্ঠান) | দেওয়ানি আদালত |
| চেক ডিসঅনার (চেক বাউন্স) | NI Act 1881, ধারা 138 — ফৌজদারি মামলা | ম্যাজিস্ট্রেট আদালত (৩০ দিনের মধ্যে লিগ্যাল নোটিশ — **deadline গুরুত্বপূর্ণ**) |
| প্রতারণা করে টাকা/সম্পত্তি নেওয়া | Penal Code ধারা 420 (প্রতারণা), 406 (আমানতে খেয়ানত) | থানায় FIR |
| জাল দলিল/জমি দখল | জালিয়াতি (PC 463–471), স্থাবর সম্পত্তি মামলা | থানায় FIR + দেওয়ানি আদালত |
| পণ্য/সেবা কিনে ঠকানো | ভোক্তা অধিকার সংরক্ষণ আইন, ২০০৯ | ভোক্তা অধিকার অধিদপ্তর — হটলাইন **16121** |
| অনলাইনে প্রতারণা (e-commerce, ফেসবুক পেজ) | Penal Code + সাইবার আইন | থানায় FIR; জাতীয় জরুরি সেবা 999; প্ল্যাটফর্মে রিপোর্ট |
| বিনিয়োগ/এমএলএম/সমবায় প্রতারণা | PC 420; সমবায়/আর্থিক প্রতিষ্ঠান আইন | থানায় FIR; বাংলাদেশ ব্যাংক/সমবায় অধিদপ্তরে অভিযোগ |
| ভবন/ফ্ল্যাট ডেভেলপার ঠকালে | চুক্তি লঙ্ঘন (দেওয়ানি) + প্রতারণা (ফৌজদারি); REHAB অভিযোগ | দেওয়ানি + ফৌজদারি উভয় পথ |

## ধাপ ৪: ফ্রি আইনি সাহায্য নিন

টাকা না থাকলে বা প্রথম পরামর্শের জন্য:

- **জাতীয় আইনগত সহায়তা (NLASO)**: হটলাইন **16430** — সরকারি ফ্রি আইনি সহায়তা
- **BLAST**: https://blast.org.bd
- **Ain o Salish Kendra (ASK)**: https://askbd.org
- জেলা আইনগত সহায়তা কমিটি (প্রতিটি জেলা জজ আদালতে)

বিস্তারিত: [legal-aid-helplines.md](legal-aid-helplines.md)

## ধাপ ৫: সময়সীমা (Limitation) মাথায় রাখুন

- দেওয়ানি মামলার **সময়সীমা (limitation period)** আছে — চুক্তি ভঙ্গের মামলায় সাধারণত ৩ বছর (Limitation Act 1908)। দেরি করলে মামলাই করা যায় না।
- চেক বাউন্সে **৩০ দিনের মধ্যে নোটিশ** — একদিনও দেরি করা যাবে না।
- তাই **আজই** একজন আইনজীবীর সাথে কথা বলুন।

## কখনও করবেন না

- ❌ নিজে গিয়ে চাপ/হুমকি দেওয়া — উল্টো মামলা হতে পারে
- ❌ সোশ্যাল মিডিয়ায় নাম-ঠিকানা ফাঁস করা — মানহানির (defamation) মামলা খেতে পারেন
- ❌ "সালিসে" বা ক্ষমতাধর ব্যক্তির মাধ্যমে আপস — লিখিত রেকর্ড ছাড়া

> **দাবিত্যাগ**: এটি সাধারণ তথ্য, আইনি পরামর্শ নয়। আপনার নির্দিষ্ট পরিস্থিতির জন্য একজন লাইসেন্সপ্রাপ্ত অ্যাডভোকেটের পরামর্শ নিন।



---

<!-- FILE: guides/victims/how-to-file-fir-gd.md -->

# FIR ও GD — কীভাবে করবেন / How to File an FIR or GD

## GD (General Diary) কী?

- থানায় করা **সাধারণ লিখিত রেকর্ড** — কোনো ঘটনা/হুমকি/হারানো জিনিস পুলিশকে জানানো।
- GD তদন্ত শুরু করে না, কিন্তু **ভবিষ্যতের প্রমাণ** হিসেবে কাজ করে (যেমন হুমকি পেলে, চেক/দলিল হারালে)।

**কীভাবে করবেন:**
1. নিকটস্থ থানায় যান (অনেক থানায় অনলাইন GD-ও আছে: https://gd.police.gov.bd — যাচাই করে নিন)
2. ঘটনাটা লিখিতভাবে দিন: তারিখ, সময়, স্থান, কী ঘটেছে, কার বিরুদ্ধে
3. GD নম্বর ও **স্বাক্ষরিত কপি** সঙ্গে নিন — এটাই আপনার প্রমাণ

## FIR (First Information Report / এজাহার) কী?

- **Cognizable অপরাধ** (যেমন প্রতারণা, চুরি, ডাকাতি, মারধর, ধর্ষণ) ঘটলে পুলিশ **তদন্ত শুরু করতে বাধ্য** — এটাই FIR (CrPC ধারা 154)।

**কীভাবে করবেন:**

1. যে এলাকায় ঘটনা ঘটেছে, সেই থানায় যান
2. মৌখিকভাবে বললেও হবে — পুলিশ লিখে আপনাকে পড়ে শোনাবে, তারপর স্বাক্ষর করুন। **পড়ে না দেখে/না বুঝে স্বাক্ষর করবেন না**
3. লিখিত অভিযোগ দিলে দুই কপি নিন — একটায় থানার সিল ও FIR নম্বর নিয়ে রাখুন

## পুলিশ FIR নিতে অস্বীকার করলে?

আইনি পথ আছে:

1. **পুলিশ সুপার (SP) / Police Commissioner**-এর কাছে লিখিত অভিযোগ (CrPC ধারা 154(3))
2. তাও না হলে **ম্যাজিস্ট্রেটের কাছে অভিযোগ** (CrPC ধারা 156(3) / 200) — ম্যাজিস্ট্রেট পুলিশকে তদন্তের নির্দেশ দিতে পারেন বা সরাসরি মামলা নিতে পারেন
3. **জাতীয় জরুরি সেবা 999** বা পুলিশের অভ্যন্তরীণ অভিযোগ ব্যবস্থা ব্যবহার করতে পারেন

## মনে রাখবেন

- FIR-এ **মিথ্যা তথ্য দেওয়া অপরাধ** — যা জানেন শুধু তা-ই বলুন, অনুমান আলাদাভাবে বলুন
- FIR করার জন্য **কোনো টাকা লাগে না** — কেউ টাকা চাইলে এটা অবৈধ
- তারিখ-সময়-নাম **সঠিক** দিন; ভুল হলে পরে সংশোধন জটিল
- FIR-এর কপি **ফ্রি**-তে পাওয়ার অধিকার আপনার আছে

## সংশ্লিষ্ট আইন

- CrPC 1898: ধারা 154 (FIR), 156 (তদন্ত), 167 (রিমান্ড), 173 (চার্জশিট/ফাইনাল রিপোর্ট)
- বিস্তারিত: [../../codes/crpc-1898.md](../../codes/crpc-1898.md)

> **দাবিত্যাগ**: সাধারণ তথ্য, আইনি পরামর্শ নয় — নির্দিষ্ট মামলায় আইনজীবীর পরামর্শ নিন।



---

<!-- FILE: guides/victims/legal-aid-helplines.md -->

# ফ্রি আইনি সাহায্য ও হেল্পলাইন / Free Legal Aid & Helplines

> ⚠️ হটলাইন নম্বর সময়ের সাথে বদলাতে পারে — ব্যবহারের আগে সংশ্লিষ্ট ওয়েবসাইটে যাচাই করুন।

## জরুরি হটলাইন

| নম্বর | সেবা |
|-------|------|
| **999** | জাতীয় জরুরি সেবা (পুলিশ/ফায়ার/অ্যাম্বুলেন্স) |
| **109** | নারী ও শিশু নির্যাতন প্রতিরোধ হেল্পলাইন |
| **1098** | শিশু হেল্পলাইন |
| **16121** | ভোক্তা অধিকার অধিদপ্তর (DNCRP) — পণ্য/সেবায় প্রতারণার অভিযোগ |
| **16430** | জাতীয় আইনগত সহায়তা (NLASO) — ফ্রি আইনি পরামর্শ ও সহায়তা |
| **106** | শ্রমিক অভিযোগ (শ্রম অধিদপ্তর) — যাচাই করে নিন |

## সরকারি ফ্রি আইনি সহায়তা

- **National Legal Aid Services Organization (NLASO)** — https://nlaso.gov.bd
  - সরকারি খরচে আইনজীবী ও মামলার খরচ (আয়সীমার নিচে থাকলে)
  - প্রতিটি **জেলা লিগ্যাল এইড অফিস** (জেলা জজ আদালত চত্বরে)
  - বিচারাধীন কারাবন্দী, গরিব ভুক্তভোগী — সবাই আবেদন করতে পারেন
- আইন: **আইনগত সহায়তা প্রদান আইন, ২০০০** ও নিয়মাবলি

## বেসরকারি সংস্থা

| সংস্থা | কী সাহায্য | ওয়েবসাইট |
|--------|-----------|-----------|
| BLAST | ফ্রি আইনি সহায়তা, মামলা, পরামর্শ | https://blast.org.bd |
| Ain o Salish Kendra (ASK) | নারী/শিশু/শ্রমিক অধিকার, লিগ্যাল এইড | https://askbd.org |
| BNWLA | নারীদের জন্য আইনি সহায়তা | https://bnwla-bd.org |
| Bangladesh Mahila Parishad | নারী অধিকার | মাঠপর্যায়ে সক্রিয় |
| Madaripur Legal Aid Association (MLAA) | গ্রামীণ আইনি সহায়তা, শালিস প্রশিক্ষণ | https://mlaa.org |

## আইনজীবী খুঁজতে

- **Bangladesh Bar Council**: https://barcouncil.gov.bd — লাইসেন্সপ্রাপ্ত আইনজীবী যাচাই
- জেলা বার অ্যাসোসিয়েশনের অফিসে গিয়ে তালিকা দেখতে পারেন
- আইনজীবী ঠিক করার আগে জিজ্ঞেস করুন: কতদিনের অভিজ্ঞতা, অনুরূপ মামলার অভিজ্ঞতা, ফি কত (লিখিতভাবে)

## ফি সম্পর্কে সতর্কতা

- প্রথম পরামর্শের ফি, মামলার ফি, খরচের খাত — **আগে থেকেই লিখিত** জেনে নিন
- "মামলা জিতবোই" — এমন গ্যারান্টি দেওয়া আইনজীবী থেকে সাবধান (কেউ গ্যারান্টি দিতে পারে না)

> **দাবিত্যাগ**: সাধারণ তথ্য, আইনি পরামর্শ নয়।



---

<!-- FILE: guides/business/business-legality-checklist.md -->

# আমার ব্যবসা কি Legal? — সম্পূর্ণ চেকলিস্ট / Business Legality Checklist

বাংলাদেশে একটি ব্যবসা আইনত চালাতে হলে নিচের ধাপগুলো চেক করুন। প্রতিটার পাশে ✅ দিন।

## ধাপ ১: ব্যবসার ধরন ঠিক করুন (Legal Structure)

| ধরন | রেজিস্ট্রেশন | কোথায় | সুবিধা/সীমাবদ্ধতা |
|-----|-------------|--------|------------------|
| **একমালিকানা (Proprietorship)** | শুধু ট্রেড লাইসেন্স | সিটি কর্পোরেশন/পৌরসভা/ইউপি | সহজ, কিন্তু মালিকের ব্যক্তিগত দায় সীমাহীন |
| **পার্টনারশিপ** | Partnership Act 1932 অনুযায়ী রেজিস্ট্রেশন (ঐচ্ছিক কিন্তু জরুরি) | RJSC | রেজিস্টার্ড না হলে মামলা করার ক্ষমতা সীমিত |
| **লিমিটেড কোম্পানি (Ltd.)** | Companies Act 1994 | **RJSC** (https://rjsc.gov.bd) | দায় শেয়ারের মধ্যে সীমিত — সবচেয়ে নিরাপদ কাঠামো |
| **সমবায়** | সমবায় আইন | সমবায় অধিদপ্তর | সদস্যভিত্তিক |
| **সোসাইটি/এনজিও** | Societies Registration Act 1860 / NGO Affairs Bureau | RJSC / এনজিও ব্যুরো | অলাভজনক |

## ধাপ ২: বেসিক রেজিস্ট্রেশন চেকলিস্ট (প্রায় সব ব্যবসার জন্য)

- [ ] **ট্রেড লাইসেন্স** — স্থানীয় সিটি কর্পোরেশন/পৌরসভা/ইউনিয়ন পরিষদ থেকে (প্রতি বছর নবায়ন)
- [ ] **e-TIN** (কর শনাক্তকরণ নম্বর) — NBR: https://nbr.gov.bd (অনলাইনে ফ্রি)
- [ ] **BIN/VAT রেজিস্ট্রেশন** — বার্ষিক টার্নওভার নির্দিষ্ট সীমা পার হলে VAT বাধ্যতামূলক (VAT Act 2012) — NBR-এ যাচাই করুন
- [ ] **ব্যাংক অ্যাকাউন্ট** ব্যবসার নামে (ট্রেড লাইসেন্স + TIN লাগে)
- [ ] ব্যবসার নাম অন্যের ট্রেডমার্কের সঙ্গে মিলছে কিনা যাচাই (DPDT: ট্রেডমার্ক অফিস)

## ধাপ ৩: ব্যবসা-নির্দিষ্ট লাইসেন্স

| ব্যবসা | অতিরিক্ত লাইসেন্স/অনুমতি |
|--------|---------------------------|
| কারখানা | ফ্যাক্টরি লাইসেন্স (DIFE), ফায়ার লাইসেন্স (FSCD), পরিবেশ ছাড়পত্র (DoE) |
| রেস্টুরেন্ট/খাবার | BSTI, ফায়ার সেফটি, সিটি কর্পোরেশনের হেলথ লাইসেন্স |
| ওষুধের দোকান | ড্রাগ লাইসেন্স (ঔষধ প্রশাসন অধিদপ্তর) |
| আমদানি-রপ্তানি | IRC/ERC (CCI&E), কাস্টমস |
| শিক্ষা প্রতিষ্ঠান | শিক্ষা মন্ত্রণালয়/বোর্ডের অনুমতি |
| হাসপাতাল/ক্লিনিক/ডায়াগনস্টিক | স্বাস্থ্য অধিদপ্তরের লাইসেন্স |
| অনলাইন/e-commerce | ট্রেড লাইসেন্স + TIN; ডিজিটাল নিরাপত্তা/ভোক্তা আইন মানা বাধ্যতামূলক |
| নির্মাণ/ডেভেলপার | RAJUK/স্থানীয় কর্তৃপক্ষের অনুমোদন, REHAB সদস্যপদ (প্র্যাকটিক্যালি জরুরি) |
| পরিবহন | BRTA ফিটনেস/রুট পারমিট |

## ধাপ ৪: কর্মচারী থাকলে

- [ ] শ্রম আইন ২০০৬ মানছেন: **নিয়োগপত্র + পরিচয়পত্র** (ধারা ৫), সার্ভিস বুক
- [ ] কাজের ঘণ্টা (৮ ঘণ্টা/দিন, ওভারটাইম দ্বিগুণ বেতন), ছুটি, ম্যাটার্নিটি ১৬ সপ্তাহ
- [ ] ১৪ বছরের নিচে কাউকে চাকরি দেওয়া **অবৈধ**
- [ ] বিস্তারিত: [../../acts/labour/labour-act-2006.md](../../acts/labour/labour-act-2006.md)

## ধাপ ৫: নিয়মিত বাধ্যবাধকতা (কোম্পানির জন্য)

- [ ] বার্ষিক রিটার্ন ও AGM — RJSC-এ ফাইল
- [ ] মাসিক VAT রিটার্ন (BIN থাকলে)
- [ ] বার্ষিক আয়কর রিটার্ন (TIN)
- [ ] ট্রেড লাইসেন্স/ফায়ার লাইসেন্স নবায়ন — মেয়াদ দেখুন

## 🚩 লাল পতাকা — এগুলো হলে আপনার ব্যবসা ঝুঁকিতে

- ট্রেড লাইসেন্স নেই বা মেয়াদ শেষ
- অন্যের নামে/ভুয়া ঠিকানায় লাইসেন্স
- দলিল/চুক্তি ছাড়া পার্টনারশিপ চালানো
- কর্মচারীকে নিয়োগপত্র না দেওয়া
- VAT বাধ্যতামূলক অথচ রেজিস্ট্রেশন নেই
- ভাড়ার দোকানে লাইসেন্সের ঠিকানা অন্যখানে

## এক ক্লিকে যাচাই করার সুবিধা

- **BIDA One Stop Service**: https://oss.bida.gov.bd — অনেক লাইসেন্স এক জায়গা থেকে
- **RJSC**: https://rjsc.gov.bd — কোম্পানি যাচাই ও রেজিস্ট্রেশন

> **দাবিত্যাগ**: এটি সাধারণ চেকলিস্ট, আইনি পরামর্শ নয়। আপনার ব্যবসার ধরন অনুযায়ী নির্দিষ্ট পরামর্শের জন্য কোম্পানি আইনজীবী/চার্টার্ড অ্যাকাউন্ট্যান্টের সাথে কথা বলুন।



---

<!-- FILE: guides/business/company-registration.md -->

# কোম্পানি রেজিস্ট্রেশন (RJSC) — ধাপে ধাপে / Company Registration Guide

**আইন**: Companies Act, 1994 | **কর্তৃপক্ষ**: RJSC (Registrar of Joint Stock Companies and Firms) — https://rjsc.gov.bd

## শুরুর আগে সিদ্ধান্ত নিন

| প্রশ্ন | সাধারণ উত্তর |
|--------|--------------|
| Private Limited নাকি Public? | ছোট/মাঝারি ব্যবসা → **Private Limited** (সদস্য ২–৫০) |
| কতজন শেয়ারহোল্ডার? | কমপক্ষে **২ জন** (পরিচালকও কমপক্ষে ২) |
| Authorized capital কত? | প্রয়োজন অনুযায়ী (ফি এর ওপর নির্ভর করে) |

## ধাপ ১: Name Clearance (নাম অনুমোদন)

1. RJSC ওয়েবসাইটে অ্যাকাউন্ট খুলুন
2. প্রস্তাবিত নাম দিয়ে name clearance-এর আবেদন + ফি
3. অনুমোদন পেলে নামটি নির্দিষ্ট সময়ের জন্য সংরক্ষিত থাকে (সাধারণত ৩০ দিন — বর্তমান নিয়ম যাচাই করুন)
4. নাম যেন অন্য কোম্পানি/ট্রেডমার্কের সঙ্গে না মিলে

## ধাপ ২: কাগজপত্র প্রস্তুত

- **Memorandum of Association (MoA)** — কোম্পানির উদ্দেশ্য, মূলধন
- **Articles of Association (AoA)** — ভেতরের শাসনবিধি
- পরিচালকদের NID, ছবি, TIN (নির্ধারিত ক্ষেত্রে)
- রেজিস্টার্ড অফিসের ঠিকানা

## ধাপ ৩: RJSC-তে অনলাইন ফাইলিং

1. RJSC পোর্টালে ফরম পূরণ (Form I, VI, IX, X ইত্যাদি — পোর্টাল গাইড দেখুন)
2. সরকারি ফি (স্ট্যাম্প + রেজিস্ট্রেশন ফি) ব্যাংকে জমা
3. সব কাগজ আপলোড → RJSC যাচাই → **Certificate of Incorporation**

## ধাপ ৪: রেজিস্ট্রেশনের পরে (সবাই ভুলে যায় — আপনি ভুলবেন না)

- [ ] **ট্রেড লাইসেন্স** নিন
- [ ] **e-TIN** কোম্পানির নামে
- [ ] **BIN/VAT** (প্রযোজ্য ক্ষেত্রে)
- [ ] কোম্পানির নামে **ব্যাংক অ্যাকাউন্ট**
- [ ] Share certificate ইস্যু, শেয়ার মূলধন জমা
- [ ] RJSC-তে **বার্ষিক রিটার্ন** ও পরিচালক পরিবর্তনের আপডেট — না দিলে জরিমানা, এমনকি কোম্পানি struck-off হতে পারে

## বিদেশি বিনিয়োগ/শাখা অফিস হলে

- **BIDA** (Bangladesh Investment Development Authority) অনুমোদন লাগতে পারে: https://bida.gov.bd

## কত খরচ/সময়?

- সরকারি ফি মূলধনভেদে কয়েক হাজার থেকে কয়েক লাখ টাকা; সময় সাধারণত কয়েক কর্মদিবস থেকে কয়েক সপ্তাহ। বর্তমান ফি RJSC-র ফি সিডিউলে যাচাই করুন — **আমার দেওয়া সংখ্যা নয়, অফিসিয়াল সূত্র দেখুন**।

> **দাবিত্যাগ**: সাধারণ তথ্য, আইনি পরামর্শ নয়। RJSC-র বর্তমান নির্দেশনা ও একজন কোম্পানি আইনজীবী/CSE-এর সাহায্য নিন।



---

<!-- FILE: guides/business/verify-deed-and-company.md -->

# দলিল ও কোম্পানি যাচাই — জালিয়াতি থেকে বাঁচুন / Verify a Deed or Company

জমি কেনা, অংশীদারি করা বা কোনো কোম্পানির সঙ্গে লেনদেনের **আগে** এই যাচাই করুন। দশ মিনিটের যাচাই লক্ষ টাকার ক্ষতি বাঁচাতে পারে।

## ১. কোম্পানি আসল কিনা — RJSC যাচাই

1. https://rjsc.gov.bd-এ যান
2. কোম্পানির নাম দিয়ে সার্চ করুন
3. দেখুন: রেজিস্ট্রেশন নম্বর, অন্তর্ভুক্তির তারিখ, ঠিকানা, **স্ট্যাটাস (active কিনা)**, পরিচালকগণ
4. কোম্পানিটি RJSC-তে নেই বা struck-off — **সঙ্গে সঙ্গে সাবধান**

> ট্রেড লাইসেন্সও যাচাই করুন — সিটি কর্পোরেশন/পৌরসভার অনলাইন ভেরিফিকেশন বা অফিসে গিয়ে লাইসেন্স নম্বর দিয়ে।

## ২. জমির দলিল যাচাই (সবচেয়ে ঝুঁকিপূর্ণ এলাকা)

**কেনার আগে অবশ্যই:**

### ক. খতিয়ান (নামজারি) যাচাই
- ভূমি অফিসে (AC Land/Tahsil) বা অনলাইনে: https://land.gov.bd, https://mutation.gov.bd
- দেখুন বিক্রেতার নাম **সর্বশেষ খতিয়ানে (BS/RS/SA)** আছে কিনা
- CS → SA → RS → BS ধারা মিলিয়ে দেখুন — মালিকানার চেইন ভাঙা কিনা

### খ. দলিল যাচাই — সাব-রেজিস্ট্রি অফিস
- যে সাব-রেজিস্ট্রি অফিসে দলিল রেজিস্ট্রি হয়েছে, সেখানে গিয়ে **দলিল নম্বর ও বছর দিয়ে খোঁজ নিন**
- নাম/ঠিকানা/দাগ-খতিয়ান মেলে কিনা দেখুন
- Directorate of Registration: https://registration.gov.bd

### গ. রেকর্ড অনুসন্ধান (Search)
- কমপক্ষে **৩০ বছরের সার্চ** করান (সাব-রেজিস্ট্রি অফিসে) — জমিতে বন্ধক/আগের বিক্রি আছে কিনা
- এটা একজন **দলিল লেখক/আইনজীবী** দিয়ে করানো নিরাপদ

### ঘ. আদালতে মামলা আছে কিনা
- সিভিল আদালতে জমিটি নিয়ে মামলা চলছে কিনা খোঁজ নিন
- ব্যাংকে বন্ধক আছে কিনা (Artha Rin/ব্যাংক রেকর্ড) জিজ্ঞেস করুন

### ঙ. ভূমি উন্নয়ন কর (খাজনা) পরিশোধিত কিনা
- হালনাগাদ DCR (ডুপ্লিকেট কার্বন রশিদ) নিন

### চ. নমুনা/নজির — প্রাক্টিক্যাল টিপস
- দলিলের ফটোকপি নিয়ে সাব-রেজিস্ট্রি অফিসের বইয়ের সঙ্গে মেলান
- জমি সরেজমিনে গিয়ে দেখুন, স্থানীয়দের জিজ্ঞেস করুন (দাবিদার/বিরোধ আছে কিনা)
- সরকারি/খাস জমি বা ভেস্টেড প্রপার্টি কিনা খতিয়ানে দেখুন — এগুলো কিনলে বিপদ

## ৩. পার্টনারশিপ/চুক্তি করার আগে

- [ ] চুক্তি **লিখিতভাবে** করুন — মৌখিক চুক্তিতে ভরসা নয়
- [ ] অংশীদারের NID, TIN, ঠিকানা যাচাই
- [ ] চুক্তিতে লিখুন: মূলধন, লাভ-ক্ষতির অনুপাত, কার কী দায়িত্ব, বের হওয়ার শর্ত, বিরোধ নিষ্পত্তির পথ (সালিসি ধারা রাখুন)
- [ ] দামি চুক্তি আইনজীবী দেখিয়ে সই করুন
- [ ] নোটারি করান (প্রমাণ শক্ত হয়), প্রয়োজনে রেজিস্ট্রি

## ৪. এজেন্ট/দালালের মাধ্যমে লেনদেন

- দালালকে টাকা নয় — **সরাসরি মালিকের ব্যাংক অ্যাকাউন্টে** পে অর্ডার/ট্রান্সফার
- প্রতিটি পেমেন্টের **রশিদ** নিন
- পাওয়ার অব অ্যাটর্নি (মোক্তারনামা) দিয়ে কেউ বিক্রি করলে — মোক্তারনামাটি **সাব-রেজিস্ট্রিতে যাচাই** করুন (জাল পাওয়ার অ্যাটর্নি খুব সাধারণ)

## 🚩 প্রতারণার সাধারণ লক্ষণ

- "আজই দিতে হবে" — তাড়াহুড়া করানো
- বাজারদরের চেয়ে অস্বাভাবিক কম দাম
- দলিলের ফটোকপি দেখায়, মূল দেখাতে চায় না
- একই জমি একাধিকবার বিক্রি (খতিয়ান চেইন ভাঙা)

> **দাবিত্যাগ**: সাধারণ তথ্য, আইনি পরামর্শ নয়। জমি কেনার মতো বড় সিদ্ধান্তে অবশ্যই একজন ভূমি আইনজীবী নিয়োগ করুন — এটা খরচ নয়, বীমা।



---

<!-- FILE: constitution/README.md -->

# Constitution of Bangladesh / গণপ্রজাতন্ত্রী বাংলাদেশের সংবিধান

The Constitution of the People's Republic of Bangladesh was adopted on **4 November 1972** and came into effect on **16 December 1972**.

## Overview

- **Adopted**: 4 November 1972
- **Effective**: 16 December 1972
- **Parts**: 11 parts, 153 articles (original)
- **Schedules**: 7
- **Fundamental principles (Part II)**: Nationalism, Socialism, Democracy, Secularism
- **Fundamental rights**: Part III (Articles 26–47A)

## Key Parts

| Part | Subject |
|------|---------|
| I | The Republic |
| II | Fundamental Principles of State Policy |
| III | Fundamental Rights |
| IV | The Executive (President, Prime Minister, Cabinet) |
| V | The Legislature (Jatiya Sangsad) |
| VI | The Judiciary |
| VII | Elections |
| VIII | The Comptroller and Auditor-General |
| IX | Services of Bangladesh |
| IXA | Emergency Provisions |
| X | Amendment of the Constitution |
| XI | Miscellaneous |

## Amendments

The Constitution has been amended multiple times since 1972 (17 amendments as of recent records). Notable ones:

| Amendment | Year | Key change |
|-----------|------|------------|
| 4th | 1975 | Introduced one-party system (BAKSAL), later repealed |
| 5th | 1979 | Ratified martial-law era actions |
| 7th | 1986 | Ratified martial law actions of 1982–86 |
| 8th | 1988 | Islam as state religion; six permanent benches of High Court |
| 12th | 1991 | Return to parliamentary system |
| 13th | 1996 | Caretaker government system (later abolished by the 15th) |
| 15th | 2011 | Abolished caretaker system; secularism restored alongside state religion |

> ⚠️ Verify current amendment status at [bdlaws.minlaw.gov.bd](https://bdlaws.minlaw.gov.bd) — constitutional developments change over time.

## Official text

- Full text (English & Bangla): https://bdlaws.minlaw.gov.bd



---

<!-- FILE: constitution/fundamental-rights.md -->

# Fundamental Rights — Part III of the Constitution / মৌলিক অধিকার (তৃতীয় ভাগ)

Articles 26–47A. Enforceable through the High Court Division under **Article 102** (writ jurisdiction). Article 26 makes inconsistent laws void.

## Article-by-article map

| Article | Right (English) | বাংলা |
|---------|-----------------|-------|
| 26 | Laws inconsistent with fundamental rights void | মৌলিক অধিকারের সঙ্গে সাংঘর্ষিক আইন বাতিল |
| 27 | Equality before law | আইনের চোখে সমান |
| 28 | No discrimination on grounds of religion, race, caste, sex, place of birth | বৈষম্য নিষিদ্ধ |
| 29 | Equal opportunity in public employment | সরকারি চাকরিতে সমান সুযোগ |
| 31 | Right to protection of law — no action except in accordance with law | আইনের আশ্রয়ের অধিকার |
| **32** | **Protection of right to life and personal liberty** — no deprivation except by law | জীবন ও ব্যক্তি স্বাধীনতার অধিকার — সবচেয়ে বেশি ব্যবহৃত ধারা |
| 33 | Safeguards as to arrest and detention | গ্রেফতার ও আটক সংক্রান্ত সুরক্ষা |
| 35 | Protection in respect of trial and punishment (no ex post facto, double jeopardy, self-incrimination) | বিচার সংক্রান্ত সুরক্ষা |
| 36 | Freedom of movement | চলাচলের স্বাধীনতা |
| 37 | Freedom of assembly | সমাবেশের স্বাধীনতা |
| 38 | Freedom of association | সংগঠনের স্বাধীনতা |
| 39 | Freedom of thought, conscience, and **speech/press** | চিন্তা, বিবেক ও বাকস্বাধীনতা |
| 40 | Freedom of profession or occupation | পেশার স্বাধীনতা |
| 41 | Freedom of religion | ধর্মীয় স্বাধীনতা |
| 42 | Rights to property (subject to restrictions) | সম্পত্তির অধিকার |
| 43 | Protection of home and correspondence | বাসভবন ও চিঠিপত্রের সুরক্ষা |
| 44 | Enforcement of fundamental rights | অধিকার প্রয়োগের অধিকার |
| 47 | Saving for certain laws (e.g., listed in First Schedule) | বিশেষ আইনের সুরক্ষা |
| 47A | Inapplicability of certain rights in specific cases | ব্যতিক্রম |

## Landmark enforcement tools

- **Article 102 writs**: habeas corpus (বন্দী প্রত্যর্পণ), mandamus, certiorari, prohibition, quo warranto
- **Public Interest Litigation (PIL)**: locus standi relaxed since *Dr. Mohiuddin Farooque v Bangladesh* (1997) — see [judgments](../judgments/README.md)

## Relationship with fundamental principles

- Part II principles (Articles 8–25) are **not judicially enforceable** (Art. 8(2)) but guide interpretation — "fundamental to the governance of Bangladesh".

> Full text: https://bdlaws.minlaw.gov.bd



---

<!-- FILE: codes/README.md -->

# Major Codes of Bangladesh

The foundational codes — mostly inherited from the colonial era but amended extensively since independence.

## The Penal Code, 1860 (Act XLV of 1860)

The principal criminal code defining offences and punishments.

- **Sections**: 511
- **Commencement**: 1860 (applies in Bangladesh as successor law)
- Key chapters: General explanations, punishments (s. 53), offences against the state, offences against the human body (murder s. 300, culpable homicide s. 299), offences against property (theft s. 378, robbery s. 390), defamation (s. 499)

## The Code of Criminal Procedure, 1898 (Act V of 1898)

Procedure for investigation, trial, and appeal in criminal matters.

- Arrest, bail, remand (s. 54, 167, 497–498)
- Trial procedures: summons cases, warrant cases, sessions trials
- Appeals and revisions

## The Code of Civil Procedure, 1908 (Act V of 1908)

Procedure for civil suits.

- Jurisdiction of civil courts
- Suits, execution of decrees (Order XXI), appeals, review, revision (s. 115)

## The Evidence Act, 1872 (Act I of 1872)

Rules of evidence in judicial proceedings.

- Relevancy of facts (ss. 5–55)
- Oral and documentary evidence
- Burden of proof (ss. 101–114A)
- Examination of witnesses

## Other important codes / related statutes

- The Contract Act, 1872
- The Specific Relief Act, 1877
- The Limitation Act, 1908
- The Registration Act, 1908
- The Transfer of Property Act, 1882
- The Stamp Act, 1899
- The Negotiable Instruments Act, 1881 (s. 138 — cheque dishonour cases)
- The Companies Act, 1994
- The Artha Rin Adalat Ain, 2003 (money loan courts)

> 📌 All texts: https://bdlaws.minlaw.gov.bd



---

<!-- FILE: codes/penal-code-1860.md -->

# The Penal Code, 1860 — Section-wise Notes / দণ্ডবিধি, ১৮৬০

The core criminal statute: defines offences and prescribes punishments. 511 sections, 23 chapters.

## Punishments (s. 53)

Death (যাবজ্জীবনের ওপরে), imprisonment for life (যাবজ্জীবন), imprisonment (rigorous/simple), forfeiture of property, fine.

## General principles

| Section | Topic |
|---------|-------|
| 34 | Common intention — joint criminal liability (যৌথ অভিপ্রায়) |
| 76–95 | General exceptions: mistake of fact, accident, necessity, unsoundness of mind, intoxication, private defence (ss. 96–106) |
| 96–106 | Right of private defence of body and property (আত্মরক্ষার অধিকার) |
| 107–120 | Abetment (দুষ্কর্মে প্ররোচণা) |
| 120A–120B | Criminal conspiracy (ফৌজদারি ষড়যন্ত্র) |
| 141–149 | Unlawful assembly (বেআইনি জমায়েত); s. 149 — constructive liability of every member |

## Offences against the human body

| Section | Offence | Notes |
|---------|---------|-------|
| 299 | Culpable homicide (মানবজীবন সংক্রান্ত অপরাধ) | Definition |
| 300 | Murder (প্রাণনাশ/খুন) | Definition & exceptions |
| 302 | Punishment for murder | Death or life imprisonment + fine |
| 304 | Culpable homicide not amounting to murder | Life or up to 10 years |
| 307 | Attempt to murder (খুনের চেষ্টা) | Up to life imprisonment |
| 309 | Attempt to commit suicide | Up to 1 year |
| 312–316 | Causing miscarriage | |
| 319–338 | Hurt & grievous hurt (আঘাত/মারাত্মক আঘাত); 325, 326 punishments | Acid attacks now under special law (2002) |
| 354 | Assault/criminal force to outrage modesty of a woman | |
| 362–369 | Kidnapping & abduction (অপহরণ); 363, 364, 364A punishments | |
| 375–376 | Rape (ধর্ষণ) and punishment | Note: definitions amended by the Nari O Shishu Ain framework; verify current text |

## Offences against property

| Section | Offence |
|---------|---------|
| 378–382 | Theft (চুরি); s. 379 — punishment |
| 383–389 | Extortion (চাঁদাবাজি) |
| 390–402 | Robbery (ডাকাতি/রাহাজানি); s. 392, 394 punishments |
| 403–404 | Criminal misappropriation |
| 405–409 | Criminal breach of trust (আমানতে খেয়ানত); s. 406 widely used |
| 410–414 | Stolen property |
| 415–420 | Cheating (প্রতারণা); s. 420 — punishment |
| 441–462 | Criminal trespass & house-breaking |

## Other notable offences

- ss. 463–477A: Forgery (জালিয়াতি) — s. 467 is the serious one (valuable security/will)
- ss. 493–498: Offences relating to marriage
- s. 499–502: Defamation (মানহানি) — criminal defamation; civil remedies also available
- ss. 503–510: Criminal intimidation, insult, annoyance

> 📌 Verify the current amended text at https://bdlaws.minlaw.gov.bd — special laws (Nari O Shishu Ain 2000, Acid laws) override or supplement many of these offences.



---

<!-- FILE: codes/crpc-1898.md -->

# The Code of Criminal Procedure, 1898 — Notes / দণ্ডবিধি... ফৌজদারি কার্যবিধি, ১৮৯৮

Procedural machinery for criminal cases: FIR → investigation → trial → appeal.

## Stages of a criminal case

```
FIR (s. 154) → Investigation (ss. 156–173) → Police Report / Charge Sheet (s. 173)
→ Cognizance (s. 190) → Charge framing → Trial → Judgment → Appeal/Revision
```

## Key sections

### Arrest & bail

| Section | Topic |
|---------|-------|
| 54 | Arrest without warrant by police (ওয়ারেন্ট ছাড়া গ্রেফতার) — misuse led to HC guidelines (BLAST case, 2003) |
| 61 | Produce before magistrate within 24 hours |
| 167 | Remand (রিমান্ড) — max 15 days total in police/magistrate custody stages |
| 344 | Remand after cognizance |
| 497 | Bail in non-bailable offences (জামিন) — general rule |
| 498 | Bail powers of High Court Division & Sessions Court |
| 435 / 439 (in part) | Revision of bail orders |

> Article 33 of the Constitution + s. 54: arrest safeguards. In 2016 the HC issued detailed directives on arrest; verify current guidelines.

### Investigation

| Section | Topic |
|---------|-------|
| 154 | FIR — First Information Report (এজাহার/অভিযোগ) |
| 155–157 | Investigation of non-cognizable/cognizable cases |
| 161 | Examination of witnesses by police |
| 164 | Confession & statement before magistrate (জবানবন্দি/স্বীকারোক্তি) |
| 173 | Police report — charge sheet (চার্জশিট) or final report |

### Trial

| Section | Topic |
|---------|-------|
| 190 | Cognizance by magistrate |
| 241A–250 | Trial of warrant cases before magistrates |
| 265A–265U | Sessions trials (সেশন আদালত) — charge framing s. 265C/265D |
| 338 | Tender of pardon to approver (রাজসাক্ষী) |
| 342 | Examination of the accused |
| 367 | Judgment requirements |

### Appeals, revision & miscellaneous

- s. 404–431: appeals (to Sessions / High Court)
- s. 435–439A: revision (রিভিশন)
- **s. 561A**: inherent power of the High Court Division — used to quash (খারিজ) proceedings for abuse of process; the single most-used provision in criminal practice before the HC
- s. 145: disputes over immovable property likely to cause breach of peace (জমিজমা সংক্রান্ত বিরোধ)

> Official text: https://bdlaws.minlaw.gov.bd



---

<!-- FILE: codes/cpc-1908.md -->

# The Code of Civil Procedure, 1908 — Notes / দেওয়ানি কার্যবিধি, ১৯০৮

Procedure for civil suits: filing → trial → decree → execution → appeal.

## Fundamental sections

| Section | Topic |
|---------|-------|
| 9 | Courts to try all civil suits unless barred (আদালতের এখতিয়ার) |
| 10 | Res sub judice — stay of parallel suits |
| 11 | Res judicata — no re-litigation of decided matters (রেস জুডিকাটা) |
| 20 | Where to sue — jurisdiction based on defendant/cause of action |
| 96 | First appeal (প্রথম আপিল) |
| 100 | Second appeal to High Court — substantial question of law |
| 115 | Revision (রিভিশন) to High Court |
| 151 | Inherent powers of court |

## Key Orders

| Order | Topic |
|-------|-------|
| I | Parties to suits — joinder, misjoinder |
| V | Summons (সমন) and service |
| VI | Pleadings generally |
| VII | Plaint (আর্জি/প্লেইন্ট) — contents; O.VII R.11 rejection of plaint |
| VIII | Written statement (জবাব) |
| IX | Appearance & consequences of non-appearance; ex parte decree, O.IX R.13 setting aside |
| XVI–XVIII | Summoning witnesses, hearing, judgment |
| XXI | **Execution of decrees (ডিক্রি জারী)** — attachment, arrest, sale; the longest order |
| XXXIX | **Temporary injunction (অস্থায়ী নিষেধাজ্ঞা)** — R.1 & R.2; most-used remedy in land cases |
| XL | Receivers |
| XLI | Appeals procedure |

## Typical civil suit timeline (district court)

1. Plaint filed with court fee (Court Fees Act, 1870)
2. Summons issued → written statement within statutory time
3. Issues framed → evidence → argument → judgment & decree
4. Execution under Order XXI if not satisfied

## Special civil courts in Bangladesh

- Assistant Judge Court (সহকারী জজ আদালত) — pecuniary limit applies
- Joint District Judge Court
- District Judge Court (জেলা জজ আদালত)
- Artha Rin Adalat — money loan cases (banks/financial institutions)

> Official text: https://bdlaws.minlaw.gov.bd



---

<!-- FILE: codes/evidence-act-1872.md -->

# The Evidence Act, 1872 — Notes / সাক্ষ্য আইন, ১৮৭২

Rules of proof in all judicial proceedings — criminal and civil.

## Core concepts

| Section | Topic |
|---------|-------|
| 3 | Definitions: "evidence", "proved", "disproved", "not proved" |
| 5 | Evidence only of facts in issue and relevant facts |
| 6–11 | Relevancy: res gestae, motive, preparation, conduct |
| 17–31 | Admissions (স্বীকৃতি) — ss. 18–21 who can make them |
| **25** | Confession to police **not admissible** (পুলিশের কাছে স্বীকারোক্তি গ্রহণযোগ্য নয়) |
| **27** | Discovery of fact from information of accused in custody — the famous exception |
| 30 | Confession of co-accused |
| **32** | Dying declaration (মৃত্যুকালীন জবানবন্দি) — exception to hearsay |

## Burden of proof & presumptions

| Section | Topic |
|---------|-------|
| 101 | Whoever asserts must prove (প্রমাণের ভার) |
| 102–103 | Burden as to particular facts |
| 105 | Burden of proving exceptions (accused proves general exceptions) |
| 111A | Presumption as to certain offences (added for special laws) |
| 114 | Court may presume existence of certain facts (স্বাভাবিক অনুমান) — incl. 114(b) accomplice evidence |

## Witnesses & examination

| Section | Topic |
|---------|-------|
| 118 | Who may testify |
| 120 | Parties to civil suits & spouses |
| 132–134 | Witness not excused from incriminating answers; s. 134 — no fixed number of witnesses needed |
| **135–137** | Order of examination; examination-in-chief (জেরা), cross-examination (জেরা/প্রতিজেরা), re-examination |
| 138 | Order of examinations |
| **145** | Cross-examination as to previous written statements (আগের জবানবন্দি নিয়ে জেরা) |
| 146 | Questions lawful in cross-examination |
| 154 | Hostile witness (বিপক্ষগামী সাক্ষী) |
| 155 | Impeaching credit of witness |

## Documentary evidence

- ss. 61–66: proof of documents — primary vs secondary evidence
- ss. 67–73A: proof of signatures & handwriting
- ss. 74–78: public documents
- ss. 79–90: presumptions as to documents (s. 90 — 30-year-old documents)
- ss. 91–92: exclusion of oral by documentary evidence

## Digital evidence

⚠️ The 1872 Act predates digital records. Courts have admitted electronic evidence via s. 65B-style interpretations and the ICT Act; verify current practice — evidentiary rules for digital records are evolving.

> Official text: https://bdlaws.minlaw.gov.bd



---

<!-- FILE: acts/labour/README.md -->

# Labour Laws / শ্রম আইন

## Bangladesh Labour Act, 2006 (বাংলাদেশ শ্রম আইন, ২০০৬)

The consolidated labour law of Bangladesh, replacing and merging 25 previous labour laws. Amended several times (notably 2013, 2018).

Key areas:

| Topic | Summary |
|-------|---------|
| Employment conditions | Appointment letter & ID card mandatory (s. 5) |
| Working hours | 8 hours/day, 48 hours/week standard (s. 100–101); overtime max 60 hours/week total |
| Leave | Casual leave (10 days), sick leave (14 days), annual earned leave, festival holidays (11 days) |
| Maternity benefit | 16 weeks maternity leave (as amended) |
| Termination | Notice pay, compensation (ss. 26–27); retrenchment (s. 20) |
| Trade unions | Right to form unions; registration requirements |
| Safety | Health, hygiene, safety obligations of employers |
| Child labour | Minimum age 14 for employment; 18 for hazardous work |
| Dispute resolution | Labour Courts (শ্রম আদালত) |

## Bangladesh Labour Rules, 2015 (বাংলাদেশ শ্রম বিধিমালা, ২০১৫)

Detailed rules implementing the 2006 Act (as amended).

## Related

- EPZ Labour Act, 2019 — special provisions for Export Processing Zones
- Minimum Wages Board — sets sector minimum wages (e.g., RMG sector)

> Official text: https://bdlaws.minlaw.gov.bd | Ministry of Labour and Employment: https://mole.gov.bd



---

<!-- FILE: acts/labour/labour-act-2006.md -->

# Bangladesh Labour Act, 2006 — Section-wise Notes / বাংলাদেশ শ্রম আইন, ২০০৬

Consolidated labour law (merged 25 previous laws). Major amendments: 2013 (post-Rana Plaza), 2018. Complemented by Labour Rules, 2015.

## Definitions (s. 2)

- **Worker (শ্রমিক)**: any person employed for wages, including apprentices — excludes managerial/administrative staff (s. 2(65))
- Employer, establishment, factory, wages definitions in s. 2

## Conditions of employment

| Section | Provision |
|---------|-----------|
| 5 | **Appointment letter & ID card mandatory** (নিয়োগপত্র ও পরিচয়পত্র বাধ্যতামূলক) |
| 6 | Service book for workers |
| 9–18 | Leave rules linked to service length |
| 20 | **Retrenchment** — compensation: 30 days' wages per completed year (রির্স্টেন্চমেন্ট/ছাঁটাই) |
| 23 | Discharge for physical/mental incapacity |
| 26 | **Termination by employer** — 120 days' notice (monthly-rated) or compensation; 30 days' wages per year |
| 27 | **Dismissal for misconduct** — after proper inquiry (অসদাচরণে বরখাস্ত; তদন্ত বাধ্যতামূলক) |
| 28 | Resignation by worker |

## Working hours & leave

| Topic | Rule |
|-------|------|
| Daily hours | 8 hours (s. 100) |
| Weekly hours | 48 hours; max 60 with overtime (s. 102/105) |
| Overtime rate | **Double** the basic wage rate (s. 108) |
| Weekly holiday | 1 day (s. 103) |
| Casual leave | 10 days/year with full wages (s. 115) |
| Sick leave | 14 days/year (s. 116) |
| Festival holidays | 11 days/year (s. 117) |
| Earned/annual leave | 1 day per 18 working days (adults) |
| **Maternity benefit** | **16 weeks** — 8 weeks before + 8 weeks after delivery; no dismissal during maternity (ss. 45–50) |

## Safety & welfare

- ss. 51–72: health, hygiene, dust/fume, waste disposal, ventilation
- ss. 61–68: safety — machinery fencing, fire safety (expanded after Rana Plaza via 2013 amendments & Rules 2015)
- ss. 92–98: welfare — first aid, canteen, rest room, children's room (50+ workers)
- Child labour: minimum working age **14**; hazardous work **18** (s. 34–44; Children Act 2013 aligns)

## Trade unions & industrial relations

- ss. 176–196: right to form trade unions (ট্রেড ইউনিয়ন), registration, unfair labour practices
- s. 210–225: collective bargaining agent (CBA), strikes/lockouts, dispute settlement
- Participation fund & welfare fund for certain companies (ss. 234–235 — Workers' Participation Fund, 5% profit sharing for eligible companies)

## Dispute resolution

- **Labour Courts (শ্রম আদালত)**: 7 divisional courts; appeals to Labour Appellate Tribunal
- Complaint timeline: act provides limitation for grievance applications
- Department of Inspection for Factories & Establishments (DIFE) — inspection & complaints: https://dife.gov.bd

> ⚠️ Section references are based on the Act as amended; always verify current text at https://bdlaws.minlaw.gov.bd



---

<!-- FILE: acts/family/README.md -->

# Family Laws / পারিবারিক আইন

Family law in Bangladesh varies by religion for personal matters (marriage, divorce, inheritance), plus general statutes.

## General statutes

- **Family Courts Ordinance, 1985** — establishes Family Courts for suits on marriage, divorce, dower (মোহরানা), maintenance, guardianship, and custody.
- **Child Marriage Restraint Act, 2017** — prohibits marriage below 18 (women) / 21 (men); special provision in exceptional cases with court/parental consent.
- **Dowry Prohibition Act, 1980** — criminalizes giving/taking dowry (যৌতুক).
- **Muslim Family Laws Ordinance, 1961** — registration of Muslim marriages, polygamy restrictions (arbitration council permission), divorce procedure (talaq notice).
- **Muslim Marriages and Divorces (Registration) Act, 1974** — mandatory registration via licensed Nikah Registrars (কাজী).
- **Muslim Personal Law (Shariat) Application Act, 1937** — applies Shariat to Muslims in personal matters.

## For other communities

- Hindu personal law applies to Hindus (marriage, inheritance — largely uncodified; Hindu Marriage Registration Act, 2012 provides optional registration).
- Christian Divorce Act, 1869; Special Marriage Act, 1872 (inter-faith marriages).

## Guardianship & custody

- Guardians and Wards Act, 1890 — court-appointed guardians; welfare of the minor is the paramount consideration.

> Official texts: https://bdlaws.minlaw.gov.bd



---

<!-- FILE: acts/cyber/README.md -->

# Cyber & ICT Laws / সাইবার ও তথ্যপ্রযুক্তি আইন

## Cyber Security Act, 2023 (সাইবার নিরাপত্তা আইন, ২০২৩)

Replaced the Digital Security Act, 2018. Key provisions include:

- Punishments for unauthorized access to computers/digital devices
- Offences related to spreading false or offensive information online
- Powers of the National Cyber Security Agency
- Investigation and trial procedures

> ⚠️ Cyber legislation in Bangladesh has changed rapidly (ICT Act 2006 → DSA 2018 → CSA 2023, with subsequent amendments and proposed replacements). Always check https://bdlaws.minlaw.gov.bd for the current law in force.

## Historical

| Law | Year | Status |
|-----|------|--------|
| Information and Communication Technology Act | 2006 | s. 57 heavily criticized; amended 2013 |
| Digital Security Act | 2018 | Replaced s. 57-era offences; repealed 2023 |
| Cyber Security Act | 2023 | Current framework (subject to change) |

## Related

- Pornography Control Act, 2012
- Right to Information Act, 2009 (ধারা ৫ — citizen information rights)
- Bangladesh Telecommunication Regulation Act, 2001 (BTRC)



---

<!-- FILE: acts/land/README.md -->

# Land & Property Laws / ভূমি ও সম্পত্তি আইন

Land law is one of the most litigated areas in Bangladesh.

## Core statutes

- **State Acquisition and Tenancy Act, 1950 (East Bengal)** — abolished zamindari; governs raiyati tenures, khas land.
- **Transfer of Property Act, 1882** — sale, mortgage, lease, gift, exchange of immovable property.
- **Registration Act, 1908** — mandatory registration of deeds (দলিল) at the Sub-Registry office.
- **Stamp Act, 1899** — stamp duty on instruments.
- **Non-Agricultural Tenancy Act, 1949** — non-agricultural land tenancies.
- **Land Development Tax Ordinance, 1976** — land development tax (ভূমি উন্নয়ন কর).
- **Vested Property Act** — property vested in the government (formerly Enemy Property Act, 1965); heavily amended.
- **Mutation (নামজারি/খারিজ)** — governed by land administration rules at AC Land / Tahsil offices.

## Land dispute forums

- Civil courts — title, possession suits
- Assistant Judge / Joint District Judge courts
- Land Survey Tribunal (ভূমি জরিপ ট্রাইব্যুনাল) — record-of-rights corrections
- AC Land / UNO offices — administrative matters

## Record systems

- CS (Cadastral Survey), SA (State Acquisition), RS (Revisional Survey), BS/বাংলাদেশ জরিপ khatians
- Land Registration: Sub-Registry offices under the Directorate of Registration (https://registration.gov.bd)
- Ministry of Land: https://minland.gov.bd | Digital services: https://land.gov.bd, https://mutation.gov.bd



---

<!-- FILE: acts/women-children/README.md -->

# Women & Children Protection Laws / নারী ও শিশু সুরক্ষা আইন

## Women

- **Nari O Shishu Nirjatan Daman Ain, 2000** (নারী ও শিশু নির্যাতন দমন আইন) — the principal law against violence against women and children: rape, acid violence, trafficking, grievous hurt; special tribunals for speedy trial.
- **Dowry Prohibition Act, 1980** — criminalizes dowry demand and giving/taking.
- **Domestic Violence (Prevention and Protection) Act, 2010** — civil protection orders, residence orders, compensation for domestic violence victims.
- **Acid Niyontron Ain, 2002** & **Acid Oporadh Daman Ain, 2002** — control of acid sale and punishment of acid attacks (including death penalty).
- **Women and Children Repression Prevention (Special Provisions) Act, 1995** — earlier special law (overlaps with the 2000 Ain).
- High Court directives on **sexual harassment (2009)** — guidelines for workplaces and educational institutions, having force of law until legislation.

## Children

- **Children Act, 2013** (শিশু আইন) — juvenile justice: Child Courts, child-friendly procedures, diversion; defines child as under 18.
- **Child Marriage Restraint Act, 2017**
- **Prevention of Human Trafficking Act, 2012**
- **Children Act, 2013** provisions on street-connected children, care homes
- Bangladesh is a party to the **UN Convention on the Rights of the Child (CRC)**.

## Helplines (verify before publishing)

- National helpline for violence against women & children: **109** (Multi-Sectoral Programme on Violence Against Women)
- Child helpline: **1098** (Child Helpline Bangladesh)
- Police emergency: **999**
- Legal aid: National Legal Aid Services Organization (https://nlaso.gov.bd), free legal aid hotline **16430**

> Official texts: https://bdlaws.minlaw.gov.bd



---

<!-- FILE: resources/README.md -->

# Legal Resources / আইনি রিসোর্স

## Official government sources

| Resource | URL |
|----------|-----|
| Laws of Bangladesh (all acts & ordinances, English + Bangla) | https://bdlaws.minlaw.gov.bd |
| Ministry of Law, Justice and Parliamentary Affairs | https://minlaw.gov.bd |
| Supreme Court of Bangladesh | https://supremecourt.gov.bd |
| Supreme Court cause lists & case status | https://supremecourt.gov.bd |
| Jatiya Sangsad (Parliament) | https://parl.gov.bd |
| Legislative drafting | https://ld.minlaw.gov.bd |
| Bangladesh Judicial Service Commission | https://bjsc.gov.bd |
| Bangladesh Bar Council | https://barcouncil.gov.bd |

## Legal aid & human rights

| Organization | URL |
|--------------|-----|
| National Legal Aid Services Organization (NLASO) | https://nlaso.gov.bd |
| Bangladesh Legal Aid and Services Trust (BLAST) | https://blast.org.bd |
| Ain o Salish Kendra (ASK) | https://askbd.org |
| Bangladesh National Women Lawyers' Association (BNWLA) | https://bnwla-bd.org |

## Court structure

```
Supreme Court of Bangladesh
├── Appellate Division (আপীল বিভাগ)
└── High Court Division (হাইকোর্ট বিভাগ)
        │
Subordinate Courts
├── District & Sessions Judge Courts (criminal: Sessions; civil: District Judge)
├── Additional/Joint District Judge, Senior/Joint Assistant Judge, Assistant Judge
├── Chief Judicial Magistrate / Chief Metropolitan Magistrate Courts
└── Specialized tribunals: Labour Court, Money Loan Court (Artha Rin),
    Nari O Shishu Tribunal, Cyber Tribunal, International Crimes Tribunal
```

## Writ jurisdiction (High Court Division)

Article 102 of the Constitution — writs of habeas corpus, mandamus, certiorari, prohibition, quo warranto.

## Research tips

1. Always verify the **latest amendment** of any act at bdlaws.minlaw.gov.bd — amendments are frequent.
2. Judgments: the Supreme Court publishes selected judgments online; commercial databases (e.g., DLR, BLC, AD law reports) are cited in practice.
3. For Bangla versions of laws, bdlaws.minlaw.gov.bd hosts official Bangla texts — in case of conflict, the Bangla text generally prevails (per the Bangla Language Introduction Act, 1987).



---

<!-- FILE: judgments/README.md -->

# Landmark Judgments of the Supreme Court of Bangladesh / সুপ্রিম কোর্টের গুরুত্বপূর্ণ রায়

Selected decisions that shaped constitutional and public law. Citations are indicative — verify against the official law reports (DLR, BLC, BLD, ADC) or the Supreme Court website before citing in court or academia.

## Constitutional cases

### 1. [Anwar Hossain Chowdhury v Bangladesh (8th Amendment Case), 1989](8th-amendment-case.md)
*41 DLR (AD) 165*

- Established the **basic structure doctrine** (সংবিধানের মৌলিক কাঠামো তত্ত্ব) — Parliament cannot amend the Constitution in a way that destroys its basic features (e.g., supremacy of the Constitution, judicial independence).
- Struck down the part of the 8th Amendment creating six permanent regional benches of the High Court Division.

### 2. [Secretary, Ministry of Finance v Md. Masdar Hossain (Separation of Judiciary Case), 1999](masdar-hossain-case.md)
*52 DLR (AD) 82*

- Issued the famous **12-point directives** for separating the judiciary from the executive.
- Implemented in 2007 — judicial magistracy separated under the CrPC amendments.

### 3. [Bangladesh v Idrisur Rahman (5th Amendment Case), 2010](5th-amendment-case.md)
- Declared the **5th Amendment** (ratifying martial-law-era actions of 1975–79) **illegal and void**.
- Reaffirmed the basic structure doctrine; held martial law proclamations cannot be ratified by constitutional amendment.

### 4. [Abdul Mannan Khan v Bangladesh (7th Amendment Case), 2011](7th-amendment-case.md)
*64 DLR (AD) 169*

- Declared the **7th Amendment** (ratifying Ershad's 1982–86 martial law actions) unconstitutional on the same reasoning as the 5th Amendment case.

### 5. [Bangladesh Italian Marble Works Ltd v Bangladesh (13th Amendment Case), 2011](13th-amendment-case.md)
- Struck down the **caretaker government system** (13th Amendment, 1996), though the Court suggested parliament could keep it for two more elections prospectively; parliament instead abolished it via the **15th Amendment (2011)**.

### 6. [Asaduzzaman Siddiqui v Bangladesh (16th Amendment Case), 2017](16th-amendment-case.md)
- Declared the **16th Amendment** (restoring Parliament's power to remove Supreme Court judges) unconstitutional — judicial independence prevails. Upheld by the Appellate Division (2017).

## Public interest & rights cases

### 7. [Dr. Mohiuddin Farooque v Bangladesh (FAP Case), 1997](mohiuddin-farooque-case.md)
*49 DLR (AD) 1*

- Landmark **PIL case** — relaxed locus standi: "any person aggrieved" includes organizations acting for the public/voiceless.
- Environmental protection recognized within the right to life (Article 32).

### 8. [BLAST v Bangladesh (Arrest & Remand Safeguards Case), 2003](blast-arrest-case.md)
- HCD issued directives against abuse of **s. 54 CrPC** arrests and custodial torture — recording reasons for arrest, informing family, medical examination. Foundation for later arrest-safeguard jurisprudence.

### 9. [BNWLA v Government of Bangladesh (Sexual Harassment Guidelines Case), 2009](bnwla-sexual-harassment-case.md)
- High Court Division issued **guidelines on sexual harassment** at workplaces and educational institutions (complaint committees, inquiry procedure) — binding until legislation is enacted.

### 10. [Ain o Salish Kendra (ASK) v Bangladesh (Fatwa / Salish Case), 2011](ask-fatwa-salish-case.md)
- Directives against extrajudicial punishments imposed through village "salish"/fatwa — reinforcing the rule of law and Articles 31–32, 35 (an earlier 2001 HCD ruling on fatwas was stayed by the AD).

## How to read a Bangladesh judgment

- **DLR** = Dhaka Law Reports; **BLD** = Bangladesh Legal Decisions; **BLC** = Bangladesh Law Chronicles; **ADC** = Appellate Division Cases
- HCD = High Court Division; AD = Appellate Division
- Selected judgments online: https://supremecourt.gov.bd

> ⚠️ Citations above are compiled from standard references; please verify the exact report citation before formal use.



---

<!-- FILE: judgments/8th-amendment-case.md -->

# Anwar Hossain Chowdhury v Bangladesh (8th Amendment Case)

**Citation**: 41 DLR (AD) 165 | **Year**: 1989 | **Forum**: Appellate Division

## Facts / পটভূমি

The 8th Amendment (1988) did two things: (1) declared **Islam the state religion**, and (2) created **six permanent benches** of the High Court Division outside Dhaka (Barisal, Comilla, Jessore, Chittagong, Rajshahi, Sylhet — styled as permanent regional benches).

Senior lawyer Anwar Hossain Chowdhury and others challenged the amendment by writ petition. The High Court Division struck down the amendment; the government appealed to the Appellate Division.

## Issues / মূল প্রশ্ন

1. Can Parliament, using its amending power under **Article 142**, alter any part of the Constitution without limit?
2. Are the permanent regional benches destructive of the **unity and integrity of the High Court Division** — a basic feature of the Constitution?

## Ratio Decidendi / রায়ের মূলনীতি

- **The amending power is a derived, limited power** — not an original constituent power. Parliament cannot amend the Constitution in a way that **destroys or damages its basic structure**.
- Basic features identified include: **supremacy of the Constitution, republican democracy, unitary character of the state, separation of powers, and independence of the judiciary**.
- The dispersal of the High Court into permanent regional benches destroyed the unity of the superior judiciary — hence void.

## Holding / ফলাফল

The Appellate Division (majority) **struck down the bench provisions** of the 8th Amendment. (The state-religion provision was not struck down in this judgment.)

## Significance / গুরুত্ব

- Foundation stone of Bangladeshi constitutional jurisprudence — every later amendment case (5th, 7th, 13th, 15th, 16th) builds on it.
- Placed Bangladesh alongside India (*Kesavananda Bharati*, 1973) in the basic-structure family of jurisdictions.

> ⚠️ Verify citations against the official DLR report before formal use.



---

<!-- FILE: judgments/masdar-hossain-case.md -->

# Secretary, Ministry of Finance v Md. Masdar Hossain (Separation of Judiciary Case)

**Citation**: 52 DLR (AD) 82 | **Judgment**: 2 December 1999 | **Forum**: Appellate Division

## Facts / পটভূমি

Masdar Hossain, a judicial officer (along with 441 fellow officers), filed a writ petition arguing that the **lower judiciary was controlled by the executive** (Ministry of Establishment) in matters of appointment, promotion, posting, and discipline — contrary to the constitutional scheme, particularly **Articles 22** (separation of judiciary from executive) and **116A** (subordinate judicial service).

The High Court Division directed the government to separate the judiciary. Successive governments appealed and obtained repeated extensions for years.

## Issues / মূল প্রশ্ন

1. Does executive control over the subordinate judiciary violate the Constitution?
2. What concrete steps must the government take to effect separation?

## Ratio Decidendi / রায়ের মূলনীতি

- **Independence of the judiciary is a basic feature** of the Constitution; subordinate courts cannot be treated as a department of the executive.
- Separation requires structural changes, not promises — hence the Court issued **12-point directives** (বারো দফা নির্দেশনা), including:
  - Creation of a separate **Bangladesh Judicial Service** pay/structure framework
  - Formation of a **Judicial Service Commission** and Judicial Service Pay Commission
  - Transfer of disciplinary control over judicial officers to the Supreme Court
  - Amendment of the CrPC to separate **judicial magistracy from executive magistracy**

## Holding / ফলাফল

The appeal was dismissed; the 12-point directives became binding. After years of delay, the **caretaker government implemented separation in 2007** (CrPC amendments effective 1 November 2007 created judicial magistrate courts).

## Significance / গুরুত্ব

- The most consequential administrative-law judgment in Bangladesh's history.
- Transformed the magistracy: criminal justice administration moved from executive magistrates to judicial magistrates.

> ⚠️ Verify citations against the official report before formal use.



---

<!-- FILE: judgments/5th-amendment-case.md -->

# Bangladesh v Idrisur Rahman (5th Amendment Case)

**Reported**: 29 BLD (AD); HCD judgment 2005, AD judgment 2010 | **Forum**: Appellate Division

## Facts / পটভূমি

The **5th Amendment (1979)** ratified — by a single blanket clause (the Fourth Schedule) — all martial law proclamations, regulations, and orders made between **15 August 1975 and 9 April 1979**, and amended numerous constitutional provisions.

The dispute reached court through a land/title matter (Italian Marble Works line of litigation involved the 13th Amendment; the 5th Amendment challenge arose via a separate writ challenging actions resting on martial law instruments). The High Court Division declared the 5th Amendment unconstitutional; the State appealed.

## Issues / মূল প্রশ্ন

1. Can Parliament ratify the suspension of the Constitution and martial law rule by constitutional amendment?
2. What survives if the ratifying amendment is void?

## Ratio Decidendi / রায়ের মূলনীতি

- **Martial law is alien to the Constitution**; its instruments cannot be legitimized ex post facto through Article 142.
- A constitutional amendment that **destroys basic features** (democracy, rule of law, judicial review) is void — applying the *Anwar Hossain Chowdhury* doctrine.
- The doctrine of condonation cannot validate the unconstitutional taking of power by extra-constitutional means.

## Holding / ফলাফল

The Appellate Division (2010) **declared the 5th Amendment illegal and void**. The Court specified which consequential changes would stand or fall, to avoid legal chaos.

## Significance / গুরুত্ব

- Reopened the constitutional basis of the state religion provision and secularism — paving the way for the **15th Amendment (2011)**, which restored secularism while retaining Islam as state religion, and restored "Bismillah" and other 1972 features selectively.
- Established firmly: **amendments ratifying martial law are per se unconstitutional**.

> ⚠️ Verify citations against the official report before formal use.



---

<!-- FILE: judgments/7th-amendment-case.md -->

# Abdul Mannan Khan v Bangladesh (7th Amendment Case)

**Citation**: 64 DLR (AD) 169 | **Year**: 2011 | **Forum**: Appellate Division

## Facts / পটভূমি

The **7th Amendment (1986)** ratified all proclamations, martial law regulations, and orders issued during **Hussain Muhammad Ershad's martial law period (24 March 1982 – 11 November 1986)**, following the same pattern as the 5th Amendment.

A writ petition challenged the validity of actions deriving authority from that ratification (the litigation arose through a specific grievance — the petitioner challenged the foundation of martial-law-era instruments).

## Issues / মূল প্রশ্ন

1. Is the 7th Amendment valid given that the 5th Amendment — identically structured — had already been declared void?
2. What is the fate of laws enacted during the Ershad martial law period?

## Ratio Decidendi / রায়ের মূলনীতি

- The reasoning of the **5th Amendment case applies with equal force**: martial law proclamations cannot be ratified by constitutional amendment; such ratification destroys the basic structure (rule of law, constitutional supremacy).
- The Court again distinguished between void instruments and those kept alive to prevent a legal vacuum.

## Holding / ফলাফল

The Appellate Division **declared the 7th Amendment unconstitutional**. It nevertheless protected certain martial-law-era enactments and settled rights to avoid administrative chaos (prospective application in effect).

## Significance / গুরুত্ব

- Completed the judicial repudiation of both martial law eras (1975–79 and 1982–86).
- Together with the 5th Amendment case, it forms the doctrinal backbone for the 15th Amendment's constitutional re-settlement.

> ⚠️ Verify citations against the official report before formal use.



---

<!-- FILE: judgments/13th-amendment-case.md -->

# Bangladesh Italian Marble Works Ltd v Bangladesh (13th Amendment Case)

**Year**: 2011 (AD judgment, May 2011) | **Forum**: Appellate Division

## Facts / পটভূমি

The **13th Amendment (1996)** inserted the **caretaker government (তত্ত্বাবধায়ক সরকার)** system into the Constitution (Articles 58B–58E): a non-partisan interim government, headed by the last retired Chief Justice, would conduct national elections after each parliament's term ended.

The writ petitioner (a private company affected by caretaker-era action) challenged the amendment. The High Court Division upheld the amendment; on appeal, the Appellate Division took a different view.

## Issues / মূল প্রশ্ন

1. Is the caretaker government system — which hands state power to unelected persons — consistent with the Constitution's basic structure of **republican democracy**?
2. If not, how should the transition be managed to avoid disruption of elections?

## Ratio Decidendi / রায়ের মূলনীতি

- **Democracy — meaning rule by elected representatives — is a basic structure.** Handing executive power to unelected caretakers, however well-intentioned, damages that basic feature.
- Elections can be free and fair under an elected political government with proper institutional safeguards.

## Holding / ফলাফল

The Appellate Division declared the **13th Amendment void**. However, the majority observed (in the nature of prospective application) that parliament *might* still hold the next one or two elections under the caretaker system if it chose.

Parliament responded by enacting the **15th Amendment (June 2011)**, which **abolished the caretaker system** outright.

## Significance / গুরুত্ব

- Reshaped Bangladesh's electoral politics: national elections since 2014 have been held under political governments.
- Illustrates how a private commercial dispute can carry a constitutional challenge to the highest level.

> ⚠️ Verify citations against the official report before formal use.



---

<!-- FILE: judgments/16th-amendment-case.md -->

# Asaduzzaman Siddiqui v Bangladesh (16th Amendment Case)

**HCD**: May 2016 | **AD**: 3 July 2017 | **Forum**: High Court Division, affirmed by Appellate Division

## Facts / পটভূমি

The original 1972 Constitution allowed Parliament to remove Supreme Court judges. In the late 1970s this was replaced by the **Supreme Judicial Council (SJC)** mechanism (Chief Justice + two senior judges investigate and recommend removal).

The **16th Amendment (2014)** restored Parliament's power: judges could be removed by a two-thirds parliamentary vote on grounds of incapacity or misconduct.

Nine Supreme Court lawyers, led by advocate Asaduzzaman Siddiqui, challenged the amendment by writ petition.

## Issues / মূল প্রশ্ন

1. Does removal of judges by Parliament damage the **independence of the judiciary**, a basic structure?
2. Is the SJC mechanism itself a basic feature, or merely one possible design?

## Ratio Decidendi / রায়ের মূলনীতি

- **Judicial independence is part of the basic structure**; giving the political branch the power to remove judges makes the judiciary vulnerable to executive/parliamentary pressure.
- The SJC — composed of judges judging judges — provides the insulation the basic structure requires; replacing it with parliamentary removal is an impermissible amendment.

## Holding / ফলাফল

- The High Court Division **struck down the 16th Amendment** (May 2016).
- The Appellate Division **unanimously upheld** the decision (July 2017), restoring the Supreme Judicial Council under Article 96.

## Significance / গুরুত্ব

- The most recent major application of the basic structure doctrine; sparked intense public debate about the balance between accountability and judicial independence.
- Confirmed that the doctrine applies even to amendments **restoring original constitutional text** — what matters is the effect on basic structure, not historical pedigree.

> ⚠️ Verify citations against the official report before formal use.



---

<!-- FILE: judgments/mohiuddin-farooque-case.md -->

# Dr. Mohiuddin Farooque v Bangladesh (FAP Case)

**Citation**: 49 DLR (AD) 1 | **Year**: 1997 | **Forum**: Appellate Division

## Facts / পটভূমি

Dr. Mohiuddin Farooque, through the organization **BELA (Bangladesh Environmental Lawyers Association)**, challenged the implementation of the **Flood Action Plan (FAP-20)** — a large flood-control project — alleging it would cause environmental harm and displace communities, affecting the life and livelihood of millions.

The government's core objection: BELA had **no standing (locus standi)** — it was not personally "aggrieved" by the project.

## Issues / মূল প্রশ্ন

1. Who is a "person aggrieved" under **Article 102** of the Constitution?
2. Can an organization sue on behalf of the public or of affected communities?
3. Does environmental protection fall within the constitutional **right to life**?

## Ratio Decidendi / রায়ের মূলনীতি

- **"Any person aggrieved"** in Article 102 is not confined to a person whose personal legal right is infringed. It includes **any individual or bona fide organization espousing the cause of the public or of a class/community unable to approach the court themselves** — provided the petitioner is not a mere busybody or interloper.
- The **right to life (Article 32)** includes the right to a healthy environment; environmental degradation affecting life and livelihood is justiciable.

## Holding / ফলাফল

BELA was held to have **standing**, and the writ was maintainable — opening the door to public interest litigation in Bangladesh.

## Significance / গুরুত্ব

- **The birth certificate of PIL in Bangladesh.** Almost every subsequent public interest case (environment, consumer rights, arrest safeguards, sexual harassment) cites this case on standing.
- Embedded environmental rights within Articles 31–32.

> ⚠️ Verify citations against the official report before formal use.



---

<!-- FILE: judgments/blast-arrest-case.md -->

# BLAST v Bangladesh (Arrest & Remand Safeguards Case)

**Citation**: 55 DLR (HCD) 363 | **Year**: 2003 | **Forum**: High Court Division

## Facts / পটভূমি

**BLAST (Bangladesh Legal Aid and Services Trust)** and other rights organizations filed a writ challenging rampant abuse of **section 54 of the CrPC** (arrest without warrant on suspicion) and **section 167** (remand) — citing deaths in custody, torture, and arbitrary arrests, often of political opponents or for extortion.

## Issues / মূল প্রশ্ন

1. Are the prevailing practices of arrest under s. 54 and remand under s. 167 consistent with **Articles 31, 32, 33 and 35** of the Constitution (protection of law, life and liberty, arrest safeguards, fair trial)?
2. What safeguards should govern arrest and detention pending legislative reform?

## Ratio Decidendi / রায়ের মূলনীতি

- Arrest is an extreme interference with liberty; "suspicion" under s. 54 must be **reasonable and recorded** — not a license for arbitrary pickup.
- Safeguards derive directly from Articles 32 and 33; courts can mandate procedures where police practice defeats constitutional rights.

## Holding / ফলাফল

The Court issued **detailed directives**, including:

- Recording the **specific reasons** for arrest at the time of arrest
- **Informing a relative/friend** of the arrestee within a set time
- Marking arrest in a register; **medical examination** before and after remand
- Disclosing identity of arresting officers; interrogation safeguards during remand
- Recommending amendments to ss. 54 and 167 CrPC to the government

## Significance / গুরুত্ব

- The foundational **arrest-safeguards jurisprudence** in Bangladesh; repeatedly invoked in custodial-death and unlawful-arrest litigation.
- The Appellate Division later (2016) considered and modified some directives — **verify the current operative guidelines** before relying on specific details.

> ⚠️ Verify citations and current status against official reports.



---

<!-- FILE: judgments/bnwla-sexual-harassment-case.md -->

# BNWLA v Government of Bangladesh (Sexual Harassment Guidelines Case)

**Reported**: 14 BLC (2009) | **Year**: 2009 | **Forum**: High Court Division

## Facts / পটভূমি

The **Bangladesh National Women Lawyers' Association (BNWLA)** filed a writ petition highlighting widespread **sexual harassment (যৌন হয়রানি)** of women and girls at workplaces and educational institutions — for which Bangladesh had **no dedicated legislation** and no effective redress mechanism. Victims faced retaliation, and institutional complaints went nowhere.

## Issues / মূল প্রশ্ন

1. In the absence of legislation, can the Court frame enforceable guidelines against sexual harassment?
2. What is the constitutional basis — equality (Arts. 27–28), dignity, and the right to life and livelihood (Arts. 31–32)?

## Ratio Decidendi / রায়ের মূলনীতি

- Sexual harassment violates **equality, dignity, and the right to safe working/learning conditions** protected by the Constitution and by international instruments (CEDAW), which courts may use to fill interpretive gaps.
- Where a legislative vacuum exists, courts may issue guidelines having the **force of law until legislation is enacted** (following the Indian *Vishaka* model).

## Holding / ফলাফল

The Court issued binding **Sexual Harassment Prevention Guidelines**, requiring:

- Every workplace and educational institution to constitute a **Complaint Committee**, headed by a woman, with majority women members
- Confidential complaint procedures, inquiry within fixed timelines, and protection against retaliation
- Disciplinary action up to dismissal; referral to criminal authorities where conduct is an offence
- Wide publicity of the guidelines within institutions

## Significance / গুরুত্ব

- The operative anti-sexual-harassment regime in Bangladesh **to this day** — institutions' complaint committees trace directly to this judgment.
- A model of judicial gap-filling pending legislation; discussions on a dedicated statute continue.

> ⚠️ Verify citations against the official report before formal use.



---

<!-- FILE: judgments/ask-fatwa-salish-case.md -->

# Ain o Salish Kendra (ASK) v Bangladesh (Fatwa / Salish Case)

**Year**: 2011 (HCD directives; earlier HCD ruling 2001 stayed by AD) | **Forum**: High Court Division

## Facts / পটভূমি

Rural **salish (শালিস)** — informal village dispute-resolution gatherings — were increasingly imposing **extrajudicial punishments in the name of fatwa**: whipping, caning, shunning, and forced marriage, overwhelmingly against women and the poor. Several victims died (the case of **Hena Akter** in Shariatpur, who died after a salish-imposed whipping in early 2011, galvanized national attention).

Earlier, in **2001**, the High Court Division had declared fatwas by unauthorized persons illegal; that ruling was stayed by the Appellate Division, leaving a grey zone.

**Ain o Salish Kendra (ASK)** and other organizations petitioned the High Court Division again in 2011.

## Issues / মূল প্রশ্ন

1. Can extrajudicial punishments imposed through salish/fatwa be tolerated under Articles **31, 32, and 35** (protection of law, life and liberty, safeguards in trial and punishment)?
2. What immediate measures can protect victims pending legislation?

## Ratio Decidendi / রায়ের মূলনীতি

- **No person may be punished except by a court of law following due process** (Art. 35). Salish bodies are not courts; punishments imposed by them are flatly unconstitutional.
- Arbitration/mediation in village disputes is permissible **only as voluntary settlement of civil disputes** — criminal punishment of any kind is beyond their competence.

## Holding / ফলাফল

The Court directed that:

- Extrajudicial penalties imposed via salish/fatwa — whipping, caning, physical or degrading punishment — are **illegal and must stop**
- Police and local administration must **prevent such punishments and prosecute** those who impose them
- Awareness measures for local government representatives; protection and remedies for victims

## Significance / গুরুত্ব

- Drew a bright constitutional line: **dispute resolution ≠ criminal punishment**.
- Central precedent in cases involving village justice, mob punishment, and religious edicts with penal consequences.

> ⚠️ Verify citations and the status of the earlier 2001 ruling before formal use.



---

<!-- FILE: data/laws-index.json -->

{
  "name": "bangladesh-law-index",
  "version": "0.1.0",
  "description": "Machine-readable starter index of major Bangladeshi laws. Not exhaustive. Always verify at https://bdlaws.minlaw.gov.bd",
  "official_source": "https://bdlaws.minlaw.gov.bd",
  "laws": [
    { "name_en": "Constitution of the People's Republic of Bangladesh", "name_bn": "গণপ্রজাতন্ত্রী বাংলাদেশের সংবিধান", "year": 1972, "category": "constitutional", "notes": "Adopted 4 Nov 1972, effective 16 Dec 1972. Multiple amendments (see constitution/README.md)." },
    { "name_en": "The Penal Code", "name_bn": "দণ্ডবিধি", "year": 1860, "category": "criminal", "notes": "511 sections. See codes/penal-code-1860.md" },
    { "name_en": "The Code of Criminal Procedure", "name_bn": "ফৌজদারি কার্যবিধি", "year": 1898, "category": "criminal-procedure", "notes": "See codes/crpc-1898.md" },
    { "name_en": "The Code of Civil Procedure", "name_bn": "দেওয়ানি কার্যবিধি", "year": 1908, "category": "civil-procedure", "notes": "See codes/cpc-1908.md" },
    { "name_en": "The Evidence Act", "name_bn": "সাক্ষ্য আইন", "year": 1872, "category": "evidence", "notes": "See codes/evidence-act-1872.md" },
    { "name_en": "The Contract Act", "name_bn": "চুক্তি আইন", "year": 1872, "category": "commercial" },
    { "name_en": "The Negotiable Instruments Act", "name_bn": "নেগোশিয়েবল ইনস্ট্রুমেন্টস আইন", "year": 1881, "category": "commercial", "notes": "s. 138 — cheque dishonour" },
    { "name_en": "The Transfer of Property Act", "name_bn": "স্থাবর সম্পত্তি হস্তান্তর আইন", "year": 1882, "category": "property" },
    { "name_en": "The Registration Act", "name_bn": "রেজিস্ট্রেশন আইন", "year": 1908, "category": "property" },
    { "name_en": "The Limitation Act", "name_bn": "পরিপালন আইন (লিমিটেশন)", "year": 1908, "category": "procedure" },
    { "name_en": "The Companies Act", "name_bn": "কোম্পানি আইন", "year": 1994, "category": "commercial", "notes": "RJSC: https://rjsc.gov.bd" },
    { "name_en": "The Partnership Act", "name_bn": "অংশীদারিত্ব আইন", "year": 1932, "category": "commercial" },
    { "name_en": "Bangladesh Labour Act", "name_bn": "বাংলাদেশ শ্রম আইন", "year": 2006, "category": "labour", "notes": "Amended 2013, 2018. See acts/labour/" },
    { "name_en": "Nari O Shishu Nirjatan Daman Ain", "name_bn": "নারী ও শিশু নির্যাতন দমন আইন", "year": 2000, "category": "criminal-special", "notes": "Special tribunals" },
    { "name_en": "Acid Oporadh Daman Ain", "name_bn": "এসিড অপরাধ দমন আইন", "year": 2002, "category": "criminal-special" },
    { "name_en": "Dowry Prohibition Act", "name_bn": "যৌতুক নিরোধ আইন", "year": 1980, "category": "family" },
    { "name_en": "Child Marriage Restraint Act", "name_bn": "বাল্যবিবাহ নিরোধ আইন", "year": 2017, "category": "family" },
    { "name_en": "Muslim Family Laws Ordinance", "name_bn": "মুসলিম পারিবারিক আইন অধ্যাদেশ", "year": 1961, "category": "family" },
    { "name_en": "Family Courts Ordinance", "name_bn": "পারিবারিক আদালত অধ্যাদেশ", "year": 1985, "category": "family" },
    { "name_en": "Children Act", "name_bn": "শিশু আইন", "year": 2013, "category": "children" },
    { "name_en": "Cyber Security Act", "name_bn": "সাইবার নিরাপত্তা আইন", "year": 2023, "category": "cyber", "notes": "Replaced Digital Security Act 2018. Verify current status — cyber legislation changes frequently." },
    { "name_en": "Consumer Rights Protection Act", "name_bn": "ভোক্তা অধিকার সংরক্ষণ আইন", "year": 2009, "category": "consumer", "notes": "DNCRP hotline 16121" },
    { "name_en": "Artha Rin Adalat Ain", "name_bn": "অর্থ ঋণ আদালত আইন", "year": 2003, "category": "commercial", "notes": "Money loan courts" },
    { "name_en": "Legal Aid Services Act", "name_bn": "আইনগত সহায়তা প্রদান আইন", "year": 2000, "category": "legal-aid", "notes": "NLASO hotline 16430" },
    { "name_en": "Right to Information Act", "name_bn": "তথ্য অধিকার আইন", "year": 2009, "category": "governance" },
    { "name_en": "Domestic Violence (Prevention and Protection) Act", "name_bn": "পারিবারিক সহিংসতা (প্রতিরোধ ও সুরক্ষা) আইন", "year": 2010, "category": "women-children" },
    { "name_en": "Prevention of Human Trafficking Act", "name_bn": "মানব পাচার প্রতিরোধ আইন", "year": 2012, "category": "criminal-special" }
  ]
}
