---
title: Тип ресурса plannerRecentPlanReference
description: 'Ресурс **plannerRecentPlanReference** введите repesents ссылку на plannerPlan, недавно просмотренный пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: bafaf6d20dc8f64ffe49eb4e2f998607708a2773
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943532"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="d37b2-103">Тип ресурса plannerRecentPlanReference</span><span class="sxs-lookup"><span data-stu-id="d37b2-103">plannerRecentPlanReference resource type</span></span>

> <span data-ttu-id="d37b2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d37b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d37b2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d37b2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d37b2-106">Ресурс **plannerRecentPlanReference** введите repesents ссылку на [plannerPlan](plannerplan.md) , недавно просмотренный пользователя.</span><span class="sxs-lookup"><span data-stu-id="d37b2-106">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="d37b2-107">**PlannerRecentPlanReferences** для пользователя, явно задаваемые с помощью приложения.</span><span class="sxs-lookup"><span data-stu-id="d37b2-107">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="d37b2-108">Все приложения, которое реализует функцию последние планы следует записать при соответствующим образом пользователь последнего просмотра записи **plannerRecentPlanReference** обновления и плана.</span><span class="sxs-lookup"><span data-stu-id="d37b2-108">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="d37b2-109">Приложения следует иметь в виду, что записи **plannerRecentPlanReference** можно ссылаться на **plannerPlans** , будут удалены, пользователь больше не может получить доступ и добавлены иное название.</span><span class="sxs-lookup"><span data-stu-id="d37b2-109">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="d37b2-110">Рекомендуется уведомлять пользователей есть несоответствия приложений и обновлять записи.</span><span class="sxs-lookup"><span data-stu-id="d37b2-110">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="d37b2-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="d37b2-111">Properties</span></span>
| <span data-ttu-id="d37b2-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="d37b2-112">Property</span></span>     | <span data-ttu-id="d37b2-113">Тип</span><span class="sxs-lookup"><span data-stu-id="d37b2-113">Type</span></span>   |<span data-ttu-id="d37b2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d37b2-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d37b2-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="d37b2-115">lastAccessedDateTime</span></span>|<span data-ttu-id="d37b2-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d37b2-116">DateTimeOffset</span></span>|<span data-ttu-id="d37b2-117">Дата и время, планирование последнего просмотра пользователем.</span><span class="sxs-lookup"><span data-stu-id="d37b2-117">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="d37b2-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d37b2-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d37b2-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d37b2-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d37b2-120">planTitle</span><span class="sxs-lookup"><span data-stu-id="d37b2-120">planTitle</span></span>|<span data-ttu-id="d37b2-121">Строка</span><span class="sxs-lookup"><span data-stu-id="d37b2-121">String</span></span>|<span data-ttu-id="d37b2-122">Название плана во время пользователь просматривать его.</span><span class="sxs-lookup"><span data-stu-id="d37b2-122">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d37b2-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d37b2-123">JSON representation</span></span>

<span data-ttu-id="d37b2-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d37b2-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
