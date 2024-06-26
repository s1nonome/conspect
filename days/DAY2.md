### ***14/05/2024***
### Содержание
- [QA/QC/Testing](#first)
- [Принципы тестирования](#second)
- [Как научиться думать как тестировщик (https://habr.com/ru/companies/otus/articles/588204/)](#third)
## <a name="first"></a>QA/QC/Testing
**Обеспечение качества** - это совокупность запланированных и систематических процессов и действий поддержки, необходимых для обеспечения надлежащего уровня уверенности в том, что процесс или рабочий продукт удовлетворяет установленным техническим требованиям или требованиям к качеству.

**Контроль качества (QC):** Рабочие методы и активности, нацеленные на выполнение требований к качеству, являющиеся частью управления качеством.

**Тестирование:** Процесс, содержащий в себе все активности жизненного цикла, как динамические, так и статические, касающиеся планирования, подготовки и оценки программного продукта и связанных с этим результатов работ с целью определить, что они соотвествуют описанным требованиям, показать, что они подходят для заявленных целей и для определения дефектов. (ISTQB)

**Обеспечение качества (QA)** - это часть Quality Management - совокупность мероприятий, охватывающих все технологические этапы разработки, выпуска и поддержки ПО, предпринимаемых на разных стадиях жизненного цикла ПО, для обеспечения требуемого уровня качества выпускаемого продукта. QA обеспечивает создание правильных процессов для получения в результате качественного продукта.

Активности QA проходят на всем протяжении SDLC: на этапе построения, анализа и улучшения процессов, формирования релизных политик, риск менеджмента.

QC подключаются на этапе составления критериев качества, quality gate-ов, метрик и способов оценки. Тестировщик вступает уже после этапа разработки (с shift left на этапе получения ТЗ и превращения его в спецификацию).

### Основными целями тестирования как части QC являются:
- предоставление информации о качестве элемента тестирования и любых остаточных рисках относительно того, до какой степени элемент тестирования был проверен;
- обнаружение дефектов в элементе тестирования до его передачи в эксплуатацию;
- смягчение рисков получения продукта низкого качества заинтересованными сторонами.
## <a name="second"></a>Принципы тестирования
1. Исчерпывающее тестирование невозможно. Насколько бы тщательным тестирование не было, нельзя учесть все возмодные сценарии и предвидеть все возможные ошибки.
2. Тестирование демонстрирует наличие дефектов, а не их отсутствие. Тестирование может выявить тот момент, что ошибки присутствуют, но не может доказать в полной мере, что дефектов нет.
3. Заблуждение об отсутствии ошибок. Можно сколько угодно находить ошибки, и даже, казалось бы, не обнаруживая их больше, нет гарантии того, что ошибки найдены все и продукт полностью качественный и готовый.
4. Раннее тестирование сохраняет время и деньги. Этот принцип говорит о том, что чем раньше выявится та или иная проблема - тем меньше средств и трудозатрат потребуется для её устранения.
5. Принцип скопления дефектов (принцип Парето). Существует такое определение - наибольшее количество дефектов обычно содержится в небольшом количестве модулей.
6. Тестирование зависит от контекста. Для разного софта будут применяться разные подходы к его тестированию.
7. Парадокс пестицида. Если к какому-либо функционалу применять постоянно повторяющийся набор тестов - то эти проверки в скором времени будут неэффективны в нахождении новых дефектов. Поэтому тест-кейсы должны постоянно обновляться и видоизменяться.
### Как понять, что тестировщик хорошо сделал свою работу?
- продукт проверен на соответствие требованиям;
- сведено к минимуму количество дефектов, которые обнаружит конечный пользователь;
- предоствалена отчетность по актуальному качеству продукта и любых остаточных рисках заинтересованным лицам.
## <a name="third"></a> Как научиться думать как тестировщик (https://habr.com/ru/companies/otus/articles/588204/)
### "Перевёрнутое" мышление и бремя доказывания.
`Когда тестируешь приложение, просто предположи, что баги есть. Если ты изначально отнесешься к приложению, так что оно работает правильно и без ошибок и попытаешься найти их, то много ошибок не найдёшь. Ты будешь видеть то, что ожидаешь увидеть. И наоборот, если ты будешь предполагать, что баги есть, то внезапно заметишь их повсюду.`

Начинать тестирование следует с предположения, что приложение не работает. Даже помыслить нельзя, что оно работает. В нем не просто есть баги, оно совершенно полностью неправильное. **`Заставь приложение доказать обратное!`**.
![alt text](../assets/cow.png)
### Сложные допущения
Сложные допущения - это не только про то, чтобы задаваться вопросом "Почему?" на всё подряд, это предполагает нечто большее, и, как и всё остальное, это требует практики.
### Признание человеческой природы
Дефекты в ПО не появляются сами по себе, из вакуума, они являются симптомами проблем в процессе. Поэтому вам, как тестировщику, следует обращать внимание на процесс разработки ПО и поведение пользователей столько же, как и на конечный продукт.

Если изучать человеческую природу, то вскоре можно понять, что люди далеки от запрограммированных роботов с идеальной памятью, неизменной мотивацией и всегда высоким уровнем внимания. На самом деле, всё совсем наоборот.

Когда начинаете тестировать продукт, помните о том, что вы сейчас смотрите на конечный продукт человеческой деятельности, страдающей от этих когнитивных искажений и других несовершенств. Ошибки, поиском которых вы занимаетесь, чаще будут их симптомами, нежели чем того, что разработчик просто неправильно реализовал алгоритм или требование. Знание и понимание человеческой машины, создавшей это ПО, поможет вам их обнаружить.

