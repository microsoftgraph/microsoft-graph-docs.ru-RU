---
author: daspek
description: Ресурс ItemActivityTimeSet предоставляет сведения о том, когда было совершено действие над элементом.
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9295337237c681fd0ec02c9fa8061bf206059600
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075667"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="2d2e6-103">Тип ресурса ItemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="2d2e6-103">ItemActivityTimeSet resource type</span></span>

<span data-ttu-id="2d2e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d2e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d2e6-105">Ресурс **ItemActivityTimeSet** предоставляет сведения о том, когда было совершено [действие][activity] над элементом.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-105">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="2d2e6-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d2e6-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2d2e6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d2e6-107">Properties</span></span>

| <span data-ttu-id="2d2e6-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2d2e6-108">Property name</span></span>    | <span data-ttu-id="2d2e6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2d2e6-109">Type</span></span>           | <span data-ttu-id="2d2e6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2d2e6-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="2d2e6-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d2e6-111">observedDateTime</span></span> | <span data-ttu-id="2d2e6-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d2e6-112">DateTimeOffset</span></span> | <span data-ttu-id="2d2e6-113">Сведения о том, когда было обнаружено действие.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="2d2e6-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d2e6-114">recordedDateTime</span></span> | <span data-ttu-id="2d2e6-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d2e6-115">DateTimeOffset</span></span> | <span data-ttu-id="2d2e6-116">Сведения о том, когда сведения об обнаружении действия были записаны в службе.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="2d2e6-117">Разница между временем **обнаружения** и **записи** особенно важна для сценариев совместной работы в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="2d2e6-118">Если пользователь добавляет комментарий к файлу в автономном режиме, то время добавления этого комментария будет указано в свойстве **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="2d2e6-119">Позже при подключении пользователя к облаку и отправке изменений это время будет указано в свойстве **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="2d2e6-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="2d2e6-120">Remarks</span></span>

<span data-ttu-id="2d2e6-121">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2d2e6-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->


