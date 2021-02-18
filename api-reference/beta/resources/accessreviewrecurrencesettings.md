---
title: Тип ресурса accessReviewRecurrenceSettings
description: Указывает, что проверка доступа повторяется с регулярными интервалами.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9a39881a7675598d12de79f2738a1e14d1c759b3
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292926"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="00cb6-103">Тип ресурса accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="00cb6-103">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="00cb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00cb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

<span data-ttu-id="00cb6-105">Тип ресурса **accessReviewRecurrenceSettings** используется в ресурсе [accessReviewSettings](accessreviewsettings.md) и указывает, что проверка доступа повторяется с регулярными интервалами.</span><span class="sxs-lookup"><span data-stu-id="00cb6-105">The **accessReviewRecurrenceSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies that the access review recurs at regular intervals.</span></span>

## <a name="properties"></a><span data-ttu-id="00cb6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="00cb6-106">Properties</span></span>

| <span data-ttu-id="00cb6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="00cb6-107">Property</span></span> | <span data-ttu-id="00cb6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="00cb6-108">Type</span></span> | <span data-ttu-id="00cb6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="00cb6-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="00cb6-110">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="00cb6-110">recurrenceType</span></span> | <span data-ttu-id="00cb6-111">String</span><span class="sxs-lookup"><span data-stu-id="00cb6-111">String</span></span> | <span data-ttu-id="00cb6-112">Интервал повторения.</span><span class="sxs-lookup"><span data-stu-id="00cb6-112">The recurrence interval.</span></span> <span data-ttu-id="00cb6-113">Возможные vaules: `onetime` , , , , или `weekly` `monthly` `quarterly` `halfyearly` `annual` .</span><span class="sxs-lookup"><span data-stu-id="00cb6-113">Possible vaules: `onetime`, `weekly`, `monthly`, `quarterly`, `halfyearly` or `annual`.</span></span>                                                                   |
| <span data-ttu-id="00cb6-114">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="00cb6-114">recurrenceEndType</span></span> | <span data-ttu-id="00cb6-115">String</span><span class="sxs-lookup"><span data-stu-id="00cb6-115">String</span></span> | <span data-ttu-id="00cb6-116">Как заканчивается повторение.</span><span class="sxs-lookup"><span data-stu-id="00cb6-116">How the recurrence ends.</span></span> <span data-ttu-id="00cb6-117">Возможные значения: `never` , , , или `endBy` `occurrences` `recurrenceCount` .</span><span class="sxs-lookup"><span data-stu-id="00cb6-117">Possible values: `never`, `endBy`, `occurrences`, or `recurrenceCount`.</span></span> <span data-ttu-id="00cb6-118">Если это так, явный конец серии `never` повторения не существует.</span><span class="sxs-lookup"><span data-stu-id="00cb6-118">If it is `never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="00cb6-119">Если это `endBy` так, то повторение завершается в определенную дату.</span><span class="sxs-lookup"><span data-stu-id="00cb6-119">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="00cb6-120">Если это так, серия завершается после завершения `occurrences` `recurrenceCount` экземпляров проверки.</span><span class="sxs-lookup"><span data-stu-id="00cb6-120">If it is `occurrences`, then the series ends after `recurrenceCount` instances of the review have completed.</span></span> |
| <span data-ttu-id="00cb6-121">durationInDays</span><span class="sxs-lookup"><span data-stu-id="00cb6-121">durationInDays</span></span> | <span data-ttu-id="00cb6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="00cb6-122">Int32</span></span> | <span data-ttu-id="00cb6-123">Продолжительность повторения в днях.</span><span class="sxs-lookup"><span data-stu-id="00cb6-123">The duration in days for recurrence.</span></span> |
| <span data-ttu-id="00cb6-124">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="00cb6-124">recurrenceCount</span></span> | <span data-ttu-id="00cb6-125">Int32</span><span class="sxs-lookup"><span data-stu-id="00cb6-125">Int32</span></span> | <span data-ttu-id="00cb6-126">Количество повторерений, если значение **recurrenceEndType** — `occurrences` или 0 в противном случае.</span><span class="sxs-lookup"><span data-stu-id="00cb6-126">The count of recurrences, if the value of **recurrenceEndType** is `occurrences`, or 0 otherwise.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="00cb6-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00cb6-127">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
```json
{
  "recurrenceType": "string",
  "recurrenceEndType": "string",
  "durationInDays": 1024,
  "recurrenceCount": 1024
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewRecurrenceSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
