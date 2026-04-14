📕 Дополнительные материалы

🔖 Подробнее про концепции и инструменты из ноутбука:

1️⃣ Текст команды Jigsaw полезен как прямое дополнение к ноутбуку. Он рассказывает про аспекты toxicity classification и почему важно смотреть, не возникает ли systematic bias на отдельных типах примеров.

🔗 Measuring and Mitigating Unintended Bias in Text Classification (https://research.google/pubs/measuring-and-mitigating-unintended-bias-in-text-classification/)

2️⃣ RealToxicityPrompts продолжает тему токсичности, но уже для генеративных моделей. Хотя статья фокусируется на генерации, она довольно удачно анализирует проблему токсичности в обучающих данных. Может работать, как дополнение к первой статье. 

🔗 RealToxicityPrompts: Evaluating Neural Toxic Degeneration in Language Models  (https://arxiv.org/abs/2009.11462)


3️⃣ Это один из канонических ранних текстов про LLM as a judge: 
🔘объясняет саму идею LLM as a judge: зачем вообще этот подход появился;
🔘объясняет основные режимы использования judge;
🔘разбирает ключевые failure modes.

🔗 Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena (https://arxiv.org/abs/2306.05685)

4️⃣ Авторы доказывают тезис: когда judge не точнее оцениваемой модели, никакой debiasing не может сократить потребность в ground truth labels больше, чем примерно вдвое, а на практике выигрыш часто еще скромнее. Иными словами, на frontier использование LLM as a judge не дает той почти бесплатной масштабируемой оценки, на которую многие надеялись.

🔗 Limits to scalable evaluation at the frontier: LLM as judge won’t beat twice the data (https://openreview.net/forum?id=NO6Tv6QcDs)

5️⃣ Еще про ограничения и режимы провала LLM as a judge: ключевой практический вывод, это что human written reference answer может быть важнее, чем просто более сильная judge model.

🔗 No Free Labels: Limitations of LLM-as-a-Judge Without Human Grounding (https://arxiv.org/abs/2503.05061)
⚡️⚡️⚡️⚡️⚡️

🔖 Подробнее о проблемах методологии evals и подходах к их решению:

1️⃣ Мориц Хардт, директор Max Planck Institute for Intelligent Systems, пишет о том, что у бенчмарков в ML странный статус: они явно были мощным двигателем прогресса, но  развивались нарушая все возможные принципы строгой научной методологии. Текст хорошо дополняет обязательную часть вокруг The Benchmark Lottery и помогает шире увидеть вопрос what the results mean.

Любой бенчмарк ценен не потому, что “истинен” в каком-то абсолютном смысле, а потому, что иногда он устойчиво сохраняет порядок моделей. Дальше статья показывает, что именно эта опора в эпоху LLM начинает ломаться из-за контаминации, невозможности агрегировать результаты множественных оценок (см. про фундаментальные проблемы теории выбора) и проблемы оценки при возрастающих способностях модели. 
 
🔗 The Emerging Science of Machine Learning Benchmarks (https://www.siam.org/publications/siam-news/articles/the-emerging-science-of-machine-learning-benchmarks/) — Moritz Hardt 


2️⃣ Текст про BenchmarkCards про то, как свои оценки нормально задокументировать. Эту статью стоит рассматривать, как дополнение к HELM и его акценту на transparency и standardized comparison.

🔗 BenchmarkCards: Standardized Documentation for Large Language Model Benchmarks  (https://arxiv.org/html/2410.12974v3)

3️⃣ Еще одна статья про теорию тестирования в применении к evals. Автор обсуждает практику приписывания LLM человеческих способностей, например, reasoning, theory of mind, morality, на основании результатов benchmark'ов. Риск в том, что такие слова автоматически вызывают у людей широкие интерпретации и сильные обобщения о поведении модели.

‼️ Статья во многих отношениях очень спорная. Она содержит интересные идеи, верные наблюдения и удачные концепции и идеи (например, то, что автор называет теоретико-эмпирическим рассогласованием). Но так же она, например, в качестве стартовой рамки предлагает обратиться к психометрическим теориям, которым самим недостает научной зрелости лишь чуть меньше чем AI safety, поэтому слепо копировать оттуда идеи не стоит. 

Итог: воспринимать критически. Читать в поисках идей на обдумывание, не верить написанному на слово, а обдумывать его. 

🔗 Establishing Construct Validity in LLM Capability Benchmarks Requires Nomological Networks (https://arxiv.org/html/2603.15121v1)