---
title: Тип ресурса plannerPlanContext
description: Ресурс **plannerPlanContext** представляет отношение plannerPlan взаимодействия с пользователем вне планировщик работы. Планы в планировщике можно отображаются в других каждый раз, такие как группами Майкрософт, для отслеживания работ в контексте этот опыт.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 76260b51bc6f77acf6fac22e80bd676edd8b8e11
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509240"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="080a4-104">Тип ресурса plannerPlanContext</span><span class="sxs-lookup"><span data-stu-id="080a4-104">plannerPlanContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="080a4-105">Ресурс **plannerPlanContext** представляет отношение [plannerPlan](plannerplan.md) взаимодействия с пользователем вне планировщик работы.</span><span class="sxs-lookup"><span data-stu-id="080a4-105">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="080a4-106">Планы в планировщике можно отображаются в других каждый раз, такие как группами Майкрософт, для отслеживания работ в контексте этот опыт.</span><span class="sxs-lookup"><span data-stu-id="080a4-106">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="080a4-107">Представляет запись **plannerPlanContext** опытом, можно определить на основе свойства **ownerAppId** .</span><span class="sxs-lookup"><span data-stu-id="080a4-107">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="080a4-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: запись контекста относится к группам Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="080a4-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="080a4-109">00000003-0000-0ff1-ce00-000000000000: запись контекста относится к SharePoint.</span><span class="sxs-lookup"><span data-stu-id="080a4-109">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="080a4-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="080a4-110">Properties</span></span>
| <span data-ttu-id="080a4-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="080a4-111">Property</span></span>     | <span data-ttu-id="080a4-112">Тип</span><span class="sxs-lookup"><span data-stu-id="080a4-112">Type</span></span>   |<span data-ttu-id="080a4-113">Описание</span><span class="sxs-lookup"><span data-stu-id="080a4-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="080a4-114">associationType</span><span class="sxs-lookup"><span data-stu-id="080a4-114">associationType</span></span>|<span data-ttu-id="080a4-115">String</span><span class="sxs-lookup"><span data-stu-id="080a4-115">String</span></span>|<span data-ttu-id="080a4-116">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="080a4-116">Nullable.</span></span> <span data-ttu-id="080a4-117">Тип связи между [plannerPlan](plannerplan.md) и приложения в определенных приложений.</span><span class="sxs-lookup"><span data-stu-id="080a4-117">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="080a4-118">Приложения могут использовать эти сведения для отслеживания различных типов отношений же [plannerPlan](plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="080a4-118">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="080a4-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="080a4-119">createdDateTime</span></span>|<span data-ttu-id="080a4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="080a4-120">DateTimeOffset</span></span>|<span data-ttu-id="080a4-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="080a4-121">Read-only.</span></span> <span data-ttu-id="080a4-122">Дата и время создания **plannerPlanContext** .</span><span class="sxs-lookup"><span data-stu-id="080a4-122">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="080a4-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="080a4-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="080a4-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="080a4-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="080a4-125">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="080a4-125">displayNameSegments</span></span>|<span data-ttu-id="080a4-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="080a4-126">String collection</span></span>|<span data-ttu-id="080a4-127">Сегменты имя внешнего интерфейса.</span><span class="sxs-lookup"><span data-stu-id="080a4-127">The segments of the name of the external experience.</span></span> <span data-ttu-id="080a4-128">Сегменты представления иерархической структуры, обеспечивающий другие приложения отобразить отношение.</span><span class="sxs-lookup"><span data-stu-id="080a4-128">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="080a4-129">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="080a4-129">ownerAppId</span></span>|<span data-ttu-id="080a4-130">String</span><span class="sxs-lookup"><span data-stu-id="080a4-130">String</span></span>|<span data-ttu-id="080a4-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="080a4-131">Read-only.</span></span> <span data-ttu-id="080a4-132">Идентификатор приложения, которые созданы **plannerPlanContext**.</span><span class="sxs-lookup"><span data-stu-id="080a4-132">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="080a4-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="080a4-133">JSON representation</span></span>

<span data-ttu-id="080a4-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="080a4-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontext.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
