# GSAP_SCROLLEFFECT

## Giới thiệu
Dự án này được phát triển sử dụng các công nghệ cơ bản:

- **HTML**: Để cấu trúc nội dung.
- **CSS**: Để tạo phong cách và giao diện.
- **JavaScript**: Để tạo các tương tác động.

Ngoài ra, dự án tích hợp hai thư viện mạnh mẽ:

- **GSAP (GreenSock Animation Platform)**: Một thư viện hoạt hình mạnh mẽ giúp tạo các hiệu ứng chuyển động mượt mà và tối ưu.
- **Three.js**: Thư viện 3D giúp hiển thị các đối tượng và hoạt cảnh 3D trên trình duyệt.

---

## Cấu trúc thư mục

```
project-root/
|-- index.html         # File HTML chính
|-- styles/
|   |-- main.css       # File CSS chính
|-- scripts/
|   |-- main.js        # File JavaScript chính
|   |-- gsap-utils.js  # Các tiện ích hỗ trợ sử dụng GSAP
|   |-- three-utils.js # Các tiện ích hỗ trợ sử dụng Three.js
|-- assets/            # Lưu trữ hình ảnh, mô hình 3D, textures...
|-- README.md          # Tài liệu hướng dẫn
```

---

## Các tính năng chính

1. **Hiệu ứng hoạt hình với GSAP**:
   - Tạo các hiệu ứng chuyển động phức tạp và tối ưu hiệu suất.
   - Sử dụng Timeline để kiểm soát chuỗi hoạt hình.

2. **Đối tượng 3D với Three.js**:
   - Hiển thị và tương tác với các mô hình 3D.
   - Tích hợp ánh sáng, textures, và camera để tạo không gian 3D sống động.

---

## Cách cài đặt

1. Clone dự án:
   ```bash
   git clone https://github.com/your-repo.git
   ```

2. Cài đặt các dependencies (nếu cần):
   - Với npm:
     ```bash
     npm install
     ```

3. Khởi chạy dự án:
   - Mở file `index.html` trong trình duyệt hoặc sử dụng Live Server nếu bạn đang làm việc với Visual Studio Code.

---

## Sử dụng

### GSAP
- Import thư viện GSAP trong file `main.js`:
  ```javascript
  import gsap from 'gsap';

  gsap.to('.element', { duration: 1, x: 100 });
  ```

### Three.js
- Khởi tạo một scene cơ bản:
  ```javascript
  import * as THREE from 'three';

  const scene = new THREE.Scene();
  const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
  const renderer = new THREE.WebGLRenderer();

  renderer.setSize(window.innerWidth, window.innerHeight);
  document.body.appendChild(renderer.domElement);
  ```

---

## Đóng góp

Nếu bạn muốn đóng góp cho dự án, vui lòng tạo một pull request hoặc báo cáo lỗi tại [issues](https://github.com/your-repo/issues).

---

## Liên hệ

Nếu bạn có bất kỳ câu hỏi nào, vui lòng liên hệ qua email: your-email@example.com

---

## Giấy phép

Dự án này được cấp phép theo [MIT License](LICENSE).

