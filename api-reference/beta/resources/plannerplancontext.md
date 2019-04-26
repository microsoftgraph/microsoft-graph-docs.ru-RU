---
title: Тип ресурса Планнерпланконтекст
description: Ресурс **планнерпланконтекст** представляет связь plannerPlan с возможностями взаимодействия с пользователем вне планировщика. Планы планировщика могут быть предоставлены в других интерфейсах, таких как Microsoft Teams, для отслеживания работы в контексте этого интерфейса.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 68d9233d2645c2176ad364fbcbfac869976f0586
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344454"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="3c790-104">Тип ресурса Планнерпланконтекст</span><span class="sxs-lookup"><span data-stu-id="3c790-104">plannerPlanContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c790-105">Ресурс **планнерпланконтекст** представляет связь [plannerPlan](plannerplan.md) с возможностями взаимодействия с пользователем вне планировщика.</span><span class="sxs-lookup"><span data-stu-id="3c790-105">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="3c790-106">Планы планировщика могут быть предоставлены в других интерфейсах, таких как Microsoft Teams, для отслеживания работы в контексте этого интерфейса.</span><span class="sxs-lookup"><span data-stu-id="3c790-106">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="3c790-107">Интерфейс повторной отправки записи **планнерпланконтекст** можно определить на основе свойства **овнераппид** :</span><span class="sxs-lookup"><span data-stu-id="3c790-107">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="3c790-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: Контекстная запись относится к Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3c790-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="3c790-109">является 00000003-0000-0ff1-ce00-000000000000: запись контекста принадлежит SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3c790-109">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="3c790-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c790-110">Properties</span></span>
| <span data-ttu-id="3c790-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c790-111">Property</span></span>     | <span data-ttu-id="3c790-112">Тип</span><span class="sxs-lookup"><span data-stu-id="3c790-112">Type</span></span>   |<span data-ttu-id="3c790-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3c790-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c790-114">Типе</span><span class="sxs-lookup"><span data-stu-id="3c790-114">associationType</span></span>|<span data-ttu-id="3c790-115">String</span><span class="sxs-lookup"><span data-stu-id="3c790-115">String</span></span>|<span data-ttu-id="3c790-116">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="3c790-116">Nullable.</span></span> <span data-ttu-id="3c790-117">Определяемый приложением тип связи между [plannerPlan](plannerplan.md) и приложением.</span><span class="sxs-lookup"><span data-stu-id="3c790-117">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="3c790-118">Приложение может использовать эту информацию для отслеживания различных видов отношений с одним и тем же [plannerPlan](plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="3c790-118">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="3c790-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c790-119">createdDateTime</span></span>|<span data-ttu-id="3c790-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c790-120">DateTimeOffset</span></span>|<span data-ttu-id="3c790-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c790-121">Read-only.</span></span> <span data-ttu-id="3c790-122">Дата и время создания **планнерпланконтекст** .</span><span class="sxs-lookup"><span data-stu-id="3c790-122">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="3c790-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3c790-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3c790-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3c790-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="3c790-125">Дисплайнамесегментс</span><span class="sxs-lookup"><span data-stu-id="3c790-125">displayNameSegments</span></span>|<span data-ttu-id="3c790-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3c790-126">String collection</span></span>|<span data-ttu-id="3c790-127">Сегменты имени внешнего интерфейса взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="3c790-127">The segments of the name of the external experience.</span></span> <span data-ttu-id="3c790-128">Сегменты представляют иерархическую структуру, которая позволяет другим приложениям отображать связь.</span><span class="sxs-lookup"><span data-stu-id="3c790-128">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="3c790-129">Овнераппид</span><span class="sxs-lookup"><span data-stu-id="3c790-129">ownerAppId</span></span>|<span data-ttu-id="3c790-130">String</span><span class="sxs-lookup"><span data-stu-id="3c790-130">String</span></span>|<span data-ttu-id="3c790-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c790-131">Read-only.</span></span> <span data-ttu-id="3c790-132">Идентификатор приложения, создавшего **планнерпланконтекст**.</span><span class="sxs-lookup"><span data-stu-id="3c790-132">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c790-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c790-133">JSON representation</span></span>

<span data-ttu-id="3c790-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c790-134">The following is a JSON representation of the resource.</span></span>

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
