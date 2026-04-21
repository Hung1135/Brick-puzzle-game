# 🎮 Business Requirement Document (BRD)
## Game Xếp Gạch (Brick Puzzle Game)

---

## 1. Giới thiệu

### 1.1 Mục tiêu
Tài liệu này mô tả các yêu cầu nghiệp vụ cho việc phát triển game xếp gạch. Mục tiêu là xây dựng một trò chơi giải trí đơn giản, dễ tiếp cận, nhưng có tính gây nghiện và cạnh tranh cao.

### 1.2 Phạm vi
- Phát triển game chạy trên:
  - Desktop (Windows/macOS) hoặc Web (tùy đồ án)
- Không bao gồm:
  - Multiplayer online phức tạp (optional nâng cao)

---

## 2. Tổng quan sản phẩm

### 2.1 Mô tả sản phẩm
Game xếp gạch là trò chơi mà người chơi điều khiển các khối hình rơi xuống để tạo thành hàng ngang hoàn chỉnh và ghi điểm.

### 2.2 Đối tượng người dùng
- Người chơi casual (giải trí)
- Sinh viên, học sinh
- Người chơi mọi lứa tuổi

### 2.3 Giá trị mang lại
- Giải trí nhanh
- Rèn luyện tư duy logic
- Tăng khả năng phản xạ

---

## 3. Yêu cầu chức năng (Functional Requirements)

### 3.1 Gameplay cơ bản
- Các khối gạch (Tetromino) rơi từ trên xuống
- Người chơi có thể:
  - Di chuyển trái/phải
  - Xoay khối
  - Thả nhanh (hard drop)
  - Thả nhanh vừa (soft drop)

### 3.2 Cơ chế ghi điểm
- Xóa 1 hàng: +100 điểm
- Xóa nhiều hàng cùng lúc:
  - 2 hàng: +300
  - 3 hàng: +500
  - 4 hàng: +800

### 3.3 Tăng độ khó
- Tốc độ rơi tăng theo thời gian hoặc level
- Level tăng sau mỗi X điểm hoặc số hàng xóa

### 3.4 Điều kiện thắng/thua
- Thua khi:
  - Gạch chạm đỉnh màn hình
- Không có điều kiện thắng (endless mode)

### 3.5 Giao diện người dùng
- Màn hình chính:
  - Start Game
  - Settings
  - Exit
- Màn hình chơi:
  - Bảng điểm
  - Level
  - Khối tiếp theo
- Màn hình Game Over:
  - Hiển thị điểm
  - Replay

---

## 4. Yêu cầu phi chức năng (Non-functional Requirements)

### 4.1 Hiệu năng
- Game chạy mượt ở ≥ 30 FPS
- Thời gian phản hồi < 100ms

### 4.2 Khả dụng (Usability)
- Giao diện đơn giản, dễ hiểu
- Điều khiển trực quan

### 4.3 Tính ổn định
- Không crash khi chơi liên tục ≥ 30 phút

### 4.4 Khả năng mở rộng
- Có thể thêm:
  - Multiplayer
  - Skin/theme
  - Leaderboard online

---

## 5. Luồng người dùng (User Flow)

1. Người chơi mở game
2. Chọn "Start Game"
3. Bắt đầu chơi:
   - Điều khiển khối gạch
   - Ghi điểm
4. Game Over:
   - Hiển thị điểm
   - Chọn chơi lại hoặc thoát

---

## 6. Use Case chính

### 6.1 Chơi game
- Actor: Người chơi
- Mô tả:
  - Người chơi điều khiển khối gạch để xếp hàng

### 6.2 Tạm dừng game
- Actor: Người chơi
- Mô tả:
  - Nhấn nút pause để tạm dừng

### 6.3 Xem điểm
- Actor: Người chơi
- Mô tả:
  - Xem điểm hiện tại và điểm cao nhất

---

## 7. Ràng buộc (Constraints)

- Thời gian phát triển giới hạn (theo đồ án)
- Công nghệ:
  - Unity / Java / Web (tùy chọn)
- Không sử dụng server (phiên bản cơ bản)

---

## 8. Giả định (Assumptions)

- Người chơi đã quen với gameplay cơ bản
- Không cần tutorial phức tạp
- Game chạy offline

---

## 9. Tiêu chí thành công (Success Criteria)

- Game chạy ổn định
- Gameplay mượt, không lag
- Người chơi có thể chơi liên tục ≥ 10 phút
- Có hệ thống điểm rõ ràng

---

## 10. Hướng phát triển tương lai

- Thêm chế độ multiplayer
- Leaderboard online
- Custom block / skin
- Sound & animation nâng cao

---

## 11. Phụ lục

### 11.1 Thuật ngữ
- Tetromino: Khối gạch gồm 4 ô
- Hard Drop: Thả gạch xuống ngay lập tức
- Soft Drop: Tăng tốc độ rơi

---

**Tác giả:**  
**Ngày:**  
**Phiên bản:** 1.0
