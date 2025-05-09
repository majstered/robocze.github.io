<!DOCTYPE html>
<html lang="pl">
<head>
  <meta charset="UTF-8">
  <link rel="icon" type="image/png" href="aplikacje.png">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Ramzi Studio – Aplikacje dla Ciebie</title>
  <style>
    body::before {
      content: "";
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: radial-gradient(circle at 30% 30%, rgba(255,255,255,0.2), transparent 60%),
                  radial-gradient(circle at 70% 70%, rgba(255,255,255,0.15), transparent 60%);
      animation: fogMove 60s infinite linear;
      z-index: -1;
    }

    @keyframes fogMove {
      0% { background-position: 0% 0%, 100% 100%; }
      100% { background-position: 100% 100%, 0% 0%; }
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(-20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes glow {
      from { text-shadow: 0 0 10px #aaa, 0 0 20px #aaa; }
      to   { text-shadow: 0 0 20px #fff, 0 0 30px #fef4d1; }
    }

    body {
      font-family: sans-serif;
      background-color: #fef4d1;
      margin: 0;
      padding: 0;
    }

    header {
      background: linear-gradient(90deg, #444, #222);
      color: white;
      padding: 40px 20px;
      text-align: center;
      text-shadow: 2px 2px 4px #00000066;
      animation: fadeIn 2s ease-out forwards;
    }

    header h1 {
      font-size: 42px;
      margin: 0;
      animation: fadeIn 2s ease-out forwards, glow 3s ease-in-out infinite alternate;
    }

    main {
      padding: 20px;
    }

    .app-card {
      background-color: #fef4d1;
      border-radius: 12px;
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.08);
      padding: 30px;
      margin: 50px auto;
      max-width: 960px;
      animation: fadeInUp 1s ease-out forwards;
      opacity: 0;
      transform: translateY(20px);
    }

    .fade-1 { animation-delay: 0.3s; }
    .fade-2 { animation-delay: 0.6s; }
    .fade-3 { animation-delay: 0.9s; }

    @keyframes fadeInUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    ul {
      margin: 10px 0 0 0;
    }

    a {
      color: #0044cc;
      text-decoration: none;
      position: relative;
    }

    a::after {
      content: '';
      position: absolute;
      width: 100%;
      height: 2px;
      bottom: 0;
      left: 0;
      background-color: #0044cc;
      visibility: hidden;
      transform: scaleX(0);
      transition: all 0.3s ease-in-out;
    }

    a:hover::after {
      visibility: visible;
      transform: scaleX(1);
    }

    footer {
      text-align: center;
      padding: 10px;
      background-color: #f9e6bd;
      font-size: 14px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Ramzi Studio – Aplikacje dla Ciebie</h1>
  </header>
  <main>
    <div class="app-card fade-1">
      <div style="text-align: center; margin-bottom: 15px;">
        <img src="favicon.png" alt="Ikona programu Twój czas, Twoje zdrowie" style="width: 64px; height: 64px; border-radius: 12px;">
      </div>
      <h2>🕰️ Twój czas, Twoje zdrowie</h2>
      <p style="text-indent: 20px;">
        To lekki, przenośny program działający w tle – bez potrzeby instalacji. Wzorowany na metodzie <strong>Pomodoro</strong>, pomaga odzyskać kontrolę nad czasem spędzanym przy komputerze. Monitoruje cykle pracy i przerw, wspierając w dbaniu o równowagę między skupieniem a odpoczynkiem.
      </p>
      <ul>
        <li>🌐 <strong>Wielojęzyczny interfejs</strong> – PL, EN, DE, FR</li>
        <li>⏳ <strong>Tryb Pomodoro</strong> – 30/2 lub 45/5</li>
        <li>💤 <strong>Wyłącznik komputera</strong> – wpisz godzinę</li>
        <li>🧠 <strong>Spokojny interfejs</strong> – działa w tle</li>
      </ul>
      <div style="margin-top: 30px; text-align: center;">
        <a href="https://www.youtube.com/watch?v=EiGnTvTr8lM" target="_blank" style="display: inline-block; background-color: #28a745; color: white; font-weight: bold; padding: 12px 24px; text-decoration: none; border-radius: 8px; font-family: sans-serif; font-size: 16px; margin-right: 16px; box-shadow: 0 2px 6px rgba(0,0,0,0.2);">▶️ Zobacz instrukcję</a>
        <a href="https://ramzi.github.io/Twój%20czas,%20twoje%20zdrowie.rar" target="_blank" style="display: inline-block; background-color: #28a745; color: white; font-weight: bold; padding: 12px 24px; text-decoration: none; border-radius: 8px; font-family: sans-serif; font-size: 16px; box-shadow: 0 2px 6px rgba(0,0,0,0.2);">⬇️ Pobierz aplikację</a>
      </div>
    </div>

    <div class="app-card fade-2">
      <div style="text-align: center; margin-bottom: 15px;">
        <img src="procesy.png" alt="Ikona programu Strażnik Procesów" style="width: 64px; height: 64px; border-radius: 12px;">
      </div>
      <h2>🛡️ Strażnik Procesów</h2>
      <p style="text-indent: 20px;">
        Narzędzie do monitorowania, wykrywania i analizowania podejrzanych procesów w systemie Windows. Pozwala bezpiecznie zarządzać aplikacjami, usuwać logi i chronić system w czasie rzeczywistym.
      </p>
      <ul>
        <li>🔍 <strong>Lista procesów</strong> – filtrowanie, zakończenie</li>
        <li>🦠 <strong>Wykrywanie antywirusów i narzędzi</strong></li>
        <li>📤 <strong>Przycisk „Zaufaj”</strong> – usuwanie podejrzanych</li>
        <li>🧹 <strong>Usuwanie logów i aktualizacji</strong></li>
        <li>🕵️ <strong>Monitoring systemu</strong> – powiadomienia</li>
      </ul>
      <div style="margin-top: 30px; text-align: center;">
        <a href="https://youtu.be/wbL2dtnEmEk" target="_blank" style="display: inline-block; background-color: #28a745; color: white; font-weight: bold; padding: 12px 24px; text-decoration: none; border-radius: 8px; font-family: sans-serif; font-size: 16px; margin-right: 16px; box-shadow: 0 2px 6px rgba(0,0,0,0.2);">▶️ Zobacz instrukcję</a>
        <a href="https://drive.google.com/uc?export=download&id=10AXvED7YUnPRvMddPyrhk3Wi89eQkCMf" target="_blank" style="display: inline-block; background-color: #28a745; color: white; font-weight: bold; padding: 12px 24px; text-decoration: none; border-radius: 8px; font-family: sans-serif; font-size: 16px; box-shadow: 0 2px 6px rgba(0,0,0,0.2);">⬇️ Pobierz aplikację</a>
      </div>
    </div>

    <div class="app-card fade-3">
      <div style="text-align: center; margin-bottom: 15px;">
        <img src="turbo_converted.png" alt="Ikona programu Yanosik Turbo" style="width: 64px; height: 64px; border-radius: 12px;">
      </div>
      <h2>🎵 Yanosik Turbo 1.0 – Twoja osobista biblioteka dźwięku</h2>
      <ul>
        <li>✅ Pobiera z YouTube, SoundCloud, Bandcamp, Facebook</li>
        <li>✅ Zapisuje pliki jako MP3</li>
        <li>✅ Tworzy bibliotekę z odtwarzaczem</li>
        <li>✅ Brak logowania i śledzenia</li>
        <li>✅ Blokuje nieprawidłowe playlisty</li>
      </ul>
      <div style="margin-top: 30px; text-align: center;">
        <a href="https://drive.google.com/uc?export=download&id=10AXvED7YUnPRvMddPyrhk3Wi89eQkCMf" target="_blank" style="display: inline-block; background-color: #28a745; color: white; font-weight: bold; padding: 12px 24px; text-decoration: none; border-radius: 8px; font-family: sans-serif; font-size: 16px; margin-right: 16px; box-shadow: 0 2px 6px rgba(0,0,0,0.2);">⬇️ Pobierz aplikację</a>
        <a href="https://www.youtube.com/watch?v=TwojFilm" target="_blank" style="display: inline-block; background-color: #28a745; color: white; font-weight: bold; padding: 12px 24px; text-decoration: none; border-radius: 8px; font-family: sans-serif; font-size: 16px; box-shadow: 0 2px 6px rgba(0,0,0,0.2);">▶️ Zobacz instrukcję</a>
      </div>
    </div>
  </main>
  <footer>
    <div style="text-align: center; margin: 60px 0;">
      <a href="https://buycoffee.to/ramzi-studio" target="_blank" style="background-color: #6f4e37; color: white; padding: 12px 24px; border-radius: 8px; text-decoration: none; font-size: 16px; font-weight: bold; box-shadow: 0 2px 6px rgba(0,0,0,0.2); transition: transform 0.2s ease; display: inline-block;">☕ Postaw nam kawę</a>
    </div>
    © 2025 Ramzi Studio – Wszystkie prawa zastrzeżone
  </footer>
</body>
</html>
