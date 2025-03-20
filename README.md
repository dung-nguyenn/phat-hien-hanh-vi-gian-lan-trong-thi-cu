# phat-hien-hanh-vi-gian-lan-trong-thi-cu
phát hiện hành vi gian lận trong thi cử
# 🎓 Phát Hiện Hành Vi Gian Lận Trong Thi Cử  
🚀 *Ứng dụng AI hỗ trợ giám sát kỳ thi trực tuyến và trực tiếp*  

![GitHub repo size](https://img.shields.io/github/repo-size/dung-nguyenn/phat-hien-hanh-vi-gian-lan-trong-thi-cu)
![GitHub stars](https://img.shields.io/github/stars/dung-nguyenn/phat-hien-hanh-vi-gian-lan-trong-thi-cu?style=social)
![License](https://img.shields.io/github/license/dung-nguyenn/phat-hien-hanh-vi-gian-lan-trong-thi-cu)

---

## 📌 Giới thiệu  

Dự án này sử dụng **Trí tuệ nhân tạo (AI) và Thị giác máy tính (Computer Vision)** để phát hiện hành vi gian lận trong thi cử.  
Hệ thống nhận diện các hành động đáng ngờ qua camera như:  
✔️ Nhìn ra ngoài màn hình  
✔️ Nói chuyện hoặc trao đổi với người khác  
✔️ Sử dụng thiết bị không được phép (điện thoại, tài liệu)  

🔹 **Mục tiêu**:  
- Giám sát kỳ thi **trực tuyến & trực tiếp**.  
- Tăng tính **công bằng & minh bạch** trong giáo dục.  
- Giảm tải công việc giám thị nhờ **AI tự động**.  

---

## 🛠 Công nghệ sử dụng  

| Công nghệ | Mô tả |
|-----------|------|
| Python 🐍 | Ngôn ngữ lập trình chính |
| OpenCV 👁 | Nhận diện hành vi qua camera |
| TensorFlow / PyTorch 🤖 | Huấn luyện mô hình AI |
| MediaPipe 🖐 | Nhận diện cử chỉ và khuôn mặt |
| NumPy / Pandas 📊 | Xử lý dữ liệu |
| Matplotlib 📈 | Hiển thị kết quả |

---

📊 Quy trình phát hiện gian lận
Hệ thống phát hiện gian lận trong thi cử sử dụng YOLOv11, với các bước chính như sau:

1️⃣ S0: Input – Nhận video đầu vào từ camera giám sát lớp học.

2️⃣ S1: Processing – Tiền xử lý dữ liệu, chuẩn hóa và tăng cường dữ liệu.

3️⃣ S2: Detection – Nhận diện học sinh, phát hiện hành vi gian lận bằng mô hình YOLOv11.

4️⃣ S3: Alert System – Cảnh báo gian lận theo thời gian thực.

5️⃣ S4: Evidence Logging – Lưu trữ bằng chứng và xuất báo cáo.

![image](https://github.com/user-attachments/assets/afaca065-ed5c-4acb-b5b5-4eed9f0a14cd)

---

## 📡 Kiến trúc hệ thống  

Hệ thống phát hiện gian lận được triển khai với các thành phần chính sau:  

1️⃣ **Camera giám sát** – Ghi lại hình ảnh trong lớp học. 

2️⃣ **Máy tính xử lý** – Chạy mô hình YOLOv11 để nhận diện hành vi gian lận.  

3️⃣ **Hệ thống mạng & lưu trữ** – Truyền và lưu trữ dữ liệu trên cloud hoặc server nội bộ. 

4️⃣ **Màn hình giám sát** – Hiển thị cảnh báo, thống kê và báo cáo.  

![image](https://github.com/user-attachments/assets/4183be86-6662-47ac-bc35-346b43419743)


Dưới đây là sơ đồ kiến trúc hệ thống:  


## 🚀 Hướng dẫn cài đặt  



```sh
🔹 1️⃣ Clone Repository  
git clone https://github.com/dung-nguyenn/phat-hien-hanh-vi-gian-lan-trong-thi-cu.git
cd phat-hien-hanh-vi-gian-lan-trong-thi-cu
🔹 2️⃣ Cài đặt môi trường Python
Bạn cần Python 3.8+ và pip. Nếu chưa có, hãy cài đặt từ Python.org.
Sau đó, tạo môi trường ảo (khuyến nghị):

sh
Sao chép
Chỉnh sửa
python -m venv venv
source venv/bin/activate  # Trên macOS & Linux
venv\Scripts\activate     # Trên Windows
🔹 3️⃣ Cài đặt các thư viện cần thiết
sh
Sao chép
Chỉnh sửa
pip install -r requirements.txt
Nếu chưa có file requirements.txt, hãy cài đặt thủ công:

sh
Sao chép
Chỉnh sửa
pip install opencv-python mediapipe numpy pandas tensorflow matplotlib
🔹 4️⃣ Chạy chương trình phát hiện gian lận
sh
Sao chép
Chỉnh sửa
python detect_camera.py
📖 Cách sử dụng
🔹 Chế độ phát hiện gian lận qua camera

Hệ thống sẽ mở webcam để giám sát thí sinh.
Nếu phát hiện hành vi đáng ngờ, nó sẽ cảnh báo.
🔹 Chế độ huấn luyện mô hình
Nếu muốn huấn luyện lại AI với dữ liệu mới, chạy:

sh
Sao chép
Chỉnh sửa
python train.py
📌 Lưu ý: Hệ thống yêu cầu webcam để hoạt động. Nếu sử dụng trên server không có camera, hãy dùng video làm đầu vào.

