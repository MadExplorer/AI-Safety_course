📚 Обязательный список чтения

🔘Evaluation and Benchmarking of LLM Agents: A Survey — SAP Labs

SAP позиционирует себя как глобального лидера в enterprise applications и business AI, а SAP Labs описывает как сеть глобальных R&D центров, которые разрабатывают и улучшают ключевые решения компании.

Текст раскладывает всю область оценки агентов на два вопроса: что оценивать и как оценивать. Авторы подразделяют evaluation objectives (что оценивать) на behavior, capabilities, reliability, safety, а evaluation process (как оценивать) на interaction modes, datasets and benchmarks, metrics и tooling.

Это именно карта области. Этот текст лучше рассматривать, как обзор, который помогает увидеть, из каких частей вообще состоит problem space agent evaluation (а не читать от корки до корки). 

Вы узнаете: 
🔘 какие измерения вообще входят в оценку агентов, кроме task success;
🔘 как можно раскладывать evaluation process на interaction mode, benchmark, metric и tooling;
🔘 в чем agent evaluation до сих пор остается фрагментированной и методологически недостроенной областью.

🔗 Evaluation and Benchmarking of LLM Agents: A Survey (https://arxiv.org/abs/2507.21504)

🔘Towards a Science of AI Agent Reliability

Статья от исследователей из Принстонского университета.

Из прошлого текста мы уже выяснили, что у агентов много важных свойств, а этот текст показывает, какие именно свойства стоит пытаться мерить отдельно. Авторы предлагают holistic reliability profile, то есть набор из 12 concrete metrics, распределенных по четырем измерениям: consistency, robustness, predictability, safety. Дальше они применяют эту рамку к 14 agentic models и показывают, что capability gains опережают reliability gains.

Вы узнаете:
🔘почему оценку безопасности нельзя усреднять, если речь идет о tail risks;
🔘как reliability framework меняет сам вопрос интерпретации результатов оценки.

🔗 Towards a Science of AI Agent Reliability (https://arxiv.org/html/2602.16666v1)

🔘METR: Guidelines for capability elicitation

METR (https://metr.org/), Model Evaluation and Threat Research, независимая исследовательская организация, которая занимается оценкой фронтирных ИИ, чтобы помогать компаниям и обществу понимать возможности таких систем и связанные с ними риски, их миссия состоит в разработке научных методов оценки catastrophic risks, связанных с автономными возможностями ИИ.

Тот самый формат практического руководства, который многие ждали. Текст представляет собой конкретный пример methodology for autonomy-focused agent evals. Главная идея документа в том, что eval должен измерять не только способности модели «как есть», но и способности, которые могут быть reasonably reached через plausible post-training enhancement, prompting, tooling и scaffolding. Их elicitation protocol задуман, как способ уменьшить риск сильно занизить возможности модели из-за слабого scaffolding, неудачного промптинга или других легко исправимых узких мест.

Вы узнаете: 
🔘 почему agent evaluation может занижать реальные возможности модели, если не учитывать elicitation;
🔘 как использовать dev set не только для улучшения агента, но и для классификации типов провалов;
🔘 чем spurious failure отличается от real failure и tradeoff;
🔘 какие red flags стоит проверять, прежде чем интерпретировать итоговый score как meaningful.

‼️ Примечание: сам METR пишет, что это beta, early working draft и current best guess, а не завершенный стандарт. Это сильный методологический ориентир, но НЕ окончательная процедура, которую надо просто копировать без критики.

🔗 METR: Guidelines for capability elicitation (https://evaluations.metr.org/elicitation-protocol/)


❔❔❔ Вопросы для обсуждения:

1️⃣ Должен ли хороший evaluation protocol пытаться измерить “максимально достижимые” возможности агента через elicitation, или полезнее оценивать агента в более естественном product-like setup? Какие риски у каждого из вариантов?

2️⃣ Как соотносятся два измерения из первого текста  (what to evaluate и how to evaluate) с процедурой elicitation у METR и с reliability dimensions из второй статьи?

3️⃣ Что в этих статьях относится к 3 шагу evaluation strategy (What the result means)?