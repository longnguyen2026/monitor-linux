# Lệnh 1 dòng duy nhất để chạy trên máy trạm

```bash
curl -fsSL https://raw.githubusercontent.com/longnguyen2026/monitor-linux/main/monitor.sh | sudo bash

```

### Lệnh gỡ trên máy trạm
```bash
sudo uninstall-monitor
```

# Cách sử dụng sau khi cài

### 1. Kiểm tra dịch vụ có đang chạy ổn định không

```bash
sudo systemctl status sys-monitor.service

```

> Trạng thái hiện `active (running)` màu xanh là dịch vụ đang chạy ngầm chính xác.

### 2. Kiểm tra log đã bắt đầu được ghi chưa

```bash
# Xem file log đang cập nhật trực tiếp theo thời gian thực (Ctrl + C để thoát)
tail -f /var/log/sys_monitor/sys_freeze.log

```

### 3. Kiểm tra lệnh tắt xem nhanh

```bash
check-hang

```

---

> **Lưu ý nhỏ:** Nếu chạy lệnh `curl ... | sudo bash` mà máy báo lỗi `curl: command not found` (một số bản Linux Mint cài tối giản chưa có sẵn `curl`), bạn có thể dùng `wget` thay thế:
> ```bash
> wget -qO- https://raw.githubusercontent.com/longnguyen2026/monitor-linux/main/monitor.sh | sudo bash
> 
> ```
> 
>
