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
  font-size: 2.4rem;
  line-height: 1.2;
}
.slidev-layout h2 {
  color: #F59E0B;
  font-weight: 600;
  font-size: 1.6rem;
}
.slidev-layout p, .slidev-layout li {
  color: #CBD5E1;
  font-size: 1.1rem;
  line-height: 1.6;
}
.slidev-layout li strong {
  color: #F0F6FF;
}
.slidev-layout code {
  background: #1E293B;
  color: #7DD3FC;
  font-size: 0.9em;
}
.slidev-layout .green { color: #34D399; }
.slidev-layout .red { color: #F87171; }
.slidev-layout .amber { color: #FBBF24; }
.slidev-layout .gray { color: #94A3B8; }
.slidev-layout .white { color: #F8FAFC; }
.slidev-layout .small { font-size: 0.85rem; }
.slidev-layout .col-left { text-align: left; }
.slidev-layout .badge-green {
  background: #065F46;
  color: #6EE7B7;
  padding: 2px 10px;
  border-radius: 6px;
  font-size: 0.85rem;
}
.slidev-layout .badge-red {
  background: #7F1D1D;
  color: #FCA5A5;
  padding: 2px 10px;
  border-radius: 6px;
  font-size: 0.85rem;
}
.slidev-layout .badge-amber {
  background: #78350F;
  color: #FCD34D;
  padding: 2px 10px;
  border-radius: 6px;
  font-size: 0.85rem;
}
</style>

---
layout: cover
---

# ИИ в работе

## Год прогресса, личный опыт и как не наступить на грабли

<div class="pt-12">
  <span class="badge-amber">Внутренний митап департамента ИТ</span>
</div>

<div class="pt-4 text-sm opacity-50">
  ДК РАЗУМ · 2026
</div>

<!--
Приветствие. Формат: 20 минут + вопросы. Цель — не лекция, а обмен опытом: что реально работает, где больно, чему научились за год.
-->

---
layout: two-cols
---

# Что случилось за год

<div class="pt-2">

**Модели научились «думать»**

- Весна 2025: Claude 4, GPT-5, DeepSeek R1/R2 — reasoning из коробки
- Gemini 2.5 Pro — контекст в 1 млн токенов + reasoning

**Агенты стали production-ready**

- Codex CLI, Claude Code, Grok Bot — ИИ работает в терминале с Git
- <span class="amber">Symphony (OpenAI): +500% PR в некоторых командах за 3 недели</span>

</div>

::right::

<div class="pl-4 pt-18">

<v-click>

### Главный тренд

Задачи, которые год назад требовали человека, сегодня решаются автономно.

</v-click>

<v-click>

<div class="pt-6 text-sm opacity-50">
Год назад: эксперименты<br>
Сегодня: агенты пишут код, проверяют задачи, собирают повестки.
</div>

</v-click>

</div>

<!--
Контекст: год назад мы только начинали. Сегодня агенты пишут код, проверяют задачи, собирают повестки. Цифры Symphony — внутренний отчёт OpenAI, не универсальный бенчмарк, но показательно.
-->

---
layout: default
---

# Исследования: что говорят цифры

<div class="grid grid-cols-2 gap-4 pt-2">

<div>
  <div class="badge-green mb-2">Параллельные задачи</div>
  <div class="green" style="font-size: 2rem; font-weight: 700;">+80.9%</div>
  <div class="text-sm opacity-60 mb-4">против одного агента — Google Research, 180 конфигураций</div>

  <div class="badge-red mb-2">Последовательное планирование</div>
  <div class="red" style="font-size: 2rem; font-weight: 700;">−39…−70%</div>
  <div class="text-sm opacity-60 mb-4">PlanCraft: агенты проигрывают одиночке на зависимых шагах</div>
</div>

<div>
  <div class="badge-red mb-2">Рост ошибок</div>
  <div class="red" style="font-size: 2rem; font-weight: 700;">до 17.2×</div>
  <div class="text-sm opacity-60 mb-2">У независимых агентов</div>
  <div class="green" style="font-size: 1.5rem; font-weight: 600;">→ 4.4×</div>
  <div class="text-sm opacity-60 mb-4">С централизованной оркестрацией</div>

  <div class="badge-amber mt-4">Расход токенов парка агентов: 15×</div>
  <div class="text-sm opacity-60">против чата, но прирост результата +90.2%</div>
</div>

</div>

<div class="pt-4 text-center amber" style="font-size: 1.3rem; font-weight: 600;">
  Больше агентов ≠ лучше. Смысл есть, только если работу можно разделить.
</div>

<div class="pt-2 text-xs opacity-30 text-center">
  Источники: Google Research (2026), Anthropic Engineering (2025). Показатели из разных исследований — не единый бенчмарк.
</div>

<!--
Важно: цифры нельзя сводить в единый бенчмарк — они из разных исследований. Но тренд ясен: мультиагентность окупается на параллельных задачах и вредит на последовательных.
-->

---
layout: default
---

# Как ИИ меняет работу

<div class="grid grid-cols-2 gap-6 pt-4">

<v-click>
<div>
  <h2 style="font-size: 1.3rem;">Презентации на GitHub + бот</h2>
  <p>Слайды = markdown в репозитории. Прямо во время показа: «добавь график» → бот коммитит → слайд обновлён.</p>
  <p class="text-sm opacity-50">Эта презентация именно так и сделана. Сейчас ты смотришь живые слайды, которые можно править на лету.</p>
</div>
</v-click>

<v-click>
<div>
  <h2 style="font-size: 1.3rem;">Код-ревью, доки, отчёты</h2>
  <p>ИИ делает черновик, человек — редактор.</p>
  <p class="green">Экономия: 60–80% времени на подготовку.</p>
</div>
</v-click>

<v-click>
<div>
  <h2 style="font-size: 1.3rem;">Единая точка входа</h2>
  <p>Агент работает с почтой, календарём, задачами, вики, диском — через один чат.</p>
</div>
</v-click>

<v-click>
<div>
  <h2 style="font-size: 1.3rem;" class="amber">Парадигма</h2>
  <p class="amber" style="font-size: 1.2rem; font-weight: 600;">
    «Человек делает» → «Человек ставит задачу и проверяет»
  </p>
</div>
</v-click>

</div>

<!--
Пример из жизни: раньше собрать повестку на день = открыть почту, календарь, Kaiten, ELMA. Теперь — одно сообщение агенту.
-->

---
layout: default
---

# MCP: почему их стало так много

<div class="pt-4">

<div class="mb-6">
  <h2 style="font-size: 1.4rem;">MCP = Model Context Protocol</h2>
  <p class="amber">Открытый стандарт (Anthropic). Как USB для ИИ: один разъём — любое устройство.</p>
</div>

<v-click>
<div class="mb-5">
  <h2 style="font-size: 1.3rem;">Почему взрывной рост</h2>
  <ul>
    <li>Любой продукт может дать MCP-сервер за <strong>1 день</strong></li>
    <li>Одна интеграция = доступ из любого агента</li>
    <li>Больше не нужны отдельные плагины под каждого ассистента</li>
  </ul>
</div>
</v-click>

<v-click>
<div class="p-4 rounded-lg" style="background: #0F2B1A;">
  <h2 style="font-size: 1.3rem;" class="green mb-2">У нас в РАЗУМ уже подключено:</h2>
  <div class="grid grid-cols-2 gap-2 text-sm">
    <span>Яндекс.Почта</span><span>Яндекс.Календарь</span>
    <span>Яндекс.Диск</span><span>Яндекс.Вики</span>
    <span>Яндекс.Телемост</span><span>Kaiten</span>
    <span>ELMA</span><span>Справочник сотрудников</span>
    <span>Фотобанк РАЗУМ</span>
  </div>
  <p class="amber text-sm mt-2">Всё доступно агенту единообразно — один протокол, один чат.</p>
</div>
</v-click>

</div>

---
layout: two-cols
---

# Чат-боты vs Агенты

<div class="pr-4">

<v-click>
<div class="mb-6">
  <span class="badge-red">Чат-бот</span>
  <ul class="pt-2">
    <li>«Спросил — ответил»</li>
    <li>Без действий в системах</li>
    <li>Нет памяти между сессиями</li>
    <li>Нет инструментов</li>
  </ul>
  <p class="text-sm opacity-50 mt-2">«Найди письма от Ивана» = выдал список</p>
</div>
</v-click>

</div>

::right::

<v-click>
<div class="pl-4">
  <span class="badge-green">Агент</span>
  <ul class="pt-2">
    <li>Принимает решения</li>
    <li>Вызывает инструменты</li>
    <li>Делает цепочки действий</li>
    <li>Контекст и состояние</li>
  </ul>
  <p class="text-sm opacity-50 mt-2">«Собери повестку на завтра» = обошёл почту, календарь, Kaiten, смержил, показал</p>
</div>
</v-click>

<v-click>
<div class="pt-6">
  <div class="amber" style="font-size: 1.2rem; font-weight: 600;">
    Разница не в intelligence, а в architecture.
  </div>
  <p class="text-sm opacity-60">Чат-бот отвечает на вопрос. Агент решает задачу.</p>
</div>
</v-click>

---
layout: default
---

# 4 топологии управления агентами

<div class="grid grid-cols-2 gap-4 pt-4">

<v-click>
<div class="p-3 rounded" style="background: #1E293B;">
  <h3>1. Жёсткое управление</h3>
  <p class="text-sm">Manager → Tools. Один агент вызывает специалистов как инструменты.</p>
  <p class="text-xs"><span class="green">✅ Одна связная работа</span> &nbsp; <span class="red">❌ Бутылочное горлышко</span></p>
</div>
</v-click>

<v-click>
<div class="p-3 rounded" style="background: #1E293B;">
  <h3>2. Локальная автономия</h3>
  <p class="text-sm">Чат агентов. Равноправные, передают управление, общаются напрямую.</p>
  <p class="text-xs"><span class="green">✅ Разбор в диалоге</span> &nbsp; <span class="red">❌ Нет единого источника истины</span></p>
</div>
</v-click>

<v-click>
<div class="p-3 rounded" style="background: #1E293B;">
  <h3>3. Явное состояние</h3>
  <p class="text-sm">Граф состояний. Plan → Act → Verify, с сохраняемым состоянием.</p>
  <p class="text-xs"><span class="green">✅ Один сложный запуск</span> &nbsp; <span class="red">❌ Граф ≠ общий бэклог</span></p>
</div>
</v-click>

<v-click>
<div class="p-3 rounded" style="background: #1E293B;">
  <h3>4. Масштаб парка <span class="badge-green" style="font-size: 0.7rem;">production</span></h3>
  <p class="text-sm">Реестр задач. Задачи со статусами, исполнители берут и возвращают доказательства.</p>
  <p class="text-xs"><span class="green">✅ Множество асинхронных работ</span> &nbsp; <span class="red">❌ Сложность эксплуатации</span></p>
</div>
</v-click>

</div>

<div class="pt-4 text-center text-xs opacity-40">
  Источник: Automatica · «Операционные системы для 1,000 ИИ-агентов»
</div>

---
layout: default
---

# 6 уровней агентной архитектуры

<div class="pt-4">

<div class="space-y-2">

<div class="flex items-center gap-3 p-2 rounded" style="background: #1E293B;">
  <span style="font-size: 1.5rem;">🏢</span>
  <div><strong>1. Рабочая ОС</strong> <span class="text-sm opacity-50">— Портфель результатов, SLA, очереди исключений. Linear / Jira / консоль.</span></div>
</div>

<div class="flex items-center gap-3 p-2 rounded" style="background: #1E293B;">
  <span style="font-size: 1.5rem;">🎛️</span>
  <div><strong>2. Контур управления</strong> <span class="text-sm opacity-50">— Состояние задач, политики, бюджеты, аудит. Аналог Symphony.</span></div>
</div>

<div class="flex items-center gap-3 p-2 rounded" style="background: #1E293B;">
  <span style="font-size: 1.5rem;">⚙️</span>
  <div><strong>3. Оркестратор</strong> <span class="text-sm opacity-50">— Зависимости, маршрутизация, повторы, регулирование нагрузки.</span></div>
</div>

<div class="flex items-center gap-3 p-2 rounded" style="background: #1E293B;">
  <span style="font-size: 1.5rem;">📦</span>
  <div><strong>4. Среда агента</strong> <span class="text-sm opacity-50">— Контекст, инструменты, песочница. Codex / Claude Code.</span></div>
</div>

<div class="flex items-center gap-3 p-2 rounded" style="background: #1E293B;">
  <span style="font-size: 1.5rem;">🔄</span>
  <div><strong>5. Цикл агента</strong> <span class="text-sm opacity-50">— Наблюдать → Рассуждать → Действовать → Оценивать</span></div>
</div>

<div class="flex items-center gap-3 p-2 rounded" style="background: #1E293B;">
  <span style="font-size: 1.5rem;">🧠</span>
  <div><strong>6. Модель</strong> <span class="text-sm opacity-50">— Инференс, выбор инструментов, планирование. GPT / Claude / Gemini.</span></div>
</div>

</div>

</div>

<div class="pt-3 text-xs opacity-40 text-center">
  Фреймворк может решать задачи одного уровня и не помогать на следующем. Выбирайте инструмент под уровень.
</div>

---
layout: default
---

# Как встроить ИИ в процесс

<div class="pt-4">

## <span class="amber">Три столпа</span> (по Automatica)

<div class="grid grid-cols-3 gap-4 pt-4">

<v-click>
<div class="text-center p-4 rounded" style="background: #1E293B;">
  <div style="font-size: 2rem;">📋</div>
  <h3 class="mt-2" style="font-size: 1.1rem;">Источник истины</h3>
  <p class="text-sm opacity-70">Задачи хранятся независимо от сессий агента. Цели, зависимости, бюджет, риск, доказательства.</p>
</div>
</v-click>

<v-click>
<div class="text-center p-4 rounded" style="background: #1E293B;">
  <div style="font-size: 2rem;">🌊</div>
  <h3 class="mt-2" style="font-size: 1.1rem;">Управление потоком</h3>
  <p class="text-sm opacity-70">Асинхронный планировщик выдаёт только задачи без блокирующих зависимостей.</p>
</div>
</v-click>

<v-click>
<div class="text-center p-4 rounded" style="background: #1E293B;">
  <div style="font-size: 2rem;">✅</div>
  <h3 class="mt-2" style="font-size: 1.1rem;">Контроль качества</h3>
  <p class="text-sm opacity-70">Done — только после проверки. И выносит его <strong>тот, кто не делал работу</strong>.</p>
</div>
</v-click>

</div>

<v-click>
<div class="pt-6 text-center">
  <p class="amber" style="font-size: 1.2rem; font-weight: 600;">
    Состояние задач и правила — в одном месте.<br>Рассуждать и выполнять — где угодно.
  </p>
  <p class="text-sm opacity-50 mt-2">Человек управляет целями и правилами. Агент — исполняет.</p>
</div>
</v-click>

</div>

---
layout: default
---

# Контракт задачи

<div class="grid grid-cols-2 gap-6 pt-2">

<div>

## <span class="green">Что указывать явно</span>

<div class="text-sm space-y-1 pt-2">

<v-click>

- **Желаемый результат** — ЧТО сделать, а не КАК
- **Критерии приёмки** — тесты, схема, контрольные итоги, снимки экрана
- **Зависимости** — какие задачи должны закрыться до старта
- **Уровень риска** → выбор песочницы и правил подтверждения
- **Бюджет** — деньги, время, число попыток
- **Доказательства** — артефакты с неизменяемыми хешами

</v-click>

</div>

</div>

<div>

## <span class="red">Что не использовать</span>

<div class="text-sm space-y-2 pt-2">

<v-click>

<p>❌ <strong>История чата</strong> — изменчива и непроверяема</p>

</v-click>
<v-click>

<p>❌ <strong>Ссылка на PR</strong> — не говорит, что именно должно пройти проверку</p>

</v-click>
<v-click>

<p>❌ <strong>«Продолжай, пока не будет идеально»</strong> — нет критерия остановки, нет предела расходов</p>

</v-click>
<v-click>

<p>❌ <strong>«Измени эти три файла»</strong> — навязывает агенту решение вместо результата</p>

</v-click>

</div>

</div>

</div>

---
layout: default
---

# План внедрения: первые 90 дней

<div class="pt-4">

<div class="space-y-3">

<v-click>
<div class="flex items-start gap-4 p-3 rounded" style="background: #1E293B;">
  <div class="amber" style="font-size: 2rem; font-weight: 700; min-width: 3rem;">01</div>
  <div>
    <h3>Недели 1–2: Контракт</h3>
    <p class="text-sm opacity-70">Схема задачи, граф состояний, правила выполнения, контрольные наборы для оценок.</p>
  </div>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-4 p-3 rounded" style="background: #1E293B;">
  <div class="amber" style="font-size: 2rem; font-weight: 700; min-width: 3rem;">02</div>
  <div>
    <h3>Недели 3–5: Два исполнителя</h3>
    <p class="text-sm opacity-70">API-агент + CLI-агент, независимый проверяющий, атомарные временные права.</p>
  </div>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-4 p-3 rounded" style="background: #1E293B;">
  <div class="amber" style="font-size: 2rem; font-weight: 700; min-width: 3rem;">03</div>
  <div>
    <h3>Недели 6–8: Возобновляемость</h3>
    <p class="text-sm opacity-70">Возобновляемый процесс, идемпотентный шлюз, подтверждения, аудит.</p>
  </div>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-4 p-3 rounded" style="background: #1E293B;">
  <div class="amber" style="font-size: 2rem; font-weight: 700; min-width: 3rem;">04</div>
  <div>
    <h3>Недели 9–12: Парк агентов</h3>
    <p class="text-sm opacity-70">Очереди по ролям, квоты, авто-масштабирование, панели SLO, kill switch.</p>
  </div>
</div>
</v-click>

</div>

<v-click>
<div class="pt-4 text-center">
  <span class="green" style="font-size: 1.1rem; font-weight: 600;">
    1 задача → 1 источник истины → 1 исполнитель → 1 пакет доказательств → 1 принятый результат
  </span>
</div>
</v-click>

</div>

---
layout: default
---

# Провалы: таксономия сбоев MAST

<div class="text-xs opacity-50 pt-2">
  Исследование: 5 систем · 150+ задач · 14 видов сбоев · экспертная разметка
</div>

<div class="grid grid-cols-3 gap-4 pt-3">

<v-click>
<div class="p-3 rounded" style="background: #1E293B;">
  <h3 class="red" style="font-size: 1.1rem;">1. Постановка задачи</h3>
  <ul class="text-sm pt-1 space-y-1">
    <li>Неверное разбиение на подзадачи</li>
    <li>Не заданы ограничения</li>
    <li>Контекст не соответствует инструментам</li>
    <li>Плохо распределены роли</li>
  </ul>
</div>
</v-click>

<v-click>
<div class="p-3 rounded" style="background: #1E293B;">
  <h3 class="red" style="font-size: 1.1rem;">2. Рассогласованность</h3>
  <ul class="text-sm pt-1 space-y-1">
    <li>Дублирование работы</li>
    <li>Игнорирование нужных сведений</li>
    <li>Допущения без коммуникации</li>
    <li>Недоверенные данные = достоверные</li>
  </ul>
</div>
</v-click>

<v-click>
<div class="p-3 rounded" style="background: #1E293B;">
  <h3 class="red" style="font-size: 1.1rem;">3. Проверка</h3>
  <ul class="text-sm pt-1 space-y-1">
    <li>Done раньше времени</li>
    <li>Никто не проверяет результат</li>
    <li>Повторы без ограничения</li>
    <li>Итог = убедительность, не верность</li>
  </ul>
</div>
</v-click>

</div>

<v-click>
<div class="pt-5 text-center">
  <h3 class="amber mb-2" style="font-size: 1.2rem;">Системные меры</h3>
  <p class="text-sm">
    Типизированные пакеты задач + достоверное состояние + временные права +
    независимая проверка + ограниченные повторы
  </p>
</div>
</v-click>

---
layout: default
---

# Личный опыт: успехи

<div class="grid grid-cols-2 gap-6 pt-4">

<div>
<v-click>
<div class="p-4 rounded" style="background: #0F2B1A;">
  <h3 class="green mb-3" style="font-size: 1.2rem;">[ВАША ИСТОРИЯ 1]</h3>
  <p class="text-sm opacity-50">Что автоматизировали, какой результат, цифры если есть.</p>
  <div class="mt-3 pt-3" style="border-top: 1px solid #065F46;">
    <p class="text-xs opacity-70">Примеры для вдохновения:</p>
    <ul class="text-xs opacity-50 space-y-1 mt-1">
      <li>Автоматизация ежедневных планёрок</li>
      <li>Дайджест почты за утро</li>
      <li>Работа с задачами через агента вместо Kaiten UI</li>
      <li>Подготовка материалов к встречам</li>
    </ul>
  </div>
</div>
</v-click>
</div>

<div>
<v-click>
<div class="p-4 rounded" style="background: #0F2B1A;">
  <h3 class="green mb-3" style="font-size: 1.2rem;">[ВАША ИСТОРИЯ 2]</h3>
  <p class="text-sm opacity-50">Второй кейс успешного применения ИИ в работе.</p>
  <div class="mt-3 pt-3" style="border-top: 1px solid #065F46;">
    <p class="text-xs opacity-70" style="font-weight: 600;">Что уже работает в РАЗУМ:</p>
    <ul class="text-xs opacity-50 space-y-1 mt-1">
      <li>Агент планирует день — собирает повестку из почты, календаря, Kaiten, ELMA</li>
      <li>Корпоративные системы через единый интерфейс</li>
      <li>Автоматизация рутинных операций: поиск, сводки, материалы</li>
    </ul>
  </div>
</div>
</v-click>
</div>

</div>

<div class="pt-4 text-center text-sm opacity-40">
  ⚠️ Заполните своими реальными кейсами — без них формат «личных историй» не складывается.
</div>

---
layout: default
---

# Личный опыт: провалы и уроки

<div class="grid grid-cols-2 gap-6 pt-4">

<div>
<v-click>
<div class="p-4 rounded" style="background: #2D1B1B;">
  <h3 class="red mb-3" style="font-size: 1.2rem;">[ВАШ ПРОВАЛ 1]</h3>
  <p class="text-sm opacity-50">Что пошло не так, почему, какой урок вынесли.</p>
</div>
</v-click>
<v-click>
<div class="p-4 rounded mt-4" style="background: #2D1B1B;">
  <h3 class="red mb-3" style="font-size: 1.2rem;">[ВАШ ПРОВАЛ 2]</h3>
  <p class="text-sm opacity-50">Второй кейс — что сломалось и как починили.</p>
</div>
</v-click>
</div>

<div>
<v-click>
<div class="p-4 rounded" style="background: #1E293B;">
  <h3 class="amber mb-3" style="font-size: 1.2rem;">Универсальные уроки</h3>
  <ul class="text-sm space-y-2">
    <li>Не доверяйте агенту статусы без проверки — «ПРОСРОЧЕНО» в Kaiten на 70%+ ложное</li>
    <li>Один промпт ≠ production. Нужен контракт задачи с критериями приёмки.</li>
    <li>Агент без бюджета и лимита попыток = бесконечный цикл за ваши деньги.</li>
    <li>Модели ошибаются. Оркестрация сдерживает ошибки в 4× лучше.</li>
  </ul>
</div>
</v-click>
</div>

</div>

<div class="pt-4 text-center text-sm opacity-40">
  ⚠️ Заполните своими реальными кейсами.
</div>

---
layout: default
---

# Главные принципы

<div class="pt-6 space-y-4">

<v-click>
<div class="flex items-start gap-3 p-3 rounded" style="background: #1E293B;">
  <span class="amber" style="font-size: 1.3rem; min-width: 1.5rem;">▸</span>
  <p style="font-size: 1.15rem;">Состояние задач и правила — в одном месте. Рассуждать и выполнять — где угодно.</p>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-3 p-3 rounded" style="background: #1E293B;">
  <span class="green" style="font-size: 1.3rem; min-width: 1.5rem;">▸</span>
  <p style="font-size: 1.15rem;">Done выносит тот, кто не делал работу.</p>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-3 p-3 rounded" style="background: #1E293B;">
  <span class="amber" style="font-size: 1.3rem; min-width: 1.5rem;">▸</span>
  <p style="font-size: 1.15rem;">Больше агентов ≠ лучше. Смысл есть, только если работу можно разделить.</p>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-3 p-3 rounded" style="background: #1E293B;">
  <span class="green" style="font-size: 1.3rem; min-width: 1.5rem;">▸</span>
  <p style="font-size: 1.15rem;">Не история чата, а контракт задачи — интерфейс между агентом и системой.</p>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-3 p-3 rounded" style="background: #1E293B;">
  <span class="amber" style="font-size: 1.3rem; min-width: 1.5rem;">▸</span>
  <p style="font-size: 1.15rem;">Человек управляет целями, правилами и исключениями. Агент — исполняет.</p>
</div>
</v-click>

<v-click>
<div class="flex items-start gap-3 p-3 rounded" style="background: #1E293B;">
  <span class="green" style="font-size: 1.3rem; min-width: 1.5rem;">▸</span>
  <p style="font-size: 1.15rem;">Модели ошибаются. Архитектура (оркестрация, проверки, повторы) — то, что держит систему.</p>
</div>
</v-click>

</div>

---
layout: default
---

# Что дальше? Прогноз на год

<div class="grid grid-cols-2 gap-6 pt-4">

<v-click>
<div class="p-4 rounded" style="background: #1E293B;">
  <h3 style="font-size: 1.2rem;">Агенты станут нормой, как email</h3>
  <p class="text-sm opacity-70">У каждого сотрудника — свой агент-ассистент для рутины.</p>
</div>
</v-click>

<v-click>
<div class="p-4 rounded" style="background: #1E293B;">
  <h3 style="font-size: 1.2rem;">Мультиагентные системы</h3>
  <p class="text-sm opacity-70">Парки агентов с разделением ролей: Plan / Build / Verify / Ops.</p>
</div>
</v-click>

<v-click>
<div class="p-4 rounded" style="background: #1E293B;">
  <h3 style="font-size: 1.2rem;">ИИ-нативный софт</h3>
  <p class="text-sm opacity-70">Интерфейсы, спроектированные под агентов, а не под людей. MCP = стандарт интеграции.</p>
</div>
</v-click>

<v-click>
<div class="p-4 rounded" style="background: #0F2B1A;">
  <h3 class="green" style="font-size: 1.2rem;">В РАЗУМ</h3>
  <p class="text-sm opacity-70">От единичных агентов — к парку с контрактами задач и оркестрацией.</p>
  <p class="text-sm green mt-1">От «спросил-ответил» → к «поставил задачу — получил результат с доказательствами».</p>
</div>
</v-click>

</div>

<!--
Не прогноз ради прогноза — это то, что уже происходит. Вопрос не «будет ли», а «когда и как мы к этому придём».
-->

---
layout: center
class: text-center
---

# Итоги

<div class="pt-8 space-y-3">

<v-click>
<p style="font-size: 1.2rem;">Модели за год: от «ответа на вопрос» до <span class="amber">автономного решения задач</span></p>
</v-click>

<v-click>
<p style="font-size: 1.2rem;">MCP делает интеграцию тривиальной — <span class="green">любой продукт = инструмент агента</span></p>
</v-click>

<v-click>
<p style="font-size: 1.2rem;">Агент ≠ чат-бот. <span class="amber">Агент действует в системах, а не отвечает.</span></p>
</v-click>

<v-click>
<p style="font-size: 1.2rem;">Архитектура: <span class="green">контракт → оркестрация → проверка → приёмка</span></p>
</v-click>

<v-click>
<p style="font-size: 1.5rem; font-weight: 700;" class="amber pt-4">Главное — не модель, а процесс вокруг неё.</p>
</v-click>

</div>

<div class="pt-12">
  <v-click>
    <span style="font-size: 2.5rem; font-weight: 700; color: #F8FAFC;">Вопросы?</span>
  </v-click>
</div>

---
layout: end
---

<div class="text-center">
  <div style="font-size: 1.5rem; font-weight: 700; color: #F59E0B;">Спасибо!</div>
  <div class="pt-4 text-sm opacity-50">
    ДК РАЗУМ · ИТ митап · 2026
  </div>
  <div class="pt-8 text-xs opacity-30">
    Слайды созданы с помощью Slidev —<br>править можно прямо во время показа через бота.
  </div>
</div>
