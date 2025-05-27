<h1 align="center">💫 About Me:</h1>
<h3 align="center">Увлеченный дата-сайентист (ML\DS)</h3>
Привет! Меня зовут Данила 👋<br>
🌇 Живу в Москве <br>
🔥 Занимаюсь машинным обучением и аналитикой данных. Активно принимаю участие в различных проектах по CV, NLP и Audio <br>

<br> 👉 Забавный факт: **"Не оценивать результаты генеративки глазами, а проводить Human Evaluation"** <br>

<h3 align="left">Интересные проекты:</h3>

<br>

⚡ <b>YAPPY Searcher — мгновенный интеллектуальный поиск по коротким видео</b>

📝 *Кратко:*  
У тебя есть база роликов — решение индексирует текст, звук и изображения в каждом видео и позволяет искать по ним по обычному текстовому запросу.

💡 *Описание:*  
Приложение для поиска нужных видео по тексту, аудио и содержимому изображений. Backend реализован на Flask. Для поиска похожих видео используется Jina-CLIP-v1 — нейросеть, преобразующая визуальный и текстовый контент в общее векторное пространство, что обеспечивает релевантный семантический поиск даже по абстрактным запросам. EasyOCR извлекает текстовые элементы непосредственно с кадров видео, повышая полноту индексации. Распознавание речи из аудиодорожек реализовано через Nvidia NeMo (FastConformer Hybrid Large), что позволяет учитывать звуковую дорожку при поиске. Интерфейс реализован с поддержкой автодополнения и мультиязычных запросов.

🛠️ *Технологии:*  
EasyOCR (OCR), Nvidia NeMo (FastConformer Hybrid Large) (ASR), Flask (Backend), Jina-CLIP-v1 (Embedder)

[Код на GitHub](https://github.com/DanilaAniva/YAPPY_searcher_SDVIG_deploy)

---

⚡ <b>DiaBERT ASR Backend — автоматизация учёта времени через голосовые команды</b>

📝 *Кратко:*  
Человек диктует голосом, что и когда делал — система превращает это в структурированный отчёт по задачам и времени.

💡 *Описание:*  
Сервис, преобразующий аудиозаписи в структурированные отчёты о задачах и временных интервалах. Ядро построено на FastAPI для высокой скорости работы. Для автоматического распознавания речи применяется Whisper-large-v3-turbo — современная модель ASR с поддержкой нескольких языков и устойчивостью к шуму. Далее, полученный текст обрабатывается LLM Vikhr-Nemo-12B, которая извлекает и маркирует временные промежутки, действия и задачи в формате JSON. Благодаря этому можно вести трекинг задач и экспортировать отчёты в DOCX одним кликом.

🛠️ *Технологии:*  
FastAPI (Backend), Whisper-large-v3-turbo (ASR), Vikhr-Nemo-12B (LLM), DOCX экспорт

[Код на GitHub](https://github.com/DanilaAniva/DiabertASRBackend)

---

⚡ <b>AI-med-service — универсальная платформа для анализа медицинских изображений</b>

📝 *Кратко:*  
Врачи могут загружать медицинские снимки — сервис автоматически выделяет органы, выявляет патологии и классифицирует заболевания с помощью нейросетей.

💡 *Описание:*  
Агрегатор сервисов ИИ для диагностики по рентгеновским снимкам. Backend построен на Flask. Для сегментации и классификации используются кастомные U-NET и U-NET++ — у моделей используется энкодеры EfficientNet с DiceBCELoss, AdamW в качестве optimizer и LearningRateWarmup + ReduceLROnPlateau в качестве scheduler. Настроено логгирование метрик в wandb. Были протестированы разные подходы и при обучении получена лучшая метрика на датасете COVID-QU-Ex (33,920 chest X-ray). Обучение проходило на Nvidia V100. В систему встроена поддержка DICOM-формата для удобства врачей. Также реализован Autoencoder для отслеживания и обработки ошибок при загрузке невалидных изображений. Пользовательский интерфейс включает историю инференсов, личный кабинет и разграничение прав доступа. 

🛠️ *Технологии:*  
Flask (Backend), U-NET, U-NET++ (CV/Segmentation), Autoencoder (Validation), DICOM support

[Код на GitHub](https://github.com/DanilaAniva/AI-med-service)

---

⚡ <b>ASR Summarizer — суммаризация длинных аудиофайлов с помощью нейросетей</b>

📝 *Кратко:*  
Берёт длинную аудиозапись (например, подкаст) и выдаёт краткое содержательное резюме по основным темам и событиям.

💡 *Описание:*  
Приложение для автоматического выделения ключевых смыслов, событий и тем из аудиозаписей. В основе — цепочка ASR и LLM: сначала аудиофайл преобразуется в текст с помощью модели распознавания речи, затем крупная языковая модель строит краткое содержательное описание. Это снижает время на ручной анализ встреч и звонков.

🛠️ *Технологии:*  
Whisper/ASR (Speech-to-Text), LLM (Summarization)

---

⚡ <b>ASR-NeMo-Comparison — сравнение и выбор ASR-моделей для задач распознавания речи</b>

📝 *Кратко:*  
Сравнивает разные модели распознавания речи на реальных видео — помогает выбрать лучший инструмент под задачу.

💡 *Описание:*  
Набор ноутбуков для анализа производительности ASR-моделей Nvidia NeMo на видеоконтенте. Каждая модель тестируется на реальных роликах, сравнивается точность и устойчивость к разным шумам и акцентам, визуализируются результаты для быстрой оценки применимости под конкретный сценарий.

🛠️ *Технологии:*  
Jupyter Notebooks, Nvidia NeMo (ASR), Python, Pandas, Matplotlib, etc

[Код на GitHub](https://github.com/DanilaAniva/ASR-NeMo-Comparison)

---

⚡ <b>MLPractice — практические ноутбуки по ML и Data Science</b>

📝 *Кратко:*  
Коллекция практических задач по машинному обучению — от классических моделей до экспериментов с современными нейросетями.

💡 *Описание:*  
Сборник ноутбуков с задачами по машинному обучению.

🛠️ *Технологии:*  
Jupyter Notebooks, Python, Scikit-learn, PyTorch, Pandas, Matplotlib, etc

[Код на GitHub](https://github.com/DanilaAniva/MLPractice)


<h3 align="left">Связаться со мной:</h3>
<p align="left">
</p>
🍊 Обязательно пиши в ТГ, если хочешь что-то спросить, предложить или просто пообщаться - [@LichPlease](https://t.me/LichPlease)<br>
<h3 align="left">Языки и библиотеки:</h3>
<p align="left"> <a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a> <a href="https://flask.palletsprojects.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/pocoo_flask/pocoo_flask-icon.svg" alt="flask" width="40" height="40"/> </a> <a href="https://hadoop.apache.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/apache_hadoop/apache_hadoop-icon.svg" alt="hadoop" width="40" height="40"/> </a> <a href="https://www.postgresql.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://pytorch.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/pytorch/pytorch-icon.svg" alt="pytorch" width="40" height="40"/> </a> <a href="https://scikit-learn.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="scikit_learn" width="40" height="40"/> </a> </p>
