# LH Synology Chunk Extension

## 🇻🇳 Tiếng Việt

### Giới thiệu

LH Synology Chunk là tiện ích mở rộng dành cho Chrome, Microsoft Edge và các trình duyệt Chromium, giúp tải file dung lượng lớn lên Synology File Station thông qua Cloudflare Tunnel mà không bị giới hạn 100 MB mỗi request.

**Tính năng chính:**
- Tự động nhận diện Synology File Station trên nhiều domain và địa chỉ IP.
- Tự động chia nhỏ file từ 90 MB trở lên.
- Tùy chỉnh kích thước chunk tối đa 99,9 MB.
- Giữ nguyên phương thức upload gốc đối với file nhỏ.
- Không cần chỉnh sửa DSM hoặc Cloudflare Tunnel.
- Không thu thập thông tin đăng nhập hoặc gửi dữ liệu ra bên ngoài.

### Hướng dẫn cài đặt

1. Tải và giải nén file ZIP của extension.
2. Mở trang quản lý tiện ích:
   - Chrome: `chrome://extensions`
   - Edge: `edge://extensions`
3. Bật **Chế độ nhà phát triển (Developer mode)**.
4. Chọn **Load unpacked** và chọn thư mục chứa file `manifest.json`.
5. Mở hoặc tải lại trang Synology DSM.
6. Nhấn biểu tượng extension để bật chức năng và tùy chỉnh kích thước chunk.

**Khuyến nghị:** Sử dụng chunk từ 64–95 MB để cân bằng tốc độ và độ ổn định. Có thể thử 99,9 MB để giảm số lượng request.

---

## 🇬🇧 English

### Overview

LH Synology Chunk is a browser extension for Google Chrome, Microsoft Edge, and other Chromium-based browsers. It enables large file uploads to Synology File Station through Cloudflare Tunnel by splitting files into smaller requests to work around the 100 MB per-request upload limit.

**Key features:**
- Automatically detects Synology File Station across multiple domains and IP addresses.
- Automatically splits files of 90 MB or larger.
- Customizable chunk size of up to 99.9 MB.
- Preserves native upload behavior for smaller files.
- No DSM or Cloudflare Tunnel modifications required.
- No credential collection or external data transmission.

### Installation

1. Download and extract the extension ZIP file.
2. Open the browser's extension management page:
   - Chrome: `chrome://extensions`
   - Edge: `edge://extensions`
3. Enable **Developer mode**.
4. Click **Load unpacked** and select the folder containing `manifest.json`.
5. Open or refresh your Synology DSM page.
6. Click the extension icon to enable chunked uploads and customize the chunk size.

**Recommendation:** Use a chunk size of 64–95 MB for a balance between performance and stability. You can also try 99.9 MB to reduce the number of upload requests.

---

**Version:** 1.1.0  
**License:** Not yet specified  
**Compatibility:** Chromium-based browsers  
**Requirements:** Synology DSM with a compatible File Station uploader

*Note: Compatibility may vary depending on the File Station version. The extension uses Synology's existing chunked upload mechanism.*
