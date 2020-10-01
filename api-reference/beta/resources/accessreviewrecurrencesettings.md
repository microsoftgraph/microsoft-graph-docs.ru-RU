---
title: Тип ресурса Акцессревиеврекурренцесеттингс
description: Указывает, что проверка доступа повторяется через регулярные промежутки времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ca66a818059efac84903f763e6be3c8a3b5c05a
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330181"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="ff105-103">Тип ресурса Акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="ff105-103">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="ff105-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff105-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff105-105">Тип ресурса **акцессревиеврекурренцесеттингс** используется в ресурсе [акцессревиевсеттингс](accessreviewsettings.md) и указывает, что проверка доступа повторяется через регулярные промежутки времени.</span><span class="sxs-lookup"><span data-stu-id="ff105-105">The **accessReviewRecurrenceSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies that the access review recurs at regular intervals.</span></span>

## <a name="properties"></a><span data-ttu-id="ff105-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff105-106">Properties</span></span>

| <span data-ttu-id="ff105-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff105-107">Property</span></span> | <span data-ttu-id="ff105-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ff105-108">Type</span></span> | <span data-ttu-id="ff105-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ff105-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="ff105-110">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="ff105-110">recurrenceType</span></span> | <span data-ttu-id="ff105-111">Строка</span><span class="sxs-lookup"><span data-stu-id="ff105-111">String</span></span> | <span data-ttu-id="ff105-112">Интервал повторения.</span><span class="sxs-lookup"><span data-stu-id="ff105-112">The recurrence interval.</span></span> <span data-ttu-id="ff105-113">Возможные ваулес: `onetime` , `weekly` , `monthly` , `quarterly` , `halfyearly` или `annual` .</span><span class="sxs-lookup"><span data-stu-id="ff105-113">Possible vaules: `onetime`, `weekly`, `monthly`, `quarterly`, `halfyearly` or `annual`.</span></span>                                                                   |
| <span data-ttu-id="ff105-114">рекурренцеендтипе</span><span class="sxs-lookup"><span data-stu-id="ff105-114">recurrenceEndType</span></span> | <span data-ttu-id="ff105-115">Строка</span><span class="sxs-lookup"><span data-stu-id="ff105-115">String</span></span> | <span data-ttu-id="ff105-116">Завершение повторения.</span><span class="sxs-lookup"><span data-stu-id="ff105-116">How the recurrence ends.</span></span> <span data-ttu-id="ff105-117">Возможные значения: `never` , `endBy` , `occurrences` , или `recurrenceCount` .</span><span class="sxs-lookup"><span data-stu-id="ff105-117">Possible values: `never`, `endBy`, `occurrences`, or `recurrenceCount`.</span></span> <span data-ttu-id="ff105-118">Если это так `never` , то отсутствует явный конец ряда повторений.</span><span class="sxs-lookup"><span data-stu-id="ff105-118">If it is `never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="ff105-119">Если это так `endBy` , повторение оканчивается на определенную дату.</span><span class="sxs-lookup"><span data-stu-id="ff105-119">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="ff105-120">Если это так `occurrences` , ряд завершается после `recurrenceCount` завершения экземпляров проверки.</span><span class="sxs-lookup"><span data-stu-id="ff105-120">If it is `occurrences`, then the series ends after `recurrenceCount` instances of the review have completed.</span></span> |
| <span data-ttu-id="ff105-121">дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="ff105-121">durationInDays</span></span> | <span data-ttu-id="ff105-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ff105-122">Int32</span></span> | <span data-ttu-id="ff105-123">Продолжительность повторения в днях.</span><span class="sxs-lookup"><span data-stu-id="ff105-123">The duration in days for recurrence.</span></span> |
| <span data-ttu-id="ff105-124">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="ff105-124">recurrenceCount</span></span> | <span data-ttu-id="ff105-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ff105-125">Int32</span></span> | <span data-ttu-id="ff105-126">Количество повторений, если значение параметра **рекурренцеендтипе** равно `occurrences` или 0 в противном случае.</span><span class="sxs-lookup"><span data-stu-id="ff105-126">The count of recurrences, if the value of **recurrenceEndType** is `occurrences`, or 0 otherwise.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff105-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff105-127">JSON representation</span></span>

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