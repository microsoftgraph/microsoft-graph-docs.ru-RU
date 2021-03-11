---
title: тип ресурса plannerPlanContext
description: Ресурс **plannerPlanContext** представляет связь планировщикаPlan с пользовательским взаимодействием за пределами Planner. Планы в Planner можно всплыть в других опытах, таких как Microsoft Teams, чтобы отслеживать работу в контексте этого опыта.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f8a3b82c35339bb8bc6b3d3d7923b41ed97ecc02
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720986"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="b27ba-104">тип ресурса plannerPlanContext</span><span class="sxs-lookup"><span data-stu-id="b27ba-104">plannerPlanContext resource type</span></span>

<span data-ttu-id="b27ba-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b27ba-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b27ba-106">Ресурс **plannerPlanContext** представляет связь планировщикаPlan с пользовательским взаимодействием за пределами Planner. [](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="b27ba-106">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="b27ba-107">Планы в Planner можно всплыть в других опытах, таких как Microsoft Teams, чтобы отслеживать работу в контексте этого опыта.</span><span class="sxs-lookup"><span data-stu-id="b27ba-107">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span> <span data-ttu-id="b27ba-108">В пользовательском интерфейсе можно отображать внешние ссылки в [планировщикеPlanContextDetails,](plannerplancontextdetails.md) что позволяет пользователям посещать эти впечатления.</span><span class="sxs-lookup"><span data-stu-id="b27ba-108">Experiences that have external links in the [plannerPlanContextDetails](plannerplancontextdetails.md) can be displayed in a user interface, allowing users to visit these experiences.</span></span>


## <a name="properties"></a><span data-ttu-id="b27ba-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b27ba-109">Properties</span></span>
| <span data-ttu-id="b27ba-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b27ba-110">Property</span></span>     | <span data-ttu-id="b27ba-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b27ba-111">Type</span></span>   |<span data-ttu-id="b27ba-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b27ba-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b27ba-113">associationType</span><span class="sxs-lookup"><span data-stu-id="b27ba-113">associationType</span></span>|<span data-ttu-id="b27ba-114">String</span><span class="sxs-lookup"><span data-stu-id="b27ba-114">String</span></span>|<span data-ttu-id="b27ba-115">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b27ba-115">Nullable.</span></span> <span data-ttu-id="b27ba-116">Определенный приложением тип связи между [планировщикомPlan](plannerplan.md) и приложением.</span><span class="sxs-lookup"><span data-stu-id="b27ba-116">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="b27ba-117">Приложение может использовать эту информацию для отслеживания различных типов отношений с одним и тем же [планировщикомPlan.](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="b27ba-117">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="b27ba-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b27ba-118">createdDateTime</span></span>|<span data-ttu-id="b27ba-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b27ba-119">DateTimeOffset</span></span>|<span data-ttu-id="b27ba-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b27ba-120">Read-only.</span></span> <span data-ttu-id="b27ba-121">Дата и время создания **планировщикаPlanContext.**</span><span class="sxs-lookup"><span data-stu-id="b27ba-121">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="b27ba-122">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b27ba-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b27ba-123">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b27ba-123">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="b27ba-124">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="b27ba-124">displayNameSegments</span></span>|<span data-ttu-id="b27ba-125">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="b27ba-125">String collection</span></span>|<span data-ttu-id="b27ba-126">Сегменты имени внешнего опыта.</span><span class="sxs-lookup"><span data-stu-id="b27ba-126">The segments of the name of the external experience.</span></span> <span data-ttu-id="b27ba-127">Сегменты представляют иерархическую структуру, которая позволяет другим приложениям отображать связь.</span><span class="sxs-lookup"><span data-stu-id="b27ba-127">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="b27ba-128">isCreationContext</span><span class="sxs-lookup"><span data-stu-id="b27ba-128">isCreationContext</span></span>|<span data-ttu-id="b27ba-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="b27ba-129">Boolean</span></span>|<span data-ttu-id="b27ba-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b27ba-130">Read-only.</span></span> <span data-ttu-id="b27ba-131">Указывает, создается ли план из указанного контекста.</span><span class="sxs-lookup"><span data-stu-id="b27ba-131">Indicates whether the plan is created from the specified context.</span></span> <span data-ttu-id="b27ba-132">Автогенерированная в зависимости от того, задан ли контекст в рамках создания плана.</span><span class="sxs-lookup"><span data-stu-id="b27ba-132">Auto-generated based on whether the context is specified as part of plan creation.</span></span>|
|<span data-ttu-id="b27ba-133">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="b27ba-133">ownerAppId</span></span>|<span data-ttu-id="b27ba-134">String</span><span class="sxs-lookup"><span data-stu-id="b27ba-134">String</span></span>|<span data-ttu-id="b27ba-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b27ba-135">Read-only.</span></span> <span data-ttu-id="b27ba-136">ID приложения, создав **планировщикPlanContext**.</span><span class="sxs-lookup"><span data-stu-id="b27ba-136">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b27ba-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b27ba-137">JSON representation</span></span>

<span data-ttu-id="b27ba-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b27ba-138">The following is a JSON representation of the resource.</span></span>

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
  "isCreationContext": false,
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
  "suppressions": []
}
-->


