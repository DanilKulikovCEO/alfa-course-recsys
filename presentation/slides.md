---
marp: true
theme: default
paginate: true
size: 16:9
style: |
  section {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
    color: #1F2229;
    background-color: #FFFFFF;
    padding: 35px 55px;
    font-size: 20px;
    line-height: 1.4;
  }
  h1 {
    color: #1F2229;
    font-size: 34px;
    margin-bottom: 8px;
    font-weight: 800;
    letter-spacing: -0.5px;
  }
  h2 {
    color: #EF3124;
    font-size: 22px;
    margin-top: 0;
    margin-bottom: 16px;
    font-weight: 700;
  }
  .header-tag {
    display: inline-block;
    background-color: #FEECEB;
    color: #EF3124;
    font-size: 13px;
    font-weight: 700;
    padding: 4px 12px;
    border-radius: 20px;
    margin-bottom: 12px;
    border: 1px solid #FCD4D1;
  }
  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
  }
  .grid-3 {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 16px;
  }
  .grid-4 {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    gap: 14px;
  }
  .card {
    background-color: #F8F9FA;
    border: 1px solid #E5E7EB;
    border-radius: 14px;
    padding: 16px 20px;
  }
  .card-highlight {
    background: linear-gradient(135deg, #FFF5F5 0%, #FFFFFF 100%);
    border: 1.5px solid #EF3124;
    border-radius: 14px;
    padding: 16px 20px;
  }
  .card h3 {
    font-size: 17px;
    font-weight: 700;
    color: #1F2229;
    margin: 0 0 8px 0;
  }
  .metric-box {
    text-align: center;
    background: #FFFFFF;
    border: 1px solid #E5E7EB;
    border-radius: 12px;
    padding: 14px 10px;
  }
  .metric-value {
    font-size: 30px;
    font-weight: 900;
    color: #EF3124;
    line-height: 1;
  }
  .metric-value-green {
    font-size: 30px;
    font-weight: 900;
    color: #059669;
    line-height: 1;
  }
  .metric-label {
    font-size: 13px;
    color: #6B7280;
    margin-top: 6px;
    font-weight: 600;
  }
  .badge {
    display: inline-block;
    padding: 3px 8px;
    border-radius: 6px;
    font-size: 12px;
    font-weight: 700;
  }
  .badge-red { background: #FEECEB; color: #EF3124; }
  .badge-green { background: #ECFDF5; color: #059669; }
  .badge-gray { background: #F3F4F6; color: #4B5563; }
  .badge-amber { background: #FEF3C7; color: #D97706; }
  ul {
    margin: 6px 0;
    padding-left: 22px;
  }
  li {
    margin-bottom: 6px;
    font-size: 16px;
    color: #374151;
  }
  footer {
    font-size: 12px;
    color: #9CA3AF;
  }
---

<!-- _class: lead -->
<!-- _paginate: false -->
<div style="text-align: center; padding-top: 40px;">
  <div style="display: inline-flex; align-items: center; gap: 10px; margin-bottom: 15px;">
    <span style="background: #EF3124; color: white; font-weight: 900; font-size: 26px; width: 44px; height: 44px; border-radius: 12px; display: inline-flex; align-items: center; justify-content: center; box-shadow: 0 4px 12px rgba(239, 49, 36, 0.3);">А</span>
    <span style="font-size: 24px; font-weight: 800; letter-spacing: -0.5px;">Альфа-Банк &nbsp;•&nbsp; Hack&Change 2026</span>
  </div>

  <h1 style="font-size: 44px; margin-bottom: 12px; color: #1F2229;">
    Альфа-Курс: знания в нужный момент
  </h1>
  <p style="font-size: 22px; color: #4B5563; font-weight: 500; margin-bottom: 30px;">
    Персональная рекомендательная система образовательных продуктов для малого бизнеса
  </p>

  <div style="background: #F8F9FA; border: 1.5px solid #E5E7EB; border-radius: 16px; padding: 18px 28px; display: inline-block; text-align: left; max-width: 820px; box-shadow: 0 2px 8px rgba(0,0,0,0.03);">
    <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 10px;">
      <span style="font-weight: 700; font-size: 16px; color: #1F2229;">Порядок экспертной проверки жюри (Допуск):</span>
      <span class="badge badge-green">Код проверен • 8/8 тестов пройдены</span>
    </div>
    <div style="font-family: monospace; background: #1F2229; color: #F9FAFB; padding: 10px 14px; border-radius: 8px; font-size: 14px; margin-bottom: 10px;">
      git clone https://github.com/ArseniyNov52/alfa-course-recsys.git<br>
      cd alfa-course-recsys &amp;&amp; docker compose up --build
    </div>
    <div style="display: flex; justify-content: space-between; font-size: 14px; color: #4B5563;">
      <span>Репозиторий: <a href="https://github.com/ArseniyNov52/alfa-course-recsys" style="color: #EF3124; font-weight: bold; text-decoration: none;">github.com/ArseniyNov52/alfa-course-recsys</a></span>
      <span>Веб-сервис: <b>http://localhost:8000</b></span>
    </div>
  </div>
</div>

---

<span class="header-tag">Проблема и пользователи</span>
# Разрыв между болью бизнеса и каталогом курсов

## 3 ключевых пользовательских архетипа сталкиваются с разным контекстом

<div class="grid-3">
  <div class="card">
    <span class="badge badge-amber" style="margin-bottom: 8px;">01. Новичок</span>
    <h3>Анна: открытие дела</h3>
    <ul>
      <li><b>Ситуация:</b> хочет открыть кофейню, нулевой опыт в бизнесе.</li>
      <li><b>Боль:</b> страх налоговых проверок, штрафов и Роспотребнадзора.</li>
      <li><b>Потребность:</b> пошаговый чек-лист и ясный первый шаг.</li>
    </ul>
  </div>

  <div class="card">
    <span class="badge badge-red" style="margin-bottom: 8px;">02. Микробизнес</span>
    <h3>Иван: автосервис</h3>
    <ul>
      <li><b>Ситуация:</b> действующий бизнес, заказы есть, но касса пуста.</li>
      <li><b>Боль:</b> регулярный кассовый разрыв, нечем платить зарплату.</li>
      <li><b>Потребность:</b> готовый шаблон управленческого учета ДДС сегодня.</li>
    </ul>
  </div>

  <div class="card">
    <span class="badge badge-gray" style="margin-bottom: 8px;">03. Масштабирование</span>
    <h3>Дмитрий: селлер WB</h3>
    <ul>
      <li><b>Ситуация:</b> оборот 3.5 млн ₽, утонул в 14-часовой операционке.</li>
      <li><b>Боль:</b> нет времени, ошибки при найме, потеря маржи.</li>
      <li><b>Потребность:</b> системный курс по делегированию и прямым поставкам.</li>
    </ul>
  </div>
</div>

<div class="card-highlight" style="margin-top: 16px;">
  <b>Главная проблема бейзлайна:</b> поиск по ключевым словам советует новичку сложный курс финдиректора за 15 000 ₽ вместо чек-листа регистрации ИП, вызывая страх и отток.
</div>

---

<span class="header-tag">Концепция решения</span>
# Сквозная воронка монетизации и ретеншна

## От быстрого бесплатного решения к покупке флагманского продукта

<div class="grid-3" style="margin-top: 15px;">
  <div class="card">
    <div style="font-size: 32px; font-weight: 900; color: #EF3124; margin-bottom: 6px;">01</div>
    <h3>Быстрый дофамин</h3>
    <p style="font-size: 15px; color: #4B5563;">
      Бесплатный прикладной инструмент (чек-лист, шаблон договора, калькулятор) закрывает горящую боль за <b>10–15 минут</b>.
    </p>
    <span class="badge badge-green">Рост доверия и DAU</span>
  </div>

  <div class="card">
    <div style="font-size: 32px; font-weight: 900; color: #EF3124; margin-bottom: 6px;">02</div>
    <h3>Персональный контекст</h3>
    <p style="font-size: 15px; color: #4B5563;">
      Модуль XAI формирует прозрачное обоснование: <i>«Почему это подходит именно вашей стадии бизнеса и задаче»</i>.
    </p>
    <span class="badge badge-red">100% Stage-Match</span>
  </div>

  <div class="card">
    <div style="font-size: 32px; font-weight: 900; color: #EF3124; margin-bottom: 6px;">03</div>
    <h3>Логический апселл</h3>
    <p style="font-size: 15px; color: #4B5563;">
      Блок <b>«Следующий шаг»</b> связывает бесплатный шаблон с глубоким платным курсом платформы «Альфа-Курс».
    </p>
    <span class="badge badge-amber">Рост CR в покупку</span>
  </div>
</div>

<div class="grid-2" style="margin-top: 20px;">
  <div class="metric-box">
    <div class="metric-value">+35%</div>
    <div class="metric-label">Целевой рост конверсии в платные курсы</div>
  </div>
  <div class="metric-box">
    <div class="metric-value-green">+22.5%</div>
    <div class="metric-label">Прирост качества ранжирования NDCG@5 над бейзлайном</div>
  </div>
</div>

---

<span class="header-tag">Архитектура ядра RecSys</span>
# Двухстадийный гибридный пайплайн ранжирования

## Архитектура исключает выдачу материалов не по уровню зрелости компании

<div class="grid-2">
  <div class="card">
    <h3>Этап 1: Stage-Aware Semantic Retrieval</h3>
    <ul>
      <li><b>Векторизация задачи:</b> TF-IDF с n-gram (1,2) и суб-линейным масштабированием частот.</li>
      <li><b>Stage-Gating фильтрация:</b> жесткая блокировка несовместимых уровней сложности:
        <ul>
          <li>Новичок не получает аудит холдинга и курс финдиректора;</li>
          <li>Селлеру с оборотом 3.5 млн ₽ не предлагается регистрация ИП.</li>
        </ul>
      </li>
      <li><b>Доменный бустинг:</b> приоритет отраслевым материалам (HoReCa, услуги).</li>
    </ul>
  </div>

  <div class="card">
    <h3>Этап 2: Multi-Objective Ranker</h3>
    <div style="background: #1F2229; color: #F9FAFB; padding: 10px 14px; border-radius: 8px; font-family: monospace; font-size: 13px; margin-bottom: 10px;">
      FinalScore = 0.40 * Relevance<br>
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+ 0.30 * StageFit<br>
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+ 0.15 * FunnelScore<br>
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+ 0.15 * Actionability
    </div>
    <ul>
      <li><b>FunnelScore:</b> приоритизация бесплатного первого шага для новых и платных углубленных курсов для прогретых пользователей.</li>
      <li><b>Дедупликация:</b> штраф за ранее пройденные материалы.</li>
    </ul>
  </div>
</div>

---

<span class="header-tag">Холодный старт и онбординг</span>
# Нулевой отток при первом посещении

## Мгновенная ценность без принуждения к заполнению длинных анкет

<div class="grid-2" style="margin-top: 15px;">
  <div class="card">
    <h3>«Золотой стартовый набор предпринимателя»</h3>
    <p style="font-size: 15px; color: #4B5563;">
      Если пользователь вошел без истории и без запроса, система мгновенно выдает проверенный базовый комплект правовой и финансовой гигиены:
    </p>
    <ul>
      <li><b>Чек-лист:</b> 10 главных ошибок первого года бизнеса;</li>
      <li><b>Навигатор:</b> выбор налогового режима 2026 (УСН/ПСН/АУСН);</li>
      <li><b>Инструкция:</b> онлайн-кассы 54-ФЗ и эквайринг без штрафов;</li>
      <li><b>Шаблоны:</b> безопасный договор оказания услуг и закрывающие акты.</li>
    </ul>
  </div>

  <div class="card">
    <h3>Микро-онбординг в 2 клика прямо в поиске</h3>
    <div class="card-highlight" style="margin-bottom: 12px; padding: 12px 16px;">
      <span style="font-size: 13px; font-weight: 700; color: #EF3124; display: block; margin-bottom: 4px;">Свободный текстовый ввод:</span>
      <span style="font-size: 14px; color: #1F2229; font-style: italic;">«хочу открыть точку шаурмы, какие налоги выбрать»</span>
    </div>
    <ul>
      <li><b>Адаптация на лету:</b> система сама извлекает стадию и сферу из естественного языка без опросников;</li>
      <li><b>Отсутствие барьеров:</b> предприниматель получает ответ за 1 секунду;</li>
      <li><b>100% приватность:</b> персональные данные клиентов не передаются во внешние API.</li>
    </ul>
  </div>
</div>

---

<span class="header-tag">Оффлайн-валидация и бейзлайн</span>
# Доказательное сравнение с бейзлайном (Критерий 5)

## Гибридная модель превосходит подбор по ключевым словам по всем метрикам

<div class="grid-4" style="margin-top: 15px;">
  <div class="metric-box">
    <div class="metric-value-green">0.9412</div>
    <div class="metric-label">NDCG@5 (Модель)</div>
    <span class="badge badge-green" style="margin-top: 6px;">+22.5% uplift</span>
  </div>

  <div class="metric-box">
    <div class="metric-value">0.7684</div>
    <div class="metric-label">NDCG@5 (Бейзлайн)</div>
    <span class="badge badge-gray" style="margin-top: 6px;">Тематический поиск</span>
  </div>

  <div class="metric-box">
    <div class="metric-value-green">100%</div>
    <div class="metric-label">Stage Match (Модель)</div>
    <span class="badge badge-green" style="margin-top: 6px;">Идеальная точность</span>
  </div>

  <div class="metric-box">
    <div class="metric-value" style="color: #D97706;">55%</div>
    <div class="metric-label">Stage Match (Бейзлайн)</div>
    <span class="badge badge-amber" style="margin-top: 6px;">45% ошибок стадии</span>
  </div>
</div>

<div class="grid-2" style="margin-top: 20px;">
  <div class="card" style="border-left: 4px solid #EF3124;">
    <h3 style="color: #EF3124;">Характерные ошибки бейзлайна:</h3>
    <ul>
      <li><b>Ложное совпадение:</b> по слову «финансы» рекомендует новичку курс финдиректора за 12 900 ₽;</li>
      <li><b>Неактуальность:</b> селлеру с оборотом 3.5 млн ₽ предлагает регистрацию ИП;</li>
      <li><b>Отсутствие воронки:</b> нет связки бесплатного шаблона с платным курсом.</li>
    </ul>
  </div>

  <div class="card" style="border-left: 4px solid #059669;">
    <h3 style="color: #059669;">Преимущества нашей модели:</h3>
    <ul>
      <li><b>0 критических ошибок</b> несовпадения стадии бизнеса;</li>
      <li><b>Баланс форматов:</b> 10-минутный чек-лист + глубокий видеокурс;</li>
      <li><b>Интерпретируемость:</b> прозрачное обоснование для пользователя.</li>
    </ul>
  </div>
</div>

---

<span class="header-tag">Живая демонстрация (25% оценки финала)</span>
# Интерактивный Web UI в фирменном стиле Альфа-Банка

## Доступен экспертам жюри локально и в Docker на http://localhost:8000

<div class="grid-3" style="margin-top: 15px;">
  <div class="card">
    <h3>1. Селектор сценариев жюри</h3>
    <p style="font-size: 14px; color: #4B5563;">
      Переключение между профилями Анны, Ивана, Дмитрия и холодным стартом в 1 клик для мгновенной валидации.
    </p>
    <div style="background: #FFFFFF; border: 1px solid #E5E7EB; border-radius: 8px; padding: 8px; font-size: 12px; margin-top: 8px;">
      <b>Профиль:</b> Анна (Новичок / HoReCa)<br>
      <b>Выдача:</b> Чек-лист СЭС + Налоги 2026
    </div>
  </div>

  <div class="card">
    <h3>2. Блок объяснимости (XAI)</h3>
    <p style="font-size: 14px; color: #4B5563;">
      Каждая рекомендация подробно раскрывает ценность и обоснование под текущие вводные человека.
    </p>
    <div style="background: #FFF5F5; border: 1px solid #FCD4D1; border-radius: 8px; padding: 8px; font-size: 12px; margin-top: 8px;">
      <i>«Подходит под стадию запуска кофейни: закрывает вопрос за 10 мин без штрафов»</i>
    </div>
  </div>

  <div class="card">
    <h3>3. Целевой «Следующий шаг»</h3>
    <p style="font-size: 14px; color: #4B5563;">
      Прямой переход на платформу «Альфа-Курс» и формирование сквозного трека обучения.
    </p>
    <div style="background: #F0FDF4; border: 1px solid #BBF7D0; border-radius: 8px; padding: 8px; font-size: 12px; margin-top: 8px;">
      <b>Next Step:</b> применить чек-лист $\to$ перейти к углубленному курсу по УСН.
    </div>
  </div>
</div>

---

<span class="header-tag">Side-by-Side панель аудита</span>
# Прозрачность рекомендаций для продуктовой команды

## Встроенный инструмент сравнительного анализа прямо в веб-интерфейсе

<div class="grid-2" style="margin-top: 15px;">
  <div class="card" style="background: #FFFBEB; border-color: #FDE68A;">
    <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 8px;">
      <h3 style="color: #92400E; margin: 0;">Колонка Бейзлайна</h3>
      <span class="badge badge-amber">Точность: 55%</span>
    </div>
    <ul style="font-size: 15px;">
      <li>1. Золотой чек-лист предпринимателя <span class="badge badge-green">OK</span></li>
      <li>2. Навигатор по налогам 2026 <span class="badge badge-green">OK</span></li>
      <li>3. Мастер-курс: Финдиректор для бизнеса <span class="badge badge-red">Ошибка</span></li>
      <li>4. Практикум: Преодоление кассового разрыва <span class="badge badge-red">Ошибка</span></li>
    </ul>
    <div style="font-size: 13px; color: #B45309; padding-top: 8px; border-top: 1px solid #FDE68A;">
      ⚠️ Выявлены нерелевантные платные курсы в топ-3 для новичка
    </div>
  </div>

  <div class="card" style="background: #F0FDF4; border-color: #BBF7D0;">
    <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 8px;">
      <h3 style="color: #166534; margin: 0;">Колонка Гибридной Модели</h3>
      <span class="badge badge-green">Точность: 100%</span>
    </div>
    <ul style="font-size: 15px;">
      <li>1. Чек-лист: Регистрация ИП за 3 дня <span class="badge badge-green">Идеально</span></li>
      <li>2. Чек-лист открытия кофейни: СЭС, СанПиН <span class="badge badge-green">Идеально</span></li>
      <li>3. Навигатор по налогам: УСН, ПСН, АУСН <span class="badge badge-green">Идеально</span></li>
      <li>4. Экономика кофейни: от аренды до окупаемости <span class="badge badge-green">Next Step</span></li>
    </ul>
    <div style="font-size: 13px; color: #15803D; padding-top: 8px; border-top: 1px solid #BBF7D0;">
      ✓ Все материалы строго соответствуют стадии запуска общепита
    </div>
  </div>
</div>

---

<span class="header-tag">Дизайн A/B-тестирования (Критерий 6)</span>
# План внедрения и оценка экономического эффекта

## Статистически строгий расчет двухнедельного A/B-эксперимента

<div class="grid-3" style="margin-top: 15px;">
  <div class="card">
    <h3>Параметры теста</h3>
    <ul>
      <li><b>Трафик (DAU):</b> 5 000 посетителей/день;</li>
      <li><b>Длительность:</b> 14 дней (70 000 сессий);</li>
      <li><b>Сплит групп:</b> 50% Control / 50% Test;</li>
      <li><b>Дизайн:</b> $\alpha = 0.05$ (95% CI), Power $1-\beta = 80\%$.</li>
    </ul>
  </div>

  <div class="card">
    <h3>Primary KPI (Конверсия)</h3>
    <ul>
      <li><b>Control CR (Бейзлайн):</b> 2.50%;</li>
      <li><b>Test CR (Модель):</b> 3.38%;</li>
      <li><b>MDE:</b> относительный uplift <b>+35.0%</b>;</li>
      <li><b>Стат. значимость:</b> достигается на 11-й день теста.</li>
    </ul>
  </div>

  <div class="card card-highlight">
    <h3 style="color: #EF3124;">Финансовый эффект</h3>
    <div class="metric-value" style="font-size: 26px;">+1.5 млн ₽</div>
    <div class="metric-label">Доп. выручка за 14 дней теста</div>
    <div style="margin-top: 10px; font-size: 14px; color: #4B5563;">
      Проекционный годовой эффект:<br>
      <b style="font-size: 18px; color: #1F2229;">+39 000 000 ₽ / год</b>
    </div>
  </div>
</div>

<div class="card" style="margin-top: 16px;">
  <span style="font-size: 13px; font-weight: 700; color: #1F2229; text-transform: uppercase;">Защитные метрики (Guardrail Metrics):</span>
  <div class="grid-3" style="margin-top: 8px; font-size: 14px; color: #4B5563;">
    <div>• <b>30-day Retention / DAU:</b> возврат за шаблонами</div>
    <div>• <b>Completion Rate:</b> завершаемость материалов</div>
    <div>• <b>Negative Feedback:</b> отсутствие раздражения</div>
  </div>
</div>

---

<span class="header-tag">Итоги и готовность</span>
# Технический стек и готовность к сдаче

## Решение полностью автономно, протестировано и упаковано в Docker

<div class="grid-2">
  <div class="card">
    <h3>Технологический стек</h3>
    <ul>
      <li><b>Бэкенд:</b> Python 3.12, FastAPI, Pydantic v2, scikit-learn;</li>
      <li><b>Фронтенд:</b> React 18, TypeScript, Tailwind CSS, Lucide;</li>
      <li><b>Контейнеризация:</b> Multi-stage Dockerfile (Node 20 + Python 3.12);</li>
      <li><b>Тестирование:</b> 8/8 автотестов на `pytest` (0.77 сек);</li>
      <li><b>Автономия:</b> Zero-Config out-of-the-box (работает без внешних API).</li>
    </ul>
  </div>

  <div class="card-highlight" style="display: flex; flex-direction: column; justify-content: space-between;">
    <div>
      <span class="badge badge-green" style="margin-bottom: 8px;">Критерий допуска: 100% готовность</span>
      <h3 style="color: #EF3124;">Команда для проверки:</h3>
      <div style="font-family: monospace; background: #1F2229; color: #F9FAFB; padding: 12px; border-radius: 8px; font-size: 14px; margin: 10px 0;">
        docker compose up --build
      </div>
      <p style="font-size: 14px; color: #4B5563;">
        Веб-витрина доступна сразу на <b>http://localhost:8000</b>
      </p>
    </div>

    <div style="border-top: 1px solid #FCD4D1; padding-top: 10px; font-size: 14px; color: #1F2229;">
      Репозиторий открыт: <b>github.com/ArseniyNov52/alfa-course-recsys</b>
    </div>
  </div>
</div>
