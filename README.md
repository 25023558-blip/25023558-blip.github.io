# NguyenVuHoangAnh.hub.io
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <style>
        /* ===================================================
           1. CÀI ĐẶT CHUNG CHO TOÀN TRANG
           =================================================== */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #1a1a1a; /* Nền tối sang trọng giống mẫu */
            color: #fff;
            margin: 0;
            padding: 40px 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        h2 {
            text-align: center;
            font-weight: 400;
            letter-spacing: 1px;
            margin-bottom: 40px;
            color: #fff;
        }

        /* ===================================================
           2. PHẦN DANH SÁCH DỰ ÁN (DẠNG LƯỚI)
           =================================================== */
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px; /* Khoảng cách giữa các ô dự án */
            margin-bottom: 80px; /* Khoảng cách xuống phần Form */
        }

        .portfolio-card {
            background-color: #262626;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .portfolio-card:hover {
            transform: translateY(-5px); /* Nhấc nhẹ ô lên khi di chuột vào */
            box-shadow: 0 10px 25px rgba(0, 255, 136, 0.2);
        }

        .card-image {
            width: 100%;
            height: 200px;
            overflow: hidden;
        }

        .card-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .portfolio-card:hover .card-image img {
            transform: scale(1.1); /* Phóng to ảnh nhẹ khi hover */
        }

        .card-info {
            padding: 20px;
        }

        .card-info h3 {
            margin: 0 0 10px 0;
            font-size: 1.3rem;
            color: #00ff88; /* Màu xanh neon điểm nhấn */
        }

        .card-info p {
            color: #cccccc;
            font-size: 0.9rem;
            line-height: 1.5;
            margin-bottom: 20px;
        }

        .btn-demo {
            display: inline-block;
            padding: 8px 16px;
            background-color: transparent;
            color: #00ff88;
            border: 1px solid #00ff88;
            border-radius: 6px;
            text-decoration: none;
            font-size: 0.9rem;
            transition: all 0.3s ease;
        }

        .btn-demo:hover {
            background-color: #00ff88;
            color: #1a1a1a;
        }

        /* ===================================================
           3. PHẦN FORM LIÊN HỆ TỐI GIẢN
           =================================================== */
        .simple-contact-container {
            max-width: 500px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .input-group {
            margin-bottom: 35px; /* Khoảng cách giữa các ô nhập */
        }

        /* Chỉ lấy 1 đường gạch dưới đáy cho đơn giản */
        .input-group input,
        .input-group textarea {
            width: 100%;
            background: transparent;
            border: none;
            border-bottom: 1px solid #444;
            color: #fff;
            padding: 10px 0;
            font-size: 1rem;
            font-family: inherit;
            outline: none;
            box-sizing: border-box;
            transition: border-color 0.4s ease;
        }

        .input-group textarea {
            resize: none;
        }

        .input-group input::placeholder,
        .input-group textarea::placeholder {
            color: #777;
            font-weight: 300;
        }

        /* Khi click vào ô nhập, đường gạch dưới sáng lên */
        .input-group input:focus,
        .input-group textarea:focus {
            border-bottom: 1px solid #00ff88;
        }

        .btn-simple-send {
            background: transparent;
            color: #00ff88;
            border: 1px solid #00ff88;
            padding: 12px 30px;
            font-size: 0.95rem;
            border-radius: 4px;
            cursor: pointer;
            display: block;
            margin: 0 auto;
            transition: all 0.3s ease;
        }

        .btn-simple-send:hover {
            background: #00ff88;
            color: #1a1a1a;
        }
    </style>
</head>
<body>

    <div class="container">
        
        <!-- PHẦN 1: DANH SÁCH DỰ ÁN -->
        <h2>Dự Án Của Tôi</h2>
        <div class="portfolio-grid">
            
            <!-- Dự án 1 -->
            <div class="portfolio-card">
                <div class="card-image">
                    <img src="https://picsum.photos/400/250?random=1" alt="Dự án 1">
                </div>
                <div class="card-info">
                    <h3>Tên Dự Án 01</h3>
                    <p>Mô tả ngắn gọn về công nghệ sử dụng (HTML, CSS, React...).</p>
                    <a href="#" class="btn-demo">Xem Chi Tiết</a>
                </div>
            </div>

            <!-- Dự án 2 -->
            <div class="portfolio-card">
                <div class="card-image">
                    <img src="https://picsum.photos/400/250?random=2" alt="Dự án 2">
                </div>
                <div class="card-info">
                    <h3>Tên Dự Án 02</h3>
                    <p>Mô tả ngắn gọn về công nghệ sử dụng (HTML, CSS, React...).</p>
                    <a href="#" class="btn-demo">Xem Chi Tiết</a>
                </div>
            </div>

        </div>

        <!-- PHẦN 2: FORM LIÊN HỆ ĐƠN GIẢN -->
        <div class="simple-contact-container">
            <h2>Liên Hệ</h2>
            
            <form class="simple-form">
                <div class="input-group">
                    <input type="text" id="name" placeholder="Họ và tên của bạn" required>
                </div>

                <div class="input-group">
                    <input type="email" id="email" placeholder="Địa chỉ email" required>
                </div>

                <div class="input-group">
                    <textarea id="message" rows="4" placeholder="Lời nhắn của bạn..." required></textarea>
                </div>

                <button type="submit" class="btn-simple-send">Gửi đi</button>
            </form>
        </div>

    </div>

</body>
</html>
