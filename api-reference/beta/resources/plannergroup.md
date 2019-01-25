---
title: Тип ресурса plannerGroup
description: Ресурс **plannerGroup** предоставляет доступ к ресурсам Планировщика для группы. Он не содержит свойства, которые можно использовать.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84bb20d0b13f9a99db2f8c59b20e0c9c7c87f93f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513783"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="a3a6e-104">Тип ресурса plannerGroup</span><span class="sxs-lookup"><span data-stu-id="a3a6e-104">plannerGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3a6e-p102">Ресурс **plannerGroup** предоставляет доступ к ресурсам Планировщика для [группы](group.md). Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="a3a6e-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="a3a6e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a3a6e-107">Methods</span></span>

| <span data-ttu-id="a3a6e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a3a6e-108">Method</span></span>           | <span data-ttu-id="a3a6e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3a6e-109">Return Type</span></span>    |<span data-ttu-id="a3a6e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a6e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3a6e-111">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="a3a6e-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="a3a6e-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="a3a6e-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="a3a6e-113">Получение коллекции объектов **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="a3a6e-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3a6e-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3a6e-114">Properties</span></span>
| <span data-ttu-id="a3a6e-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3a6e-115">Property</span></span>     | <span data-ttu-id="a3a6e-116">Тип</span><span class="sxs-lookup"><span data-stu-id="a3a6e-116">Type</span></span>   |<span data-ttu-id="a3a6e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a6e-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3a6e-118">id</span><span class="sxs-lookup"><span data-stu-id="a3a6e-118">id</span></span>|<span data-ttu-id="a3a6e-119">String</span><span class="sxs-lookup"><span data-stu-id="a3a6e-119">String</span></span>| <span data-ttu-id="a3a6e-p103">Только для чтения. Идентификатор объекта **plannerGroup**.</span><span class="sxs-lookup"><span data-stu-id="a3a6e-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3a6e-122">Связи</span><span class="sxs-lookup"><span data-stu-id="a3a6e-122">Relationships</span></span>
| <span data-ttu-id="a3a6e-123">Связь</span><span class="sxs-lookup"><span data-stu-id="a3a6e-123">Relationship</span></span> | <span data-ttu-id="a3a6e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a3a6e-124">Type</span></span>   |<span data-ttu-id="a3a6e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a6e-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3a6e-126">plans</span><span class="sxs-lookup"><span data-stu-id="a3a6e-126">plans</span></span>|<span data-ttu-id="a3a6e-127">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="a3a6e-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="a3a6e-p104">Только для чтения. Допускает значение null. Возвращает экземпляры [plannerPlan](plannerplan.md), принадлежащие группе.</span><span class="sxs-lookup"><span data-stu-id="a3a6e-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3a6e-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a3a6e-131">JSON representation</span></span>
<span data-ttu-id="a3a6e-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3a6e-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
