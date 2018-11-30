---
title: Тип ресурса plannerPlanContext
description: Ресурс **plannerPlanContext** представляет отношение plannerPlan взаимодействия с пользователем вне планировщик работы. Планы в планировщике можно отображаются в других каждый раз, такие как группами Майкрософт, для отслеживания работ в контексте этот опыт.
ms.openlocfilehash: 84512c03081a3e1fd2b15456c64cecf3f9c39435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078967"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="27911-104">Тип ресурса plannerPlanContext</span><span class="sxs-lookup"><span data-stu-id="27911-104">plannerPlanContext resource type</span></span>

> <span data-ttu-id="27911-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="27911-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27911-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27911-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27911-107">Ресурс **plannerPlanContext** представляет отношение [plannerPlan](plannerplan.md) взаимодействия с пользователем вне планировщик работы.</span><span class="sxs-lookup"><span data-stu-id="27911-107">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="27911-108">Планы в планировщике можно отображаются в других каждый раз, такие как группами Майкрософт, для отслеживания работ в контексте этот опыт.</span><span class="sxs-lookup"><span data-stu-id="27911-108">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="27911-109">Представляет запись **plannerPlanContext** опытом, можно определить на основе свойства **ownerAppId** .</span><span class="sxs-lookup"><span data-stu-id="27911-109">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="27911-110">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: запись контекста относится к группам Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="27911-110">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="27911-111">00000003-0000-0ff1-ce00-000000000000: запись контекста относится к SharePoint.</span><span class="sxs-lookup"><span data-stu-id="27911-111">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="27911-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="27911-112">Properties</span></span>
| <span data-ttu-id="27911-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="27911-113">Property</span></span>     | <span data-ttu-id="27911-114">Тип</span><span class="sxs-lookup"><span data-stu-id="27911-114">Type</span></span>   |<span data-ttu-id="27911-115">Description</span><span class="sxs-lookup"><span data-stu-id="27911-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27911-116">associationType</span><span class="sxs-lookup"><span data-stu-id="27911-116">associationType</span></span>|<span data-ttu-id="27911-117">String</span><span class="sxs-lookup"><span data-stu-id="27911-117">String</span></span>|<span data-ttu-id="27911-118">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="27911-118">Nullable.</span></span> <span data-ttu-id="27911-119">Тип связи между [plannerPlan](plannerplan.md) и приложения в определенных приложений.</span><span class="sxs-lookup"><span data-stu-id="27911-119">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="27911-120">Приложения могут использовать эти сведения для отслеживания различных типов отношений же [plannerPlan](plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="27911-120">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="27911-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27911-121">createdDateTime</span></span>|<span data-ttu-id="27911-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27911-122">DateTimeOffset</span></span>|<span data-ttu-id="27911-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27911-123">Read-only.</span></span> <span data-ttu-id="27911-124">Дата и время создания **plannerPlanContext** .</span><span class="sxs-lookup"><span data-stu-id="27911-124">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="27911-125">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="27911-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="27911-126">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="27911-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="27911-127">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="27911-127">displayNameSegments</span></span>|<span data-ttu-id="27911-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="27911-128">String collection</span></span>|<span data-ttu-id="27911-129">Сегменты имя внешнего интерфейса.</span><span class="sxs-lookup"><span data-stu-id="27911-129">The segments of the name of the external experience.</span></span> <span data-ttu-id="27911-130">Сегменты представления иерархической структуры, обеспечивающий другие приложения отобразить отношение.</span><span class="sxs-lookup"><span data-stu-id="27911-130">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="27911-131">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="27911-131">ownerAppId</span></span>|<span data-ttu-id="27911-132">String</span><span class="sxs-lookup"><span data-stu-id="27911-132">String</span></span>|<span data-ttu-id="27911-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27911-133">Read-only.</span></span> <span data-ttu-id="27911-134">Идентификатор приложения, которые созданы **plannerPlanContext**.</span><span class="sxs-lookup"><span data-stu-id="27911-134">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27911-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27911-135">JSON representation</span></span>

<span data-ttu-id="27911-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27911-136">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
