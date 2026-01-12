# Wallist_Euphoria

Aidrop Free : https://t.me/HVchannelss/229

Auto Wallist_Euphoria 

<img width="1920" height="1080" alt="Screenshot (28)" src="https://github.com/user-attachments/assets/ad3e0595-87e5-4629-9b73-d3b34c1d7346" />

Tham Gia Discor ( Vip ) : https://discord.gg/gKxvTNu5

Tham gia NHóm VIp Với Chi Phí 8u/1thang Lợi ích tham gia nhóm ViP Sẽ được cấp keey sử dụng các tool vip trong discor hỗ trợ Và tham khao Code các tool dự án mà các bạn đề xuất

Gửi Phí tháng vào đây và chụp hình gửi trực tiếp cho tôi tại discor để xác nhận Role VIp ☕ https://huynhviet933.github.io/donate_viet_mmo/ Có thể tặng tôi ít cafe tại đây

# 🚀 GetWaitlist Auto Signup Tool (Multi-thread + Proxy + Ref)

Tool Node.js giúp **tự động signup GetWaitlist**, hỗ trợ:
- Proxy xoay vòng (tự loại proxy die)
- Ref theo danh sách
- Tự lưu mail đã chạy
- Log màu dễ nhìn
- Chạy lại không trùng mail

---

## 📁 1. Cấu trúc thư mục

Sau khi clone hoặc tải tool, thư mục cần có dạng:

```
GetWaitlist/
├─ main.js
├─ profilemanager.js
├─ mail.txt
├─ user_agents.txt
├─ proxy.txt
├─ ref.txt
├─ maildone.txt        (tự tạo)
├─ coderef.txt         (tự tạo)
├─ profiles.json       (tự tạo)
└─ package.json
```

---

## 📦 2. Cài đặt môi trường

### Yêu cầu
- **Node.js >= 18** (khuyên dùng 20 hoặc 22)
- Proxy HTTP/HTTPS

### Cài thư viện
```bash
npm install axios https-proxy-agent
```

---

## ✉️ 3. Tạo các file `.txt`

### 📄 `mail.txt`
Danh sách email cần signup  
➡️ **1 dòng = 1 email**

```
abc123@airsworld.net
xyz789@airsworld.net
mailtest01@gmail.com
```

Mail chạy xong sẽ:
- ❌ Bị xóa khỏi `mail.txt`
- ✅ Được ghi vào `maildone.txt`

---

### 🌐 `proxy.txt`
Danh sách proxy (HTTP / HTTPS)

Hỗ trợ:
```
http://ip:port
http://user:pass@ip:port
```

Ví dụ:
```
http://103.179.189.46:8000
http://user123:pass123@45.77.88.99:3128
```

🔹 Proxy lỗi sẽ **tự động bị ẩn và bỏ qua**, không log lỗi.

---

### 🧭 `user_agents.txt`
Danh sách User-Agent  
➡️ Hết UA sẽ **quay lại từ đầu**

```
Mozilla/5.0 (Windows NT 10.0; Win64; x64) Chrome/120.0.0.0
Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) Safari/605.1.15
Mozilla/5.0 (X11; Linux x86_64) Chrome/119.0.0.0

---

## ▶️ 4. Chạy tool

```bash
node main.js
```

---

## 🖥 5. Log hiển thị (ví dụ)

```
W 2 | mail : ayg9uu75@airsworld.net | IP : 172.111.171.186 | UA : OK | UUID : b98dd348-479f-457a-8a49-82b09fbfffb0 | Waitlist : Success | Delay : 34s...
```

### Ý nghĩa:
- **W 2**: số thứ tự mail
- **mail**: email signup
- **IP**: IP proxy đang dùng
- **UA**: User-Agent hợp lệ
- **UUID**: định danh cố định cho mail
- **Waitlist**: trạng thái signup
- **Delay**: thời gian nghỉ trước mail tiếp theo

---

## 📂 6. File sinh tự động

| File | Mô tả |
|----|----|
| `maildone.txt` | Mail đã signup thành công |
| `profiles.json` | Lưu UUID + UA + proxy cố định cho mail |

➡️ Restart tool **không chạy lại mail cũ**.


---

## 📜 Disclaimer
Tool chỉ dùng cho **test / research / automation cá nhân**.  
Người dùng tự chịu trách nhiệm khi sử dụng.

---

