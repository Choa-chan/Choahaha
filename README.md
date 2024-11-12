
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chào bạn yêu</title>
    <style>
        body {
            background-color: #f0f8ff;  /* Màu nền xanh nhạt */
            font-family: "Times New Roman", serif; 
            font-size: 20px;
            background-image: url('hoa.jpg'); /* Sử dụng url() thay vì <img> */
            background-size: cover; /* Đảm bảo hình ảnh phủ toàn bộ nền */
            background-position: center; /* Căn giữa hình nền */
        }
    </style>
    <script>
        function showLink() {
            // Lấy tất cả các radio button
            var radios = document.getElementsByName('option');
            var linkContainer = document.getElementById('linkContainer');

            // Kiểm tra từng radio button
            for (var i = 0; i < radios.length; i++) {
                if (radios[i].checked) {
                    // Hiển thị link dựa trên radio button đã chọn
                    if (radios[i].value === 'Một ngày tích cực') {
                        linkContainer.innerHTML = '<a href= "https://www.youtube.com/watch?v=nfQa4QgRovA" alt ="Bạn cười lên đẹp lắm" target="_blank">Chỗ này có điều thú vị nè</a>';
                    } else if (radios[i].value === 'Hơi mệt một chút') {
                        linkContainer.innerHTML = '<a href="https://www.youtube.com/watch?v=ECxVfrwwTp0" target="_blank">Bạn của tôi đã rất cố gắng rồi =))</a>';
                    } else if (radios[i].value === 'Mình không buồn cũng không vui') {
                        linkContainer.innerHTML = '<a href="https://www.youtube.com/watch?v=q5WO3n0FLeA" target="_blank">Không sao hết ở đây có niềm vui nè =)))</a>';
                    }
                    break;
                }
            }
        }
    </script>
</head>
<body>

    <h3 >Bạn thân mến,<br>
 		Ngày hôm nay của bạn thế nào, nói mình nghe nha =))   
    
    </h3>
    
    <input type="radio" id="Một ngày tích cực" name="option" value="Một ngày tích cực" onclick="showLink()"> Một ngày tích cực <br>
    <br>
    <input type="radio" id="Hơi mệt một chút" name="option" value="Hơi mệt một chút" onclick="showLink()"> Hơi mệt một chút<br>
    <br>
    <input type="radio" id="Mình không buồn cũng không vui" name="option" value="Mình không buồn cũng không vui" onclick="showLink()"> Mình không buồn cũng không vui<br>

    <div id="linkContainer"></div>

</body>
</html>
