# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="84e18-101">Планирование повторных встреч, как повторяющихся событий в Outlook</span><span class="sxs-lookup"><span data-stu-id="84e18-101">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="84e18-102">Повторяющиеся события — важная составляющая работы с календарями в Outlook.</span><span class="sxs-lookup"><span data-stu-id="84e18-102">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="84e18-103">Будь то еженедельная личная встреча с руководителем или обзорное совещание для всего отдела, проходящее во второй вторник каждого месяца, повторяющиеся события достаточно создать один раз, и сервер автоматически продолжит серию.</span><span class="sxs-lookup"><span data-stu-id="84e18-103">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="84e18-104">Главный элемент, благодаря которому повторяющиеся события превращаются в отдельные экземпляры, — это правило повторения.</span><span class="sxs-lookup"><span data-stu-id="84e18-104">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="84e18-105">Правило указывает частоту и продолжительность повторения события.</span><span class="sxs-lookup"><span data-stu-id="84e18-105">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="84e18-106">REST API для Outlook моделирует правила повторения в свойстве **recurrence**[ресурса event](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="84e18-106">The Outlook REST APIs model recurrence rules in the **** property of the [event resource](../api-reference/v1.0/resources/event.md).</span></span> 

<span data-ttu-id="84e18-107">Каждое свойство recurrence состоит из двух частей: расписания повторения (частота) и диапазона повторения (продолжительность).</span><span class="sxs-lookup"><span data-stu-id="84e18-107">Each  is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="84e18-108">Расписания повторения</span><span class="sxs-lookup"><span data-stu-id="84e18-108">Recurrence patterns</span></span>

<span data-ttu-id="84e18-109">Первая часть правила повторения — расписание.</span><span class="sxs-lookup"><span data-stu-id="84e18-109">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="84e18-110">Оно задает частоту повторения события.</span><span class="sxs-lookup"><span data-stu-id="84e18-110">This specifies how often the event repeats.</span></span> <span data-ttu-id="84e18-111">Например, событие может повторяться каждые 3 дня, каждый четверг или каждый год 22 июля.</span><span class="sxs-lookup"><span data-stu-id="84e18-111">For example, an event could repeat "every 3 days", "every Thursday", or "on July 22 every year".</span></span> <span data-ttu-id="84e18-112">Расписание представлено в API [ресурсом recurrencePattern](../api-reference/v1.0/resources/recurrencepattern.md).</span><span class="sxs-lookup"><span data-stu-id="84e18-112">A pattern is represented in the API by the [recurrencePattern resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="84e18-113">В зависимости от того, каков тип расписания, те или иные поля ресурса **recurrencePattern** могут быть обязательными, необязательными или игнорируемыми.</span><span class="sxs-lookup"><span data-stu-id="84e18-113">Depending on the type of pattern, certain fields of the **** are required, optional, or ignored.</span></span>

> <span data-ttu-id="84e18-114">**Примечание.** Даже если поле игнорируется, оно все равно проверяется.</span><span class="sxs-lookup"><span data-stu-id="84e18-114">Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="84e18-115">Если для поля задан список возможных значений, то при использовании значения, не входящего в этот список, возникнет ошибка, даже если поле игнорируется.</span><span class="sxs-lookup"><span data-stu-id="84e18-115">If a field has a set list of possible values, using a value outside the allowed set will cause an error, even if that field is ignored.</span></span>

<span data-ttu-id="84e18-116">Рассмотрим все возможные типы расписаний.</span><span class="sxs-lookup"><span data-stu-id="84e18-116">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="84e18-117">Ежедневное</span><span class="sxs-lookup"><span data-stu-id="84e18-117">Daily</span></span>

<span data-ttu-id="84e18-118">При использовании ежедневного расписания повторения событие повторяется в соответствии с указанным количеством дней между экземплярами.</span><span class="sxs-lookup"><span data-stu-id="84e18-118">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="84e18-119">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="84e18-119">Relevant properties</span></span>

| <span data-ttu-id="84e18-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="84e18-120">Property</span></span> | <span data-ttu-id="84e18-121">Важность</span><span class="sxs-lookup"><span data-stu-id="84e18-121">Relevance</span></span> | <span data-ttu-id="84e18-122">Описание</span><span class="sxs-lookup"><span data-stu-id="84e18-122">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="84e18-123">**interval**</span><span class="sxs-lookup"><span data-stu-id="84e18-123">**interval**</span></span> | <span data-ttu-id="84e18-124">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-124">Required</span></span> | <span data-ttu-id="84e18-125">Задает количество дней между повторениями.</span><span class="sxs-lookup"><span data-stu-id="84e18-125">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="84e18-126">**type**</span><span class="sxs-lookup"><span data-stu-id="84e18-126">**type**</span></span> | <span data-ttu-id="84e18-127">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-127">Required</span></span> | <span data-ttu-id="84e18-128">Необходимо указать значение `daily`.</span><span class="sxs-lookup"><span data-stu-id="84e18-128">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="84e18-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="84e18-129">Examples</span></span>

- <span data-ttu-id="84e18-130">Повторять это событие каждый день</span><span class="sxs-lookup"><span data-stu-id="84e18-130">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="84e18-131">Повторять это событие каждые три дня</span><span class="sxs-lookup"><span data-stu-id="84e18-131">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="84e18-132">Еженедельное</span><span class="sxs-lookup"><span data-stu-id="84e18-132">Weekly</span></span>

<span data-ttu-id="84e18-133">При использовании еженедельного расписания повторения событие повторяется в одни и те же дни недели в соответствии с указанным количеством недель между последовательностями экземпляров.</span><span class="sxs-lookup"><span data-stu-id="84e18-133">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="84e18-134">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="84e18-134">Relevant properties</span></span>

| <span data-ttu-id="84e18-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="84e18-135">Property</span></span> | <span data-ttu-id="84e18-136">Важность</span><span class="sxs-lookup"><span data-stu-id="84e18-136">Relevance</span></span> | <span data-ttu-id="84e18-137">Описание</span><span class="sxs-lookup"><span data-stu-id="84e18-137">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="84e18-138">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="84e18-138">**daysOfWeek**</span></span> | <span data-ttu-id="84e18-139">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-139">Required</span></span> | <span data-ttu-id="84e18-140">Указывает, в какие дни недели происходит событие.</span><span class="sxs-lookup"><span data-stu-id="84e18-140">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="84e18-141">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="84e18-141">**firstDayOfWeek**</span></span> | <span data-ttu-id="84e18-142">Необязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-142">Optional</span></span> | <span data-ttu-id="84e18-143">Указывает, с какого дня начинается неделя.</span><span class="sxs-lookup"><span data-stu-id="84e18-143">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="84e18-144">Значение по умолчанию: `Sunday`.</span><span class="sxs-lookup"><span data-stu-id="84e18-144">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="84e18-145">**interval**</span><span class="sxs-lookup"><span data-stu-id="84e18-145">**interval**</span></span> | <span data-ttu-id="84e18-146">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-146">Required</span></span> | <span data-ttu-id="84e18-147">Задает количество недель между наборами повторений.</span><span class="sxs-lookup"><span data-stu-id="84e18-147">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="84e18-148">**type**</span><span class="sxs-lookup"><span data-stu-id="84e18-148">**type**</span></span> | <span data-ttu-id="84e18-149">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-149">Required</span></span> | <span data-ttu-id="84e18-150">Необходимо указать значение `weekly`.</span><span class="sxs-lookup"><span data-stu-id="84e18-150">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="84e18-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="84e18-151">Examples</span></span>

- <span data-ttu-id="84e18-152">Повторять это событие каждый четверг</span><span class="sxs-lookup"><span data-stu-id="84e18-152">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="84e18-153">Повторять это событие каждый понедельник и вторник</span><span class="sxs-lookup"><span data-stu-id="84e18-153">Repeat this event every other Monday and Tuesday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 2,
      "daysOfWeek": [
        "Monday",
        "Tuesday"
      ]
    }
  ```

### <a name="absolute-monthly"></a><span data-ttu-id="84e18-154">Абсолютное ежемесячное</span><span class="sxs-lookup"><span data-stu-id="84e18-154">Absolute monthly</span></span>

<span data-ttu-id="84e18-155">При использовании абсолютного ежемесячного расписания событие повторяется в одно и то же число месяца (например, 15-е) в соответствии с указанным количеством месяцев между повторениями.</span><span class="sxs-lookup"><span data-stu-id="84e18-155">The absolute monthly pattern causes an event to repeat on the same day of the month (e.g. the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="84e18-156">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="84e18-156">Relevant properties</span></span>

| <span data-ttu-id="84e18-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="84e18-157">Property</span></span> | <span data-ttu-id="84e18-158">Важность</span><span class="sxs-lookup"><span data-stu-id="84e18-158">Relevance</span></span> | <span data-ttu-id="84e18-159">Описание</span><span class="sxs-lookup"><span data-stu-id="84e18-159">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="84e18-160">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="84e18-160">**dayOfMonth**</span></span> | <span data-ttu-id="84e18-161">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-161">Required</span></span> | <span data-ttu-id="84e18-162">Указывает, в какой день месяца происходит событие.</span><span class="sxs-lookup"><span data-stu-id="84e18-162">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="84e18-163">**interval**</span><span class="sxs-lookup"><span data-stu-id="84e18-163">**interval**</span></span> | <span data-ttu-id="84e18-164">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-164">Required</span></span> | <span data-ttu-id="84e18-165">Задает количество месяцев между повторениями.</span><span class="sxs-lookup"><span data-stu-id="84e18-165">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="84e18-166">**type**</span><span class="sxs-lookup"><span data-stu-id="84e18-166">**type**</span></span> | <span data-ttu-id="84e18-167">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-167">Required</span></span> | <span data-ttu-id="84e18-168">Необходимо указать значение `absoluteMonthly`.</span><span class="sxs-lookup"><span data-stu-id="84e18-168">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="84e18-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="84e18-169">Examples</span></span>

- <span data-ttu-id="84e18-170">Повторять это событие 15-го числа каждого месяца</span><span class="sxs-lookup"><span data-stu-id="84e18-170">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="84e18-171">Повторять это событие ежеквартально (каждые 3 месяца) 7-го числа</span><span class="sxs-lookup"><span data-stu-id="84e18-171">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="84e18-172">Относительное ежемесячное</span><span class="sxs-lookup"><span data-stu-id="84e18-172">Relative monthly</span></span>

<span data-ttu-id="84e18-173">При использовании относительного ежемесячного расписания повторения событие повторяется в один и тот же день одной и той же (по счету) недели месяца в соответствии с указанным количеством месяцев между повторениями.</span><span class="sxs-lookup"><span data-stu-id="84e18-173">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="84e18-174">Пример: "каждую вторую среду месяца".</span><span class="sxs-lookup"><span data-stu-id="84e18-174">For example, "every second Wednesday of the month".</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="84e18-175">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="84e18-175">Relevant properties</span></span>

| <span data-ttu-id="84e18-176">Свойство</span><span class="sxs-lookup"><span data-stu-id="84e18-176">Property</span></span> | <span data-ttu-id="84e18-177">Важность</span><span class="sxs-lookup"><span data-stu-id="84e18-177">Relevance</span></span> | <span data-ttu-id="84e18-178">Описание</span><span class="sxs-lookup"><span data-stu-id="84e18-178">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="84e18-179">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="84e18-179">**daysOfWeek**</span></span> | <span data-ttu-id="84e18-180">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-180">Required</span></span> | <span data-ttu-id="84e18-181">Указывает, в какие дни недели может происходить событие.</span><span class="sxs-lookup"><span data-stu-id="84e18-181">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="84e18-182">Относительные ежемесячные события происходят только раз в месяц, поэтому если указать несколько значений, событие будет назначено на первый день, соответствующий расписанию.</span><span class="sxs-lookup"><span data-stu-id="84e18-182">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="84e18-183">**index**</span><span class="sxs-lookup"><span data-stu-id="84e18-183">**index**</span></span> | <span data-ttu-id="84e18-184">Необязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-184">Optional</span></span> | <span data-ttu-id="84e18-185">Указывает, в какой из разрешенных дней, указанных в **daysOfsWeek**, происходит событие (начиная с первого экземпляра за месяц).</span><span class="sxs-lookup"><span data-stu-id="84e18-185">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="84e18-186">Возможные значения: `first`, `second`, `third`, `fourth` и `last`.</span><span class="sxs-lookup"><span data-stu-id="84e18-186">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="84e18-187">Значение по умолчанию: `first`.</span><span class="sxs-lookup"><span data-stu-id="84e18-187">Default value: `first`.</span></span> |
| <span data-ttu-id="84e18-188">**interval**</span><span class="sxs-lookup"><span data-stu-id="84e18-188">**interval**</span></span> | <span data-ttu-id="84e18-189">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-189">Required</span></span> | <span data-ttu-id="84e18-190">Задает количество месяцев между повторениями.</span><span class="sxs-lookup"><span data-stu-id="84e18-190">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="84e18-191">**type**</span><span class="sxs-lookup"><span data-stu-id="84e18-191">**type**</span></span> | <span data-ttu-id="84e18-192">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-192">Required</span></span> | <span data-ttu-id="84e18-193">Необходимо указать значение `relativeMonthly`.</span><span class="sxs-lookup"><span data-stu-id="84e18-193">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="84e18-194">Примеры</span><span class="sxs-lookup"><span data-stu-id="84e18-194">Examples</span></span>

- <span data-ttu-id="84e18-195">Повторять это событие во вторую среду каждого месяца</span><span class="sxs-lookup"><span data-stu-id="84e18-195">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="84e18-196">Повторять это событие в первый четверг или первую пятницу каждого месяца</span><span class="sxs-lookup"><span data-stu-id="84e18-196">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="84e18-197">Абсолютное ежегодное</span><span class="sxs-lookup"><span data-stu-id="84e18-197">Absolute yearly</span></span>

<span data-ttu-id="84e18-198">При использовании абсолютного ежегодного расписания событие повторяется в одни и те же месяц и день года (например, 15 апреля) в соответствии с указанным количеством лет между повторениями.</span><span class="sxs-lookup"><span data-stu-id="84e18-198">The absolute yearly pattern causes an event to repeat on the same month and day (e.g. April 15th), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="84e18-199">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="84e18-199">Relevant properties</span></span>

| <span data-ttu-id="84e18-200">Свойство</span><span class="sxs-lookup"><span data-stu-id="84e18-200">Property</span></span> | <span data-ttu-id="84e18-201">Важность</span><span class="sxs-lookup"><span data-stu-id="84e18-201">Relevance</span></span> | <span data-ttu-id="84e18-202">Описание</span><span class="sxs-lookup"><span data-stu-id="84e18-202">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="84e18-203">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="84e18-203">**dayOfMonth**</span></span> | <span data-ttu-id="84e18-204">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-204">Required</span></span> | <span data-ttu-id="84e18-205">Указывает, в какой день месяца происходит событие.</span><span class="sxs-lookup"><span data-stu-id="84e18-205">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="84e18-206">**month**</span><span class="sxs-lookup"><span data-stu-id="84e18-206">**month**</span></span> | <span data-ttu-id="84e18-207">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-207">Required</span></span> | <span data-ttu-id="84e18-208">Указывает, в какой месяц происходит событие.</span><span class="sxs-lookup"><span data-stu-id="84e18-208">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="84e18-209">**interval**</span><span class="sxs-lookup"><span data-stu-id="84e18-209">**interval**</span></span> | <span data-ttu-id="84e18-210">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-210">Required</span></span> | <span data-ttu-id="84e18-211">Задает количество лет между повторениями.</span><span class="sxs-lookup"><span data-stu-id="84e18-211">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="84e18-212">**type**</span><span class="sxs-lookup"><span data-stu-id="84e18-212">**type**</span></span> | <span data-ttu-id="84e18-213">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-213">Required</span></span> | <span data-ttu-id="84e18-214">Необходимо указать значение `absoluteYearly`.</span><span class="sxs-lookup"><span data-stu-id="84e18-214">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="84e18-215">Пример</span><span class="sxs-lookup"><span data-stu-id="84e18-215">Example</span></span>

- <span data-ttu-id="84e18-216">Повторять это событие 15 апреля каждого года</span><span class="sxs-lookup"><span data-stu-id="84e18-216">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="84e18-217">Относительное ежегодное</span><span class="sxs-lookup"><span data-stu-id="84e18-217">Relative yearly</span></span>

<span data-ttu-id="84e18-218">При использовании относительного ежегодного расписания повторения событие повторяется в один и тот же день одной и той же недели определенного месяца в соответствии с указанным количеством лет между повторениями.</span><span class="sxs-lookup"><span data-stu-id="84e18-218">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="84e18-219">Пример: "каждую последнюю среду ноября".</span><span class="sxs-lookup"><span data-stu-id="84e18-219">For example, "every last Wednesday of November".</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="84e18-220">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="84e18-220">Relevant properties</span></span>

| <span data-ttu-id="84e18-221">Свойство</span><span class="sxs-lookup"><span data-stu-id="84e18-221">Property</span></span> | <span data-ttu-id="84e18-222">Важность</span><span class="sxs-lookup"><span data-stu-id="84e18-222">Relevance</span></span> | <span data-ttu-id="84e18-223">Описание</span><span class="sxs-lookup"><span data-stu-id="84e18-223">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="84e18-224">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="84e18-224">**daysOfWeek**</span></span> | <span data-ttu-id="84e18-225">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-225">Required</span></span> | <span data-ttu-id="84e18-226">Указывает, в какие дни недели может происходить событие.</span><span class="sxs-lookup"><span data-stu-id="84e18-226">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="84e18-227">Относительные ежегодные события происходят только раз в год, поэтому если указать несколько значений, событие будет назначено на первый день, соответствующий расписанию.</span><span class="sxs-lookup"><span data-stu-id="84e18-227">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="84e18-228">**index**</span><span class="sxs-lookup"><span data-stu-id="84e18-228">**index**</span></span> | <span data-ttu-id="84e18-229">Необязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-229">Optional</span></span> | <span data-ttu-id="84e18-230">Указывает, в какой из разрешенных дней, указанных в **daysOfsWeek**, происходит событие (начиная с первого экземпляра за месяц).</span><span class="sxs-lookup"><span data-stu-id="84e18-230">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="84e18-231">Возможные значения: `first`, `second`, `third`, `fourth` и `last`.</span><span class="sxs-lookup"><span data-stu-id="84e18-231">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="84e18-232">Значение по умолчанию: `first`.</span><span class="sxs-lookup"><span data-stu-id="84e18-232">Default value: `first`.</span></span> |
| <span data-ttu-id="84e18-233">**month**</span><span class="sxs-lookup"><span data-stu-id="84e18-233">**month**</span></span> | <span data-ttu-id="84e18-234">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-234">Required</span></span> | <span data-ttu-id="84e18-235">Указывает, в какой месяц происходит событие.</span><span class="sxs-lookup"><span data-stu-id="84e18-235">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="84e18-236">**interval**</span><span class="sxs-lookup"><span data-stu-id="84e18-236">**interval**</span></span> | <span data-ttu-id="84e18-237">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-237">Required</span></span> | <span data-ttu-id="84e18-238">Задает количество лет между повторениями.</span><span class="sxs-lookup"><span data-stu-id="84e18-238">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="84e18-239">**type**</span><span class="sxs-lookup"><span data-stu-id="84e18-239">**type**</span></span> | <span data-ttu-id="84e18-240">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-240">Required</span></span> | <span data-ttu-id="84e18-241">Необходимо указать значение `relativeMonthly`.</span><span class="sxs-lookup"><span data-stu-id="84e18-241">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="84e18-242">Примеры</span><span class="sxs-lookup"><span data-stu-id="84e18-242">Examples</span></span>

- <span data-ttu-id="84e18-243">Повторять это событие в последнюю среду ноября каждого года</span><span class="sxs-lookup"><span data-stu-id="84e18-243">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="84e18-244">Диапазоны повторения</span><span class="sxs-lookup"><span data-stu-id="84e18-244">Recurrence ranges</span></span>

<span data-ttu-id="84e18-245">Вторая часть правила повторения — диапазон.</span><span class="sxs-lookup"><span data-stu-id="84e18-245">The second part of a recurrence is the range.</span></span> <span data-ttu-id="84e18-246">Он задает продолжительность повторения расписания.</span><span class="sxs-lookup"><span data-stu-id="84e18-246">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="84e18-247">Например, событие может быть отменено после 10 повторений, в указанную дату или повторяться бесконечно.</span><span class="sxs-lookup"><span data-stu-id="84e18-247">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="84e18-248">Диапазон представлен в API [ресурсом recurrenceRange](../api-reference/v1.0/resources/recurrencepattern.md).</span><span class="sxs-lookup"><span data-stu-id="84e18-248">A range is represented in the API by the [recurrenceRange resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="84e18-249">В зависимости от того, каков тип диапазона, те или иные поля ресурса **recurrenceRange** могут быть обязательными или игнорируемыми.</span><span class="sxs-lookup"><span data-stu-id="84e18-249">Depending on the type of range, certain fields of the **** are required or ignored.</span></span>

> <span data-ttu-id="84e18-250">**Примечание.** Даже если поле игнорируется, оно все равно проверяется.</span><span class="sxs-lookup"><span data-stu-id="84e18-250">Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="84e18-251">Если для поля задан список возможных значений, то при использовании значения, не входящего в этот список, возникнет ошибка, даже если поле игнорируется.</span><span class="sxs-lookup"><span data-stu-id="84e18-251">If a field has a set list of possible values, using a value outside the allowed set will cause an error, even if that field is ignored.</span></span>

<span data-ttu-id="84e18-252">Рассмотрим все возможные типы диапазонов.</span><span class="sxs-lookup"><span data-stu-id="84e18-252">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="84e18-253">Нумерованный диапазон</span><span class="sxs-lookup"><span data-stu-id="84e18-253">Numbered range</span></span>

<span data-ttu-id="84e18-254">Нумерованный диапазон задает фиксированное количество повторений события (в соответствии с расписанием) с даты начала.</span><span class="sxs-lookup"><span data-stu-id="84e18-254">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="84e18-255">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="84e18-255">Relevant properties</span></span>

| <span data-ttu-id="84e18-256">Свойство</span><span class="sxs-lookup"><span data-stu-id="84e18-256">Property</span></span> | <span data-ttu-id="84e18-257">Важность</span><span class="sxs-lookup"><span data-stu-id="84e18-257">Relevance</span></span> | <span data-ttu-id="84e18-258">Описание</span><span class="sxs-lookup"><span data-stu-id="84e18-258">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="84e18-259">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="84e18-259">**numberOfOccurences**</span></span> | <span data-ttu-id="84e18-260">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-260">Required</span></span> | <span data-ttu-id="84e18-261">Задает количество повторений.</span><span class="sxs-lookup"><span data-stu-id="84e18-261">Specifies the number of occurrences.</span></span> <span data-ttu-id="84e18-262">Это должно быть положительное целое число.</span><span class="sxs-lookup"><span data-stu-id="84e18-262">Must be a positive integer.</span></span> |
| <span data-ttu-id="84e18-263">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="84e18-263">**recurrenceTimeZone**</span></span> | <span data-ttu-id="84e18-264">Необязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-264">Optional</span></span> | <span data-ttu-id="84e18-265">Задает часовой пояс для свойства **startDate**.</span><span class="sxs-lookup"><span data-stu-id="84e18-265">Specifies the time zone for the **** property.</span></span> <span data-ttu-id="84e18-266">Если это свойство не задано, используется часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="84e18-266">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="84e18-267">**startDate**</span><span class="sxs-lookup"><span data-stu-id="84e18-267">**startDate**</span></span> | <span data-ttu-id="84e18-268">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-268">Required</span></span> | <span data-ttu-id="84e18-269">Задает дату, с которой начинает применяться расписание.</span><span class="sxs-lookup"><span data-stu-id="84e18-269">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="84e18-270">Значение свойства **startDate** ДОЛЖНО соответствовать значению даты в свойстве **start**[ресурса event](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="84e18-270">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="84e18-271">Обратите внимание, что первого собрания может не быть в этот день, если он не соответствует расписанию.</span><span class="sxs-lookup"><span data-stu-id="84e18-271">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="84e18-272">**type**</span><span class="sxs-lookup"><span data-stu-id="84e18-272">**type**</span></span> | <span data-ttu-id="84e18-273">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-273">Required</span></span> | <span data-ttu-id="84e18-274">Необходимо указать значение `numbered`.</span><span class="sxs-lookup"><span data-stu-id="84e18-274">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="84e18-275">Примеры</span><span class="sxs-lookup"><span data-stu-id="84e18-275">Examples</span></span>

- <span data-ttu-id="84e18-276">Повторять это событие 10 раз</span><span class="sxs-lookup"><span data-stu-id="84e18-276">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="84e18-277">Диапазон с датой окончания</span><span class="sxs-lookup"><span data-stu-id="84e18-277">End date range</span></span>

<span data-ttu-id="84e18-278">При использовании диапазона с датой окончания событие повторяется во все дни, соответствующие применимому расписанию, между датами начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="84e18-278">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="84e18-279">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="84e18-279">Relevant properties</span></span>

| <span data-ttu-id="84e18-280">Свойство</span><span class="sxs-lookup"><span data-stu-id="84e18-280">Property</span></span> | <span data-ttu-id="84e18-281">Важность</span><span class="sxs-lookup"><span data-stu-id="84e18-281">Relevance</span></span> | <span data-ttu-id="84e18-282">Описание</span><span class="sxs-lookup"><span data-stu-id="84e18-282">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="84e18-283">**endDate**</span><span class="sxs-lookup"><span data-stu-id="84e18-283">**endDate**</span></span> | <span data-ttu-id="84e18-284">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-284">Required</span></span> | <span data-ttu-id="84e18-285">Задает дату, с которой расписание перестает применяться.</span><span class="sxs-lookup"><span data-stu-id="84e18-285">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="84e18-286">Обратите внимание, что последнего собрания может не быть в этот день, если он не соответствует расписанию.</span><span class="sxs-lookup"><span data-stu-id="84e18-286">Note: the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="84e18-287">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="84e18-287">**recurrenceTimeZone**</span></span> | <span data-ttu-id="84e18-288">Необязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-288">Optional</span></span> | <span data-ttu-id="84e18-289">Задает часовой пояс для свойств **startDate** и **endDate**.</span><span class="sxs-lookup"><span data-stu-id="84e18-289">Specifies the time zone for the **** and **** properties.</span></span> <span data-ttu-id="84e18-290">Если это свойство не задано, используется часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="84e18-290">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="84e18-291">**startDate**</span><span class="sxs-lookup"><span data-stu-id="84e18-291">**startDate**</span></span> | <span data-ttu-id="84e18-292">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-292">Required</span></span> | <span data-ttu-id="84e18-293">Задает дату, с которой начинает применяться расписание.</span><span class="sxs-lookup"><span data-stu-id="84e18-293">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="84e18-294">Значение свойства **startDate** ДОЛЖНО соответствовать значению даты в свойстве **start**[ресурса event](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="84e18-294">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="84e18-295">Обратите внимание, что первого собрания может не быть в этот день, если он не соответствует расписанию.</span><span class="sxs-lookup"><span data-stu-id="84e18-295">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="84e18-296">**type**</span><span class="sxs-lookup"><span data-stu-id="84e18-296">**type**</span></span> | <span data-ttu-id="84e18-297">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-297">Required</span></span> | <span data-ttu-id="84e18-298">Необходимо указать значение **endDate**.</span><span class="sxs-lookup"><span data-stu-id="84e18-298">Must be set to ****.</span></span> |

#### <a name="examples"></a><span data-ttu-id="84e18-299">Примеры</span><span class="sxs-lookup"><span data-stu-id="84e18-299">Examples</span></span>

- <span data-ttu-id="84e18-300">Повторять это событие с 1 июля 2017 г. до 31 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="84e18-300">Repeat this event from July 1 2017 to July 31 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="84e18-301">Бесконечный диапазон</span><span class="sxs-lookup"><span data-stu-id="84e18-301">No end range</span></span>

<span data-ttu-id="84e18-302">При использовании бесконечного диапазона событие происходит во все дни, соответствующие применимому расписанию, после даты начала.</span><span class="sxs-lookup"><span data-stu-id="84e18-302">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="84e18-303">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="84e18-303">Relevant properties</span></span>

| <span data-ttu-id="84e18-304">Свойство</span><span class="sxs-lookup"><span data-stu-id="84e18-304">Property</span></span> | <span data-ttu-id="84e18-305">Важность</span><span class="sxs-lookup"><span data-stu-id="84e18-305">Relevance</span></span> | <span data-ttu-id="84e18-306">Описание</span><span class="sxs-lookup"><span data-stu-id="84e18-306">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="84e18-307">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="84e18-307">**recurrenceTimeZone**</span></span> | <span data-ttu-id="84e18-308">Необязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-308">Optional</span></span> | <span data-ttu-id="84e18-309">Задает часовой пояс для свойства **startDate**.</span><span class="sxs-lookup"><span data-stu-id="84e18-309">Specifies the time zone for the **** property.</span></span> <span data-ttu-id="84e18-310">Если это свойство не задано, используется часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="84e18-310">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="84e18-311">**startDate**</span><span class="sxs-lookup"><span data-stu-id="84e18-311">**startDate**</span></span> | <span data-ttu-id="84e18-312">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-312">Required</span></span> | <span data-ttu-id="84e18-313">Задает дату, с которой начинает применяться расписание.</span><span class="sxs-lookup"><span data-stu-id="84e18-313">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="84e18-314">Значение свойства **startDate** ДОЛЖНО соответствовать значению даты в свойстве **start**[ресурса event](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="84e18-314">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="84e18-315">Обратите внимание, что первого собрания может не быть в этот день, если он не соответствует расписанию.</span><span class="sxs-lookup"><span data-stu-id="84e18-315">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="84e18-316">**type**</span><span class="sxs-lookup"><span data-stu-id="84e18-316">**type**</span></span> | <span data-ttu-id="84e18-317">Обязательный</span><span class="sxs-lookup"><span data-stu-id="84e18-317">Required</span></span> | <span data-ttu-id="84e18-318">Необходимо указать значение `noEnd`.</span><span class="sxs-lookup"><span data-stu-id="84e18-318">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="84e18-319">Примеры</span><span class="sxs-lookup"><span data-stu-id="84e18-319">Examples</span></span>

- <span data-ttu-id="84e18-320">Бесконечно повторять это событие с 15 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="84e18-320">Repeat this event from May 15 2017 forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="84e18-321">Создание повторяющихся событий с помощью расписаний и диапазонов</span><span class="sxs-lookup"><span data-stu-id="84e18-321">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="84e18-322">Теперь, когда мы рассмотрели расписания и диапазоны по отдельности, посмотрим на их совместную работу и взаимодействие со свойствами **start** и **end** события.</span><span class="sxs-lookup"><span data-stu-id="84e18-322">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **** and **** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="84e18-323">Создание правила повторения</span><span class="sxs-lookup"><span data-stu-id="84e18-323">Creating a recurrence rule</span></span>

<span data-ttu-id="84e18-324">Чтобы создать правило повторения, необходимо указать и расписание, и диапазон.</span><span class="sxs-lookup"><span data-stu-id="84e18-324">In order to create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="84e18-325">Расписания всех типов совместимы с диапазонами всех типов.</span><span class="sxs-lookup"><span data-stu-id="84e18-325">Any pattern type can work with any range type.</span></span> <span data-ttu-id="84e18-326">Вот несколько примеров.</span><span class="sxs-lookup"><span data-stu-id="84e18-326">Here are a few suggestions:</span></span>

#### <a name="examples"></a><span data-ttu-id="84e18-327">Примеры</span><span class="sxs-lookup"><span data-stu-id="84e18-327">Examples</span></span>

- <span data-ttu-id="84e18-328">**Проведение собраний с 13:00 до 13:30 каждый понедельник, начиная с 4 сентября 2017 г., до конца года**</span><span class="sxs-lookup"><span data-stu-id="84e18-328">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017 until the end of the year**</span></span>

  - <span data-ttu-id="84e18-329">Требование "каждый понедельник" легко соблюдается с помощью расписания повторения типа `weekly`.</span><span class="sxs-lookup"><span data-stu-id="84e18-329">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="84e18-330">Требование "до конца года" указывает на диапазон повторения типа `endDate`.</span><span class="sxs-lookup"><span data-stu-id="84e18-330">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

  ```json
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
        "daysOfWeek": [ "Monday" ]
      },
      "range": {
        "type": "endDate",
        "startDate": "2017-09-04",
        "endDate": "2017-12-31"
      }
    }
  ```

  <span data-ttu-id="84e18-331">31 декабря 2017 г. выпадает на воскресенье, поэтому последнее событие в этой серии произойдет в понедельник, 25 декабря.</span><span class="sxs-lookup"><span data-stu-id="84e18-331">Because December 31, 2017 is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="84e18-332">**Проведение собраний с 14:00 до 15:00 в первый четверг каждого второго месяца, начиная с 29 августа 2017 г.**</span><span class="sxs-lookup"><span data-stu-id="84e18-332">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="84e18-333">Требование "первый четверг каждого второго месяца" можно соблюдать с помощью относительного ежемесячного расписания.</span><span class="sxs-lookup"><span data-stu-id="84e18-333">The "first Thursday of every other month" requirement is achievable using a relative monthly pattern.</span></span> <span data-ttu-id="84e18-334">Фрагмент "каждого второго месяца" указывает, что для свойства **interval** необходимо задать значение `2`.</span><span class="sxs-lookup"><span data-stu-id="84e18-334">The "every other month" portion indicates the **** should be set to `2`.</span></span>
  - <span data-ttu-id="84e18-335">Дата окончания не указана, поэтому можно использовать диапазон типа `noEnd`.</span><span class="sxs-lookup"><span data-stu-id="84e18-335">Since there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

  ```json
    "recurrence": {
      "pattern": {
        "type": "relativeMonthly",
        "interval": 2,
        "daysOfWeek": [ "Thursday" ],
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "startDate": "2017-08-29"
      }
    }
  ```

  <span data-ttu-id="84e18-336">Значение свойства **startDate** является более поздней датой, чем первый четверг августа, поэтому первое событие в этой серии произойдет в сентябре.</span><span class="sxs-lookup"><span data-stu-id="84e18-336">Because the value of **** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="84e18-337">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="84e18-337">Next steps</span></span>
    
<span data-ttu-id="84e18-338">Узнайте больше об [интеграции с календарем Outlook](outlook-calendar-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="84e18-338">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
