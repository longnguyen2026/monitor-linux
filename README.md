### Lệnh 1 dòng duy nhất để chạy trên máy trạm

```bash
curl -fsSL https://raw.githubusercontent.com/<username>/<repo>/main/install_monitor.sh | sudo bash

```

### Cách sử dụng sau khi cài

1. **Khi máy vừa bị treo và bật lại:**
Không cần nhớ đường dẫn file log phức tạp, chỉ cần mở Terminal gõ:
```bash
check-hang

```

Lệnh sẽ in ngay 35 dòng log cuối cùng kèm thời gian, lượng RAM/Swap và top tiến trình ngốn bộ nhớ nhất trước khi tắt máy.
2. **Gỡ bỏ hoàn toàn khỏi máy trạm:**
```bash
sudo uninstall-monitor

```
