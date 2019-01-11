---
title: Тип ресурса plannerRecentPlanReference
description: 'Ресурс **plannerRecentPlanReference** введите repesents ссылку на plannerPlan, недавно просмотренный пользователя. '
localization_priority: Normal
ms.openlocfilehash: 6ac17cd0a99d384cbc1f42e2e0d243c582204101
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805679"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="51084-103">Тип ресурса plannerRecentPlanReference</span><span class="sxs-lookup"><span data-stu-id="51084-103">plannerRecentPlanReference resource type</span></span>

> <span data-ttu-id="51084-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51084-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51084-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51084-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51084-106">Ресурс **plannerRecentPlanReference** введите repesents ссылку на [plannerPlan](plannerplan.md) , недавно просмотренный пользователя.</span><span class="sxs-lookup"><span data-stu-id="51084-106">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="51084-107">**PlannerRecentPlanReferences** для пользователя, явно задаваемые с помощью приложения.</span><span class="sxs-lookup"><span data-stu-id="51084-107">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="51084-108">Все приложения, которое реализует функцию последние планы следует записать при соответствующим образом пользователь последнего просмотра записи **plannerRecentPlanReference** обновления и плана.</span><span class="sxs-lookup"><span data-stu-id="51084-108">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="51084-109">Приложения следует иметь в виду, что записи **plannerRecentPlanReference** можно ссылаться на **plannerPlans** , будут удалены, пользователь больше не может получить доступ и добавлены иное название.</span><span class="sxs-lookup"><span data-stu-id="51084-109">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="51084-110">Рекомендуется уведомлять пользователей есть несоответствия приложений и обновлять записи.</span><span class="sxs-lookup"><span data-stu-id="51084-110">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="51084-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="51084-111">Properties</span></span>
| <span data-ttu-id="51084-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="51084-112">Property</span></span>     | <span data-ttu-id="51084-113">Тип</span><span class="sxs-lookup"><span data-stu-id="51084-113">Type</span></span>   |<span data-ttu-id="51084-114">Описание</span><span class="sxs-lookup"><span data-stu-id="51084-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51084-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="51084-115">lastAccessedDateTime</span></span>|<span data-ttu-id="51084-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51084-116">DateTimeOffset</span></span>|<span data-ttu-id="51084-117">Дата и время, планирование последнего просмотра пользователем.</span><span class="sxs-lookup"><span data-stu-id="51084-117">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="51084-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="51084-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="51084-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="51084-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="51084-120">planTitle</span><span class="sxs-lookup"><span data-stu-id="51084-120">planTitle</span></span>|<span data-ttu-id="51084-121">Строка</span><span class="sxs-lookup"><span data-stu-id="51084-121">String</span></span>|<span data-ttu-id="51084-122">Название плана во время пользователь просматривать его.</span><span class="sxs-lookup"><span data-stu-id="51084-122">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51084-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51084-123">JSON representation</span></span>

<span data-ttu-id="51084-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51084-124">The following is a JSON representation of the resource.</span></span>

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
