<h1 align="center">💫 About Me:</h1>
<h3 align="center">Увлеченный дата-сайентист (ML\DS)</h3>
Привет! Меня зовут Данила 👋<br>
🌇 Живу в Москве <br>
🔥 Занимаюсь машинным обучением и аналитикой данных. Активно принимаю участие в различных проектах по CV, NLP и Audio <br>

<br> 👉 Забавный факт: **"Не оценивать результаты генеративки глазами, а проводить Human Evaluation"** <br>

<h3 align="left">Интересные проекты:</h3>
<p align="left">
</p>
<br>
⚡ <b>YAPPY Searcher — мгновенный интеллектуальный поиск по коротким видео</b><br>
<b>Кратко:</b> У тебя есть база роликов — решение индексирует текст, звук и изображения в каждом видео и позволяет искать по ним по обычному текстовому запросу.<br>
Приложение для поиска нужных видео по тексту, аудио и содержимому изображений.  
Backend реализован на Flask. Для поиска похожих видео используется Jina-CLIP-v1 — нейросеть, преобразующая визуальный и текстовый контент в общее векторное пространство, что обеспечивает релевантный семантический поиск даже по абстрактным запросам. EasyOCR извлекает текстовые элементы непосредственно с кадров видео, повышая полноту индексации. Распознавание речи из аудиодорожек реализовано через Nvidia NeMo (FastConformer Hybrid Large), что позволяет учитывать звуковую дорожку при поиске. Интерфейс реализован с поддержкой автодополнения и мультиязычных запросов.<br>
<a href="https://github.com/DanilaAniva/YAPPY_searcher_SDVIG_deploy">Код на GitHub</a>

<br>
⚡ <b>DiaBERT ASR Backend — автоматизация учёта времени через голосовые команды</b><br>
<b>Кратко:</b> Человек диктует голосом, что и когда делал — система превращает это в структурированный отчёт по задачам и времени.<br>
Сервис, преобразующий аудиозаписи в структурированные отчёты о задачах и временных интервалах.  
Ядро построено на FastAPI для высокой скорости работы. Для автоматического распознавания речи применяется Whisper-large-v3-turbo — современная модель ASR с поддержкой нескольких языков и устойчивостью к шуму. Далее, полученный текст обрабатывается LLM Vikhr-Nemo-12B, которая извлекает и маркирует временные промежутки, действия и задачи в формате JSON. Благодаря этому можно вести трекинг задач и экспортировать отчёты в DOCX одним кликом.<br>
<a href="https://github.com/DanilaAniva/DiabertASRBackend">Код на GitHub</a>

<br>
⚡ <b>AI-med-service — универсальная платформа для анализа медицинских изображений</b><br>
<b>Кратко:</b> Врачи могут загружать медицинские снимки — сервис автоматически выделяет органы, выявляет патологии и классифицирует заболевания с помощью нейросетей.<br>
Агрегатор сервисов ИИ для диагностики по рентгеновским снимкам.  
Backend построен на Flask. Для сегментации и классификации используются кастомные U-NET и U-NET++ — эти модели показывают высокую точность при выделении органов и патологий даже на сложных данных. В систему встроена поддержка DICOM-формата для удобства врачей. Также реализован Autoencoder для отслеживания и обработки ошибок при загрузке невалидных изображений. Пользовательский интерфейс включает историю инференсов, личный кабинет и разграничение прав доступа.<br>
<a href="https://github.com/DanilaAniva/AI-med-service">Код на GitHub</a>

<br>
⚡ <b>ASR Summarizer — суммаризация длинных аудиофайлов с помощью нейросетей</b><br>
<b>Кратко:</b> Берёт длинную аудиозапись (например, подкаст) и выдаёт краткое содержательное резюме по основным темам и событиям.<br>
Приложение для автоматического выделения ключевых смыслов, событий и тем из аудиозаписей.  
В основе — цепочка ASR и LLM: сначала аудиофайл преобразуется в текст с помощью модели распознавания речи, затем крупная языковая модель строит краткое содержательное описание. Это снижает время на ручной анализ встреч и звонков.<br>

<br>
⚡ <b>ASR-NeMo-Comparison — сравнение и выбор ASR-моделей для задач распознавания речи</b><br>
<b>Кратко:</b> Сравнивает разные модели распознавания речи на реальных видео — помогает выбрать лучший инструмент под задачу.<br>
Набор ноутбуков для анализа производительности ASR-моделей Nvidia NeMo на видеоконтенте.  
Каждая модель тестируется на реальных роликах, сравнивается точность и устойчивость к разным шумам и акцентам, визуализируются результаты для быстрой оценки применимости под конкретный сценарий.<br>
<a href="https://github.com/DanilaAniva/ASR-NeMo-Comparison">Код на GitHub</a>

<br>
⚡ <b>MLPractice — практические ноутбуки по ML и Data Science</b><br>
<b>Кратко:</b> Коллекция практических задач по машинному обучению — от классических моделей до экспериментов с современными нейросетями.<br>
Сборник ноутбуков с задачами по машинному обучению.
<a href="https://github.com/DanilaAniva/MLPractice">Код на GitHub</a>


<h3 align="left">Связаться со мной:</h3>
<p align="left">
</p>
🍊 Обязательно пиши в ТГ, если хочешь что-то спросить, предложить или просто пообщаться - [@LichPlease](https://t.me/LichPlease)<br>
<h3 align="left">Языки и библиотеки:</h3>
<p align="left"> <a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a> <a href="https://flask.palletsprojects.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/pocoo_flask/pocoo_flask-icon.svg" alt="flask" width="40" height="40"/> </a> <a href="https://hadoop.apache.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/apache_hadoop/apache_hadoop-icon.svg" alt="hadoop" width="40" height="40"/> </a> <a href="https://www.postgresql.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://pytorch.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/pytorch/pytorch-icon.svg" alt="pytorch" width="40" height="40"/> </a> <a href="https://scikit-learn.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="scikit_learn" width="40" height="40"/> </a> </p>
