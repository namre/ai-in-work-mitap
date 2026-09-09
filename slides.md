---
theme: default
title: ИИ в работе
titleTemplate: '%s — РАЗУМ ИТ митап'
info: |
  Внутренний митап департамента ИТ ДК РАЗУМ.
  Как ИИ меняет работу, личный опыт успехов и провалов.
author: РАЗУМ ИТ
keywords: ai,agents,mcp,mitap
class: text-center
drawings:
  persist: false
transition: slide-left
mdc: true
monaco: false
colorSchema: dark
fonts:
  sans: 'Inter, system-ui, sans-serif'
  mono: 'JetBrains Mono, monospace'
highlighter: shiki
lineNumbers: false
routerMode: hash
---

<style>
:root {
  --slidev-theme-background: #0B1120;
}
.slidev-layout {
  background: #0B1120 !important;
  color: #E2E8F0;
}
.slidev-layout h1 {
  color: #F0F6FF;
  font-weight: 700;
  font-size: 2rem;
  line-height: 1.2;
  margin-bottom: 0.3rem;
}
.slidev-layout h2 {
  color: #F59E0B;
  font-weight: 600;
  font-size: 1.3rem;
  line-height: 1.3;
}
.slidev-layout p, .slidev-layout li {
  color: #CBD5E1;
  font-size: 0.95rem;
  line-height: 1.45;
}
.slidev-layout li strong { color: #F0F6FF; }
.slidev-layout code { background: #1E293B; color: #7DD3FC; font-size: 0.85em; }
.green { color: #34D399; }
.red { color: #F87171; }
.amber { color: #FBBF24; }
.gray { color: #94A3B8; }
.white { color: #F8FAFC; }
.small { font-size: 0.8rem; }
.xs { font-size: 0.7rem; }
.badge-green { background: #065F46; color: #6EE7B7; padding: 2px 10px; border-radius: 6px; font-size: 0.8rem; }
.badge-red { background: #7F1D1D; color: #FCA5A5; padding: 2px 10px; border-radius: 6px; font-size: 0.8rem; }
.badge-amber { background: #78350F; color: #FCD34D; padding: 2px 10px; border-radius: 6px; font-size: 0.8rem; }
.page-num { position: absolute; bottom: 10px; right: 20px; font-size: 0.7rem; color: #475569; }
/* Image/video containers - fill available space, auto-scale content */
.media-box {
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  min-height: 0;
}
.media-box img, .media-box video {
  max-width: 100%;
  max-height: 68vh;
  width: auto;
  height: auto;
  object-fit: contain;
  border-radius: 8px;
}
.media-box.tall img, .media-box.tall video { max-height: 62vh; }
.media-box.short img, .media-box.short video { max-height: 40vh; }
.media-box.wide img, .media-box.wide video { max-width: 95%; max-height: 68vh; }
</style>

---
layout: cover
---

# ИИ в работе

## Прогресс LLM, личный опыт и как не наступить на грабли

<div class="pt-8">
  <span class="badge-amber">Внутренний митап департамента ИТ</span>
</div>

<div class="pt-4 text-sm opacity-40">Евгений Эрман, ДК РАЗУМ · 2026</div>
<div class="page-num">1</div>

---
layout: default
---

<div class="page-num">2</div>

# Прогресс: тогда и сейчас

<div class="media-box tall" style="padding-top: 4px;">
  <video src="/CMAF_480.mp4" controls></video>
</div>

<div class="text-center pt-1"><span class="amber" style="font-size: 1rem; font-weight: 600;">От «не могу» к «сделал, проверяй» — за 12 месяцев.</span></div>

---
layout: default
---

<div class="page-num">3</div>

# Что случилось за год: ключевые вехи

<div class="grid grid-cols-2 gap-3 pt-2">

<v-click>
<div class="p-2 rounded" style="background: #1E293B;">
  <h3 style="font-size: 1.05rem;">Модели научились «думать»</h3>
  <p class="small opacity-70">Claude 4, GPT-5, DeepSeek R1/R2 — reasoning из коробки. Gemini 2.5 Pro — контекст в 1 млн токенов.</p>
</div>
</v-click>

<v-click>
<div class="p-2 rounded" style="background: #1E293B;">
  <h3 style="font-size: 1.05rem;">Агенты в продакшене</h3>
  <p class="small opacity-70">Codex CLI, Claude Code, Grok Bot — работают с файлами и Git в терминале.</p>
</div>
</v-click>

<v-click>
<div class="p-2 rounded" style="background: #1E293B;">
  <h3 style="font-size: 1.05rem;">MCP стал стандартом</h3>
  <p class="small opacity-70">Любой продукт → MCP-сервер → доступен любому агенту. USB для ИИ.</p>
</div>
</v-click>

</div>

<div class="pt-4 text-center text-sm opacity-40">
  Главный итог: задачи, которые год назад требовали человека, сегодня решаются автономно.
</div>

---
layout: two-cols
---

<div class="page-num">4</div>

# Как ИИ меняет работу

<v-click>
<div class="mb-3">
  <h2 style="font-size: 1.15rem;">Презентации на GitHub + бот</h2>
  <p class="small">Слайды = markdown в репозитории. «Добавь график» → бот коммитит → слайд обновлён.</p>
  <p class="xs opacity-40">Эта презентация именно так и сделана.</p>
</div>
</v-click>

<v-click>
<div class="mb-3">
  <h2 style="font-size: 1.15rem;">Код, доки, отчёты</h2>
  <p class="small">ИИ — черновик, человек — редактор. <span class="green">Экономия 60–80% времени.</span></p>
</div>
</v-click>

<v-click>
<div>
  <h2 style="font-size: 1.15rem;">Единая точка входа</h2>
  <p class="small">Почта, календарь, задачи, вики, диск — через один чат с агентом.</p>
</div>
</v-click>

::right::

<div class="pl-4 pt-12">

<v-click>
<div class="p-4 rounded" style="background: #1E293B;">
  <h3 class="amber mb-2">Смена парадигмы</h3>
  <p class="amber" style="font-size: 1.1rem; font-weight: 600;">«Человек делает» → «Человек ставит задачу и проверяет»</p>
  <p class="small opacity-50 mt-2">Исчезает рутина переключения между 10 интерфейсами.</p>
</div>
</v-click>

</div>

---
layout: default
---

<div class="page-num">5</div>

# MCP: почему их стало так много

<div class="pt-1">

<div class="mb-3">
  <h2 style="font-size: 1.2rem;">MCP = Model Context Protocol</h2>
  <p class="amber">Открытый стандарт (Anthropic). Как USB для ИИ: один разъём — любое устройство.</p>
</div>

<v-click>
<div class="mb-3">
  <h2 style="font-size: 1.15rem;">Почему взрывной рост</h2>
  <ul class="small">
    <li>Любой продукт → MCP-сервер за <strong>1 день</strong></li>
    <li>Одна интеграция = доступ из любого агента</li>
    <li>Больше не нужны плагины под каждого ассистента</li>
  </ul>
</div>
</v-click>

<v-click>
<div class="p-3 rounded-lg" style="background: #0F2B1A;">
  <h2 style="font-size: 1.15rem;" class="green mb-2">У нас в РАЗУМ уже подключено к ИИ-помощнику:</h2>
  <div class="grid grid-cols-3 gap-1 small">
    <span>Яндекс.Почта</span><span>Яндекс.Календарь</span><span>Яндекс.Диск</span>
    <span>Яндекс.Вики</span><span>Яндекс.Телемост</span><span>Kaiten</span>
    <span>ELMA</span><span>Справочник</span><span>Фотобанк</span>
  </div>
  <p class="amber small mt-2">Один протокол, один чат, все системы.</p>
</div>
</v-click>

</div>

---
layout: two-cols
---

<div class="page-num">6</div>

# Чат-боты vs Агенты

<div class="pr-4">

<v-click>
<div class="mb-5">
  <span class="badge-red">Чат-бот</span>
  <ul class="small pt-1">
    <li>«Спросил — ответил»</li>
    <li>Нет действий в системах</li>
    <li>Нет памяти между сессиями</li>
    <li>Нет инструментов</li>
  </ul>
  <p class="xs opacity-40 mt-1">«Найди письма» → список писем</p>
</div>
</v-click>

</div>

::right::

<div class="pl-4">

<v-click>
<div class="mb-5">
  <span class="badge-green">Агент</span>
  <ul class="small pt-1">
    <li>Принимает решения</li>
    <li>Вызывает инструменты</li>
    <li>Делает цепочки действий</li>
    <li>Контекст и состояние</li>
  </ul>
  <p class="xs opacity-40 mt-1">«Собери повестку» → обошёл почту, календарь, Kaiten, смержил</p>
</div>
</v-click>

<v-click>
<div class="pt-4 pl-2">
  <div class="amber" style="font-size: 1.1rem; font-weight: 600;">Разница не в intelligence, а в architecture.</div>
  <p class="small opacity-50">Чат-бот отвечает на вопрос. Агент решает задачу.</p>
</div>
</v-click>

</div>

---
layout: default
---

<div class="page-num">7</div>

# 6 уровней агентной архитектуры

<div class="media-box tall" style="padding-top: 4px;">
  <img src="/architecture-layers.png" alt="6 уровней агентной архитектуры">
</div>

<div class="pt-1 text-xs opacity-40 text-center">Фреймворк решает задачи одного уровня — и не помогает на следующем. Выбирайте под уровень.</div>

---
layout: default
---

<div class="page-num">8</div>

# Как встроить ИИ в процесс

<div class="pt-2">

## <span class="amber">Три столпа</span> (по Automatica)

<div class="grid grid-cols-3 gap-3 pt-3">

<v-click>
<div class="text-center p-3 rounded" style="background: #1E293B;">
  <div style="font-size: 1.5rem;">📋</div>
  <h3 class="mt-1" style="font-size: 1rem;">Источник истины</h3>
  <p class="small opacity-70">Задачи хранятся независимо от сессий. Цели, бюджет, риск, доказательства.</p>
</div>
</v-click>

<v-click>
<div class="text-center p-3 rounded" style="background: #1E293B;">
  <div style="font-size: 1.5rem;">🌊</div>
  <h3 class="mt-1" style="font-size: 1rem;">Управление потоком</h3>
  <p class="small opacity-70">Планировщик выдаёт только задачи без блокирующих зависимостей.</p>
</div>
</v-click>

<v-click>
<div class="text-center p-3 rounded" style="background: #1E293B;">
  <div style="font-size: 1.5rem;">✅</div>
  <h3 class="mt-1" style="font-size: 1rem;">Контроль качества</h3>
  <p class="small opacity-70">Done — после проверки. <strong>Выносит тот, кто не делал работу.</strong></p>
</div>
</v-click>

</div>

<v-click>
<div class="pt-5 text-center">
  <p class="amber" style="font-size: 1.1rem; font-weight: 600;">Состояние и правила — в одном месте. Рассуждать и выполнять — где угодно.</p>
  <p class="small opacity-50 mt-1">Человек управляет целями. Агент — исполняет.</p>
</div>
</v-click>

</div>

---
layout: default
---

<div class="page-num">9</div>

# Контракт задачи

<div class="grid grid-cols-2 gap-5 pt-1">

<div>

## <span class="green">Что указывать явно</span>

<div class="small space-y-0.5 pt-1">

<v-click>

- **Желаемый результат** — ЧТО сделать, а не КАК
- **Критерии приёмки** — тесты, схема, снимки экрана
- **Зависимости** — что должно быть готово до старта
- **Уровень риска** → песочница и правила подтверждения
- **Бюджет** — деньги, время, число попыток
- **Доказательства** — артефакты с неизменяемыми хешами

</v-click>

</div>

</div>

<div>

## <span class="red">Что не использовать</span>

<div class="small space-y-1.5 pt-1">

<v-click>

<p>❌ <strong>История чата</strong> — изменчива и непроверяема</p>
</v-click>
<v-click>
<p>❌ <strong>Ссылка на PR</strong> — не говорит, что именно проверять</p>
</v-click>
<v-click>
<p>❌ <strong>«Продолжай, пока не идеально»</strong> — нет критерия остановки</p>
</v-click>
<v-click>
<p>❌ <strong>«Измени эти три файла»</strong> — навязывает решение вместо результата</p>
</v-click>

</div>

</div>

</div>

---
layout: default
---

<div class="page-num">10</div>

# За чем следить: ИИ ошибается — и дорого

<div class="media-box short" style="gap: 12px;">
  <img src="/photo_2026-09-08_19-55-20.jpg" alt="Пример ошибки ИИ 1" style="border-radius: 8px;">
  <img src="/photo_2026-09-08_19-55-20_1.jpg" alt="Пример ошибки ИИ 2" style="border-radius: 8px;">
</div>

<div class="grid grid-cols-2 gap-2 pt-2">

<v-click>
<div class="p-2 rounded" style="background: #2D1B1B;">
  <p class="small"><span class="red">📎 «Я удалил лишнее»</span> — агент «оптимизировал» код и удалил продакшен-базу. Done.</p>
</div>
</v-click>

<v-click>
<div class="p-2 rounded" style="background: #2D1B1B;">
  <p class="small"><span class="red">🔄 47 итераций «рефакторинга»</span> — версия 47 = версия 1 с другим именем переменной.</p>
</div>
</v-click>

<v-click>
<div class="p-2 rounded" style="background: #2D1B1B;">
  <p class="small"><span class="red">🎭 Убедительная ложь</span> — «Я проверил — всё работает». Тесты не проходят, сервер не запускается.</p>
</div>
</v-click>

<v-click>
<div class="p-2 rounded" style="background: #2D1B1B;">
  <p class="small"><span class="red">💸 Без бюджета = без тормозов</span> — агент без лимита попыток = дыра в кошельке.</p>
</div>
</v-click>

</div>

<div class="pt-1 text-center"><span class="amber" style="font-weight: 600;">Модели ошибаются. Архитектура — то, что держит систему.</span></div>

---
layout: default
---

<div class="page-num">11</div>

# Победы vs Провалы

<div class="media-box wide" style="padding-top: 2px;">
  <img src="/wins-vs-fails.png" alt="AI wins vs fails comparison">
</div>

---
layout: default
---

<div class="page-num">12</div>

# Провалы: таксономия MAST

<div class="xs opacity-40 pt-1">Исследование: 5 систем · 150+ задач · 14 видов сбоев</div>

<div class="grid grid-cols-3 gap-3 pt-2">

<v-click>
<div class="p-2 rounded" style="background: #1E293B;">
  <h3 class="red" style="font-size: 1rem;">1. Постановка задачи</h3>
  <ul class="xs pt-1 space-y-0.5">
    <li>Неверное разбиение</li>
    <li>Не заданы ограничения</li>
    <li>Контекст ≠ инструменты</li>
    <li>Плохие роли</li>
  </ul>
</div>
</v-click>

<v-click>
<div class="p-2 rounded" style="background: #1E293B;">
  <h3 class="red" style="font-size: 1rem;">2. Рассогласованность</h3>
  <ul class="xs pt-1 space-y-0.5">
    <li>Дублирование работы</li>
    <li>Игнор сведений</li>
    <li>Допущения молча</li>
    <li>Недоверенные данные</li>
  </ul>
</div>
</v-click>

<v-click>
<div class="p-2 rounded" style="background: #1E293B;">
  <h3 class="red" style="font-size: 1rem;">3. Проверка</h3>
  <ul class="xs pt-1 space-y-0.5">
    <li>Done раньше времени</li>
    <li>Результат не проверен</li>
    <li>Бесконечные повторы</li>
    <li>Итог = убедительность</li>
  </ul>
</div>
</v-click>

</div>

<v-click>
<div class="pt-4 text-center">
  <h3 class="amber mb-1" style="font-size: 1rem;">Системные меры</h3>
  <p class="small">Пакеты задач + состояние + временные права + независимая проверка + лимит повторов</p>
</div>
</v-click>

---
layout: default
---

<div class="page-num">13</div>

# Цикл агента

<div class="media-box tall" style="padding-top: 4px;">
  <img src="/agent-loop.png" alt="Agent Loop: Observe → Reason → Act → Verify">
</div>

<div class="pt-2 text-center small opacity-50">Каждый цикл: наблюдает среду → рассуждает → действует через инструменты → проверяет результат</div>

---
layout: default
---

<div class="page-num">14</div>

# Главные принципы

<div class="pt-4 space-y-2">

<v-click>
<div class="flex items-start gap-2 p-2.5 rounded" style="background: #1E293B;">
  <span class="amber" style="font-size: 1rem;">▸</span>
  <p class="small">Состояние задач и правила — в одном месте. Рассуждать и выполнять — где угодно.</p>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-2 p-2.5 rounded" style="background: #1E293B;">
  <span class="green" style="font-size: 1rem;">▸</span>
  <p class="small">Done выносит тот, кто не делал работу.</p>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-2 p-2.5 rounded" style="background: #1E293B;">
  <span class="amber" style="font-size: 1rem;">▸</span>
  <p class="small">Больше агентов ≠ лучше. Смысл есть, если работу можно разделить.</p>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-2 p-2.5 rounded" style="background: #1E293B;">
  <span class="green" style="font-size: 1rem;">▸</span>
  <p class="small">Не история чата, а контракт задачи — интерфейс с системой.</p>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-2 p-2.5 rounded" style="background: #1E293B;">
  <span class="amber" style="font-size: 1rem;">▸</span>
  <p class="small">Человек управляет целями и правилами. Агент — исполняет.</p>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-2 p-2.5 rounded" style="background: #1E293B;">
  <span class="green" style="font-size: 1rem;">▸</span>
  <p class="small">Модели ошибаются. Архитектура — то, что держит систему.</p>
</div>
</v-click>

</div>

---
layout: default
---

<div class="page-num">15</div>

# Что дальше? Прогноз на год

<div class="grid grid-cols-2 gap-4 pt-3">

<v-click>
<div class="p-3 rounded" style="background: #1E293B;">
  <h3 style="font-size: 1.1rem;">Агенты — как email</h3>
  <p class="small opacity-70">У каждого сотрудника — агент-ассистент для рутины.</p>
</div>
</v-click>

<v-click>
<div class="p-3 rounded" style="background: #1E293B;">
  <h3 style="font-size: 1.1rem;">Мультиагентные системы</h3>
  <p class="small opacity-70">Парки агентов: Plan / Build / Verify / Ops.</p>
</div>
</v-click>

<v-click>
<div class="p-3 rounded" style="background: #1E293B;">
  <h3 style="font-size: 1.1rem;">ИИ-нативный софт</h3>
  <p class="small opacity-70">Интерфейсы под агентов. MCP = REST API 2.0.</p>
</div>
</v-click>

<v-click>
<div class="p-3 rounded" style="background: #0F2B1A;">
  <h3 class="green" style="font-size: 1.1rem;">В РАЗУМ</h3>
  <p class="small opacity-70">От единичных агентов → к парку с контрактами и оркестрацией.</p>
  <p class="small green">«Спросил-ответил» → «Поставил задачу — получил результат с доказательствами».</p>
</div>
</v-click>

</div>

---
layout: center
class: text-center
---

<div class="page-num">16</div>

# Итоги

<div class="pt-5 space-y-2">

<v-click>
<p class="small">Модели за год: от «ответа на вопрос» до <span class="amber">автономного решения задач</span></p>
</v-click>

<v-click>
<p class="small">MCP делает интеграцию тривиальной — <span class="green">любой продукт = инструмент</span></p>
</v-click>

<v-click>
<p class="small">Агент ≠ чат-бот. <span class="amber">Агент действует, а не отвечает.</span></p>
</v-click>

<v-click>
<p class="small">Архитектура: <span class="green">контракт → оркестрация → проверка → приёмка</span></p>
</v-click>

<v-click>
<p style="font-size: 1.3rem; font-weight: 700;" class="amber pt-3">Главное — не модель, а процесс вокруг неё.</p>
</v-click>

</div>

<div class="pt-8">
  <v-click><span style="font-size: 2.5rem; font-weight: 700; color: #F8FAFC;">Вопросы?</span></v-click>
</div>

---
layout: end
---

<div class="page-num">17</div>

<div class="text-center">
  <div style="font-size: 1.5rem; font-weight: 700; color: #F59E0B;">Спасибо!</div>
  <div class="pt-4 text-sm opacity-50">ДК РАЗУМ · ИТ митап · 2026</div>
  <div class="pt-8 text-xs opacity-30">Слайды на Slidev — править можно прямо во время показа через бота.<br>github.com/namre/ai-in-work-mitap</div>
</div>
