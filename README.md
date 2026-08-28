# T-Download — kho manifest cập nhật

Kho này chỉ phục vụ **một file**: `manifest.json`, để app T-Download tự kiểm tra
bản mới. Không chứa mã nguồn, không chứa file cài đặt.

File được phục vụ qua GitHub Pages tại:
`https://tikz-physics.github.io/t-download-update/manifest.json`

## Vì sao manifest phải được ký

App chỉ chấp nhận manifest có chữ ký Ed25519 khớp với khoá công khai nhúng sẵn
trong app. Nếu không có lớp này, bất kỳ ai chiếm được kho này — hoặc chen được
vào giữa đường truyền — đều có thể trỏ toàn bộ người dùng sang một file `.exe`
bất kỳ.

Khoá riêng dùng để ký **không bao giờ** nằm trong kho này, cũng không nằm trong
app. Nó giữ offline trên máy của tác giả.
