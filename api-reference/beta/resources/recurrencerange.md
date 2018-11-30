---
title: Тип ресурса recurrenceRange
description: 'Описывает диапазон дат, согласно которому повторяется событие. '
ms.openlocfilehash: f3d627606dc9d0d41dd52f735ab87052d731af0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077906"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="04afa-103">Тип ресурса recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="04afa-103">recurrenceRange resource type</span></span>

> <span data-ttu-id="04afa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04afa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04afa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04afa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04afa-106">Описывает диапазон дат, согласно которому повторяется [событие](event.md).</span><span class="sxs-lookup"><span data-stu-id="04afa-106">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="04afa-107">Вы можете задать диапазон дат для повторяющегося события одним из 3 способов (в зависимости от сценария).</span><span class="sxs-lookup"><span data-stu-id="04afa-107">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="04afa-108">Необходимо всегда указывать значение **startDate** для диапазона дат, но вы можете задать повторяющееся событие, которое перестает повторяться в определенный день либо повторяется бесконечно или определенное количество раз.</span><span class="sxs-lookup"><span data-stu-id="04afa-108">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="04afa-109">Обратите внимание, что фактические экземпляры события в диапазоне дат всегда соответствуют расписанию повторения, заданному для повторяющегося события.</span><span class="sxs-lookup"><span data-stu-id="04afa-109">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="04afa-110">Повторяющееся событие всегда определяется соответствующими ресурсами [recurrencePattern](recurrencepattern.md) (частотой повторения события) и **recurrenceRange** (продолжительностью повторения).</span><span class="sxs-lookup"><span data-stu-id="04afa-110">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>


## <a name="properties"></a><span data-ttu-id="04afa-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="04afa-111">Properties</span></span>

| <span data-ttu-id="04afa-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="04afa-112">Property</span></span>     | <span data-ttu-id="04afa-113">Тип</span><span class="sxs-lookup"><span data-stu-id="04afa-113">Type</span></span>   |<span data-ttu-id="04afa-114">Описание</span><span class="sxs-lookup"><span data-stu-id="04afa-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04afa-115">endDate</span><span class="sxs-lookup"><span data-stu-id="04afa-115">endDate</span></span>|<span data-ttu-id="04afa-116">Date</span><span class="sxs-lookup"><span data-stu-id="04afa-116">Date</span></span>|<span data-ttu-id="04afa-117">Дата, с которой перестает применяться расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="04afa-117">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="04afa-118">В зависимости от того, каково расписание повторения события, последний экземпляр собрания может приходиться на другую дату.</span><span class="sxs-lookup"><span data-stu-id="04afa-118">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="04afa-119">Обязательное, если для **type** задано значение `endDate`.</span><span class="sxs-lookup"><span data-stu-id="04afa-119">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="04afa-120">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="04afa-120">numberOfOccurrences</span></span>|<span data-ttu-id="04afa-121">Int32</span><span class="sxs-lookup"><span data-stu-id="04afa-121">Int32</span></span>|<span data-ttu-id="04afa-122">Количество повторений события.</span><span class="sxs-lookup"><span data-stu-id="04afa-122">The number of times to repeat the event.</span></span> <span data-ttu-id="04afa-123">Обязательное свойство, которое должно быть положительным, если для **type** задано значение `numbered`.</span><span class="sxs-lookup"><span data-stu-id="04afa-123">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="04afa-124">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="04afa-124">recurrenceTimeZone</span></span>|<span data-ttu-id="04afa-125">String</span><span class="sxs-lookup"><span data-stu-id="04afa-125">String</span></span> |<span data-ttu-id="04afa-126">Часовой пояс для свойств **startDate** и **endDate**.</span><span class="sxs-lookup"><span data-stu-id="04afa-126">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="04afa-127">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="04afa-127">Optional.</span></span> <span data-ttu-id="04afa-128">Если это свойство не задано, используется часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="04afa-128">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="04afa-129">startDate</span><span class="sxs-lookup"><span data-stu-id="04afa-129">startDate</span></span>|<span data-ttu-id="04afa-130">Date</span><span class="sxs-lookup"><span data-stu-id="04afa-130">Date</span></span>|<span data-ttu-id="04afa-131">Дата, с которой начинает применяться расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="04afa-131">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="04afa-132">В зависимости от того, каково расписание повторения события, первый экземпляр собрания может приходиться на эту или более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="04afa-132">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="04afa-133">Должно быть задано то же значение, что и для свойства **start** повторяющегося [события](event.md).</span><span class="sxs-lookup"><span data-stu-id="04afa-133">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="04afa-134">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="04afa-134">Required.</span></span>|
|<span data-ttu-id="04afa-135">type</span><span class="sxs-lookup"><span data-stu-id="04afa-135">type</span></span>|<span data-ttu-id="04afa-136">String</span><span class="sxs-lookup"><span data-stu-id="04afa-136">String</span></span>|<span data-ttu-id="04afa-137">Диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="04afa-137">The recurrence range.</span></span> <span data-ttu-id="04afa-138">Возможные значения: `endDate`, `noEnd`, `numbered`.</span><span class="sxs-lookup"><span data-stu-id="04afa-138">Possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="04afa-139">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="04afa-139">Required.</span></span>|

<span data-ttu-id="04afa-140">С помощью свойства **type** можно указывать различные типы для **recurrenceRange**.</span><span class="sxs-lookup"><span data-stu-id="04afa-140">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="04afa-141">Обратите внимание на обязательные свойства для каждого типа, описанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="04afa-141">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="04afa-142">Свойство type</span><span class="sxs-lookup"><span data-stu-id="04afa-142">type property</span></span>  | <span data-ttu-id="04afa-143">Тип диапазона повторения</span><span class="sxs-lookup"><span data-stu-id="04afa-143">Type of recurrence range</span></span> | <span data-ttu-id="04afa-144">Описание</span><span class="sxs-lookup"><span data-stu-id="04afa-144">Description</span></span> | <span data-ttu-id="04afa-145">Пример</span><span class="sxs-lookup"><span data-stu-id="04afa-145">Example</span></span> | <span data-ttu-id="04afa-146">Обязательные свойства</span><span class="sxs-lookup"><span data-stu-id="04afa-146">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="04afa-147">Диапазон с датой окончания</span><span class="sxs-lookup"><span data-stu-id="04afa-147">Range with end date</span></span> | <span data-ttu-id="04afa-148">Событие повторяется во все дни, входящие в соответствующее расписание повторения, с даты **startDate** и до даты **endDate** включительно.</span><span class="sxs-lookup"><span data-stu-id="04afa-148">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="04afa-149">Повторение события с 1 июня 2017 г. до 15 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="04afa-149">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="04afa-150">**type**, **startDate**, **endDate**</span><span class="sxs-lookup"><span data-stu-id="04afa-150">**type**, **startDate**, **endDate**</span></span> | 
|`noEnd`   |<span data-ttu-id="04afa-151">Диапазон без даты окончания</span><span class="sxs-lookup"><span data-stu-id="04afa-151">Range without an end date</span></span> | <span data-ttu-id="04afa-152">Событие повторяется во все дни, входящие в соответствующее расписание повторения, начиная с даты **startDate**.</span><span class="sxs-lookup"><span data-stu-id="04afa-152">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="04afa-153">Бесконечное повторение события с 1 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="04afa-153">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="04afa-154">**type**, **startDate**</span><span class="sxs-lookup"><span data-stu-id="04afa-154">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="04afa-155">Диапазон с определенным количеством повторений</span><span class="sxs-lookup"><span data-stu-id="04afa-155">Range with specific number of occurrences</span></span> | <span data-ttu-id="04afa-156">Событие повторяется определенное количество раз (указанное в **numberOfOccurrences**) в соответствии с расписанием повторения, начиная с даты **startDate**.</span><span class="sxs-lookup"><span data-stu-id="04afa-156">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="04afa-157">Повторение события 10 раз с 1 июня 2017 г.</span><span class="sxs-lookup"><span data-stu-id="04afa-157">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="04afa-158">**type**, **startDate**, **numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="04afa-158">**type**, **startDate**, **numberOfOccurrences**</span></span> |

## <a name="json-representation"></a><span data-ttu-id="04afa-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04afa-159">JSON representation</span></span>

<span data-ttu-id="04afa-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04afa-160">Here is a JSON representation of the resource</span></span>

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
      "Warning: /api-reference/beta/resources/recurrencerange.md:
      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ],
  "tocPath": ""
}-->
