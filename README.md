<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selvi Branded Batam</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to right, #ff5722, #ffc107);
            color: #212121;
            text-align: center;
            padding: 50px;
            margin: 0;
        }
        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(255, 255, 255, 0.7);
        }
        p {
            font-size: 1.2em;
            margin-bottom: 30px;
            text-shadow: 1px 1px 2px rgba(255, 255, 255, 0.5);
        }
        .container {
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 6px 30px rgba(0, 0, 0, 0.5);
            display: inline-block;
            max-width: 600px;
            margin: auto;
        }
        .link {
            display: block;
            background-color: #00796b;
            color: #fff;
            text-decoration: none;
            padding: 15px;
            margin: 15px 0;
            border-radius: 30px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
            transition: background-color 0.3s, transform 0.3s;
            font-size: 1.1em;
        }
        .link:hover {
            background-color: #004d40;
            transform: translateY(-2px);
        }
        img.logo {
            max-width: 120px; /* Ukuran gambar lebih kecil */
            margin-bottom: 20px;
            border-radius: 50%;
            border: 2px solid #fff;
            cursor: pointer;
            transition: transform 0.3s;
        }
        img.logo:hover {
            transform: scale(1.05);
        }
        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            opacity: 0;
            transition: opacity 0.5s ease;
        }
        .modal.show {
            display: flex;
            opacity: 1;
        }
        .modal-content {
            max-width: 80%; /* Ukuran modal yang lebih kecil */
            max-height: 80%; /* Ukuran tinggi modal */
            border: 1px solid #fff;
            border-radius: 10px;
            animation: fadeIn 0.5s;
        }
        @keyframes fadeIn {
            from { transform: scale(0.7); opacity: 0; }
            to { transform: scale(1); opacity: 1; }
        }
        .close {
            position: absolute;
            top: 20px;
            right: 35px;
            color: #fff;
            font-size: 40px;
            font-weight: bold;
            cursor: pointer;
        }
        footer {
            margin-top: 30px;
            font-size: 0.9em;
            color: #212121;
            text-shadow: 1px 1px 2px rgba(255, 255, 255, 0.5);
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="c:\Users\DELL\Downloads\WhatsApp Image 2024-10-21 at 08.37.08.jpeg" alt="Logo Toko" class="logo" id="logoImage"> <!-- Ganti dengan URL logo Anda -->
        <h1>Selvi Branded Batam</h1>
        <p>𝗧𝗼𝗸𝗼 𝗧𝗮𝘀 𝗧𝗟 𝗦𝗶𝗻𝗴𝗮𝗽𝗼𝗿𝗲, 𝗡𝗼 𝗠𝗶𝗻𝘂𝘀, 𝗔𝘀𝗹𝗶 💯℅</p>
        <a class="link" href="https://wa.me/62895383014411" target="_blank">Hubungi Kami via WhatsApp</a>
        <a class="link" href="https://www.facebook.com/profile.php?id=100048502543083&mibextid=ZbWKwL" target="_blank">Ikuti Kami di Facebook</a>
        <a class="link" href="https://www.tiktok.com/@selvi_batam?_t=8qiWJLBOB3S&_r=1" target="_blank">Tonton di TikTok</a>
    </div>
    
    <div id="myModal" class="modal">
        <span class="close" id="closeModal">&times;</span>
        <img class="modal-content" id="modalImage" alt="Logo Toko">
    </div>
    
    <footer>
        <p>&copy; 2024 Selvi Branded Batam</p>
    </footer>

    <script>
        var modal = document.getElementById("myModal");
        var img = document.getElementById("logoImage");
        var modalImg = document.getElementById("modalImage");
        var closeModal = document.getElementById("closeModal");

        img.onclick = function(){
            modal.classList.add('show');
            modalImg.src = this.src; 
        }

        closeModal.onclick = function() {
            modal.classList.remove('show');
        }

        window.onclick = function(event) {
            if (event.target == modal) {
                modal.classList.remove('show');
            }
        }
    </script>
</body>
</html>
