# SemenStory2
<!DOCTYPE html>
    <html>
        <head>
            <meta charset="UTF-8">
            <title>СеменМакТрахер</title>
            <style>
        body {
            margin: 0;
            padding: 0;
            display: flex; 
            min-height: 100vh; 
            font-family: sans-serif;
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='200'%3E%3Ctext x='10' y='40' font-size='30'%3E😂%3C/text%3E%3Ctext x='100' y='90' font-size='30'%3E🤣%3C/text%3E%3Ctext x='30' y='150' font-size='30'%3E😭%3C/text%3E%3Ctext x='140' y='180' font-size='30'%3E💀%3C/text%3E%3C/svg%3E");
            background-repeat: repeat;
            overflow-x: hidden;
        }

        body::after {
            content: "";
            position: fixed;
            inset: 0;
            pointer-events: none;
            z-index: 1000;
            background:
                repeating-linear-gradient(0deg, rgba(255,0,255,0.06) 0px, rgba(0,255,255,0.06) 1px, transparent 2px, transparent 4px),
                repeating-linear-gradient(90deg, rgba(255,255,0,0.05) 0px, rgba(0,0,255,0.05) 1px, transparent 2px, transparent 5px);
            mix-blend-mode: screen;
            animation: gdiShift 0.15s steps(2) infinite;
        }

        @keyframes gdiShift {
            0%   { transform: translate(0,0); }
            50%  { transform: translate(1px,-1px); }
            100% { transform: translate(-1px,1px); }
        }

        .side-panel {
            width: 15%; 
            background-color:deeppink; 
            color: white;
            padding: 20px;
            position: relative;
            overflow: hidden;
        }

        .side-panel::before {
            content: "🇷🇺 🚩  🏴 ☪️  ✡️  🚩  🏴 ☪️  ✡️  🚩  🏴 ☪️  ✡️  🚩  🏴 ☪️  ✡️ 🇷🇺 🚩  🏴 ☪️  ✡️ 🇷🇺 🚩  🏴 ☪️  ✡️ 🇷🇺 🚩  🏴 ☪️  ✡️  🚩  🏴 ☪️  ✡️";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            font-size: 28px;
            line-height: 2.2;
            opacity: 0.35;
            pointer-events: none;
            word-break: break-all;
            z-index: 0;
        }

        .side-panel > * {
            position: relative;
            z-index: 1;
        }

        .side-panel .verticle-abuse {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            writing-mode: vertical-rl;
            text-orientation: mixed;
            font-size: 14px;
            font-weight: bold;
            color: #ffff00;
            text-shadow: 1px 1px 0 #000, -1px -1px 0 #ff00ff;
            letter-spacing: 2px;
            opacity: 0.9;
            pointer-events: none;
            z-index: 2;
            animation: abuseFlicker 1.2s steps(2) infinite;
        }

        .side-panel .verticle-abuse.left { left: 4px; }
        .side-panel .verticle-abuse.right { right: 4px; }

        @keyframes abuseFlicker {
            0%, 100% { opacity: 0.9; }
            50% { opacity: 0.4; }
        }

        .main-content {
            flex: 1; 
            background-color: #c55757; 
            padding: 20px;
            position: relative;
        }

        .main-content::before {
            content: "⚠️ GDI+ ERROR: 0x80004005 — СЕМЁН НЕ НАЙДЕН ⚠️";
            display: block;
            text-align: center;
            font-family: "Courier New", monospace;
            font-size: 16px;
            font-weight: bold;
            color: #fff;
            background: #000080;
            border: 2px outset #c0c0c0;
            padding: 4px;
            margin-bottom: 10px;
            text-shadow: 1px 1px 0 #ff00ff, -1px -1px 0 #00ffff;
            animation: gdiBlink 1s steps(2) infinite;
        }

        @keyframes gdiBlink {
            0%, 100% { background: #000080; }
            50% { background: #800000; }
        }

        .main-content::after {
            content: "⚠️ GDI+ ERROR: 0x80004005 — СЕМЁН НЕ НАЙДЕН ⚠️";
            display: block;
            text-align: center;
            font-family: "Courier New", monospace;
            font-size: 16px;
            font-weight: bold;
            color: #fff;
            background: #000080;
            border: 2px outset #c0c0c0;
            padding: 4px;
            margin-top: 20px;
            text-shadow: 1px 1px 0 #ff00ff, -1px -1px 0 #00ffff;
            animation: gdiBlink 1s steps(2) infinite;
        }

        h1, h2, h3, h4 {
            text-shadow: 2px 0 0 rgba(255,0,255,0.7), -2px 0 0 rgba(0,255,255,0.7);
            animation: gdiJitter 0.3s steps(2) infinite;
        }

        @keyframes gdiJitter {
            0%   { transform: translate(0,0); }
            33%  { transform: translate(1px,0); }
            66%  { transform: translate(-1px,1px); }
            100% { transform: translate(0,0); }
        }

        p {
            text-shadow: 1px 0 0 rgba(255,0,255,0.5), -1px 0 0 rgba(0,255,255,0.5);
        }

        .emoji-rain {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 999;
            overflow: hidden;
        }

        .emoji-rain span {
            position: absolute;
            top: -50px;
            font-size: 30px;
            animation: fall linear infinite;
        }

        @keyframes fall {
            to { transform: translateY(110vh) rotate(360deg); }
        }

        .bismillah {
            text-align: center;
            font-size: 26px;
            color: gold;
            text-shadow: 2px 2px 4px black, 0 0 8px #ff00ff;
            margin: 10px 0;
        }

        .hebrew-phrase {
            text-align: center;
            font-size: 20px;
            color: #00bfff;
            direction: rtl;
            text-shadow: 1px 1px 3px black, 0 0 6px #ffffff;
            margin: 8px 0;
            font-weight: bold;
        }

        .gdi-dialog {
            position: fixed;
            right: 20px;
            bottom: 20px;
            width: 260px;
            background: #c0c0c0;
            border: 2px outset #fff;
            font-family: "MS Sans Serif", Tahoma, sans-serif;
            font-size: 12px;
            z-index: 1001;
            box-shadow: 4px 4px 0 rgba(0,0,0,0.5);
            animation: dialogShake 0.2s steps(2) infinite;
        }

        .gdi-dialog .titlebar {
            background: linear-gradient(90deg, #000080, #1084d0);
            color: #fff;
            padding: 3px 6px;
            font-weight: bold;
            display: flex;
            justify-content: space-between;
        }

        .gdi-dialog .titlebar span:last-child {
            background: #c0c0c0;
            color: #000;
            border: 1px outset #fff;
            padding: 0 4px;
        }

        .gdi-dialog .body {
            padding: 12px 10px;
            display: flex;
            gap: 10px;
            align-items: flex-start;
        }

        .gdi-dialog .body .icon {
            font-size: 28px;
        }

        .gdi-dialog .buttons {
            text-align: center;
            padding: 6px;
        }

        .gdi-dialog .buttons button {
            font-family: "MS Sans Serif", Tahoma, sans-serif;
            font-size: 12px;
            padding: 2px 14px;
            border: 2px outset #fff;
            background: #c0c0c0;
            cursor: pointer;
        }

        @keyframes dialogShake {
            0%   { transform: translate(0,0); }
            50%  { transform: translate(1px,-1px); }
            100% { transform: translate(-1px,0); }
        }

        .main-content p:nth-of-type(7) {
            color: #00ff00;
            background: #000;
            font-family: "Courier New", monospace;
        }

        .abuse-strip {
            position: fixed;
            left: 0;
            right: 0;
            text-align: center;
            font-family: "Courier New", monospace;
            font-size: 14px;
            font-weight: bold;
            color: #ff0;
            background: rgba(0,0,0,0.6);
            padding: 3px 0;
            z-index: 1002;
            white-space: nowrap;
            overflow: hidden;
            text-shadow: 1px 1px 0 #f0f, -1px -1px 0 #0ff;
            pointer-events: none;
        }

        .abuse-strip.top { top: 0; }
        .abuse-strip.bottom { bottom: 0; }

        .abuse-strip span {
            display: inline-block;
            padding-left: 100%;
            animation: marquee 18s linear infinite;
        }

        @keyframes marquee {
            0% { transform: translateX(0); }
            100% { transform: translateX(-50%); }
        }
    </style>
        </head>
        <body style="background-color:rgb(223, 99, 99);">
            <div class="emoji-rain" id="rain"></div>

            <div class="abuse-strip top"><span>🤡 СЕМЁН-ЛОХ 🐷 СЕМЁН-ЧМО 💩 СЕМЁН-ПЕТУХ 🐔 СЕМЁН-ТЕРПИЛА 😭 СЕМЁН-ДЫРКА 🕳️ СЕМЁН-ТРЯПКА 🧻 СЕМЁН-ОБОСРАНЕЦ 💩 СЕМЁН-ШЛЮХА 👠 СЕМЁН-ПОДСТИЛКА 🛏️ СЕМЁН-ГЕМОРРОЙ 🍩 СЕМЁН-ТУАЛЕТ 🚽 СЕМЁН-ПОМОЙКА 🗑️ 🤡 СЕМЁН-ЛОХ 🐷 СЕМЁН-ЧМО 💩 СЕМЁН-ПЕТУХ 🐔 СЕМЁН-ТЕРПИЛА 😭 СЕМЁН-ДЫРКА 🕳️ СЕМЁН-ТРЯПКА 🧻 СЕМЁН-ОБОСРАНЕЦ 💩 СЕМЁН-ШЛЮХА 👠 СЕМЁН-ПОДСТИЛКА 🛏️ СЕМЁН-ГЕМОРРОЙ 🍩 СЕМЁН-ТУАЛЕТ 🚽 СЕМЁН-ПОМОЙКА 🗑️</span></div>

            <div class="side-panel">
                <div class="verticle-abuse left">🤡 ЛОХ 🐷 ЧМО 💩 ПЕТУХ 🐔 ТЕРПИЛА 😭 ДЫРКА 🕳️</div>
                <div class="verticle-abuse right">ТРЯПКА 🧻 ОБОСРАНЕЦ 💩 ШЛЮХА 👠 ПОДСТИЛКА 🛏️ ГЕМОРРОЙ 🍩</div>
                <h3>ДА ЭТО ПРАВДА</h3>
                <p>Я люблю сосать члены</p>
                <div class="bismillah">بِسْمِ اللَّهِ</div>
                <div class="hebrew-phrase">שָׁלוֹם עֲלֵיכֶם 🇮🇱 ✡️</div>
                <div class="hebrew-phrase">סמיון הוא לוזר 🐷</div>
                <p>🇷🇺 🚩 ☪️ 🇸🇦 🏴 🇮🇱 ✡️</p>
                <p>😂 🤣 😭 💀 🤲</p>
                <div class="hebrew-phrase">ברוך הבא לבית המשוגעים</div>
                <div class="hebrew-phrase">סמיון המטומטם 🤡</div>
            </div>
            <div class="main-content">
                <div class="bismillah">بِسْمِ اللَّهِ الرَّحْمَٰنِ الرَّحِيمِ 🤲</div>
                <div class="hebrew-phrase">ברוך הבא, סמיון המטומטם 🇮🇱</div>
                <h1 align="center">Привет, я - Семен и я - МакСакер</h1>
            <p align="left">
                Мой первый пассивный половой акт произошел не в таких приятных условиях
                как я хотел, однако мне очень понравилось.
            </p>
            <p>
                Ни смотря на большие анальные разрывы и кровотечения я действительно наслаждался 
                процессом и хотел бы это повторить это
            </p>
            <p>
                Моим первым половым партнером был Щеглов Никита Александрович. В связи со 
                своей неопытностью он делал все больно и быстро, даже не воспользовавшись 
                смазкой.
            </p>
            <p>
                Ни смотря на это мы закончили со всем достаточно быстро и он даже поцеловал меня 
                в лоб и оставил на память клеймо "Оральный хулиган"
            </p>
            <p>
                Оглядываясь на это я могу сказатьЮ что это был лучший день во всей моей жизни. 
                Каждый мой половой акт я вспоминаю именно мой первый, и не смотря на его жесткость
                он был самым значительным в моей жизни. 

                
            </p>
            <h2>
                Как я увлекся этим
            </h2>
            <p>
                Желание этого захватило меня полностью! Я стал грезить этим каждый день
                ожидая когда кто-нибудь снова меня выебет, однако Никита чуть не стал отцом и нам
                пришлось расстаться
            </p>
            <p>
                После этого я стал судорожно искать нового партнера и моим следующим выбором
                стал мой дед - Александр, экей "Когда он уже сдохнет". 
                Он всегда злился, когда я до поздна играл в компьютер с моими вымешленными 
                интернет-друзьями и в один из дней помимо ремня он взял бутылку
            </p>
            <P>
                Так как член у него не стоял уж как 30 лет, он износиловал меня чикушкой
                водки "Русский стандарт". Это было незабываемо! Как он входил в меня, 
                как он был груб! Я получил такой оргазм, который вам и не снился. 
                Чекунец все входил и входил, пока не вошел в меня полностью. 
            </P>
            <p>
                Дед увидив это очень сильно испугался и убежал, раняя кал, а я и позабыл про нее 
                на целые сутки, пока после очередного похода в туалет мне не пришлось очень
                сильно потужится, и тогда чекунец со свистом вылетел из моего заднего прохода
            </p>
            <p>
                После всей этой истории у меня вылез геморой и я схожил к врачу, который 
                брал за прием нутром, что только усугубило мое положение. Он выписал мне 
                мазь, котороя помимо свой прямой функции в лечении сего дифекта так же служила
                очень хорошей смазкой для моих озорных ночей.
            </p>
            <p>
                Помимо насилия надо мной мой дед очень любил меня фотографировать ногишом
            </p>
            <img scr="popa.png" alt="Одна из таких фотографий" width="400">
            <p>
                После моего гемороя моя половая жизнь начала улчучшаться. Каждый день, когда ко 
                мне приезжали друзья, они поочередно имели меня в туза. Кайф с каждым разом 
                только увеличивался и я уже позабыл о всех своих проблемах, пока не поступил в радио
            </p>
            <h3>
                Радейка
            </h3>
            <p>
                Когда я поступил в радио ничего не предвещало беды, пока я не увидил одну из 
                своих одногруппниц: единый симбиоз женщины и мужчины с весом под 150 кг и парой 
                потных яиц можду ног, облегающх плотными лосинами.
            </p>
            <p>
                Она шпуняла меня каждый день, заставляя гонять ей за сушняком и томпонами, пока 
                не произожло страшно. В один из дней она застала меня в мужсом туалете, в который 
                сама редко ходила, преподчитая женский, и приступила к действияи.
            </p>
            <p>
                Сначала она заставила меня сосать ее потные яички, не разрешая закрыть нос 
                из-за чего мне приходилось принимать этот аромат всем своим носом, а после 
                сняла с меня штанишки и отымела меня в туза 
            </p>
            <p>
                Ни смотря на то, что она наполовину женщина, дилдак у нее толщиной был с две мои 
                руки, я моя тугая попка, которая привыкла только к бутылкам и молодым подростковым 
                членам, по началу кровоточила, но после смогла принять в себя все 30 см ярости
            </p>
            <p>
                Когда она кончила в меня, дотянувшись своей битой аж до двенадцатиперстной кишки
                она оставила меня в слезах и дрожащими ножками прямо там же, где меня нашел мой 
                курато Юрий Юрьевич и добавил мне порцию своего семени.
            </p>
            <p>
                Однако его член после биты моей одногруппницы не козался мне таким уж большим, и 
                плакал я от горя не от изнасилования, а от того, как все это произошло.
            </p>
            <p>
                После этого я стал прогуливать шарагу воизбижании половых актов с Гигантшей, но 
                моя мама и дед заставляли ходить туда, не смотря на мои дрожащие ножки, пока после 
                очередного изнасилования со стороны моего деда я не переехал к матери
            </p>
            <img scr="CemR.png" alt="Моя так называемая мама" width="500">
            <p>
                Когда я переехал к мое матери, приставть ко мне стала уже сестра, однако она 
                как полностью созревшая девушка хотела, чтобы Я ЕЕ ТРАХАЛ, а не наоборот. 
                Секс в роли актива меня не вдохновлял и очень сильно не нравился, так что я просто 
                уединялся в туалете, пока моя мама не застукала меня с трясущемися ногами и не 
                дала пизды, прогнав из дома за скаченый часом ранее троян
            </p>
            <h4>
                Как я по лесу скитался
            </h4>
            <p>
                После того как моя мать прогнала меня из дома, мне ничего не оставалось кроме 
                того, как запустить стрим в дс с телефона и не начать мытся прямо там под проливным 
                дождем
            </p>
            <p>
                Мои друзья, как только увидили это сразу же поклеили по всему городу листовки, 
                чтобы найти меня
            </p>
            <img scr="PotepR.jpg" alt="Фотография той листовки" width="600">
            <p>
                После того как все эти листовки были расклеяны по городу вся сотня моих половых 
                партнеров начали меня искть, пока в конечном итоге не нашли около Края Света, 
                попутно опять изнасиловав, и вернули домой в целости и сохранности, не считая 
                мой сфинктер, откуда я и записываю данную историю
            </p>
            <div class="hebrew-phrase">סמיון, לך הביתה, אתה לוזר 🐷</div>
        </div>
         <div class="side-panel">
            <div class="verticle-abuse left">🤡 ЛОХ 🐷 ЧМО 💩 ПЕТУХ 🐔 ТЕРПИЛА 😭 ДЫРКА 🕳️</div>
            <div class="verticle-abuse right">ТРЯПКА 🧻 ОБОСРАНЕЦ 💩 ШЛЮХА 👠 ПОДСТИЛКА 🛏️ ГЕМОРРОЙ 🍩</div>
            <h3>К написанию этой истории я приступил, пдохновившись сериалом Дневники Вампиров</h3>
            <p>Пошел Нахуй попрашайка</p>
            <div class="bismillah">بِسْمِ اللَّهِ</div>
            <div class="hebrew-phrase">שָׁלוֹם עֲלֵיכֶם 🇮🇱 ✡️</div>
            <div class="hebrew-phrase">סמיון הוא לוזר 🐷</div>
            <p>🇷🇺 🚩 ☪️ 🇸🇦 🏴 🇮🇱 ✡️</p>
            <p>😂 🤣 😭 💀 🤲</p>
            <div class="hebrew-phrase">ברוך הבא לבית המשוגעים</div>
            <div class="hebrew-phrase">סמיון המטומטם 🤡</div>
        </div>

        <div class="abuse-strip bottom"><span>🤡 СЕМЁН-ЛОХ 🐷 СЕМЁН-ЧМО 💩 СЕМЁН-ПЕТУХ 🐔 СЕМЁН-ТЕРПИЛА 😭 СЕМЁН-ДЫРКА 🕳️ СЕМЁН-ТРЯПКА 🧻 СЕМЁН-ОБОСРАНЕЦ 💩 СЕМЁН-ШЛЮХА 👠 СЕМЁН-ПОДСТИЛКА 🛏️ СЕМЁН-ГЕМОРРОЙ 🍩 СЕМЁН-ТУАЛЕТ 🚽 СЕМЁН-ПОМОЙКА 🗑️ 🤡 СЕМЁН-ЛОХ 🐷 СЕМЁН-ЧМО 💩 СЕМЁН-ПЕТУХ 🐔 СЕМЁН-ТЕРПИЛА 😭 СЕМЁН-ДЫРКА 🕳️ СЕМЁН-ТРЯПКА 🧻 СЕМЁН-ОБОСРАНЕЦ 💩 СЕМЁН-ШЛЮХА 👠 СЕМЁН-ПОДСТИЛКА 🛏️ СЕМЁН-ГЕМОРРОЙ 🍩 СЕМЁН-ТУАЛЕТ 🚽 СЕМЁН-ПОМОЙКА 🗑️</span></div>

        <div class="gdi-dialog">
            <div class="titlebar"><span>СеменМакТрахер.exe</span><span>✕</span></div>
            <div class="body">
                <div class="icon">⚠️</div>
                <div>GDI+ произошла ошибка.<br>Код: 0x80004005<br>Сфинктер: повреждён.</div>
            </div>
            <div class="buttons"><button>OK</button></div>
        </div>

            <script>
                const emojis = ["😂","🤣","💀","😭","🤲","🚩","☪️","🏴","🇷🇺","🇸🇦","🇮🇱","✡️"];
                const rain = document.getElementById("rain");
                for (let i = 0; i < 25; i++) {
                    const span = document.createElement("span");
                    span.textContent = emojis[Math.floor(Math.random() * emojis.length)];
                    span.style.left = Math.random() * 100 + "vw";
                    span.style.animationDuration = (3 + Math.random() * 5) + "s";
                    span.style.animationDelay = (Math.random() * 5) + "s";
                    span.style.fontSize = (20 + Math.random() * 30) + "px";
                    rain.appendChild(span);
                }

                const paras = document.querySelectorAll(".main-content p");
                setInterval(() => {
                    const p = paras[Math.floor(Math.random() * paras.length)];
                    p.style.transform = "translate(" + (Math.random()*4-2) + "px," + (Math.random()*4-2) + "px)";
                    p.style.filter = "hue-rotate(" + Math.floor(Math.random()*360) + "deg)";
                    setTimeout(() => {
                        p.style.transform = "";
                        p.style.filter = "";
                    }, 120);
                }, 800);

                const btn = document.querySelector(".gdi-dialog button");
                btn.addEventListener("click", () => {
                    const dlg = document.querySelector(".gdi-dialog");
                    dlg.style.display = "none";
                    setTimeout(() => { dlg.style.display = "block"; }, 3000);
                });
            </script>
        </body>
    </html>
