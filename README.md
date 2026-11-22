# DoAn_StarboundRemnant_MTA
# ĐỒ ÁN MÔN HỌC: TƯƠNG TÁC ĐỐI TƯỢNG (MTA)

* **Tên đề tài:** Game 3D Action-Adventure "Starbound Remnant"
* **Sinh viên thực hiện:** Phạm Tiến Đạt
* **Mã sinh viên:** 2924124641
* **Lớp:** TH29.23 | Công nghệ Thông tin - MTA

---

## 1. Giới thiệu Game & Cốt truyện
"Starbound Remnant" là tựa game phiêu lưu hành động 3D kết hợp giải đố góc nhìn thứ ba, được phát triển trên nền tảng Unity Engine.

Cốt truyện xoay quanh nữ kỹ sư phi hành gia Ellen sau khi phi thuyền của cô gặp sự cố và rơi xuống một hành tinh hoang phế ngập tràn tàn tích cổ xưa của nền văn minh Remnant. Ellen phải vượt qua các hòn đảo đá bay lơ lửng, chiến đấu với bầy quái vật bản địa hung hãn (Chomper, Spitter) và giải mã các cơ quan phong ấn để kích hoạt Đài Dịch Chuyển Không Gian (Transition Destination) nhằm thoát khỏi hành tinh.

---

## 2. Các quy luật chơi chính (Game Rules & Mechanics)

### a. Quy luật Di chuyển & Rơi vực
* Người chơi điều khiển nhân vật ở góc nhìn thứ 3 (phím W, A, S, D để di chuyển, Space để nhảy, Shift để chạy nhanh).
* Nếu sẩy chân rơi khỏi đảo bay xuống vực thẳm, bộ giáp bảo hộ sinh học sẽ tự động trừ 1 điểm HP và dịch chuyển nhân vật về vị trí an toàn/Checkpoint gần nhất.

### b. Quy luật Chiến đấu & Sinh lực
* **Tấn công:** Tấn công cận chiến bằng gậy năng lượng cứu hộ theo chuỗi combo 3 nhịp; có thể phá hủy các hòm gỗ để nhặt tinh thể nạp lại máu (HP).
* **Máu & Sinh tồn:** Bắt đầu với thanh máu tối đa. Khi nhận sát thương từ quái vật hoặc bẫy, nhân vật bị trừ máu và có 1 giây chớp nháy bất tử tạm thời. Nếu HP = 0 sẽ thất bại (Game Over).

### c. Quy luật Kẻ thù (AI Behaviors)
* **Quái cận chiến (Chomper):** Tuần tra theo vùng, khi phát hiện người chơi sẽ gầm lên và lao vào cắn xé.
* **Quái tầm xa (Spitter):** Giữ khoảng cách và liên tục bắn ra các viên cầu axit độc hại.
* **Trùm cuối (Grenadier - Boss):** Quái vật đá khổng lồ canh giữ lối thoát, có khả năng ném lựu đạn năng lượng diện rộng.

### d. Quy luật Giải đố & Mở cổng phong ấn
* Người chơi phải tương tác với môi trường: dẫm lên các phiến đá cảm ứng áp lực (Pressure Plates) hoặc kích hoạt cần gạt để mở khóa các cổng đá cổ đại và gọi cầu đá di động vượt vực sâu.

### e. Điều kiện Thắng / Thua
* **Thua:** Điểm máu cạn kiệt (HP = 0).
* **Thắng:** Vượt qua bầy quái vật, giải hết các câu đố cơ quan và bước vào trung tâm Cổng Dịch Chuyển (Transition Destination) ở đỉnh tàn tích.

---

## 3. Cấu trúc Mã nguồn (Code Submission)
Toàn bộ mã nguồn C# lập trình tạo đối tượng và xử lý các sự kiện trong game đã được nén đóng gói đầy đủ trong file:
* **`SourceCode_Scripts.zip`** (gồm hơn 160 file code C# về Player Controller, Enemy AI, Damageable, Game Event và Interactable Systems).
