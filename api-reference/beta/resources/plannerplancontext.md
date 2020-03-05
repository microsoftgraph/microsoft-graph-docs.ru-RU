---
title: Тип ресурса Планнерпланконтекст
description: Ресурс **планнерпланконтекст** представляет связь plannerPlan с возможностями взаимодействия с пользователем вне планировщика. Планы планировщика могут быть предоставлены в других интерфейсах, таких как Microsoft Teams, для отслеживания работы в контексте этого интерфейса.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 99732cd99dafc67d9e82a7eba5676e41bcf7251b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521708"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="6c8fe-104">Тип ресурса Планнерпланконтекст</span><span class="sxs-lookup"><span data-stu-id="6c8fe-104">plannerPlanContext resource type</span></span>

<span data-ttu-id="6c8fe-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6c8fe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c8fe-106">Ресурс **планнерпланконтекст** представляет связь [plannerPlan](plannerplan.md) с возможностями взаимодействия с пользователем вне планировщика.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-106">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="6c8fe-107">Планы планировщика могут быть предоставлены в других интерфейсах, таких как Microsoft Teams, для отслеживания работы в контексте этого интерфейса.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-107">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="6c8fe-108">Интерфейс повторной отправки записи **планнерпланконтекст** можно определить на основе свойства **овнераппид** :</span><span class="sxs-lookup"><span data-stu-id="6c8fe-108">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
- <span data-ttu-id="6c8fe-109">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: Контекстная запись относится к Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-109">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
- <span data-ttu-id="6c8fe-110">является 00000003-0000-0ff1-ce00-000000000000: запись контекста принадлежит SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-110">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="6c8fe-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c8fe-111">Properties</span></span>
| <span data-ttu-id="6c8fe-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c8fe-112">Property</span></span>     | <span data-ttu-id="6c8fe-113">Тип</span><span class="sxs-lookup"><span data-stu-id="6c8fe-113">Type</span></span>   |<span data-ttu-id="6c8fe-114">Описание</span><span class="sxs-lookup"><span data-stu-id="6c8fe-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c8fe-115">Типе</span><span class="sxs-lookup"><span data-stu-id="6c8fe-115">associationType</span></span>|<span data-ttu-id="6c8fe-116">String</span><span class="sxs-lookup"><span data-stu-id="6c8fe-116">String</span></span>|<span data-ttu-id="6c8fe-117">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-117">Nullable.</span></span> <span data-ttu-id="6c8fe-118">Определяемый приложением тип связи между [plannerPlan](plannerplan.md) и приложением.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-118">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="6c8fe-119">Приложение может использовать эту информацию для отслеживания различных видов отношений с одним и тем же [plannerPlan](plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="6c8fe-119">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="6c8fe-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c8fe-120">createdDateTime</span></span>|<span data-ttu-id="6c8fe-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c8fe-121">DateTimeOffset</span></span>|<span data-ttu-id="6c8fe-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-122">Read-only.</span></span> <span data-ttu-id="6c8fe-123">Дата и время создания **планнерпланконтекст** .</span><span class="sxs-lookup"><span data-stu-id="6c8fe-123">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="6c8fe-124">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6c8fe-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c8fe-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6c8fe-126">дисплайнамесегментс</span><span class="sxs-lookup"><span data-stu-id="6c8fe-126">displayNameSegments</span></span>|<span data-ttu-id="6c8fe-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6c8fe-127">String collection</span></span>|<span data-ttu-id="6c8fe-128">Сегменты имени внешнего интерфейса взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-128">The segments of the name of the external experience.</span></span> <span data-ttu-id="6c8fe-129">Сегменты представляют иерархическую структуру, которая позволяет другим приложениям отображать связь.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-129">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="6c8fe-130">овнераппид</span><span class="sxs-lookup"><span data-stu-id="6c8fe-130">ownerAppId</span></span>|<span data-ttu-id="6c8fe-131">String</span><span class="sxs-lookup"><span data-stu-id="6c8fe-131">String</span></span>|<span data-ttu-id="6c8fe-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-132">Read-only.</span></span> <span data-ttu-id="6c8fe-133">Идентификатор приложения, создавшего **планнерпланконтекст**.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-133">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c8fe-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c8fe-134">JSON representation</span></span>

<span data-ttu-id="6c8fe-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c8fe-135">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
