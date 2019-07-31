---
title: Тип ресурса Планнеррецентпланреференце
description: 'Тип ресурса **планнеррецентпланреференце** репесентс ссылку на plannerPlan, которая недавно была просмотрена пользователем. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8439502aa1214e1ef2bbedd9864ef4724abf8021
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965868"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="97368-103">Тип ресурса Планнеррецентпланреференце</span><span class="sxs-lookup"><span data-stu-id="97368-103">plannerRecentPlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97368-104">Тип ресурса **планнеррецентпланреференце** репесентс ссылку на [plannerPlan](plannerplan.md) , которая недавно была просмотрена пользователем.</span><span class="sxs-lookup"><span data-stu-id="97368-104">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="97368-105">**Планнеррецентпланреференцес** для пользователя явным образом сохраняется в приложениях.</span><span class="sxs-lookup"><span data-stu-id="97368-105">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="97368-106">Любое приложение, в котором реализована функция последних планов, должно записываться, когда пользователь последний раз просмотрел план, и соответствующим образом обновит записи **планнеррецентпланреференце** .</span><span class="sxs-lookup"><span data-stu-id="97368-106">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="97368-107">Приложения должны иметь в виду, что записи **планнеррецентпланреференце** могут ссылаться на **планов** , которые были удалены, что пользователь больше не может получить доступ, или он был обновлен с другим названием.</span><span class="sxs-lookup"><span data-stu-id="97368-107">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="97368-108">Мы рекомендуем пользователям уведомлять пользователей о наличии расхождений и регулярного обновления записей.</span><span class="sxs-lookup"><span data-stu-id="97368-108">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="97368-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="97368-109">Properties</span></span>
| <span data-ttu-id="97368-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="97368-110">Property</span></span>     | <span data-ttu-id="97368-111">Тип</span><span class="sxs-lookup"><span data-stu-id="97368-111">Type</span></span>   |<span data-ttu-id="97368-112">Описание</span><span class="sxs-lookup"><span data-stu-id="97368-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97368-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="97368-113">lastAccessedDateTime</span></span>|<span data-ttu-id="97368-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97368-114">DateTimeOffset</span></span>|<span data-ttu-id="97368-115">Дата и время последнего просмотра плана пользователем.</span><span class="sxs-lookup"><span data-stu-id="97368-115">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="97368-116">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="97368-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97368-117">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="97368-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="97368-118">Плантитле</span><span class="sxs-lookup"><span data-stu-id="97368-118">planTitle</span></span>|<span data-ttu-id="97368-119">String</span><span class="sxs-lookup"><span data-stu-id="97368-119">String</span></span>|<span data-ttu-id="97368-120">Название плана на момент просмотра его пользователем.</span><span class="sxs-lookup"><span data-stu-id="97368-120">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97368-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97368-121">JSON representation</span></span>

<span data-ttu-id="97368-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97368-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
