---
title: Тип ресурса Планнеррецентпланреференце
description: 'Тип ресурса **планнеррецентпланреференце** репесентс ссылку на plannerPlan, которая недавно была просмотрена пользователем. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1dc33d8a5f2ae34776154a2a0f11df854dea51e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521666"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="8ff01-103">Тип ресурса Планнеррецентпланреференце</span><span class="sxs-lookup"><span data-stu-id="8ff01-103">plannerRecentPlanReference resource type</span></span>

<span data-ttu-id="8ff01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ff01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff01-105">Тип ресурса **планнеррецентпланреференце** репесентс ссылку на [plannerPlan](plannerplan.md) , которая недавно была просмотрена пользователем.</span><span class="sxs-lookup"><span data-stu-id="8ff01-105">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="8ff01-106">**Планнеррецентпланреференцес** для пользователя явным образом сохраняется в приложениях.</span><span class="sxs-lookup"><span data-stu-id="8ff01-106">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="8ff01-107">Любое приложение, в котором реализована функция последних планов, должно записываться, когда пользователь последний раз просмотрел план, и соответствующим образом обновит записи **планнеррецентпланреференце** .</span><span class="sxs-lookup"><span data-stu-id="8ff01-107">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="8ff01-108">Приложения должны иметь в виду, что записи **планнеррецентпланреференце** могут ссылаться на **планов** , которые были удалены, что пользователь больше не может получить доступ, или он был обновлен с другим названием.</span><span class="sxs-lookup"><span data-stu-id="8ff01-108">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="8ff01-109">Мы рекомендуем пользователям уведомлять пользователей о наличии расхождений и регулярного обновления записей.</span><span class="sxs-lookup"><span data-stu-id="8ff01-109">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="8ff01-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ff01-110">Properties</span></span>
| <span data-ttu-id="8ff01-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ff01-111">Property</span></span>     | <span data-ttu-id="8ff01-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8ff01-112">Type</span></span>   |<span data-ttu-id="8ff01-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8ff01-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ff01-114">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ff01-114">lastAccessedDateTime</span></span>|<span data-ttu-id="8ff01-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ff01-115">DateTimeOffset</span></span>|<span data-ttu-id="8ff01-116">Дата и время последнего просмотра плана пользователем.</span><span class="sxs-lookup"><span data-stu-id="8ff01-116">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="8ff01-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8ff01-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8ff01-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8ff01-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8ff01-119">плантитле</span><span class="sxs-lookup"><span data-stu-id="8ff01-119">planTitle</span></span>|<span data-ttu-id="8ff01-120">Строка</span><span class="sxs-lookup"><span data-stu-id="8ff01-120">String</span></span>|<span data-ttu-id="8ff01-121">Название плана на момент просмотра его пользователем.</span><span class="sxs-lookup"><span data-stu-id="8ff01-121">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ff01-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ff01-122">JSON representation</span></span>

<span data-ttu-id="8ff01-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ff01-123">The following is a JSON representation of the resource.</span></span>

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
