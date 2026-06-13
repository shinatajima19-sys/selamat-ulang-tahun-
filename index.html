<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Surprise Ulang Tahun</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            font-family: 'Poppins', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow: hidden;
            color: white;
        }

        .step {
            display: none;
            text-align: center;
            padding: 30px;
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            box-shadow: 0 8px 32px rgba(0,0,0,0.2);
            border: 1px solid rgba(255,255,255,0.2);
            max-width: 450px;
            width: 90%;
            animation: fadeIn 0.8s ease;
        }

        .step.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h1, h2 {
            margin-bottom: 20px;
            font-weight: 700;
        }

        h1 { font-size: 2rem; }
        h2 { font-size: 1.5rem; }

        input {
            width: 100%;
            padding: 15px;
            border: none;
            border-radius: 50px;
            font-size: 1rem;
            text-align: center;
            margin-bottom: 20px;
            font-family: 'Poppins', sans-serif;
            outline: none;
        }

        .btn {
            background: #fff;
            color: #764ba2;
            border: none;
            padding: 15px 35px;
            border-radius: 50px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            font-family: 'Poppins', sans-serif;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
        }

        .btn-music {
            background: #FFD700;
            color: #333;
            margin-top: 10px;
            font-size: 0.9rem;
            padding: 12px 25px;
        }

        .btn-music.playing {
            background: #4CAF50;
            color: #fff;
        }

        .emoji {
            font-size: 5rem;
            margin: 20px 0 10px 0;
            cursor: pointer;
            display: inline-block;
            transition: transform 0.3s ease;
        }

        .emoji:hover {
            transform: scale(1.2);
        }

        .gift {
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }

        video {
            width: 100%;
            border-radius: 15px;
            margin: 15px 0;
            max-height: 300px;
            background: #000;
        }

        .nama-text {
            font-size: 1.3rem;
            font-weight: 600;
            margin-bottom: 10px;
            color: #FFD700;
        }

        .doa {
            line-height: 1.8;
            font-size: 1rem;
            margin: 20px 0;
            text-align: left;
            background: rgba(0,0,0,0.2);
            padding: 20px;
            border-radius: 15px;
        }

        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background: #f0f;
            animation: confetti-fall 3s linear infinite;
        }

        @keyframes confetti-fall {
            to {
                transform: translateY(100vh) rotate(360deg);
                opacity: 0;
            }
        }
    </style>
</head>
<body>

    <!-- MUSIK LU -->
    <audio id="musikKue" loop>
        <source src="https://litter.catbox.moe/gmakai.mp3" type="audio/mpeg">
    </audio>

    <!-- 1. ISI NAMA -->
    <div class="step active" id="step1">
        <h1>Haii! 👋</h1>
        <p>Masukin nama kamu dulu ya</p>
        <input type="text" id="namaInput" placeholder="Nama kamu siapa?" autocomplete="off">
        <button class="btn" onclick="nextStep(2)">Lanjut</button>
    </div>

    <!-- 2. KUE + TOMBOL MUSIK DI BAWAH -->
    <div class="step" id="step2">
        <h2>Ada yang ultah nih! 🎉</h2>
        <div class="emoji" onclick="nextStep(3)">🎂</div>
        <button class="btn btn-music" id="btnMusic" onclick="toggleMusic()">🔊 Klik Buat Nyalain Musik</button>
        <p style="margin-top:15px">Klik kuenya buat lanjut yaa</p>
    </div>

    <!-- 3. MUNCUL KADO -->
    <div class="step" id="step3">
        <h2>Ada hadiah buat kamu!</h2>
        <div class="emoji gift" onclick="nextStep(4)">🎁</div>
        <p>Klik kadonya buat buka</p>
    </div>

    <!-- 4. VIDEO + TEKS NAMA -->
    <div class="step" id="step4">
        <div class="nama-text" id="namaDisplay">Selamat Ulang Tahun!</div>
        <video id="vid" controls>
            <source src="https://litter.catbox.moe/q8fzxl.mp4" type="video/mp4">
            Browser kamu ga support video
        </video>
        <button class="btn" onclick="nextStep(5)">Lanjut ke Doa →</button>
    </div>

    <!-- 5. DOA DARI GUE -->
    <div class="step" id="step5">
        <h2>Ini Doa Dari Aku 🤍</h2>
        <div class="doa" id="doaText"></div>
        <button class="btn" onclick="nextStep(1)">Ulang Lagi</button>
    </div>

    <script>
        let namaUser = '';
        const musikKue = document.getElementById('musikKue');
        const video = document.getElementById('vid');
        const btnMusic = document.getElementById('btnMusic');

        function toggleMusic() {
            if (musikKue.paused) {
                musikKue.play();
                btnMusic.innerHTML = '⏸️ Musik Nyala - Klik Buat Pause';
                btnMusic.classList.add('playing');
            } else {
                musikKue.pause();
                btnMusic.innerHTML = '🔊 Klik Buat Nyalain Musik';
                btnMusic.classList.remove('playing');
            }
        }

        function nextStep(step) {
            if (step === 2) {
                namaUser = document.getElementById('namaInput').value.trim();
                if (namaUser === '') {
                    alert('Isi nama dulu dong 😅');
                    return;
                }
                document.getElementById('namaDisplay').innerHTML = `Selamat Ulang Tahun, ${namaUser}! 🎉`;
                buatDoa();
            }

            document.querySelectorAll('.step').forEach(s => s.classList.remove('active'));
            document.getElementById('step' + step).classList.add('active');

            if (step === 5) {
                createConfetti();
                musikKue.pause();
            }

            if (step === 4) {
                musikKue.pause();
                btnMusic.innerHTML = '🔊 Klik Buat Nyalain Musik';
                btnMusic.classList.remove('playing');
                video.play().catch(e => {});
            }

            if (step === 1) {
                document.getElementById('namaInput').value = '';
                video.pause();
                musikKue.pause();
                musikKue.currentTime = 0;
                btnMusic.innerHTML = '🔊 Klik Buat Nyalain Musik';
                btnMusic.classList.remove('playing');
            }
        }

        function buatDoa() {
            const doa = `
                <p>Buat <b>${namaUser}</b>,</p>
                <p>Selamat nambah umur ya! 🎂 Di hari spesial kamu ini, aku doain semoga ${namaUser} selalu dikasih kesehatan, rezeki yang ga putus-putus, dan hati yang selalu bahagia.</p>
                <p>Semoga di umur baru ini, semua hal baik dateng ke ${namaUser}. Yang lagi diusahain semoga dilancarin, yang lagi ditunggu semoga cepet dateng, dan yang bikin sedih semoga diganti sama hal-hal yang bikin ketawa.</p>
                <p>Jangan lupa bahagia terus ya, ${namaUser}. Kamu pantes dapet semua hal baik di dunia ini.</p>
                <br>
                <p>Aamiin 🤍</p>
                <p><i>- Dari Shiina Tajima 🧸</i></p>
            `;
            document.getElementById('doaText').innerHTML = doa;
        }

        function createConfetti() {
            for (let i = 0; i < 50; i++) {
                const confetti = document.createElement('div');
                confetti.classList.add('confetti');
                confetti.style.left = Math.random() * 100 + 'vw';
                confetti.style.animationDuration = Math.random() * 2 + 2 + 's';
                confetti.style.background = `hsl(${Math.random() * 360}, 100%, 50%)`;
                confetti.style.animationDelay = Math.random() * 2 + 's';
                document.body.appendChild(confetti);
                
                setTimeout(() => confetti.remove(), 4000);
            }
        }

        document.getElementById('namaInput').addEventListener('keypress', function(e) {
            if (e.key === 'Enter') nextStep(2);
        });
    </script>

</body>
</html>
