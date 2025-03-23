```
blog/
├── backend/
│   ├── cmd/
│   │   └── main.go           # Điểm vào của ứng dụng (entry point)
│   ├── internal/
│   │   ├── config/
│   │   │   └── config.go     # Cấu hình ứng dụng (cơ sở dữ liệu, cổng, ...)
│   │   ├── controllers/
│   │   │   ├── postController.go # Điều khiển API bài viết
│   │   │   └── authController.go # Điều khiển API xác thực
│   │   ├── models/
│   │   │   └── post.go       # Mô hình dữ liệu bài viết
│   │   ├── routes/
│   │   │   └── routes.go     # Định nghĩa các route API
│   │   ├── services/
│   │   │   ├── postService.go # Logic xử lý dữ liệu bài viết
│   │   │   └── authService.go # Logic xác thực
│   │   ├── middlewares/
│   │   │   └── authMiddleware.go # Middleware xử lý xác thực
│   │   ├── utils/
│   │   │   └── response.go   # Các hàm trợ giúp trả về phản hồi
│   ├── Dockerfile            # Dockerfile để đóng gói ứng dụng backend
│   ├── go.mod                # Quản lý các dependency của Go
│   ├── go.sum                # Danh sách các phiên bản của các thư viện đã sử dụng
│
├── frontend/
│   ├── public/
│   │   ├── index.html        # HTML template chính
│   │   └── favicon.ico       # Biểu tượng trang web
│   ├── src/
│   │   ├── assets/           # Tài nguyên như hình ảnh, icon
│   │   ├── components/       # Các component React như Header, Footer, PostCard
│   │   ├── pages/            # Các trang React như Home, PostDetail
│   │   ├── services/         # API calls, chẳng hạn như fetching bài viết từ backend
│   │   ├── App.js            # Component chính của ứng dụng
│   │   ├── index.js          # Điểm vào của ứng dụng React
│   │   └── styles/           # Các tệp CSS hoặc SCSS
│   ├── .env                  # Các biến môi trường như API_URL
│   ├── package.json          # Quản lý các dependencies của React
│   ├── package-lock.json     # Phiên bản cụ thể của các dependencies
│   └── Dockerfile            # Dockerfile để đóng gói ứng dụng frontend
│
├── .gitignore                # Danh sách các tệp và thư mục không cần theo dõi trong git
└── README.md                 # Tài liệu hướng dẫn sử dụng dự án

```
