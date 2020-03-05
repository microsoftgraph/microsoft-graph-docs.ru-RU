---
author: daspek
description: Ресурс ItemActivityTimeSet предоставляет сведения о том, когда было совершено действие над элементом.
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 33a9f4c42393c0c77c331889d8e77244de6226e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523109"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="65c5e-103">Тип ресурса ItemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="65c5e-103">ItemActivityTimeSet resource type</span></span>

<span data-ttu-id="65c5e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="65c5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65c5e-105">Ресурс **ItemActivityTimeSet** предоставляет сведения о том, когда было совершено [действие][activity] над элементом.</span><span class="sxs-lookup"><span data-stu-id="65c5e-105">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="65c5e-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65c5e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="65c5e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="65c5e-107">Properties</span></span>

| <span data-ttu-id="65c5e-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="65c5e-108">Property name</span></span>    | <span data-ttu-id="65c5e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="65c5e-109">Type</span></span>           | <span data-ttu-id="65c5e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="65c5e-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="65c5e-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="65c5e-111">observedDateTime</span></span> | <span data-ttu-id="65c5e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65c5e-112">DateTimeOffset</span></span> | <span data-ttu-id="65c5e-113">Сведения о том, когда было обнаружено действие.</span><span class="sxs-lookup"><span data-stu-id="65c5e-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="65c5e-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="65c5e-114">recordedDateTime</span></span> | <span data-ttu-id="65c5e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65c5e-115">DateTimeOffset</span></span> | <span data-ttu-id="65c5e-116">Сведения о том, когда сведения об обнаружении действия были записаны в службе.</span><span class="sxs-lookup"><span data-stu-id="65c5e-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="65c5e-117">Разница между временем **обнаружения** и **записи** особенно важна для сценариев совместной работы в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="65c5e-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="65c5e-118">Если пользователь добавляет комментарий к файлу в автономном режиме, то время добавления этого комментария будет указано в свойстве **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="65c5e-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="65c5e-119">Позже при подключении пользователя к облаку и отправке изменений это время будет указано в свойстве **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="65c5e-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="65c5e-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="65c5e-120">Remarks</span></span>

<span data-ttu-id="65c5e-121">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="65c5e-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
