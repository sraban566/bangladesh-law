# Claude-এ ইনস্টল / Install on Claude

## পদ্ধতি ১: Claude.ai Project (সবচেয়ে সহজ, যেকোনো ব্যবহারকারীর জন্য)

1. https://claude.ai-এ যান → **Projects** → **Create Project** → নাম দিন "Bangladesh Law"
2. **Project Knowledge**-এ এই repo-র markdown ফাইলগুলো আপলোড করুন (বা GitHub থেকে zip নামিয়ে আপলোড)
3. **Custom Instructions**-এ `SKILL.md`-এর পুরো কনটেন্ট কপি-পেস্ট করুন
4. ব্যস! এখন Project-এর ভেতরে যেকোনো প্রশ্ন করলে Claude এই repo-র তথ্য দিয়ে ডিজিটাল আইন সহকারী হিসেবে উত্তর দেবে

## পদ্ধতি ২: Claude Code (ডেভেলপারদের জন্য)

Repo-টি clone করুন — Claude Code স্বয়ংক্রিয়ভাবে `CLAUDE.md`/`AGENTS.md` পড়ে নেয়:

```bash
git clone https://github.com/<username>/bangladesh-law.git
cd bangladesh-law
claude
```

এই repo-তে `AGENTS.md` আছে; চাইলে এটিকে `CLAUDE.md` হিসেবেও কপি করতে পারেন।

## পদ্ধতি ৩: Claude Skill

`SKILL.md` ফাইলটি Claude-এর skill ফরম্যাটে লেখা (frontmatter সহ)। Skills সাপোর্ট করা এনভায়রনমেন্টে এই ফাইলটি skill ডিরেক্টরিতে রাখলেই কাজ করবে।
