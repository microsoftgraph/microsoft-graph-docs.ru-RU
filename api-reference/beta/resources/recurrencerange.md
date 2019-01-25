---
title: Тип ресурса recurrenceRange
description: 'Описывает диапазон дат, согласно которому повторяется событие. '
localization_priority: Normal
ms.openlocfilehash: cee5a06d8f76264cd7c98924c532c8f864cab87d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518970"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="e4938-103">Тип ресурса recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="e4938-103">recurrenceRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4938-104">Описывает диапазон дат, согласно которому повторяется [событие](event.md).</span><span class="sxs-lookup"><span data-stu-id="e4938-104">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="e4938-105">Вы можете задать диапазон дат для повторяющегося события одним из 3 способов (в зависимости от сценария).</span><span class="sxs-lookup"><span data-stu-id="e4938-105">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="e4938-106">Необходимо всегда указывать значение **startDate** для диапазона дат, но вы можете задать повторяющееся событие, которое перестает повторяться в определенный день либо повторяется бесконечно или определенное количество раз.</span><span class="sxs-lookup"><span data-stu-id="e4938-106">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="e4938-107">Обратите внимание, что фактические экземпляры события в диапазоне дат всегда соответствуют расписанию повторения, заданному для повторяющегося события.</span><span class="sxs-lookup"><span data-stu-id="e4938-107">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="e4938-108">Повторяющееся событие всегда определяется соответствующими ресурсами [recurrencePattern](recurrencepattern.md) (частотой повторения события) и **recurrenceRange** (продолжительностью повторения).</span><span class="sxs-lookup"><span data-stu-id="e4938-108">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>


## <a name="properties"></a><span data-ttu-id="e4938-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4938-109">Properties</span></span>

| <span data-ttu-id="e4938-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4938-110">Property</span></span>     | <span data-ttu-id="e4938-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e4938-111">Type</span></span>   |<span data-ttu-id="e4938-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e4938-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4938-113">endDate</span><span class="sxs-lookup"><span data-stu-id="e4938-113">endDate</span></span>|<span data-ttu-id="e4938-114">дата;</span><span class="sxs-lookup"><span data-stu-id="e4938-114">Date</span></span>|<span data-ttu-id="e4938-115">Дата, с которой перестает применяться расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="e4938-115">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="e4938-116">В зависимости от того, каково расписание повторения события, последний экземпляр собрания может приходиться на другую дату.</span><span class="sxs-lookup"><span data-stu-id="e4938-116">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="e4938-117">Обязательное, если для **type** задано значение `endDate`.</span><span class="sxs-lookup"><span data-stu-id="e4938-117">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="e4938-118">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="e4938-118">numberOfOccurrences</span></span>|<span data-ttu-id="e4938-119">Int32</span><span class="sxs-lookup"><span data-stu-id="e4938-119">Int32</span></span>|<span data-ttu-id="e4938-120">Количество повторений события.</span><span class="sxs-lookup"><span data-stu-id="e4938-120">The number of times to repeat the event.</span></span> <span data-ttu-id="e4938-121">Обязательное свойство, которое должно быть положительным, если для **type** задано значение `numbered`.</span><span class="sxs-lookup"><span data-stu-id="e4938-121">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="e4938-122">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="e4938-122">recurrenceTimeZone</span></span>|<span data-ttu-id="e4938-123">String</span><span class="sxs-lookup"><span data-stu-id="e4938-123">String</span></span> |<span data-ttu-id="e4938-124">Часовой пояс для свойств **startDate** и **endDate**.</span><span class="sxs-lookup"><span data-stu-id="e4938-124">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="e4938-125">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="e4938-125">Optional.</span></span> <span data-ttu-id="e4938-126">Если это свойство не задано, используется часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="e4938-126">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="e4938-127">startDate</span><span class="sxs-lookup"><span data-stu-id="e4938-127">startDate</span></span>|<span data-ttu-id="e4938-128">Date</span><span class="sxs-lookup"><span data-stu-id="e4938-128">Date</span></span>|<span data-ttu-id="e4938-129">Дата, с которой начинает применяться расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="e4938-129">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="e4938-130">В зависимости от того, каково расписание повторения события, первый экземпляр собрания может приходиться на эту или более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="e4938-130">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="e4938-131">Должно быть задано то же значение, что и для свойства **start** повторяющегося [события](event.md).</span><span class="sxs-lookup"><span data-stu-id="e4938-131">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="e4938-132">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="e4938-132">Required.</span></span>|
|<span data-ttu-id="e4938-133">type</span><span class="sxs-lookup"><span data-stu-id="e4938-133">type</span></span>|<span data-ttu-id="e4938-134">String</span><span class="sxs-lookup"><span data-stu-id="e4938-134">String</span></span>|<span data-ttu-id="e4938-135">Диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="e4938-135">The recurrence range.</span></span> <span data-ttu-id="e4938-136">Возможные значения: `endDate`, `noEnd`, `numbered`.</span><span class="sxs-lookup"><span data-stu-id="e4938-136">Possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="e4938-137">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="e4938-137">Required.</span></span>|

<span data-ttu-id="e4938-138">С помощью свойства **type** можно указывать различные типы для **recurrenceRange**.</span><span class="sxs-lookup"><span data-stu-id="e4938-138">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="e4938-139">Обратите внимание на обязательные свойства для каждого типа, описанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="e4938-139">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="e4938-140">Свойство type</span><span class="sxs-lookup"><span data-stu-id="e4938-140">type property</span></span>  | <span data-ttu-id="e4938-141">Тип диапазона повторения</span><span class="sxs-lookup"><span data-stu-id="e4938-141">Type of recurrence range</span></span> | <span data-ttu-id="e4938-142">Описание</span><span class="sxs-lookup"><span data-stu-id="e4938-142">Description</span></span> | <span data-ttu-id="e4938-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e4938-143">Example</span></span> | <span data-ttu-id="e4938-144">Обязательные свойства</span><span class="sxs-lookup"><span data-stu-id="e4938-144">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="e4938-145">Диапазон с датой окончания</span><span class="sxs-lookup"><span data-stu-id="e4938-145">Range with end date</span></span> | <span data-ttu-id="e4938-146">Событие повторяется во все дни, входящие в соответствующее расписание повторения, с даты **startDate** и до даты **endDate** включительно.</span><span class="sxs-lookup"><span data-stu-id="e4938-146">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="e4938-147">Повторение события с 1 июня 2017 г. до 15 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e4938-147">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="e4938-148">**type**, **startDate**, **endDate**</span><span class="sxs-lookup"><span data-stu-id="e4938-148">**type**, **startDate**, **endDate**</span></span> | 
|`noEnd`   |<span data-ttu-id="e4938-149">Диапазон без даты окончания</span><span class="sxs-lookup"><span data-stu-id="e4938-149">Range without an end date</span></span> | <span data-ttu-id="e4938-150">Событие повторяется во все дни, входящие в соответствующее расписание повторения, начиная с даты **startDate**.</span><span class="sxs-lookup"><span data-stu-id="e4938-150">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="e4938-151">Бесконечное повторение события с 1 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e4938-151">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="e4938-152">**type**, **startDate**</span><span class="sxs-lookup"><span data-stu-id="e4938-152">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="e4938-153">Диапазон с определенным количеством повторений</span><span class="sxs-lookup"><span data-stu-id="e4938-153">Range with specific number of occurrences</span></span> | <span data-ttu-id="e4938-154">Событие повторяется определенное количество раз (указанное в **numberOfOccurrences**) в соответствии с расписанием повторения, начиная с даты **startDate**.</span><span class="sxs-lookup"><span data-stu-id="e4938-154">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="e4938-155">Повторение события 10 раз с 1 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e4938-155">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="e4938-156">**type**, **startDate**, **numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="e4938-156">**type**, **startDate**, **numberOfOccurrences**</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e4938-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4938-157">JSON representation</span></span>

<span data-ttu-id="e4938-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4938-158">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/recurrencerange.md:\r\n      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |",
    "Error: /api-reference/beta/resources/recurrencerange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
