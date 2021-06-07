---
title: тип ресурса accessReviewRecurrenceSettings
description: Указывает, что обзор доступа повторяется через регулярные промежутки времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb2a05589bfa92331a213a489bfb2a5129850065
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755660"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="cbfcf-103">тип ресурса accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="cbfcf-103">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="cbfcf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbfcf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

<span data-ttu-id="cbfcf-105">Тип **ресурса accessReviewRecurrenceSettings** используется в [ресурсе accessReviewSettings](accessreviewsettings.md) и указывает, что обзор доступа повторяется регулярно.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-105">The **accessReviewRecurrenceSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies that the access review recurs at regular intervals.</span></span>

## <a name="properties"></a><span data-ttu-id="cbfcf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbfcf-106">Properties</span></span>

| <span data-ttu-id="cbfcf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbfcf-107">Property</span></span> | <span data-ttu-id="cbfcf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cbfcf-108">Type</span></span> | <span data-ttu-id="cbfcf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cbfcf-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="cbfcf-110">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="cbfcf-110">recurrenceType</span></span> | <span data-ttu-id="cbfcf-111">String</span><span class="sxs-lookup"><span data-stu-id="cbfcf-111">String</span></span> | <span data-ttu-id="cbfcf-112">Интервал повторяемости.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-112">The recurrence interval.</span></span> <span data-ttu-id="cbfcf-113">Возможные vaules: `onetime` , , , , или `weekly` `monthly` `quarterly` `halfyearly` `annual` .</span><span class="sxs-lookup"><span data-stu-id="cbfcf-113">Possible vaules: `onetime`, `weekly`, `monthly`, `quarterly`, `halfyearly` or `annual`.</span></span>                                                                   |
| <span data-ttu-id="cbfcf-114">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="cbfcf-114">recurrenceEndType</span></span> | <span data-ttu-id="cbfcf-115">String</span><span class="sxs-lookup"><span data-stu-id="cbfcf-115">String</span></span> | <span data-ttu-id="cbfcf-116">Как заканчивается повторение.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-116">How the recurrence ends.</span></span> <span data-ttu-id="cbfcf-117">Возможные значения: `never` `endBy` , , или `occurrences` `recurrenceCount` .</span><span class="sxs-lookup"><span data-stu-id="cbfcf-117">Possible values: `never`, `endBy`, `occurrences`, or `recurrenceCount`.</span></span> <span data-ttu-id="cbfcf-118">Если это так, то явный конец серии рецидивов `never` не существует.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-118">If it is `never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="cbfcf-119">Если это `endBy` так, то повторение заканчивается в определенный срок.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-119">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="cbfcf-120">Если это так, то серия заканчивается после завершения экземпляров `occurrences` `recurrenceCount` проверки.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-120">If it is `occurrences`, then the series ends after `recurrenceCount` instances of the review have completed.</span></span> |
| <span data-ttu-id="cbfcf-121">durationInDays</span><span class="sxs-lookup"><span data-stu-id="cbfcf-121">durationInDays</span></span> | <span data-ttu-id="cbfcf-122">Int32</span><span class="sxs-lookup"><span data-stu-id="cbfcf-122">Int32</span></span> | <span data-ttu-id="cbfcf-123">Продолжительность в днях для повторения.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-123">The duration in days for recurrence.</span></span> |
| <span data-ttu-id="cbfcf-124">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="cbfcf-124">recurrenceCount</span></span> | <span data-ttu-id="cbfcf-125">Int32</span><span class="sxs-lookup"><span data-stu-id="cbfcf-125">Int32</span></span> | <span data-ttu-id="cbfcf-126">Количество повторерений, если значение **recurrenceEndType** является `occurrences` или `0` иным образом.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-126">The count of recurrences, if the value of **recurrenceEndType** is `occurrences`, or `0` otherwise.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cbfcf-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbfcf-127">JSON representation</span></span>

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
