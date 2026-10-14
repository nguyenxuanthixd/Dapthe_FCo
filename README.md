# Phòng Lab Đập Thẻ FCO

App tính dây mồi đập thẻ FC Online: nhập dây, tính tỷ lệ vô theo dây/vạch/bảng tỷ lệ, màn đập thẻ mô phỏng.

Mở `index.html` trên trình duyệt hoặc bật GitHub Pages (Settings → Pages → branch `main`, `/ (root)`).

Dữ liệu dây lưu trong trình duyệt (localStorage) của từng máy.

## Đăng nhập (Firebase)

1. Tạo project Firebase, bật Authentication (Google, Email/Password), thêm `nguyenxuanthixd.github.io` vào Authorized domains.
2. Tạo Firestore Database, dán nội dung `firestore.rules` vào tab Rules rồi Publish.
3. Dán `firebaseConfig` vào hằng `FIREBASE_CONFIG` trong `index.html`.

Dữ liệu mỗi tài khoản lưu ở `users/{uid}`, chỉ chủ tài khoản đọc/ghi được.
