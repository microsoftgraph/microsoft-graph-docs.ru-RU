---
title: Тип ресурса recurrenceRange
description: 'Описывает диапазон дат, согласно которому повторяется событие. '
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 337187058c923adec27de26e6e5a25d850487d04
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292457"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="91529-103">Тип ресурса recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="91529-103">recurrenceRange resource type</span></span>

<span data-ttu-id="91529-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91529-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91529-105">Описывает диапазон дат, согласно которому повторяется [событие](event.md).</span><span class="sxs-lookup"><span data-stu-id="91529-105">Describes a date range over which a recurring [event](event.md) repeats.</span></span>

<span data-ttu-id="91529-106">Вы можете задать диапазон дат для повторяющегося события одним из 3 способов (в зависимости от сценария).</span><span class="sxs-lookup"><span data-stu-id="91529-106">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="91529-107">Необходимо всегда указывать значение **startDate** для диапазона дат, но вы можете задать повторяющееся событие, которое перестает повторяться в определенный день либо повторяется бесконечно или определенное количество раз.</span><span class="sxs-lookup"><span data-stu-id="91529-107">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="91529-108">Обратите внимание, что фактические экземпляры события в диапазоне дат всегда соответствуют расписанию повторения, заданному для повторяющегося события.</span><span class="sxs-lookup"><span data-stu-id="91529-108">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="91529-109">Повторяющееся событие всегда определяется соответствующими ресурсами [recurrencePattern](recurrencepattern.md) (частотой повторения события) и **recurrenceRange** (продолжительностью повторения).</span><span class="sxs-lookup"><span data-stu-id="91529-109">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>

## <a name="properties"></a><span data-ttu-id="91529-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="91529-110">Properties</span></span>

| <span data-ttu-id="91529-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="91529-111">Property</span></span>     | <span data-ttu-id="91529-112">Тип</span><span class="sxs-lookup"><span data-stu-id="91529-112">Type</span></span>   |<span data-ttu-id="91529-113">Описание</span><span class="sxs-lookup"><span data-stu-id="91529-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91529-114">endDate</span><span class="sxs-lookup"><span data-stu-id="91529-114">endDate</span></span>|<span data-ttu-id="91529-115">Date</span><span class="sxs-lookup"><span data-stu-id="91529-115">Date</span></span>|<span data-ttu-id="91529-116">Дата, с которой перестает применяться расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="91529-116">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="91529-117">В зависимости от того, каково расписание повторения события, последний экземпляр собрания может приходиться на другую дату.</span><span class="sxs-lookup"><span data-stu-id="91529-117">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="91529-118">Обязательное, если для **type** задано значение `endDate`.</span><span class="sxs-lookup"><span data-stu-id="91529-118">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="91529-119">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="91529-119">numberOfOccurrences</span></span>|<span data-ttu-id="91529-120">Int32</span><span class="sxs-lookup"><span data-stu-id="91529-120">Int32</span></span>|<span data-ttu-id="91529-121">Количество повторений события.</span><span class="sxs-lookup"><span data-stu-id="91529-121">The number of times to repeat the event.</span></span> <span data-ttu-id="91529-122">Обязательное свойство, которое должно быть положительным, если для **type** задано значение `numbered`.</span><span class="sxs-lookup"><span data-stu-id="91529-122">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="91529-123">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="91529-123">recurrenceTimeZone</span></span>|<span data-ttu-id="91529-124">String</span><span class="sxs-lookup"><span data-stu-id="91529-124">String</span></span> |<span data-ttu-id="91529-125">Часовой пояс для свойств **startDate** и **endDate**.</span><span class="sxs-lookup"><span data-stu-id="91529-125">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="91529-126">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="91529-126">Optional.</span></span> <span data-ttu-id="91529-127">Если это свойство не задано, используется часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="91529-127">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="91529-128">startDate</span><span class="sxs-lookup"><span data-stu-id="91529-128">startDate</span></span>|<span data-ttu-id="91529-129">Date</span><span class="sxs-lookup"><span data-stu-id="91529-129">Date</span></span>|<span data-ttu-id="91529-130">Дата, с которой начинает применяться расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="91529-130">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="91529-131">В зависимости от того, каково расписание повторения события, первый экземпляр собрания может приходиться на эту или более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="91529-131">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="91529-132">Должно быть задано то же значение, что и для свойства **start** повторяющегося [события](event.md).</span><span class="sxs-lookup"><span data-stu-id="91529-132">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="91529-133">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="91529-133">Required.</span></span>|
|<span data-ttu-id="91529-134">type</span><span class="sxs-lookup"><span data-stu-id="91529-134">type</span></span>|<span data-ttu-id="91529-135">recurrenceRangeType</span><span class="sxs-lookup"><span data-stu-id="91529-135">recurrenceRangeType</span></span>|<span data-ttu-id="91529-136">Диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="91529-136">The recurrence range.</span></span> <span data-ttu-id="91529-137">Допустимые значения: `endDate`, `noEnd`, `numbered`.</span><span class="sxs-lookup"><span data-stu-id="91529-137">The possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="91529-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91529-138">Required.</span></span>|

<span data-ttu-id="91529-139">С помощью свойства **type** можно указывать различные типы для **recurrenceRange**.</span><span class="sxs-lookup"><span data-stu-id="91529-139">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="91529-140">Обратите внимание на обязательные свойства для каждого типа, описанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="91529-140">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="91529-141">Свойство type</span><span class="sxs-lookup"><span data-stu-id="91529-141">type property</span></span>  | <span data-ttu-id="91529-142">Тип диапазона повторения</span><span class="sxs-lookup"><span data-stu-id="91529-142">Type of recurrence range</span></span> | <span data-ttu-id="91529-143">Описание</span><span class="sxs-lookup"><span data-stu-id="91529-143">Description</span></span> | <span data-ttu-id="91529-144">Пример</span><span class="sxs-lookup"><span data-stu-id="91529-144">Example</span></span> | <span data-ttu-id="91529-145">Обязательные свойства</span><span class="sxs-lookup"><span data-stu-id="91529-145">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="91529-146">Диапазон с датой окончания</span><span class="sxs-lookup"><span data-stu-id="91529-146">Range with end date</span></span> | <span data-ttu-id="91529-147">Событие повторяется во все дни, входящие в соответствующее расписание повторения, с даты **startDate** и до даты **endDate** включительно.</span><span class="sxs-lookup"><span data-stu-id="91529-147">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="91529-148">Повторение события с 1 июня 2017 г. до 15 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="91529-148">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="91529-149">**type**, **startDate**, **endDate**</span><span class="sxs-lookup"><span data-stu-id="91529-149">**type**, **startDate**, **endDate**</span></span> |
|`noEnd`  |<span data-ttu-id="91529-150">Диапазон без даты окончания</span><span class="sxs-lookup"><span data-stu-id="91529-150">Range without an end date</span></span> | <span data-ttu-id="91529-151">Событие повторяется во все дни, входящие в соответствующее расписание повторения, начиная с даты **startDate**.</span><span class="sxs-lookup"><span data-stu-id="91529-151">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="91529-152">Бесконечное повторение события с 1 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="91529-152">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="91529-153">**type**, **startDate**</span><span class="sxs-lookup"><span data-stu-id="91529-153">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="91529-154">Диапазон с определенным количеством повторений</span><span class="sxs-lookup"><span data-stu-id="91529-154">Range with specific number of occurrences</span></span> | <span data-ttu-id="91529-155">Событие повторяется определенное количество раз (указанное в **numberOfOccurrences**) в соответствии с расписанием повторения, начиная с даты **startDate**.</span><span class="sxs-lookup"><span data-stu-id="91529-155">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="91529-156">Повторение события 10 раз с 1 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="91529-156">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="91529-157">**type**, **startDate**, **numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="91529-157">**type**, **startDate**, **numberOfOccurrences**</span></span> |


## <a name="json-representation"></a><span data-ttu-id="91529-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91529-158">JSON representation</span></span>

<span data-ttu-id="91529-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91529-159">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrenceRange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->

