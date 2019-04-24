---
title: Тип ресурса Планнеррецентпланреференце
description: 'Тип ресурса **планнеррецентпланреференце** репесентс ссылку на plannerPlan, которая недавно была просмотрена пользователем. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 55ccf34055d7d181dbbeecd5b6c30a3843f211d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522156"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="e64af-103">Тип ресурса Планнеррецентпланреференце</span><span class="sxs-lookup"><span data-stu-id="e64af-103">plannerRecentPlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e64af-104">Тип ресурса **планнеррецентпланреференце** репесентс ссылку на [plannerPlan](plannerplan.md) , которая недавно была просмотрена пользователем.</span><span class="sxs-lookup"><span data-stu-id="e64af-104">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="e64af-105">**Планнеррецентпланреференцес** для пользователя явным образом сохраняется в приложениях.</span><span class="sxs-lookup"><span data-stu-id="e64af-105">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="e64af-106">Любое приложение, в котором реализована функция последних планов, должно записываться, когда пользователь последний раз просмотрел план, и соответствующим образом обновит записи **планнеррецентпланреференце** .</span><span class="sxs-lookup"><span data-stu-id="e64af-106">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="e64af-107">Приложения должны иметь в виду, что записи **планнеррецентпланреференце** могут ссылаться на **планов** , которые были удалены, что пользователь больше не может получить доступ, или он был обновлен с другим названием.</span><span class="sxs-lookup"><span data-stu-id="e64af-107">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="e64af-108">Мы рекомендуем пользователям уведомлять пользователей о наличии расхождений и регулярного обновления записей.</span><span class="sxs-lookup"><span data-stu-id="e64af-108">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="e64af-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e64af-109">Properties</span></span>
| <span data-ttu-id="e64af-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e64af-110">Property</span></span>     | <span data-ttu-id="e64af-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e64af-111">Type</span></span>   |<span data-ttu-id="e64af-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e64af-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e64af-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="e64af-113">lastAccessedDateTime</span></span>|<span data-ttu-id="e64af-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e64af-114">DateTimeOffset</span></span>|<span data-ttu-id="e64af-115">Дата и время последнего просмотра плана пользователем.</span><span class="sxs-lookup"><span data-stu-id="e64af-115">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="e64af-116">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e64af-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e64af-117">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e64af-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e64af-118">Плантитле</span><span class="sxs-lookup"><span data-stu-id="e64af-118">planTitle</span></span>|<span data-ttu-id="e64af-119">String</span><span class="sxs-lookup"><span data-stu-id="e64af-119">String</span></span>|<span data-ttu-id="e64af-120">Название плана на момент просмотра его пользователем.</span><span class="sxs-lookup"><span data-stu-id="e64af-120">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e64af-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e64af-121">JSON representation</span></span>

<span data-ttu-id="e64af-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e64af-122">The following is a JSON representation of the resource.</span></span>

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
