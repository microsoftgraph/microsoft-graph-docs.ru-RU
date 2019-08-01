---
author: daspek
ms.author: dspektor
title: Тип ресурса itemActivityTimeSet
description: Объект itemActionSet предоставляет сведения о действиях, которые были выполнены над элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9dce21afc1acc8e93181204e026f74a597c9120f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036591"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="05e6d-103">Тип ресурса itemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="05e6d-103">itemActivityTimeSet resource type</span></span>

<span data-ttu-id="05e6d-104">Ресурс **itemActivityTimeSet** предоставляет сведения о том, когда выполнялось [действие][activity] для элемента.</span><span class="sxs-lookup"><span data-stu-id="05e6d-104">The **itemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

><span data-ttu-id="05e6d-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="05e6d-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="05e6d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="05e6d-106">Properties</span></span>

| <span data-ttu-id="05e6d-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="05e6d-107">Property name</span></span>    | <span data-ttu-id="05e6d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="05e6d-108">Type</span></span>           | <span data-ttu-id="05e6d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="05e6d-109">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="05e6d-110">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="05e6d-110">observedDateTime</span></span> | <span data-ttu-id="05e6d-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05e6d-111">DateTimeOffset</span></span> | <span data-ttu-id="05e6d-112">Сведения о том, когда было обнаружено действие.</span><span class="sxs-lookup"><span data-stu-id="05e6d-112">When the activity was observed to take place.</span></span>
| <span data-ttu-id="05e6d-113">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="05e6d-113">recordedDateTime</span></span> | <span data-ttu-id="05e6d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05e6d-114">DateTimeOffset</span></span> | <span data-ttu-id="05e6d-115">Сведения о том, когда сведения об обнаружении действия были записаны в службе.</span><span class="sxs-lookup"><span data-stu-id="05e6d-115">When the observation was recorded on the service.</span></span>

<span data-ttu-id="05e6d-116">Разница между временем **обнаружения** и **записи** особенно важна для сценариев совместной работы в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="05e6d-116">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="05e6d-117">Если пользователь добавляет комментарий к файлу в автономном режиме, то время добавления этого комментария будет указано в свойстве **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="05e6d-117">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="05e6d-118">Позже при подключении пользователя к облаку и отправке изменений это время будет указано в свойстве **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="05e6d-118">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05e6d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05e6d-119">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
