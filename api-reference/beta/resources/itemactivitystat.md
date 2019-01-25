---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517633"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="fac2d-102">Тип ресурса itemActivityStat</span><span class="sxs-lookup"><span data-stu-id="fac2d-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fac2d-103">Ресурс **itemActivityStat** содержит сведения о действиях, выполняемых в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="fac2d-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fac2d-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fac2d-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "baseType": "microsoft.graph.entity",
  "@type": "microsoft.graph.itemActivityStat",
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "incompleteData": {"@odata.type": "microsoft.graph.incompleteData"},
  "isTrending": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "create": {"@odata.type": "microsoft.graph.itemActionStat"},
  "delete": {"@odata.type": "microsoft.graph.itemActionStat"},
  "edit": {"@odata.type": "microsoft.graph.itemActionStat"},
  "move": {"@odata.type": "microsoft.graph.itemActionStat"},
  "access": {"@odata.type": "microsoft.graph.itemActionStat"}
}
```

## <a name="properties"></a><span data-ttu-id="fac2d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fac2d-105">Properties</span></span>

| <span data-ttu-id="fac2d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fac2d-106">Property</span></span>         | <span data-ttu-id="fac2d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fac2d-107">Type</span></span>                    | <span data-ttu-id="fac2d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fac2d-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="fac2d-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="fac2d-109">incompleteData</span></span>   | <span data-ttu-id="fac2d-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="fac2d-110">[incompleteData][]</span></span>      | <span data-ttu-id="fac2d-111">Указывает, что Статистика ожидания основаны на неполные данные.</span><span class="sxs-lookup"><span data-stu-id="fac2d-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="fac2d-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fac2d-112">Read-only.</span></span>
| <span data-ttu-id="fac2d-113">isTrending</span><span class="sxs-lookup"><span data-stu-id="fac2d-113">isTrending</span></span>       | <span data-ttu-id="fac2d-114">Логическое</span><span class="sxs-lookup"><span data-stu-id="fac2d-114">Boolean</span></span>                 | <span data-ttu-id="fac2d-115">Указывает, является ли элемент «прибора.»</span><span class="sxs-lookup"><span data-stu-id="fac2d-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="fac2d-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fac2d-116">Read-only.</span></span>
| <span data-ttu-id="fac2d-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fac2d-117">startDateTime</span></span>    | <span data-ttu-id="fac2d-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fac2d-118">DateTimeOffset</span></span>          | <span data-ttu-id="fac2d-119">При запуске интервала.</span><span class="sxs-lookup"><span data-stu-id="fac2d-119">When the interval starts.</span></span> <span data-ttu-id="fac2d-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fac2d-120">Read-only.</span></span>
| <span data-ttu-id="fac2d-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fac2d-121">endDateTime</span></span>      | <span data-ttu-id="fac2d-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fac2d-122">DateTimeOffset</span></span>          | <span data-ttu-id="fac2d-123">Окончания интервала.</span><span class="sxs-lookup"><span data-stu-id="fac2d-123">When the interval ends.</span></span> <span data-ttu-id="fac2d-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fac2d-124">Read-only.</span></span>
| <span data-ttu-id="fac2d-125">create</span><span class="sxs-lookup"><span data-stu-id="fac2d-125">create</span></span>           | <span data-ttu-id="fac2d-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="fac2d-126">[itemActionStat][]</span></span>      | <span data-ttu-id="fac2d-127">Сведения о действия **Создание** ожидания.</span><span class="sxs-lookup"><span data-stu-id="fac2d-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="fac2d-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fac2d-128">Read-only.</span></span>
| <span data-ttu-id="fac2d-129">edit</span><span class="sxs-lookup"><span data-stu-id="fac2d-129">edit</span></span>             | <span data-ttu-id="fac2d-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="fac2d-130">[itemActionStat][]</span></span>      | <span data-ttu-id="fac2d-131">Сведения о действия **редактирования** в этот интервал.</span><span class="sxs-lookup"><span data-stu-id="fac2d-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="fac2d-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fac2d-132">Read-only.</span></span>
| <span data-ttu-id="fac2d-133">delete</span><span class="sxs-lookup"><span data-stu-id="fac2d-133">delete</span></span>           | <span data-ttu-id="fac2d-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="fac2d-134">[itemActionStat][]</span></span>      | <span data-ttu-id="fac2d-135">Сведения о действиям **удаления** ожидания.</span><span class="sxs-lookup"><span data-stu-id="fac2d-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="fac2d-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fac2d-136">Read-only.</span></span>
| <span data-ttu-id="fac2d-137">move</span><span class="sxs-lookup"><span data-stu-id="fac2d-137">move</span></span>             | <span data-ttu-id="fac2d-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="fac2d-138">[itemActionStat][]</span></span>      | <span data-ttu-id="fac2d-139">Сведения о действия **переместить** в этот интервал.</span><span class="sxs-lookup"><span data-stu-id="fac2d-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="fac2d-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fac2d-140">Read-only.</span></span>
| <span data-ttu-id="fac2d-141">Access</span><span class="sxs-lookup"><span data-stu-id="fac2d-141">access</span></span>           | <span data-ttu-id="fac2d-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="fac2d-142">[itemActionStat][]</span></span>      | <span data-ttu-id="fac2d-143">Сведения о действия **клиента** в этот интервал.</span><span class="sxs-lookup"><span data-stu-id="fac2d-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="fac2d-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fac2d-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="fac2d-147">Связи</span><span class="sxs-lookup"><span data-stu-id="fac2d-147">Relationships</span></span>

| <span data-ttu-id="fac2d-148">Имя связи</span><span class="sxs-lookup"><span data-stu-id="fac2d-148">Relationship name</span></span> | <span data-ttu-id="fac2d-149">Тип</span><span class="sxs-lookup"><span data-stu-id="fac2d-149">Type</span></span>                        | <span data-ttu-id="fac2d-150">Описание</span><span class="sxs-lookup"><span data-stu-id="fac2d-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="fac2d-151">activities</span><span class="sxs-lookup"><span data-stu-id="fac2d-151">activities</span></span>        | <span data-ttu-id="fac2d-152">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="fac2d-152">[itemActivity][] collection</span></span> | <span data-ttu-id="fac2d-153">Предоставляет **itemActivities** , представленного в этом **itemActivityStat** ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fac2d-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="fac2d-155">Замечания</span><span class="sxs-lookup"><span data-stu-id="fac2d-155">Remarks</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitystat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
