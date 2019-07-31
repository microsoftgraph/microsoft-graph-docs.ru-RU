---
author: daspek
description: Ресурс ItemActivityTimeSet предоставляет сведения о том, когда было совершено действие над элементом.
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c81bf7885ee1466e293236a987e90e21323daefd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010093"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="212be-103">Тип ресурса ItemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="212be-103">ItemActivityTimeSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="212be-104">Ресурс **ItemActivityTimeSet** предоставляет сведения о том, когда было совершено [действие][activity] над элементом.</span><span class="sxs-lookup"><span data-stu-id="212be-104">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="212be-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="212be-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="212be-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="212be-106">Properties</span></span>

| <span data-ttu-id="212be-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="212be-107">Property name</span></span>    | <span data-ttu-id="212be-108">Тип</span><span class="sxs-lookup"><span data-stu-id="212be-108">Type</span></span>           | <span data-ttu-id="212be-109">Описание</span><span class="sxs-lookup"><span data-stu-id="212be-109">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="212be-110">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="212be-110">observedDateTime</span></span> | <span data-ttu-id="212be-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="212be-111">DateTimeOffset</span></span> | <span data-ttu-id="212be-112">Сведения о том, когда было обнаружено действие.</span><span class="sxs-lookup"><span data-stu-id="212be-112">When the activity was observed to take place.</span></span>
| <span data-ttu-id="212be-113">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="212be-113">recordedDateTime</span></span> | <span data-ttu-id="212be-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="212be-114">DateTimeOffset</span></span> | <span data-ttu-id="212be-115">Сведения о том, когда сведения об обнаружении действия были записаны в службе.</span><span class="sxs-lookup"><span data-stu-id="212be-115">When the observation was recorded on the service.</span></span>

<span data-ttu-id="212be-116">Разница между временем **обнаружения** и **записи** особенно важна для сценариев совместной работы в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="212be-116">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="212be-117">Если пользователь добавляет комментарий к файлу в автономном режиме, то время добавления этого комментария будет указано в свойстве **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="212be-117">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="212be-118">Позже при подключении пользователя к облаку и отправке изменений это время будет указано в свойстве **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="212be-118">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="212be-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="212be-119">Remarks</span></span>

<span data-ttu-id="212be-120">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="212be-120">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
