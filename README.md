# ZaloQT - Linux Release Build

<div align="center">
  <img src="mainIco.png" alt="ZaloQT Icon" width="500" height="500">
</div>

[![Linux](https://img.shields.io/badge/OS-Linux-blue.svg)](https://www.linux.org/) [![Qt6](https://img.shields.io/badge/Qt-6-green.svg)](https://www.qt.io/) [![C++](https://img.shields.io/badge/Language-C%2B%2B-orange.svg)](https://isocpp.org/) [![OpenAI](https://img.shields.io/badge/AI-OpenAI-412991.svg)](https://openai.com/)

**ZaloQT: An Unofficial Qt6-based Zalo Client for Linux**

## 📋 Description

ZaloQT is an unofficial desktop client for Zalo, built with Qt6/C++ specifically for Linux. This project offers an unofficial Zalo desktop experience for Linux users, developed using C++ with Qt 6 and Qt WebEngine. It aims to provide a more integrated, feature-rich, and responsive alternative to web versions or Electron ports, with a key focus on message translation powered by OpenAI API.

## ✨ Key Features

- 🖥️ **Native Qt6 Application**: Built specifically for Linux with optimal performance
- 🌐 **Core Zalo Web Integration**: Displays Zalo Web (`https://chat.zalo.me/`) via QtWebEngine
- 🔐 **Persistent User Sessions**: Remembers your login across sessions, eliminating frequent QR code scans
- 🤖 **Integrated OpenAI-Powered Translation**:
  - Per-chat language configuration with auto-detect option
  - Automatic incoming message translation
  - Outgoing message translation before sending
  - On-demand translation with "⤾ Translate" button
  - Persistent translation settings per chat
- 🎨 **Enhanced UI Features**:
  - Dynamic UI injection with custom controls
  - Automatic ad/banner hiding
  - Custom window style and system tray integration
- 🔧 **Advanced Settings**: GPU acceleration control and debug tools
- 📝 **Developer Tools**: Web Inspector and JavaScript logging window

## 🚀 Quick Start

1. **Download the executable:**
   ```bash
   wget https://github.com/DXVSI/ZaloQT/raw/main/ZaloQT
   chmod +x ZaloQT
   ```

2. **Run the application:**
   ```bash
   ./ZaloQT
   ```

## 📦 System Requirements

### Minimum Requirements:
- **OS**: Linux (tested on Fedora 42)
- **Architecture**: x86_64
- **RAM**: 2GB free memory
- **Disk Space**: 50MB

### Dependencies:
The application uses system Qt6 libraries. On most modern distributions they are already installed. If you encounter errors on startup, install:

**Fedora/RHEL/CentOS:**
```bash
sudo dnf install -y qt6-qtbase qt6-qtwebengine qt6-qtdeclarative
```

## ⚙️ OpenAI Translator Setup

1. Go to **OpenAISettings** → **Install OpenAI API Key**
2. Enter your OpenAI API key (starts with `sk-`)
3. Select model in **OpenAISettings** → **Choose OpenAI Model**
4. Available models:
   - `o3-2025-04-16` (latest)
   - `gpt-4o-2024-11-20` (recommended)
   - `gpt-4-turbo-2024-04-09`
   - `gpt-3.5-turbo-0125`
   - `o1-mini-2024-09-12`
   - And other latest models

## 🔧 Translation Features

- **Automatic incoming message translation**
- **Outgoing message translation before sending**
- **On-demand translation via "⤾ Translate" button**
- **Multi-language support**
- **Automatic source language detection**

## 🛠️ Additional Settings

### GPU Acceleration:
If you experience display issues, disable GPU acceleration in **Settings** → **Disable GPU acceleration**.

### Debug Mode:
Developer tools available via hotkeys:
- `Ctrl+Shift+I` - Developer Tools
- `Ctrl+Shift+L` - JavaScript Log Window

## 🐛 Troubleshooting

### Application won't start:
```bash
# Check dependencies
ldd ZaloQT

# Run with debug output
QT_LOGGING_RULES="*=true" ./ZaloQT
```

### WebEngine issues:
```bash
# Run without GPU acceleration
./ZaloQT --disable-gpu
```

---

# ZaloQT - Bản Build cho Linux

**ZaloQT: Ứng dụng Zalo không chính thức dựa trên Qt6 cho Linux**

## 📋 Mô tả

ZaloQT là một ứng dụng Zalo không chính thức cho desktop, được xây dựng bằng Qt6/C++ đặc biệt dành cho Linux. Dự án này cung cấp trải nghiệm Zalo desktop không chính thức cho người dùng Linux, được phát triển bằng C++ với Qt 6 và Qt WebEngine. Mục tiêu là cung cấp một giải pháp thay thế tích hợp hơn, giàu tính năng hơn và phản hồi nhanh hơn so với các phiên bản web hoặc Electron ports, với trọng tâm chính là dịch thuật tin nhắn được hỗ trợ bởi OpenAI API.

## ✨ Tính năng chính

- 🖥️ **Ứng dụng Qt6 gốc**: Được xây dựng đặc biệt cho Linux với hiệu suất tối ưu
- 🌐 **Tích hợp Zalo Web**: Hiển thị Zalo Web (`https://chat.zalo.me/`) qua QtWebEngine
- 🔐 **Phiên đăng nhập liên tục**: Ghi nhớ đăng nhập qua các phiên, loại bỏ việc quét mã QR thường xuyên
- 🤖 **Dịch thuật tích hợp OpenAI**:
  - Cấu hình ngôn ngữ cho từng cuộc trò chuyện với tùy chọn tự động phát hiện
  - Dịch tự động tin nhắn đến
  - Dịch tin nhắn đi trước khi gửi
  - Dịch theo yêu cầu với nút "⤾ Translate"
  - Cài đặt dịch thuật liên tục cho từng cuộc trò chuyện
- 🎨 **Tính năng UI nâng cao**:
  - Chèn UI động với các điều khiển tùy chỉnh
  - Tự động ẩn quảng cáo/banner
  - Phong cách cửa sổ tùy chỉnh và tích hợp system tray
- 🔧 **Cài đặt nâng cao**: Kiểm soát gia tốc GPU và công cụ debug
- 📝 **Công cụ phát triển**: Web Inspector và cửa sổ logging JavaScript

## 🚀 Bắt đầu nhanh

1. **Tải xuống file thực thi:**
   ```bash
   wget https://github.com/DXVSI/ZaloQT/raw/main/ZaloQT
   chmod +x ZaloQT
   ```

2. **Chạy ứng dụng:**
   ```bash
   ./ZaloQT
   ```

## 📦 Yêu cầu hệ thống

### Yêu cầu tối thiểu:
- **OS**: Linux (đã test trên Fedora 42)
- **Kiến trúc**: x86_64
- **RAM**: 2GB bộ nhớ trống
- **Dung lượng đĩa**: 50MB

### Phụ thuộc:
Ứng dụng sử dụng thư viện Qt6 hệ thống. Trên hầu hết các bản phân phối hiện đại chúng đã được cài sẵn. Nếu gặp lỗi khi khởi động, hãy cài đặt:

**Fedora/RHEL/CentOS:**
```bash
sudo dnf install -y qt6-qtbase qt6-qtwebengine qt6-qtdeclarative
```

## ⚙️ Thiết lập OpenAI Translator

1. Vào **OpenAISettings** → **Install OpenAI API Key**
2. Nhập API key OpenAI của bạn (bắt đầu bằng `sk-`)
3. Chọn model trong **OpenAISettings** → **Choose OpenAI Model**
4. Các model có sẵn:
   - `o3-2025-04-16` (mới nhất)
   - `gpt-4o-2024-11-20` (khuyến nghị)
   - `gpt-4-turbo-2024-04-09`
   - `gpt-3.5-turbo-0125`
   - `o1-mini-2024-09-12`
   - Và các model mới nhất khác

## 🔧 Tính năng dịch thuật

- **Dịch tự động tin nhắn đến**
- **Dịch tin nhắn đi trước khi gửi**
- **Dịch theo yêu cầu qua nút "⤾ Translate"**
- **Hỗ trợ đa ngôn ngữ**
- **Tự động phát hiện ngôn ngữ nguồn**

## 🛠️ Cài đặt bổ sung

### Gia tốc GPU:
Nếu gặp vấn đề hiển thị, tắt gia tốc GPU trong **Settings** → **Disable GPU acceleration**.

### Chế độ debug:
Công cụ phát triển có sẵn qua phím tắt:
- `Ctrl+Shift+I` - Developer Tools
- `Ctrl+Shift+L` - JavaScript Log Window

## 🐛 Xử lý sự cố

### Ứng dụng không khởi động:
```bash
# Kiểm tra phụ thuộc
ldd ZaloQT

# Chạy với output debug
QT_LOGGING_RULES="*=true" ./ZaloQT
```

### Vấn đề WebEngine:
```bash
# Chạy không có gia tốc GPU
./ZaloQT --disable-gpu
```

## 📄 Giấy phép

Đây là ứng dụng không chính thức. Zalo là thương hiệu của VNG Corporation.

## 🤝 Hỗ trợ

Nếu bạn gặp vấn đề:
1. Kiểm tra phần "Xử lý sự cố" ở trên
2. Tạo Issue trong repository mã nguồn chính
3. Đảm bảo hệ thống của bạn đáp ứng yêu cầu tối thiểu

---

**Version**: 1.0  
**Build Date**: 2024-12-31  
**Build System**: Fedora Linux 42 KDE Plasma + qmake + Qt6 
