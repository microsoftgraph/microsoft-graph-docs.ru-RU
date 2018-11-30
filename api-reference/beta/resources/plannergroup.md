---
title: Тип ресурса plannerGroup
description: Ресурс **plannerGroup** предоставляет доступ к ресурсам планировщик работы группы. Он не содержит какие-либо можно использовать свойства.
ms.openlocfilehash: 03db48d9525915ec58ee902922fa0292c0fd89ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077192"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="8c203-104">Тип ресурса plannerGroup</span><span class="sxs-lookup"><span data-stu-id="8c203-104">plannerGroup resource type</span></span>

> <span data-ttu-id="8c203-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8c203-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c203-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c203-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c203-p103">Ресурс **plannerGroup** предоставляет доступ к ресурсам Планировщика для [группы](group.md). Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="8c203-p103">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="8c203-109">Методы</span><span class="sxs-lookup"><span data-stu-id="8c203-109">Methods</span></span>

| <span data-ttu-id="8c203-110">Метод</span><span class="sxs-lookup"><span data-stu-id="8c203-110">Method</span></span>           | <span data-ttu-id="8c203-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8c203-111">Return Type</span></span>    |<span data-ttu-id="8c203-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8c203-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c203-113">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="8c203-113">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="8c203-114">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="8c203-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="8c203-115">Получение коллекции объектов **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="8c203-115">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c203-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c203-116">Properties</span></span>
| <span data-ttu-id="8c203-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c203-117">Property</span></span>     | <span data-ttu-id="8c203-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8c203-118">Type</span></span>   |<span data-ttu-id="8c203-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8c203-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c203-120">id</span><span class="sxs-lookup"><span data-stu-id="8c203-120">id</span></span>|<span data-ttu-id="8c203-121">String</span><span class="sxs-lookup"><span data-stu-id="8c203-121">String</span></span>| <span data-ttu-id="8c203-p104">Только для чтения. Идентификатор объекта **plannerGroup**.</span><span class="sxs-lookup"><span data-stu-id="8c203-p104">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c203-124">Связи</span><span class="sxs-lookup"><span data-stu-id="8c203-124">Relationships</span></span>
| <span data-ttu-id="8c203-125">Связь</span><span class="sxs-lookup"><span data-stu-id="8c203-125">Relationship</span></span> | <span data-ttu-id="8c203-126">Тип</span><span class="sxs-lookup"><span data-stu-id="8c203-126">Type</span></span>   |<span data-ttu-id="8c203-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8c203-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c203-128">plans</span><span class="sxs-lookup"><span data-stu-id="8c203-128">plans</span></span>|<span data-ttu-id="8c203-129">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="8c203-129">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="8c203-p105">Только для чтения. Допускает значение null. Возвращает экземпляры [plannerPlan](plannerplan.md), принадлежащие группе.</span><span class="sxs-lookup"><span data-stu-id="8c203-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c203-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8c203-133">JSON representation</span></span>
<span data-ttu-id="8c203-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c203-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->