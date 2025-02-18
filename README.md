<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gửi lời chúc</title>
</head>
<body>

    <h3>GỬI LỜI CHÚC YÊU THƯƠNG</h3>
    <textarea id="loiChuc" placeholder="Nhập lời chúc của bạn..."></textarea>
    <button onclick="guiLoiChuc()">Gửi</button>

    <p id="phanHoi" style="color: green; font-weight: bold; display: none;">Cảm ơn bạn đã gửi lời chúc!</p>

    <script>
        function guiLoiChuc() {
            var loiChuc = document.getElementById("loiChuc").value;
            if (loiChuc.trim() !== "") {
                document.getElementById("phanHoi").style.display = "block";
                document.getElementById("loiChuc").value = ""; // Xóa nội dung sau khi gửi
            } else {
                alert("Vui lòng nhập lời chúc trước khi gửi!");
            }
        }
