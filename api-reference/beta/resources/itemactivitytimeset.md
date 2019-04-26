---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 474d20e08d96294a30029e764d0b01f5b0c6bfcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581619"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="48aea-102">Тип ресурса ItemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="48aea-102">ItemActivityTimeSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48aea-103">Ресурс **ItemActivityTimeSet** предоставляет сведения о том, когда было совершено [действие][activity] над элементом.</span><span class="sxs-lookup"><span data-stu-id="48aea-103">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="48aea-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="48aea-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="48aea-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="48aea-105">Properties</span></span>

| <span data-ttu-id="48aea-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="48aea-106">Property name</span></span>    | <span data-ttu-id="48aea-107">Тип</span><span class="sxs-lookup"><span data-stu-id="48aea-107">Type</span></span>           | <span data-ttu-id="48aea-108">Описание</span><span class="sxs-lookup"><span data-stu-id="48aea-108">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="48aea-109">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="48aea-109">observedDateTime</span></span> | <span data-ttu-id="48aea-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48aea-110">DateTimeOffset</span></span> | <span data-ttu-id="48aea-111">Сведения о том, когда было обнаружено действие.</span><span class="sxs-lookup"><span data-stu-id="48aea-111">When the activity was observed to take place.</span></span>
| <span data-ttu-id="48aea-112">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="48aea-112">recordedDateTime</span></span> | <span data-ttu-id="48aea-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48aea-113">DateTimeOffset</span></span> | <span data-ttu-id="48aea-114">Сведения о том, когда сведения об обнаружении действия были записаны в службе.</span><span class="sxs-lookup"><span data-stu-id="48aea-114">When the observation was recorded on the service.</span></span>

<span data-ttu-id="48aea-115">Разница между временем **обнаружения** и **записи** особенно важна для сценариев совместной работы в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="48aea-115">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="48aea-116">Если пользователь добавляет комментарий к файлу в автономном режиме, то время добавления этого комментария будет указано в свойстве **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="48aea-116">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="48aea-117">Позже при подключении пользователя к облаку и отправке изменений это время будет указано в свойстве **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="48aea-117">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="48aea-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="48aea-118">Remarks</span></span>

<span data-ttu-id="48aea-119">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="48aea-119">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
