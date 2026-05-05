# 🛰️ Network Scanner 🔥  
### ⚡ ARP ভিত্তিক লোকাল নেটওয়ার্ক স্ক্যানার

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Platform](https://img.shields.io/badge/Platform-Linux-green)
![Status](https://img.shields.io/badge/Status-Active-success)
![Purpose](https://img.shields.io/badge/Purpose-Ethical%20Hacking-red)

---

## 🚀 প্রজেক্ট পরিচিতি

এই টুলটি ব্যবহার করে আপনি খুব সহজে আপনার লোকাল নেটওয়ার্কে  
কোন কোন ডিভাইস চালু আছে তা খুঁজে বের করতে পারবেন।

👉 এটি ARP (Address Resolution Protocol) ব্যবহার করে কাজ করে।

---

## ✨ ফিচারসমূহ

- 🔍 সাবনেট স্ক্যান (192.168.0.1/24)
- 🟢 লাইভ হোস্ট ডিটেকশন
- 🌐 IP Address সংগ্রহ
- 🔗 MAC Address শনাক্তকরণ
- 🏢 Vendor Lookup (যদি পাওয়া যায়)

---

## 🖼️ Output Preview


+---------------+-------------------+---------+
| IP | MAC | Vendor |
+---------------+-------------------+---------+
| 192.168.0.1 | xx:xx:xx:xx:xx:xx | Unknown |
+---------------+-------------------+---------+


---

## ⚙️ Setup Guide

### 1️⃣ Virtual Environment তৈরি করুন

```
python3 -m venv myenv
```
2️⃣ Activate করুন
```
source myenv/bin/activate
```
3️⃣ প্রয়োজনীয় প্যাকেজ ইন্সটল করুন
```
pip install scapy prettytable mac_vendor_lookup
```
🚀 Usage
```
source myenv/bin/activate
sudo /home/kali/myenv/bin/python3 netscanner.py --h 192.168.0.1/24
```
🧠 Working Process
📡 ARP Broadcast Packet পাঠানো হয়
🌐 Network এর সব IP-তে Request যায়
🟢 Active Device Response দেয়
📊 Data collect করে Table আকারে দেখানো হয়
⚠️ Important Notes
🔒 sudo ছাড়া কাজ করবে না (Raw Socket দরকার)
⏱️ Timeout এর কারণে কিছু host miss হতে পারে
📶 Network condition অনুযায়ী result change হতে পারে
😴 Sleep mode device detect নাও হতে পারে
🧰 Tools Used
🐍 Scapy → Packet crafting
📊 PrettyTable → Output formatting
🏢 MAC Vendor Lookup → Vendor detection
📌 Future Improvements (Idea 💡)
⚡ Multi-threading (fast scan)
📁 Export (CSV / JSON)
🌍 GUI Version
⚖️ Disclaimer

এই টুলটি শুধুমাত্র
👉 Educational & Ethical Hacking purpose এর জন্য।

অন্য কারো নেটওয়ার্কে অনুমতি ছাড়া ব্যবহার করা আইনত দণ্ডনীয়।

👨‍💻 Author

SHAJALAL
Ethical Hacker | Cybersecurity Learner 🚀
