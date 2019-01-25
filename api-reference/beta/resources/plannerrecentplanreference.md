---
title: Тип ресурса plannerRecentPlanReference
description: 'Ресурс **plannerRecentPlanReference** введите repesents ссылку на plannerPlan, недавно просмотренный пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 55ccf34055d7d181dbbeecd5b6c30a3843f211d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509163"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="30dfe-103">Тип ресурса plannerRecentPlanReference</span><span class="sxs-lookup"><span data-stu-id="30dfe-103">plannerRecentPlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30dfe-104">Ресурс **plannerRecentPlanReference** введите repesents ссылку на [plannerPlan](plannerplan.md) , недавно просмотренный пользователя.</span><span class="sxs-lookup"><span data-stu-id="30dfe-104">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="30dfe-105">**PlannerRecentPlanReferences** для пользователя, явно задаваемые с помощью приложения.</span><span class="sxs-lookup"><span data-stu-id="30dfe-105">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="30dfe-106">Все приложения, которое реализует функцию последние планы следует записать при соответствующим образом пользователь последнего просмотра записи **plannerRecentPlanReference** обновления и плана.</span><span class="sxs-lookup"><span data-stu-id="30dfe-106">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="30dfe-107">Приложения следует иметь в виду, что записи **plannerRecentPlanReference** можно ссылаться на **plannerPlans** , будут удалены, пользователь больше не может получить доступ и добавлены иное название.</span><span class="sxs-lookup"><span data-stu-id="30dfe-107">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="30dfe-108">Рекомендуется уведомлять пользователей есть несоответствия приложений и обновлять записи.</span><span class="sxs-lookup"><span data-stu-id="30dfe-108">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="30dfe-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="30dfe-109">Properties</span></span>
| <span data-ttu-id="30dfe-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="30dfe-110">Property</span></span>     | <span data-ttu-id="30dfe-111">Тип</span><span class="sxs-lookup"><span data-stu-id="30dfe-111">Type</span></span>   |<span data-ttu-id="30dfe-112">Описание</span><span class="sxs-lookup"><span data-stu-id="30dfe-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30dfe-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="30dfe-113">lastAccessedDateTime</span></span>|<span data-ttu-id="30dfe-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30dfe-114">DateTimeOffset</span></span>|<span data-ttu-id="30dfe-115">Дата и время, планирование последнего просмотра пользователем.</span><span class="sxs-lookup"><span data-stu-id="30dfe-115">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="30dfe-116">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="30dfe-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30dfe-117">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="30dfe-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="30dfe-118">planTitle</span><span class="sxs-lookup"><span data-stu-id="30dfe-118">planTitle</span></span>|<span data-ttu-id="30dfe-119">String</span><span class="sxs-lookup"><span data-stu-id="30dfe-119">String</span></span>|<span data-ttu-id="30dfe-120">Название плана во время пользователь просматривать его.</span><span class="sxs-lookup"><span data-stu-id="30dfe-120">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30dfe-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30dfe-121">JSON representation</span></span>

<span data-ttu-id="30dfe-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30dfe-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
