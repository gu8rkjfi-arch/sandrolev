<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
    <title>Влияние соцмедиа | Общественное мнение в цифровую эпоху</title>
    <!-- Google Fonts & Preconnect -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #05070a;
            font-family: 'Inter', sans-serif;
            color: #eef2ff;
            line-height: 1.5;
            scroll-behavior: smooth;
        }

        /* custom gradient & tech bg */
        .bg-glow {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -2;
            background: radial-gradient(circle at 20% 30%, rgba(20, 30, 70, 0.6), rgba(0, 0, 0, 0.95));
        }

        .noise {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
            opacity: 0.08;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 400 400' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='3'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)'/%3E%3C/svg%3E");
            background-repeat: repeat;
        }

        /* container */
        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 2rem;
            position: relative;
            z-index: 2;
        }

        /* header / nav */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.8rem 0;
            flex-wrap: wrap;
            border-bottom: 1px solid rgba(72, 187, 255, 0.2);
        }

        .logo {
            font-weight: 800;
            font-size: 1.6rem;
            background: linear-gradient(135deg, #a0e9ff, #3b82f6, #6366f1);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            letter-spacing: -0.02em;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
        }

        .nav-links a {
            color: #cbd5e6;
            text-decoration: none;
            font-weight: 500;
            transition: 0.2s;
            font-size: 0.95rem;
        }

        .nav-links a:hover {
            color: #60a5fa;
            border-bottom: 1px solid #60a5fa;
        }

        /* hero */
        .hero {
            padding: 4rem 0 3rem 0;
            text-align: center;
        }

        .hero h1 {
            font-size: 3.2rem;
            font-weight: 800;
            background: linear-gradient(to right, #ffffff, #94a3f8, #38bdf8);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            line-height: 1.2;
            margin-bottom: 1rem;
        }

        .hero .sub {
            font-size: 1.25rem;
            color: #94a3b8;
            max-width: 700px;
            margin: 0 auto;
        }

        .hero-badge {
            display: inline-block;
            background: rgba(59, 130, 246, 0.15);
            backdrop-filter: blur(4px);
            border-radius: 40px;
            padding: 0.3rem 1rem;
            font-size: 0.8rem;
            border: 1px solid rgba(59, 130, 246, 0.4);
            margin-bottom: 1.5rem;
        }

        /* cards and sections */
        .section {
            margin: 6rem 0;
        }

        .section-title {
            font-size: 2.2rem;
            font-weight: 700;
            margin-bottom: 2rem;
            position: relative;
            display: inline-block;
        }

        .section-title:after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 60%;
            height: 3px;
            background: linear-gradient(90deg, #3b82f6, #a78bfa);
            border-radius: 4px;
        }

        .grid-2col {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 2rem;
        }

        .card {
            background: rgba(15, 23, 42, 0.6);
            backdrop-filter: blur(8px);
            border-radius: 2rem;
            padding: 2rem;
            border: 1px solid rgba(56, 189, 248, 0.2);
            transition: all 0.25s ease;
            box-shadow: 0 20px 35px -12px rgba(0, 0, 0, 0.3);
        }

        .card:hover {
            border-color: #3b82f6;
            transform: translateY(-5px);
            background: rgba(20, 30, 55, 0.7);
        }

        .card h3 {
            font-size: 1.6rem;
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .card p, .card li {
            color: #cbd5e1;
            margin-bottom: 0.75rem;
        }

        .icon-emoj {
            font-size: 2rem;
        }

        .list-styled {
            padding-left: 1.5rem;
            margin: 1rem 0;
        }

        .list-styled li {
            margin: 0.5rem 0;
        }

        .stat-badge {
            background: #0f172a;
            border-radius: 2rem;
            padding: 0.2rem 0.8rem;
            font-weight: 500;
            font-size: 0.8rem;
            color: #7dd3fc;
        }

        .quote {
            font-style: italic;
            border-left: 4px solid #3b82f6;
            padding-left: 1.5rem;
            margin: 1.5rem 0;
            color: #b9c7da;
        }

        .fight-tips {
            display: flex;
            flex-wrap: wrap;
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .tip-item {
            flex: 1 1 200px;
            background: rgba(0, 0, 0, 0.35);
            border-radius: 1.5rem;
            padding: 1.2rem;
            text-align: center;
            backdrop-filter: blur(4px);
            border: 1px solid #2d3a5e;
        }

        .footer {
            border-top: 1px solid rgba(59, 130, 246, 0.2);
            padding: 2.5rem 0;
            margin-top: 3rem;
            text-align: center;
            color: #94a3b8;
        }

        .creator {
            font-size: 1.1rem;
            font-weight: 500;
            margin-top: 1rem;
            background: linear-gradient(120deg, #a5f3fc, #818cf8);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
        }

        button {
            background: none;
            border: none;
        }

        @media (max-width: 800px) {
            .grid-2col {
                grid-template-columns: 1fr;
            }
            .hero h1 {
                font-size: 2.2rem;
            }
            .container {
                padding: 0 1.5rem;
            }
            .navbar {
                flex-direction: column;
                gap: 1rem;
            }
        }

        /* animated underline for links */
        a {
            text-decoration: none;
        }

        .btn-soft {
            display: inline-block;
            margin-top: 1rem;
            background: rgba(59, 130, 246, 0.2);
            padding: 0.5rem 1.2rem;
            border-radius: 40px;
            font-weight: 500;
            transition: 0.2s;
            border: 1px solid #3b82f6;
        }

        .btn-soft:hover {
            background: #3b82f6;
            color: white;
        }
    </style>
</head>
<body>
<div class="bg-glow"></div>
<div class="noise"></div>

<div class="container">
    <!-- навигация -->
    <div class="navbar">
        <div class="logo">✦ echoVox</div>
        <div class="nav-links">
            <a href="#influence">Влияние</a>
            <a href="#negative">Риски</a>
            <a href="#fight">Как бороться</a>
            <a href="#author">Об авторе</a>
        </div>
    </div>

    <!-- Hero -->
    <div class="hero">
        <div class="hero-badge">🔍 Социальные медиа · Общественное мнение · Цифровая эпоха</div>
        <h1>Влияние соцмедиа <br> на общественное мнение</h1>
        <div class="sub">Алгоритмы, тренды, фейки — как миллиарды постов формируют реальность и почему мы должны научиться мыслить критически.</div>
    </div>

    <!-- раздел 1: влияние -->
    <div class="section" id="influence">
        <div class="section-title">📱 Как соцмедиа формируют реальность</div>
        <div class="grid-2col">
            <div class="card">
                <h3><span class="icon-emoj">🎯</span> Эхо-камеры и фильтры</h3>
                <p>Социальные платформы используют персонализированные алгоритмы, которые показывают нам контент, соответствующий нашим убеждениям. Это создаёт «информационные пузыри»: пользователи редко сталкиваются с альтернативными точками зрения, что усиливает поляризацию общества. Общественное мнение становится более радикальным, а диалог между разными группами — практически невозможным.</p>
                <div class="quote">«Человек склонен доверять тому, что видит чаще. Алгоритмы знают это лучше всех.»</div>
            </div>
            <div class="card">
                <h3><span class="icon-emoj">⚡</span> Вирусность vs достоверность</h3>
                <p>Эмоциональные, сенсационные и часто ложные новости распространяются в 6 раз быстрее правдивых. Соцмедиа награждают громкие заголовки и провокации. Общественное мнение формируется не фактами, а реакциями: лайки, репосты, комментарии — новая валюта влияния. Так создаются искусственные тренды, способные повлиять на выборы, здоровье и социальные движения.</p>
                <span class="stat-badge">📊 Исследования MIT: ложь распространяется на 70% быстрее</span>
            </div>
        </div>
        <div class="card" style="margin-top: 1.5rem;">
            <h3>📈 Цифровые манипуляции и микшер мнений</h3>
            <p>Боты, тролли и скоординированные кампании активно используют соцсети для искажения общественной дискуссии. Современные методы «астротурфинга» (искусственное создание народной поддержки) способны за пару часов изменить тональность обсуждения любого события. Люди, не подозревая об этом, становятся частью информационной войны. Более того, социальные платформы монетизируют внимание, а не истину, поэтому даже крупные компании косвенно заинтересованы в провокационном контенте.</p>
        </div>
    </div>

    <!-- раздел 2: негативные последствия -->
    <div class="section" id="negative">
        <div class="section-title">⚠️ Негативное влияние: от тревожности до раскола общества</div>
        <div class="grid-2col">
            <div class="card">
                <h3><span class="icon-emoj">🧠</span> Психологический прессинг</h3>
                <p>Постоянное сравнение себя с идеальными образами в соцсетях ведёт к снижению самооценки, развитию тревожности и депрессии. Алгоритмы фиксируют слабости пользователя и подсовывают контент, усиливающий неуверенность или гнев. Общественное мнение становится более пессимистичным и агрессивным. Кроме того, феномен FOMO (страх упустить выгоду) заставляет людей проводить в соцмедиа до 6-8 часов в день.</p>
            </div>
            <div class="card">
                <h3><span class="icon-emoj">🌪️</span> Дезинформация и угроза демократии</h3>
                <p>Фейковые новости, манипуляции статистикой, теории заговора — всё это находит благодатную почву в соцмедиа. Исследования показывают, что ложные политические нарративы запоминаются лучше опровержений. Общественное мнение раскалывается на враждующие лагеря, снижается доверие к традиционным институтам и СМИ. Выборы, референдумы и гражданские инициативы становятся заложниками цифровых манипуляций.</p>
                <div class="quote">«Мы перестали проверять факты, но мгновенно делимся эмоциями» — Рената Салес, медиаэксперт</div>
            </div>
        </div>
        <div class="card" style="margin-top: 1rem;">
            <h3>📉 Поляризация и потеря эмпатии</h3>
            <p>Соцмедиа создают среду, где анонимность и дистанция позволяют людям проявлять жестокость, которую они не показали бы в реальной жизни. Кибербуллинг, отмена (cancel culture) и массовые травли формируют токсичную среду. Общественное мнение под влиянием агрессивных групп становится нетерпимым, а конструктивный диалог заменяется взаимными обвинениями. Особенно уязвимы подростки и молодёжь, чья психика ещё формируется.</p>
        </div>
    </div>

    <!-- раздел 3: как бороться -->
    <div class="section" id="fight">
        <div class="section-title">🛡️ Как бороться с негативным влиянием соцмедиа</div>
        <div class="card">
            <h3>💡 Инструменты цифровой гигиены и медиаграмотности</h3>
            <p>Справиться с деструктивным воздействием соцсетей можно, но для этого нужна система: от личных привычек до общественных инициатив. Ниже — ключевые стратегии, которые помогают защитить критическое мышление и восстановить контроль над информационным полем.</p>
            <div class="fight-tips">
                <div class="tip-item">🔍 <strong>Фактчекинг</strong><br>Проверяйте информацию через сервисы вроде Snopes, «Лапша Медиа» или FactCheck.org. До репоста — задайте вопрос: кто автор, какие доказательства?</div>
                <div class="tip-item">🧠 <strong>Критическое мышление</strong><br>Не поддавайтесь эмоциональным заголовкам. Ищите первоисточники, анализируйте, кому выгодна та или иная новость.</div>
                <div class="tip-item">⏳ <strong>Цифровой детокс</strong><br>Ограничьте время в соцсетях (используйте таймеры приложений). Выделите часы без экранов — для чтения, спорта, живого общения.</div>
                <div class="tip-item">🌐 <strong>Разнообразие источников</strong><br>Подписывайтесь на разные медиа, включая оппозиционные вашим взглядам. Это ломает эхо-камеру.</div>
            </div>
            <p style="margin-top: 1.8rem;">Также важно обучать медиаграмотности в школах и университетах. Европейские программы показывают: уже после 10 часов тренингов люди на 40% реже верят дезинформации. Технологические компании должны внедрять алгоритмы, снижающие охват фейков, а государство — поддерживать независимую журналистику. На личном уровне полезно отключать персонализированную рекламу и периодически чистить ленту.</p>
        </div>
        <div class="grid-2col" style="margin-top: 2rem;">
            <div class="card">
                <h3>📚 Образование и осознанное потребление</h3>
                <p>Создавайте среду, где правда ценится выше лайков. Не стесняйтесь блокировать токсичных пользователей. Обсуждайте с друзьями и семьёй важность проверки информации. И помните: любой алгоритм можно «обмануть» — ищите информацию осознанно, пользуйтесь поиском, а не только рекомендательной лентой. Также полезно раз в месяц анализировать, на кого вы подписаны и какой контент вызывает у вас гнев или тревогу — возможно, пришло время отписаться.</p>
            </div>
            <div class="card">
                <h3>⚖️ Регулирование и ответственность платформ</h3>
                <p>Акты цифровых услуг (DSA в ЕС) и другие законы обязывают соцсети маркировать рекламу, бороться с ботами и дезинформацией. Поддерживайте петиции за прозрачность алгоритмов. Кроме того, не стоит недооценивать роль сообществ — совместный фактчекинг и модерация пользователями снижают влияние пропаганды. Будьте активным гражданином: сообщайте о фейках и ненависти.</p>
            </div>
        </div>
        <div class="card" style="margin-top: 1rem;">
            <h3>🧩 Личная стратегия устойчивости к информационным бурям</h3>
            <p>Создайте для себя «информационный фильтр»: доверяйте только проверенным авторам, используйте RSS или агрегаторы новостей, которые не зависят от алгоритмов. Практикуйте «медитацию на новости» — делайте паузу перед тем, как что-то репостнуть. Исследования показывают, что 5-минутная задержка снижает репосты ложной информации на 30%. Будьте примером для других: комментируйте рационально, избегайте оскорблений, цените конструктив. Только так мы сможем вернуть общественному мнению здоровую основу.</p>
        </div>
    </div>

    <!-- раздел про автора и создателя -->
    <div class="section" id="author">
        <div class="section-title">✨ О проекте и создателе</div>
        <div class="card" style="text-align: center; background: linear-gradient(145deg, #0f172a, #111827);">
            <span style="font-size: 3rem;">👨‍🎓</span>
            <h3 style="margin-top: 0.5rem;">Шервашидзе Сандро</h3>
            <p style="font-size: 1.2rem; font-weight: 500;">Ученик 10Б класса</p>
            <p style="max-width: 600px; margin: 1rem auto;">«Этот проект создан, чтобы привлечь внимание к важнейшей проблеме нашего времени — как социальные сети манипулируют нашими взглядами и что мы можем сделать, чтобы сохранить свободу мышления. Я глубоко изучил тему влияния соцмедиа, проанализировал десятки исследований, и моя цель — помочь людям, особенно подросткам, стать устойчивее к цифровым манипуляциям. Каждый из нас способен управлять своей лентой, а не быть марионеткой алгоритмов. Надеюсь, эта информация вдохновит вас на перемены!»</p>
            <div class="creator">✧ digital citizen & медиаактивист ✧</div>
            <div style="margin-top: 1rem; font-size: 0.85rem; color: #7e8aa2;">Сайт создан в рамках учебного проекта · 2025</div>
        </div>
    </div>

    <!-- дополнительный блок с объемной статистикой -->
    <div class="section">
        <div class="section-title">📊 Факты, которые заставляют задуматься</div>
        <div class="grid-2col">
            <div class="card">
                <h3>🌍 Глобальные цифры</h3>
                <ul class="list-styled">
                    <li>📌 4,9 млрд человек активно пользуются соцсетями (2025)</li>
                    <li>📌 64% пользователей хотя бы раз сталкивались с фейковыми новостями</li>
                    <li>📌 Алгоритмы Facebook увеличивают время просмотра контента на 34% за счёт эмоциональных постов</li>
                    <li>📌 Только 2% подростков умеют полноценно проверять источники информации</li>
                </ul>
            </div>
            <div class="card">
                <h3>🧪 Эксперименты и последствия</h3>
                <ul class="list-styled">
                    <li>🔬 Эксперимент в США: ложный твит о кандидате менял мнение 15% избирателей</li>
                    <li>📉 После блокировки новостей в соцсетях уровень поляризации упал на 23%</li>
                    <li>💬 71% людей чувствуют тревогу, когда видят агрессивные политические дискуссии в сети</li>
                    <li>🎓 Курсы медиаграмотности снижают веру в фейки на 46% за 2 месяца</li>
                </ul>
            </div>
        </div>
    </div>

    <!-- footer -->
    <div class="footer">
        <p>© 2025 Влияние соцмедиа на общественное мнение | Проект ученика 10Б класса Шервашидзе Сандро</p>
        <p style="font-size: 0.8rem; margin-top: 0.5rem;">Осознанное потребление контента — залог здорового общества. Будьте критичны, проверяйте факты, защищайте свой разум.</p>
        <div style="margin-top: 1rem;">
            <a href="#" class="btn-soft" style="font-size: 0.8rem;">Наверх ↑</a>
        </div>
    </div>
</div>

<!-- small smooth scroll -->
<script>
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function(e) {
            const targetId = this.getAttribute('href');
            if(targetId === "#") return;
            const targetElement = document.querySelector(targetId);
            if(targetElement) {
                e.preventDefault();
                targetElement.scrollIntoView({ behavior: 'smooth', block: 'start' });
            }
        });
    });
    // tiny interactive effect for cards (already cool)
    console.log("Сайт создан Шервашидзе Сандро, 10Б класс — влияние соцмедиа и методы борьбы с негативом")
</script>
</body>
</html>
