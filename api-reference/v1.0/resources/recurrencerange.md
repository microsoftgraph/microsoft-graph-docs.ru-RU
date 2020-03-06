---
title: Тип ресурса recurrenceRange
description: 'Описывает диапазон дат, согласно которому повторяется событие. '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4aa03f133206ef5e4f4fd9106b1389b0c6ce1299
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533892"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="6e124-103">Тип ресурса recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="6e124-103">recurrenceRange resource type</span></span>

<span data-ttu-id="6e124-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e124-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e124-105">Описывает диапазон дат, согласно которому повторяется [событие](event.md).</span><span class="sxs-lookup"><span data-stu-id="6e124-105">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="6e124-106">Вы можете задать диапазон дат для повторяющегося события одним из 3 способов (в зависимости от сценария).</span><span class="sxs-lookup"><span data-stu-id="6e124-106">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="6e124-107">Необходимо всегда указывать значение **startDate** для диапазона дат, но вы можете задать повторяющееся событие, которое перестает повторяться в определенный день либо повторяется бесконечно или определенное количество раз.</span><span class="sxs-lookup"><span data-stu-id="6e124-107">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="6e124-108">Обратите внимание, что фактические экземпляры события в диапазоне дат всегда соответствуют расписанию повторения, заданному для повторяющегося события.</span><span class="sxs-lookup"><span data-stu-id="6e124-108">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="6e124-109">Повторяющееся событие всегда определяется соответствующими ресурсами [recurrencePattern](recurrencepattern.md) (частотой повторения события) и **recurrenceRange** (продолжительностью повторения).</span><span class="sxs-lookup"><span data-stu-id="6e124-109">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>

## <a name="properties"></a><span data-ttu-id="6e124-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e124-110">Properties</span></span>

| <span data-ttu-id="6e124-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e124-111">Property</span></span>     | <span data-ttu-id="6e124-112">Тип</span><span class="sxs-lookup"><span data-stu-id="6e124-112">Type</span></span>   |<span data-ttu-id="6e124-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6e124-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e124-114">endDate</span><span class="sxs-lookup"><span data-stu-id="6e124-114">endDate</span></span>|<span data-ttu-id="6e124-115">Date</span><span class="sxs-lookup"><span data-stu-id="6e124-115">Date</span></span>|<span data-ttu-id="6e124-116">Дата, с которой перестает применяться расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="6e124-116">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="6e124-117">В зависимости от того, каково расписание повторения события, последний экземпляр собрания может приходиться на другую дату.</span><span class="sxs-lookup"><span data-stu-id="6e124-117">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="6e124-118">Обязательное, если для **type** задано значение `endDate`.</span><span class="sxs-lookup"><span data-stu-id="6e124-118">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="6e124-119">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="6e124-119">numberOfOccurrences</span></span>|<span data-ttu-id="6e124-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6e124-120">Int32</span></span>|<span data-ttu-id="6e124-121">Количество повторений события.</span><span class="sxs-lookup"><span data-stu-id="6e124-121">The number of times to repeat the event.</span></span> <span data-ttu-id="6e124-122">Обязательное свойство, которое должно быть положительным, если для **type** задано значение `numbered`.</span><span class="sxs-lookup"><span data-stu-id="6e124-122">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="6e124-123">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="6e124-123">recurrenceTimeZone</span></span>|<span data-ttu-id="6e124-124">String</span><span class="sxs-lookup"><span data-stu-id="6e124-124">String</span></span> |<span data-ttu-id="6e124-125">Часовой пояс для свойств **startDate** и **endDate**.</span><span class="sxs-lookup"><span data-stu-id="6e124-125">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="6e124-126">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="6e124-126">Optional.</span></span> <span data-ttu-id="6e124-127">Если это свойство не задано, используется часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="6e124-127">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="6e124-128">startDate</span><span class="sxs-lookup"><span data-stu-id="6e124-128">startDate</span></span>|<span data-ttu-id="6e124-129">Date</span><span class="sxs-lookup"><span data-stu-id="6e124-129">Date</span></span>|<span data-ttu-id="6e124-130">Дата, с которой начинает применяться расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="6e124-130">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="6e124-131">В зависимости от того, каково расписание повторения события, первый экземпляр собрания может приходиться на эту или более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="6e124-131">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="6e124-132">Должно быть задано то же значение, что и для свойства **start** повторяющегося [события](event.md).</span><span class="sxs-lookup"><span data-stu-id="6e124-132">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="6e124-133">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="6e124-133">Required.</span></span>|
|<span data-ttu-id="6e124-134">type</span><span class="sxs-lookup"><span data-stu-id="6e124-134">type</span></span>|<span data-ttu-id="6e124-135">рекурренцеранжетипе</span><span class="sxs-lookup"><span data-stu-id="6e124-135">recurrenceRangeType</span></span>|<span data-ttu-id="6e124-136">Диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="6e124-136">The recurrence range.</span></span> <span data-ttu-id="6e124-137">Допустимые значения: `endDate`, `noEnd`, `numbered`.</span><span class="sxs-lookup"><span data-stu-id="6e124-137">The possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="6e124-138">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="6e124-138">Required.</span></span>|

<span data-ttu-id="6e124-139">С помощью свойства **type** можно указывать различные типы для **recurrenceRange**.</span><span class="sxs-lookup"><span data-stu-id="6e124-139">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="6e124-140">Обратите внимание на обязательные свойства для каждого типа, описанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="6e124-140">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="6e124-141">Свойство type</span><span class="sxs-lookup"><span data-stu-id="6e124-141">type property</span></span>  | <span data-ttu-id="6e124-142">Тип диапазона повторения</span><span class="sxs-lookup"><span data-stu-id="6e124-142">Type of recurrence range</span></span> | <span data-ttu-id="6e124-143">Описание</span><span class="sxs-lookup"><span data-stu-id="6e124-143">Description</span></span> | <span data-ttu-id="6e124-144">Пример</span><span class="sxs-lookup"><span data-stu-id="6e124-144">Example</span></span> | <span data-ttu-id="6e124-145">Обязательные свойства</span><span class="sxs-lookup"><span data-stu-id="6e124-145">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="6e124-146">Диапазон с датой окончания</span><span class="sxs-lookup"><span data-stu-id="6e124-146">Range with end date</span></span> | <span data-ttu-id="6e124-147">Событие повторяется во все дни, входящие в соответствующее расписание повторения, с даты **startDate** и до даты **endDate** включительно.</span><span class="sxs-lookup"><span data-stu-id="6e124-147">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="6e124-148">Повторение события с 1 июня 2017 г. до 15 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="6e124-148">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="6e124-149">**type**, **startDate**, **endDate**</span><span class="sxs-lookup"><span data-stu-id="6e124-149">**type**, **startDate**, **endDate**</span></span> | 
|`noEnd`  |<span data-ttu-id="6e124-150">Диапазон без даты окончания</span><span class="sxs-lookup"><span data-stu-id="6e124-150">Range without an end date</span></span> | <span data-ttu-id="6e124-151">Событие повторяется во все дни, входящие в соответствующее расписание повторения, начиная с даты **startDate**.</span><span class="sxs-lookup"><span data-stu-id="6e124-151">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="6e124-152">Бесконечное повторение события с 1 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="6e124-152">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="6e124-153">**type**, **startDate**</span><span class="sxs-lookup"><span data-stu-id="6e124-153">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="6e124-154">Диапазон с определенным количеством повторений</span><span class="sxs-lookup"><span data-stu-id="6e124-154">Range with specific number of occurrences</span></span> | <span data-ttu-id="6e124-155">Событие повторяется определенное количество раз (указанное в **numberOfOccurrences**) в соответствии с расписанием повторения, начиная с даты **startDate**.</span><span class="sxs-lookup"><span data-stu-id="6e124-155">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="6e124-156">Повторение события 10 раз с 1 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="6e124-156">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="6e124-157">**type**, **startDate**, **numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="6e124-157">**type**, **startDate**, **numberOfOccurrences**</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6e124-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e124-158">JSON representation</span></span>

<span data-ttu-id="6e124-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e124-159">Here is a JSON representation of the resource</span></span>

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
      "Warning: /api-reference/v1.0/resources/recurrencerange.md:
      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ],
  "tocPath": ""
}-->
