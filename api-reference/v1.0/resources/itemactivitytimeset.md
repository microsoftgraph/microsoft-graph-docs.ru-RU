---
author: daspek
title: Тип ресурса itemActivityTimeSet
description: Объект itemActionSet предоставляет сведения о действии, которое произошло с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1f614c597efdb95b04c4079bd68240aa865d66dd
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238675"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="ca0a0-103">Тип ресурса itemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="ca0a0-103">itemActivityTimeSet resource type</span></span>

<span data-ttu-id="ca0a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca0a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca0a0-105">Ресурс **itemActivityTimeSet** предоставляет сведения [][activity] о том, когда произошло действие с элементом.</span><span class="sxs-lookup"><span data-stu-id="ca0a0-105">The **itemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

><span data-ttu-id="ca0a0-106">**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ca0a0-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="ca0a0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca0a0-107">Properties</span></span>

| <span data-ttu-id="ca0a0-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ca0a0-108">Property name</span></span>    | <span data-ttu-id="ca0a0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ca0a0-109">Type</span></span>           | <span data-ttu-id="ca0a0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ca0a0-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="ca0a0-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca0a0-111">observedDateTime</span></span> | <span data-ttu-id="ca0a0-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca0a0-112">DateTimeOffset</span></span> | <span data-ttu-id="ca0a0-113">Сведения о том, когда было обнаружено действие.</span><span class="sxs-lookup"><span data-stu-id="ca0a0-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="ca0a0-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca0a0-114">recordedDateTime</span></span> | <span data-ttu-id="ca0a0-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca0a0-115">DateTimeOffset</span></span> | <span data-ttu-id="ca0a0-116">Сведения о том, когда сведения об обнаружении действия были записаны в службе.</span><span class="sxs-lookup"><span data-stu-id="ca0a0-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="ca0a0-117">Разница между временем **обнаружения** и **записи** особенно важна для сценариев совместной работы в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="ca0a0-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="ca0a0-118">Если пользователь добавляет комментарий к файлу в автономном режиме, то время добавления этого комментария будет указано в свойстве **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="ca0a0-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="ca0a0-119">Позже при подключении пользователя к облаку и отправке изменений это время будет указано в свойстве **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="ca0a0-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca0a0-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca0a0-120">JSON representation</span></span>

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

