📕 Дополнительные материалы

🔖 Подробнее про концепции и инструменты из ноутбука

1️⃣ ReAct: Synergizing Reasoning and Acting in Language Models

Текст введен в интересах тех, кому хочется почитать слов про подход, который они реализовывали в ноутбуке этой недели. 

Этот текст вводит ReAct — подход, где модель чередует рассуждение и действия, чтобы решать задачи с инструментами и внешней средой.

🔗 ReAct: Synergizing Reasoning and Acting in Language Models (https://openreview.net/forum?id=WE_vluYUL-X) 

2️⃣ Measuring Mathematical Problem Solving With the MATH Dataset

Текст приведен ради исторического контекста (просто для любопытных).

Ноутбук использует MATH-500. Статья про него дает представление, что это за класс задач, и почему математическое рассуждение трудно для моделей, а dataset card MATH-500 поясняет, что это отдельный 500-problem subset. Это полезно, чтобы понимать, на каком типе benchmark мы оптимизируем агента. 

🔗 Measuring Mathematical Problem Solving With the MATH Dataset (https://arxiv.org/abs/2103.03874)
⚡️⚡️⚡️⚡️

🔖 Про агентов и методы их создания

1️⃣ Large Language Model Agent: A Survey on Methodology, Applications and Challenges

Текст приведен в интересах тех, кто хочет понять объект оценки до того, как переходить к вопросам дизайна оценки.  

Статья дает представление о том, какие design choices вообще существуют при создании агентов, и почему они ведут к разным типам поведения. Это широкий обзор “про агентов вообще”, так что в каком-то смысле он предваряет (или дополняет) Evaluation and Benchmarking of LLM Agents: A Survey из обязательного списка. 

🔗 Large Language Model Agent: A Survey on Methodology, Applications and Challenges (https://arxiv.org/abs/2503.21460)

⚡️⚡️⚡️⚡️

🔖 Подробнее о практике оценки агентов 

1️⃣ Measuring AI agent autonomy in practice

Текст рассказывает, как Anthropic пытается измерять автономность агентов в реальном использовании, на данных из миллионов human agent interactions в Claude Code и public API.

🔗 Measuring AI agent autonomy in practice  (https://www.anthropic.com/research/measuring-agent-autonomy)

2️⃣ SWE-bench

Эта статья вводит SWE-bench — бенчмарк на реальных GitHub issues, где модель должна менять кодовую базу так, чтобы пройти тесты и исправить проблему. Её можно воспринимать, как пример сложного agentic benchmark для задач на кодинг.

🔗 SWE-bench: Can Language Models Resolve Real-World GitHub Issues (https://arxiv.org/abs/2310.06770)
🔗 Introducing SWE-bench Verified (https://openai.com/index/introducing-swe-bench-verified/) 

3️⃣ Resources | METR’s Autonomy Evaluation Resources

Это главная страница-индекс всего набора ресурсов METR по автономным evals. Ее функция: показать, из каких частей состоит их подход. Там перечислены:
🔘task suite,
🔘guidelines for capability elicitation,
🔘task standard and workbench,
🔘example evaluation protocol,
🔘исследовательский блок про measuring the impact of elicitation.

🔗 Resources | METR’s Autonomy Evaluation Resources (https://evaluations.metr.org/)