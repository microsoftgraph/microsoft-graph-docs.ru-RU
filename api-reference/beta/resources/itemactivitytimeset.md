---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 2ff3e1a2356c43457fe251928728632bd2228b10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809894"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="b9c00-102">Тип ресурса ItemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="b9c00-102">ItemActivityTimeSet resource type</span></span>

> <span data-ttu-id="b9c00-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9c00-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9c00-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9c00-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9c00-105">Ресурс **ItemActivityTimeSet** предоставляет сведения о том, когда было совершено [действие][activity] над элементом.</span><span class="sxs-lookup"><span data-stu-id="b9c00-105">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b9c00-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b9c00-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="b9c00-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9c00-107">Properties</span></span>

| <span data-ttu-id="b9c00-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b9c00-108">Property name</span></span>    | <span data-ttu-id="b9c00-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b9c00-109">Type</span></span>           | <span data-ttu-id="b9c00-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9c00-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="b9c00-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9c00-111">observedDateTime</span></span> | <span data-ttu-id="b9c00-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9c00-112">DateTimeOffset</span></span> | <span data-ttu-id="b9c00-113">Сведения о том, когда было обнаружено действие.</span><span class="sxs-lookup"><span data-stu-id="b9c00-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="b9c00-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9c00-114">recordedDateTime</span></span> | <span data-ttu-id="b9c00-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9c00-115">DateTimeOffset</span></span> | <span data-ttu-id="b9c00-116">Сведения о том, когда сведения об обнаружении действия были записаны в службе.</span><span class="sxs-lookup"><span data-stu-id="b9c00-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="b9c00-117">Разница между временем **обнаружения** и **записи** особенно важна для сценариев совместной работы в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="b9c00-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="b9c00-118">Если пользователь добавляет комментарий к файлу в автономном режиме, то время добавления этого комментария будет указано в свойстве **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="b9c00-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="b9c00-119">Позже при подключении пользователя к облаку и отправке изменений это время будет указано в свойстве **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="b9c00-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="b9c00-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="b9c00-120">Remarks</span></span>

<span data-ttu-id="b9c00-121">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b9c00-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
