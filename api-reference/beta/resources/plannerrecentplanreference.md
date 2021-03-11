---
title: тип ресурса plannerRecentPlanReference
description: 'Тип **ресурса plannerRecentPlanReference** покаяется ссылкой на планировщикПлан, который недавно был просмотрен пользователем. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8a8fbf3ce9f39c49dde4bbeee96a3aab15a00077
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720979"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="3eee9-103">тип ресурса plannerRecentPlanReference</span><span class="sxs-lookup"><span data-stu-id="3eee9-103">plannerRecentPlanReference resource type</span></span>

<span data-ttu-id="3eee9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eee9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3eee9-105">Тип **ресурса plannerRecentPlanReference** покаяется ссылкой на [планировщикПлан,](plannerplan.md) который недавно был просмотрен пользователем.</span><span class="sxs-lookup"><span data-stu-id="3eee9-105">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="3eee9-106">**ПланировщикRecentPlanReferences** для пользователя явно поддерживается приложениями.</span><span class="sxs-lookup"><span data-stu-id="3eee9-106">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="3eee9-107">Любое приложение, которое реализует функцию последних планов, должно записывать, когда пользователь последний раз просматривал план, и обновлять записи **plannerRecentPlanReference** соответственно.</span><span class="sxs-lookup"><span data-stu-id="3eee9-107">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="3eee9-108">Приложения должны отметить, что записи **plannerRecentPlanReference** могут ссылаться на планировщикПланы, которые удаляются, что пользователь больше не может получить доступ или которые были обновлены с другим названием. </span><span class="sxs-lookup"><span data-stu-id="3eee9-108">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="3eee9-109">Мы рекомендуем приложениям уведомлять пользователей о несоответствиях и поддерживать записи в курсе.</span><span class="sxs-lookup"><span data-stu-id="3eee9-109">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="3eee9-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="3eee9-110">Properties</span></span>
| <span data-ttu-id="3eee9-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="3eee9-111">Property</span></span>     | <span data-ttu-id="3eee9-112">Тип</span><span class="sxs-lookup"><span data-stu-id="3eee9-112">Type</span></span>   |<span data-ttu-id="3eee9-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3eee9-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3eee9-114">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="3eee9-114">lastAccessedDateTime</span></span>|<span data-ttu-id="3eee9-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eee9-115">DateTimeOffset</span></span>|<span data-ttu-id="3eee9-116">Дата и время последнего просмотра плана пользователем.</span><span class="sxs-lookup"><span data-stu-id="3eee9-116">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="3eee9-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3eee9-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3eee9-118">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3eee9-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="3eee9-119">planTitle</span><span class="sxs-lookup"><span data-stu-id="3eee9-119">planTitle</span></span>|<span data-ttu-id="3eee9-120">String</span><span class="sxs-lookup"><span data-stu-id="3eee9-120">String</span></span>|<span data-ttu-id="3eee9-121">Название плана во время просмотра пользователем.</span><span class="sxs-lookup"><span data-stu-id="3eee9-121">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3eee9-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3eee9-122">JSON representation</span></span>

<span data-ttu-id="3eee9-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3eee9-123">The following is a JSON representation of the resource.</span></span>

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


