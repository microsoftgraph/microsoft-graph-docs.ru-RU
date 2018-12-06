---
title: Планирование повторных встреч, как повторяющихся событий в Outlook
description: Повторяющиеся события — важная составляющая работы с календарями в Outlook. Будь то еженедельная личная встреча с руководителем или обзорное совещание для всего отдела, проходящее во второй вторник каждого месяца, повторяющиеся события достаточно создать один раз, и сервер автоматически продолжит серию.
ms.openlocfilehash: 1af082a32d79f6011e93a7fc0c5fc9d553d16712
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092575"
---
# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="efa28-104">Планирование повторных встреч как повторяющихся событий в Outlook</span><span class="sxs-lookup"><span data-stu-id="efa28-104">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="efa28-105">Повторяющиеся события — важная составляющая работы с календарями в Outlook.</span><span class="sxs-lookup"><span data-stu-id="efa28-105">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="efa28-106">Будь то еженедельная личная встреча с руководителем или обзорное совещание для всего отдела, проходящее во второй вторник каждого месяца, повторяющиеся события достаточно создать один раз, и сервер автоматически продолжит серию.</span><span class="sxs-lookup"><span data-stu-id="efa28-106">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="efa28-107">Главный элемент, благодаря которому повторяющиеся события превращаются в отдельные экземпляры, — это правило повторения.</span><span class="sxs-lookup"><span data-stu-id="efa28-107">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="efa28-108">Правило указывает частоту и продолжительность повторения события.</span><span class="sxs-lookup"><span data-stu-id="efa28-108">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="efa28-109">REST API для Outlook моделирует правила повторения в свойстве **recurrence**[ресурса event](/graph/api/resources/event?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="efa28-109">The Outlook REST APIs model recurrence rules in the **recurrence** property of the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> 

<span data-ttu-id="efa28-110">Каждое свойство recurrence состоит из двух частей: расписания повторения (частота) и диапазона повторения (продолжительность).</span><span class="sxs-lookup"><span data-stu-id="efa28-110">Each recurrence is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="efa28-111">Расписания повторения</span><span class="sxs-lookup"><span data-stu-id="efa28-111">Recurrence patterns</span></span>

<span data-ttu-id="efa28-112">Первая часть правила повторения — расписание.</span><span class="sxs-lookup"><span data-stu-id="efa28-112">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="efa28-113">Оно задает частоту повторения события.</span><span class="sxs-lookup"><span data-stu-id="efa28-113">This specifies how often the event repeats.</span></span> <span data-ttu-id="efa28-114">Например, событие может повторяться каждые 3 дня, каждый четверг или каждый год 22 июля.</span><span class="sxs-lookup"><span data-stu-id="efa28-114">For example, an event could repeat "every 3 days," "every Thursday," or "on July 22 every year."</span></span> <span data-ttu-id="efa28-115">Расписание представлено в API [ресурсом recurrencePattern](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="efa28-115">A pattern is represented in the API by the [recurrencePattern resource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span></span>

<span data-ttu-id="efa28-116">В зависимости от того, каков тип расписания, те или иные поля ресурса **recurrencePattern** могут быть обязательными, необязательными или игнорируемыми.</span><span class="sxs-lookup"><span data-stu-id="efa28-116">Depending on the type of pattern, certain fields of the **recurrencePattern** are required, optional, or ignored.</span></span>

> <span data-ttu-id="efa28-117">**Примечание.** Даже если поле игнорируется, оно все равно проверяется.</span><span class="sxs-lookup"><span data-stu-id="efa28-117">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="efa28-118">Если для поля задан список возможных значений, то при использовании значения, не входящего в этот список, возникнет ошибка, даже если поле игнорируется.</span><span class="sxs-lookup"><span data-stu-id="efa28-118">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="efa28-119">Рассмотрим все возможные типы расписаний.</span><span class="sxs-lookup"><span data-stu-id="efa28-119">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="efa28-120">Ежедневное</span><span class="sxs-lookup"><span data-stu-id="efa28-120">Daily</span></span>

<span data-ttu-id="efa28-121">При использовании ежедневного расписания повторения событие повторяется в соответствии с указанным количеством дней между экземплярами.</span><span class="sxs-lookup"><span data-stu-id="efa28-121">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="efa28-122">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="efa28-122">Relevant properties</span></span>

| <span data-ttu-id="efa28-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="efa28-123">Property</span></span> | <span data-ttu-id="efa28-124">Важность</span><span class="sxs-lookup"><span data-stu-id="efa28-124">Relevance</span></span> | <span data-ttu-id="efa28-125">Описание</span><span class="sxs-lookup"><span data-stu-id="efa28-125">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="efa28-126">**interval**</span><span class="sxs-lookup"><span data-stu-id="efa28-126">**interval**</span></span> | <span data-ttu-id="efa28-127">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-127">Required</span></span> | <span data-ttu-id="efa28-128">Задает количество дней между повторениями.</span><span class="sxs-lookup"><span data-stu-id="efa28-128">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="efa28-129">**type**</span><span class="sxs-lookup"><span data-stu-id="efa28-129">**type**</span></span> | <span data-ttu-id="efa28-130">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-130">Required</span></span> | <span data-ttu-id="efa28-131">Необходимо указать значение `daily`.</span><span class="sxs-lookup"><span data-stu-id="efa28-131">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="efa28-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa28-132">Examples</span></span>

- <span data-ttu-id="efa28-133">Повторять это событие каждый день</span><span class="sxs-lookup"><span data-stu-id="efa28-133">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="efa28-134">Повторять это событие каждые три дня</span><span class="sxs-lookup"><span data-stu-id="efa28-134">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="efa28-135">Еженедельное</span><span class="sxs-lookup"><span data-stu-id="efa28-135">Weekly</span></span>

<span data-ttu-id="efa28-136">При использовании еженедельного расписания повторения событие повторяется в одни и те же дни недели в соответствии с указанным количеством недель между последовательностями экземпляров.</span><span class="sxs-lookup"><span data-stu-id="efa28-136">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="efa28-137">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="efa28-137">Relevant properties</span></span>

| <span data-ttu-id="efa28-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="efa28-138">Property</span></span> | <span data-ttu-id="efa28-139">Важность</span><span class="sxs-lookup"><span data-stu-id="efa28-139">Relevance</span></span> | <span data-ttu-id="efa28-140">Описание</span><span class="sxs-lookup"><span data-stu-id="efa28-140">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="efa28-141">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="efa28-141">**daysOfWeek**</span></span> | <span data-ttu-id="efa28-142">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-142">Required</span></span> | <span data-ttu-id="efa28-143">Указывает, в какие дни недели происходит событие.</span><span class="sxs-lookup"><span data-stu-id="efa28-143">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="efa28-144">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="efa28-144">**firstDayOfWeek**</span></span> | <span data-ttu-id="efa28-145">Необязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-145">Optional</span></span> | <span data-ttu-id="efa28-146">Указывает, с какого дня начинается неделя.</span><span class="sxs-lookup"><span data-stu-id="efa28-146">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="efa28-147">Значение по умолчанию: `Sunday`.</span><span class="sxs-lookup"><span data-stu-id="efa28-147">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="efa28-148">**interval**</span><span class="sxs-lookup"><span data-stu-id="efa28-148">**interval**</span></span> | <span data-ttu-id="efa28-149">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-149">Required</span></span> | <span data-ttu-id="efa28-150">Задает количество недель между наборами повторений.</span><span class="sxs-lookup"><span data-stu-id="efa28-150">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="efa28-151">**type**</span><span class="sxs-lookup"><span data-stu-id="efa28-151">**type**</span></span> | <span data-ttu-id="efa28-152">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-152">Required</span></span> | <span data-ttu-id="efa28-153">Необходимо указать значение `weekly`.</span><span class="sxs-lookup"><span data-stu-id="efa28-153">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="efa28-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa28-154">Examples</span></span>

- <span data-ttu-id="efa28-155">Повторять это событие каждый четверг</span><span class="sxs-lookup"><span data-stu-id="efa28-155">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="efa28-156">Повторять это событие каждый понедельник и вторник</span><span class="sxs-lookup"><span data-stu-id="efa28-156">Repeat this event every other Monday and Tuesday</span></span>

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

### <a name="absolute-monthly"></a><span data-ttu-id="efa28-157">Абсолютное ежемесячное</span><span class="sxs-lookup"><span data-stu-id="efa28-157">Absolute monthly</span></span>

<span data-ttu-id="efa28-158">При использовании абсолютного ежемесячного расписания событие повторяется в одно и то же число месяца (например, 15-е) в соответствии с указанным количеством месяцев между повторениями.</span><span class="sxs-lookup"><span data-stu-id="efa28-158">The absolute monthly pattern causes an event to repeat on the same day of the month (for example, the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="efa28-159">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="efa28-159">Relevant properties</span></span>

| <span data-ttu-id="efa28-160">Свойство</span><span class="sxs-lookup"><span data-stu-id="efa28-160">Property</span></span> | <span data-ttu-id="efa28-161">Важность</span><span class="sxs-lookup"><span data-stu-id="efa28-161">Relevance</span></span> | <span data-ttu-id="efa28-162">Описание</span><span class="sxs-lookup"><span data-stu-id="efa28-162">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="efa28-163">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="efa28-163">**dayOfMonth**</span></span> | <span data-ttu-id="efa28-164">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-164">Required</span></span> | <span data-ttu-id="efa28-165">Указывает, в какой день месяца происходит событие.</span><span class="sxs-lookup"><span data-stu-id="efa28-165">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="efa28-166">**interval**</span><span class="sxs-lookup"><span data-stu-id="efa28-166">**interval**</span></span> | <span data-ttu-id="efa28-167">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-167">Required</span></span> | <span data-ttu-id="efa28-168">Задает количество месяцев между повторениями.</span><span class="sxs-lookup"><span data-stu-id="efa28-168">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="efa28-169">**type**</span><span class="sxs-lookup"><span data-stu-id="efa28-169">**type**</span></span> | <span data-ttu-id="efa28-170">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-170">Required</span></span> | <span data-ttu-id="efa28-171">Необходимо указать значение `absoluteMonthly`.</span><span class="sxs-lookup"><span data-stu-id="efa28-171">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="efa28-172">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa28-172">Examples</span></span>

- <span data-ttu-id="efa28-173">Повторять это событие 15-го числа каждого месяца</span><span class="sxs-lookup"><span data-stu-id="efa28-173">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="efa28-174">Повторять это событие ежеквартально (каждые 3 месяца) 7-го числа</span><span class="sxs-lookup"><span data-stu-id="efa28-174">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="efa28-175">Относительное ежемесячное</span><span class="sxs-lookup"><span data-stu-id="efa28-175">Relative monthly</span></span>

<span data-ttu-id="efa28-176">При использовании относительного ежемесячного расписания повторения событие повторяется в один и тот же день одной и той же (по счету) недели месяца в соответствии с указанным количеством месяцев между повторениями.</span><span class="sxs-lookup"><span data-stu-id="efa28-176">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="efa28-177">Пример: "каждую вторую среду месяца".</span><span class="sxs-lookup"><span data-stu-id="efa28-177">For example, "every second Wednesday of the month."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="efa28-178">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="efa28-178">Relevant properties</span></span>

| <span data-ttu-id="efa28-179">Свойство</span><span class="sxs-lookup"><span data-stu-id="efa28-179">Property</span></span> | <span data-ttu-id="efa28-180">Важность</span><span class="sxs-lookup"><span data-stu-id="efa28-180">Relevance</span></span> | <span data-ttu-id="efa28-181">Описание</span><span class="sxs-lookup"><span data-stu-id="efa28-181">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="efa28-182">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="efa28-182">**daysOfWeek**</span></span> | <span data-ttu-id="efa28-183">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-183">Required</span></span> | <span data-ttu-id="efa28-184">Указывает, в какие дни недели может происходить событие.</span><span class="sxs-lookup"><span data-stu-id="efa28-184">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="efa28-185">Относительные ежемесячные события происходят только раз в месяц, поэтому если указать несколько значений, событие будет назначено на первый день, соответствующий расписанию.</span><span class="sxs-lookup"><span data-stu-id="efa28-185">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="efa28-186">**index**</span><span class="sxs-lookup"><span data-stu-id="efa28-186">**index**</span></span> | <span data-ttu-id="efa28-187">Необязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-187">Optional</span></span> | <span data-ttu-id="efa28-188">Указывает, в какой из разрешенных дней, указанных в **daysOfsWeek**, происходит событие (начиная с первого экземпляра за месяц).</span><span class="sxs-lookup"><span data-stu-id="efa28-188">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="efa28-189">Возможные значения: `first`, `second`, `third`, `fourth` и `last`.</span><span class="sxs-lookup"><span data-stu-id="efa28-189">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="efa28-190">Значение по умолчанию: `first`.</span><span class="sxs-lookup"><span data-stu-id="efa28-190">Default value: `first`.</span></span> |
| <span data-ttu-id="efa28-191">**interval**</span><span class="sxs-lookup"><span data-stu-id="efa28-191">**interval**</span></span> | <span data-ttu-id="efa28-192">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-192">Required</span></span> | <span data-ttu-id="efa28-193">Задает количество месяцев между повторениями.</span><span class="sxs-lookup"><span data-stu-id="efa28-193">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="efa28-194">**type**</span><span class="sxs-lookup"><span data-stu-id="efa28-194">**type**</span></span> | <span data-ttu-id="efa28-195">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-195">Required</span></span> | <span data-ttu-id="efa28-196">Необходимо указать значение `relativeMonthly`.</span><span class="sxs-lookup"><span data-stu-id="efa28-196">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="efa28-197">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa28-197">Examples</span></span>

- <span data-ttu-id="efa28-198">Повторять это событие во вторую среду каждого месяца</span><span class="sxs-lookup"><span data-stu-id="efa28-198">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="efa28-199">Повторять это событие в первый четверг или первую пятницу каждого месяца</span><span class="sxs-lookup"><span data-stu-id="efa28-199">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="efa28-200">Абсолютное ежегодное</span><span class="sxs-lookup"><span data-stu-id="efa28-200">Absolute yearly</span></span>

<span data-ttu-id="efa28-201">При использовании абсолютного ежегодного расписания событие повторяется в одни и те же месяц и день года (например, 15 апреля) в соответствии с указанным количеством лет между повторениями.</span><span class="sxs-lookup"><span data-stu-id="efa28-201">The absolute yearly pattern causes an event to repeat on the same month and day (for example, April 15), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="efa28-202">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="efa28-202">Relevant properties</span></span>

| <span data-ttu-id="efa28-203">Свойство</span><span class="sxs-lookup"><span data-stu-id="efa28-203">Property</span></span> | <span data-ttu-id="efa28-204">Важность</span><span class="sxs-lookup"><span data-stu-id="efa28-204">Relevance</span></span> | <span data-ttu-id="efa28-205">Описание</span><span class="sxs-lookup"><span data-stu-id="efa28-205">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="efa28-206">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="efa28-206">**dayOfMonth**</span></span> | <span data-ttu-id="efa28-207">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-207">Required</span></span> | <span data-ttu-id="efa28-208">Указывает, в какой день месяца происходит событие.</span><span class="sxs-lookup"><span data-stu-id="efa28-208">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="efa28-209">**month**</span><span class="sxs-lookup"><span data-stu-id="efa28-209">**month**</span></span> | <span data-ttu-id="efa28-210">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-210">Required</span></span> | <span data-ttu-id="efa28-211">Указывает, в какой месяц происходит событие.</span><span class="sxs-lookup"><span data-stu-id="efa28-211">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="efa28-212">**interval**</span><span class="sxs-lookup"><span data-stu-id="efa28-212">**interval**</span></span> | <span data-ttu-id="efa28-213">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-213">Required</span></span> | <span data-ttu-id="efa28-214">Задает количество лет между повторениями.</span><span class="sxs-lookup"><span data-stu-id="efa28-214">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="efa28-215">**type**</span><span class="sxs-lookup"><span data-stu-id="efa28-215">**type**</span></span> | <span data-ttu-id="efa28-216">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-216">Required</span></span> | <span data-ttu-id="efa28-217">Необходимо указать значение `absoluteYearly`.</span><span class="sxs-lookup"><span data-stu-id="efa28-217">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="efa28-218">Пример</span><span class="sxs-lookup"><span data-stu-id="efa28-218">Example</span></span>

- <span data-ttu-id="efa28-219">Повторять это событие 15 апреля каждого года</span><span class="sxs-lookup"><span data-stu-id="efa28-219">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="efa28-220">Относительное ежегодное</span><span class="sxs-lookup"><span data-stu-id="efa28-220">Relative yearly</span></span>

<span data-ttu-id="efa28-221">При использовании относительного ежегодного расписания повторения событие повторяется в один и тот же день одной и той же недели определенного месяца в соответствии с указанным количеством лет между повторениями.</span><span class="sxs-lookup"><span data-stu-id="efa28-221">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="efa28-222">Пример: "каждую последнюю среду ноября".</span><span class="sxs-lookup"><span data-stu-id="efa28-222">For example, "every last Wednesday of November."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="efa28-223">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="efa28-223">Relevant properties</span></span>

| <span data-ttu-id="efa28-224">Свойство</span><span class="sxs-lookup"><span data-stu-id="efa28-224">Property</span></span> | <span data-ttu-id="efa28-225">Важность</span><span class="sxs-lookup"><span data-stu-id="efa28-225">Relevance</span></span> | <span data-ttu-id="efa28-226">Описание</span><span class="sxs-lookup"><span data-stu-id="efa28-226">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="efa28-227">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="efa28-227">**daysOfWeek**</span></span> | <span data-ttu-id="efa28-228">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-228">Required</span></span> | <span data-ttu-id="efa28-229">Указывает, в какие дни недели может происходить событие.</span><span class="sxs-lookup"><span data-stu-id="efa28-229">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="efa28-230">Относительные ежегодные события происходят только раз в год, поэтому если указать несколько значений, событие будет назначено на первый день, соответствующий расписанию.</span><span class="sxs-lookup"><span data-stu-id="efa28-230">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="efa28-231">**index**</span><span class="sxs-lookup"><span data-stu-id="efa28-231">**index**</span></span> | <span data-ttu-id="efa28-232">Необязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-232">Optional</span></span> | <span data-ttu-id="efa28-233">Указывает, в какой из разрешенных дней, указанных в **daysOfsWeek**, происходит событие (начиная с первого экземпляра за месяц).</span><span class="sxs-lookup"><span data-stu-id="efa28-233">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="efa28-234">Возможные значения: `first`, `second`, `third`, `fourth` и `last`.</span><span class="sxs-lookup"><span data-stu-id="efa28-234">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="efa28-235">Значение по умолчанию: `first`.</span><span class="sxs-lookup"><span data-stu-id="efa28-235">Default value: `first`.</span></span> |
| <span data-ttu-id="efa28-236">**month**</span><span class="sxs-lookup"><span data-stu-id="efa28-236">**month**</span></span> | <span data-ttu-id="efa28-237">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-237">Required</span></span> | <span data-ttu-id="efa28-238">Указывает, в какой месяц происходит событие.</span><span class="sxs-lookup"><span data-stu-id="efa28-238">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="efa28-239">**interval**</span><span class="sxs-lookup"><span data-stu-id="efa28-239">**interval**</span></span> | <span data-ttu-id="efa28-240">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-240">Required</span></span> | <span data-ttu-id="efa28-241">Задает количество лет между повторениями.</span><span class="sxs-lookup"><span data-stu-id="efa28-241">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="efa28-242">**type**</span><span class="sxs-lookup"><span data-stu-id="efa28-242">**type**</span></span> | <span data-ttu-id="efa28-243">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-243">Required</span></span> | <span data-ttu-id="efa28-244">Необходимо указать значение `relativeMonthly`.</span><span class="sxs-lookup"><span data-stu-id="efa28-244">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="efa28-245">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa28-245">Examples</span></span>

- <span data-ttu-id="efa28-246">Повторять это событие в последнюю среду ноября каждого года</span><span class="sxs-lookup"><span data-stu-id="efa28-246">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="efa28-247">Диапазоны повторения</span><span class="sxs-lookup"><span data-stu-id="efa28-247">Recurrence ranges</span></span>

<span data-ttu-id="efa28-248">Вторая часть правила повторения — диапазон.</span><span class="sxs-lookup"><span data-stu-id="efa28-248">The second part of a recurrence is the range.</span></span> <span data-ttu-id="efa28-249">Он задает продолжительность повторения расписания.</span><span class="sxs-lookup"><span data-stu-id="efa28-249">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="efa28-250">Например, событие может быть отменено после 10 повторений, в указанную дату или повторяться бесконечно.</span><span class="sxs-lookup"><span data-stu-id="efa28-250">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="efa28-251">Диапазон представлен в API [ресурсом recurrenceRange](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="efa28-251">A range is represented in the API by the [recurrenceRange resource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span></span>

<span data-ttu-id="efa28-252">В зависимости от того, каков тип диапазона, те или иные поля ресурса **recurrenceRange** могут быть обязательными или игнорируемыми.</span><span class="sxs-lookup"><span data-stu-id="efa28-252">Depending on the type of range, certain fields of **recurrenceRange** are required or ignored.</span></span>

> <span data-ttu-id="efa28-253">**Примечание.** Даже если поле игнорируется, оно все равно проверяется.</span><span class="sxs-lookup"><span data-stu-id="efa28-253">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="efa28-254">Если для поля задан список возможных значений, то при использовании значения, не входящего в этот список, возникнет ошибка, даже если поле игнорируется.</span><span class="sxs-lookup"><span data-stu-id="efa28-254">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="efa28-255">Рассмотрим все возможные типы диапазонов.</span><span class="sxs-lookup"><span data-stu-id="efa28-255">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="efa28-256">Нумерованный диапазон</span><span class="sxs-lookup"><span data-stu-id="efa28-256">Numbered range</span></span>

<span data-ttu-id="efa28-257">Нумерованный диапазон задает фиксированное количество повторений события (в соответствии с расписанием) с даты начала.</span><span class="sxs-lookup"><span data-stu-id="efa28-257">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="efa28-258">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="efa28-258">Relevant properties</span></span>

| <span data-ttu-id="efa28-259">Свойство</span><span class="sxs-lookup"><span data-stu-id="efa28-259">Property</span></span> | <span data-ttu-id="efa28-260">Важность</span><span class="sxs-lookup"><span data-stu-id="efa28-260">Relevance</span></span> | <span data-ttu-id="efa28-261">Описание</span><span class="sxs-lookup"><span data-stu-id="efa28-261">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="efa28-262">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="efa28-262">**numberOfOccurences**</span></span> | <span data-ttu-id="efa28-263">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-263">Required</span></span> | <span data-ttu-id="efa28-264">Задает количество повторений.</span><span class="sxs-lookup"><span data-stu-id="efa28-264">Specifies the number of occurrences.</span></span> <span data-ttu-id="efa28-265">Это должно быть положительное целое число.</span><span class="sxs-lookup"><span data-stu-id="efa28-265">Must be a positive integer.</span></span> |
| <span data-ttu-id="efa28-266">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="efa28-266">**recurrenceTimeZone**</span></span> | <span data-ttu-id="efa28-267">Необязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-267">Optional</span></span> | <span data-ttu-id="efa28-268">Задает часовой пояс для свойства **startDate**.</span><span class="sxs-lookup"><span data-stu-id="efa28-268">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="efa28-269">Если это свойство не задано, используется часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="efa28-269">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="efa28-270">**startDate**</span><span class="sxs-lookup"><span data-stu-id="efa28-270">**startDate**</span></span> | <span data-ttu-id="efa28-271">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-271">Required</span></span> | <span data-ttu-id="efa28-272">Задает дату, с которой начинает применяться расписание.</span><span class="sxs-lookup"><span data-stu-id="efa28-272">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="efa28-273">Значение свойства **startDate** ДОЛЖНО соответствовать значению даты в свойстве **start**[ресурса event](/graph/api/resources/event?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="efa28-273">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="efa28-274">Обратите внимание, что первого собрания может не быть в этот день, если он не соответствует расписанию.</span><span class="sxs-lookup"><span data-stu-id="efa28-274">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="efa28-275">**type**</span><span class="sxs-lookup"><span data-stu-id="efa28-275">**type**</span></span> | <span data-ttu-id="efa28-276">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-276">Required</span></span> | <span data-ttu-id="efa28-277">Необходимо указать значение `numbered`.</span><span class="sxs-lookup"><span data-stu-id="efa28-277">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="efa28-278">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa28-278">Examples</span></span>

- <span data-ttu-id="efa28-279">Повторять это событие 10 раз</span><span class="sxs-lookup"><span data-stu-id="efa28-279">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="efa28-280">Диапазон с датой окончания</span><span class="sxs-lookup"><span data-stu-id="efa28-280">End date range</span></span>

<span data-ttu-id="efa28-281">При использовании диапазона с датой окончания событие повторяется во все дни, соответствующие применимому расписанию, между датами начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="efa28-281">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="efa28-282">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="efa28-282">Relevant properties</span></span>

| <span data-ttu-id="efa28-283">Свойство</span><span class="sxs-lookup"><span data-stu-id="efa28-283">Property</span></span> | <span data-ttu-id="efa28-284">Важность</span><span class="sxs-lookup"><span data-stu-id="efa28-284">Relevance</span></span> | <span data-ttu-id="efa28-285">Описание</span><span class="sxs-lookup"><span data-stu-id="efa28-285">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="efa28-286">**endDate**</span><span class="sxs-lookup"><span data-stu-id="efa28-286">**endDate**</span></span> | <span data-ttu-id="efa28-287">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-287">Required</span></span> | <span data-ttu-id="efa28-288">Задает дату, с которой расписание перестает применяться.</span><span class="sxs-lookup"><span data-stu-id="efa28-288">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="efa28-289">Обратите внимание, что последнего собрания может не быть в этот день, если он не соответствует расписанию.</span><span class="sxs-lookup"><span data-stu-id="efa28-289">Note that the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="efa28-290">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="efa28-290">**recurrenceTimeZone**</span></span> | <span data-ttu-id="efa28-291">Необязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-291">Optional</span></span> | <span data-ttu-id="efa28-292">Задает часовой пояс для свойств **startDate** и **endDate**.</span><span class="sxs-lookup"><span data-stu-id="efa28-292">Specifies the time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="efa28-293">Если это свойство не задано, используется часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="efa28-293">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="efa28-294">**startDate**</span><span class="sxs-lookup"><span data-stu-id="efa28-294">**startDate**</span></span> | <span data-ttu-id="efa28-295">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-295">Required</span></span> | <span data-ttu-id="efa28-296">Задает дату, с которой начинает применяться расписание.</span><span class="sxs-lookup"><span data-stu-id="efa28-296">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="efa28-297">Значение свойства **startDate** ДОЛЖНО соответствовать значению даты в свойстве **start**[ресурса event](/graph/api/resources/event?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="efa28-297">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="efa28-298">Обратите внимание, что первого собрания может не быть в этот день, если он не соответствует расписанию.</span><span class="sxs-lookup"><span data-stu-id="efa28-298">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="efa28-299">**type**</span><span class="sxs-lookup"><span data-stu-id="efa28-299">**type**</span></span> | <span data-ttu-id="efa28-300">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-300">Required</span></span> | <span data-ttu-id="efa28-301">Необходимо указать значение **endDate**.</span><span class="sxs-lookup"><span data-stu-id="efa28-301">Must be set to **endDate**.</span></span> |

#### <a name="examples"></a><span data-ttu-id="efa28-302">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa28-302">Examples</span></span>

- <span data-ttu-id="efa28-303">Повторять это событие с 1 июля 2017 г. до 31 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="efa28-303">Repeat this event from July 1, 2017, to July 31, 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="efa28-304">Бесконечный диапазон</span><span class="sxs-lookup"><span data-stu-id="efa28-304">No end range</span></span>

<span data-ttu-id="efa28-305">При использовании бесконечного диапазона событие происходит во все дни, соответствующие применимому расписанию, после даты начала.</span><span class="sxs-lookup"><span data-stu-id="efa28-305">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="efa28-306">Соответствующие свойства</span><span class="sxs-lookup"><span data-stu-id="efa28-306">Relevant properties</span></span>

| <span data-ttu-id="efa28-307">Свойство</span><span class="sxs-lookup"><span data-stu-id="efa28-307">Property</span></span> | <span data-ttu-id="efa28-308">Важность</span><span class="sxs-lookup"><span data-stu-id="efa28-308">Relevance</span></span> | <span data-ttu-id="efa28-309">Описание</span><span class="sxs-lookup"><span data-stu-id="efa28-309">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="efa28-310">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="efa28-310">**recurrenceTimeZone**</span></span> | <span data-ttu-id="efa28-311">Необязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-311">Optional</span></span> | <span data-ttu-id="efa28-312">Задает часовой пояс для свойства **startDate**.</span><span class="sxs-lookup"><span data-stu-id="efa28-312">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="efa28-313">Если это свойство не задано, используется часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="efa28-313">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="efa28-314">**startDate**</span><span class="sxs-lookup"><span data-stu-id="efa28-314">**startDate**</span></span> | <span data-ttu-id="efa28-315">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-315">Required</span></span> | <span data-ttu-id="efa28-316">Задает дату, с которой начинает применяться расписание.</span><span class="sxs-lookup"><span data-stu-id="efa28-316">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="efa28-317">Значение свойства **startDate** ДОЛЖНО соответствовать значению даты в свойстве **start**[ресурса event](/graph/api/resources/event?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="efa28-317">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="efa28-318">Обратите внимание, что первого собрания может не быть в этот день, если он не соответствует расписанию.</span><span class="sxs-lookup"><span data-stu-id="efa28-318">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="efa28-319">**type**</span><span class="sxs-lookup"><span data-stu-id="efa28-319">**type**</span></span> | <span data-ttu-id="efa28-320">Обязательный</span><span class="sxs-lookup"><span data-stu-id="efa28-320">Required</span></span> | <span data-ttu-id="efa28-321">Необходимо указать значение `noEnd`.</span><span class="sxs-lookup"><span data-stu-id="efa28-321">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="efa28-322">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa28-322">Examples</span></span>

- <span data-ttu-id="efa28-323">Бесконечно повторять это событие с 15 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="efa28-323">Repeat this event from May 15, 2017, forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="efa28-324">Создание повторяющихся событий с помощью расписаний и диапазонов</span><span class="sxs-lookup"><span data-stu-id="efa28-324">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="efa28-325">Теперь, когда мы рассмотрели расписания и диапазоны по отдельности, посмотрим на их совместную работу и взаимодействие со свойствами **start** и **end** события.</span><span class="sxs-lookup"><span data-stu-id="efa28-325">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **start** and **end** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="efa28-326">Создание правила повторения</span><span class="sxs-lookup"><span data-stu-id="efa28-326">Creating a recurrence rule</span></span>

<span data-ttu-id="efa28-327">Чтобы создать правило повторения, необходимо указать и расписание, и диапазон.</span><span class="sxs-lookup"><span data-stu-id="efa28-327">To create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="efa28-328">Расписания всех типов совместимы с диапазонами всех типов.</span><span class="sxs-lookup"><span data-stu-id="efa28-328">Any pattern type can work with any range type.</span></span> <span data-ttu-id="efa28-329">Вот несколько примеров.</span><span class="sxs-lookup"><span data-stu-id="efa28-329">Here are a few examples.</span></span>

#### <a name="examples"></a><span data-ttu-id="efa28-330">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa28-330">Examples</span></span>

- <span data-ttu-id="efa28-331">**Проведение собраний с 13:00 до 13:30 каждый понедельник, начиная с 4 сентября 2017 г., до конца года**</span><span class="sxs-lookup"><span data-stu-id="efa28-331">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017, until the end of the year**</span></span>

  - <span data-ttu-id="efa28-332">Требование "каждый понедельник" легко соблюдается с помощью расписания повторения типа `weekly`.</span><span class="sxs-lookup"><span data-stu-id="efa28-332">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="efa28-333">Требование "до конца года" указывает на диапазон повторения типа `endDate`.</span><span class="sxs-lookup"><span data-stu-id="efa28-333">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

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

  <span data-ttu-id="efa28-334">31 декабря 2017 г. выпадает на воскресенье, поэтому последнее событие в этой серии произойдет в понедельник, 25 декабря.</span><span class="sxs-lookup"><span data-stu-id="efa28-334">Because December 31, 2017, is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="efa28-335">**Проведение собраний с 14:00 до 15:00 в первый четверг каждого второго месяца, начиная с 29 августа 2017 г.**</span><span class="sxs-lookup"><span data-stu-id="efa28-335">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="efa28-336">Требование "первый четверг каждого второго месяца" можно соблюдать с помощью относительного ежемесячного расписания.</span><span class="sxs-lookup"><span data-stu-id="efa28-336">The "first Thursday of every other month" requirement is achievable by using a relative monthly pattern.</span></span> <span data-ttu-id="efa28-337">Фрагмент "каждого второго месяца" указывает, что для свойства **interval** необходимо задать значение `2`.</span><span class="sxs-lookup"><span data-stu-id="efa28-337">The "every other month" portion indicates that the **interval** should be set to `2`.</span></span>
  - <span data-ttu-id="efa28-338">Дата окончания не указана, поэтому можно использовать диапазон типа `noEnd`.</span><span class="sxs-lookup"><span data-stu-id="efa28-338">Because there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

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

  <span data-ttu-id="efa28-339">Значение свойства **startDate** является более поздней датой, чем первый четверг августа, поэтому первое событие в этой серии произойдет в сентябре.</span><span class="sxs-lookup"><span data-stu-id="efa28-339">Because the value of **startDate** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="efa28-340">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="efa28-340">Next steps</span></span>
    
<span data-ttu-id="efa28-341">Узнайте больше об [интеграции с календарем Outlook](outlook-calendar-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="efa28-341">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
