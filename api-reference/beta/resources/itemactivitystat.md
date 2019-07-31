---
author: daspek
description: Ресурс Итемактивитистат предоставляет сведения о действиях, которые выполнялись в течение интервала времени.
ms.date: 09/14/2017
title: Итемактивитистат
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 61c410d807869615ed35365743d1ae87b5b6e890
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967103"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="7d747-103">Тип ресурса Итемактивитистат</span><span class="sxs-lookup"><span data-stu-id="7d747-103">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d747-104">Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="7d747-104">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d747-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d747-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7d747-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d747-106">Properties</span></span>

| <span data-ttu-id="7d747-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d747-107">Property</span></span>         | <span data-ttu-id="7d747-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7d747-108">Type</span></span>                    | <span data-ttu-id="7d747-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7d747-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="7d747-110">Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="7d747-110">incompleteData</span></span>   | <span data-ttu-id="7d747-111">[Инкомплетедата][]</span><span class="sxs-lookup"><span data-stu-id="7d747-111">[incompleteData][]</span></span>      | <span data-ttu-id="7d747-112">Указывает, что статистика в этом интервале основана на неполных данных.</span><span class="sxs-lookup"><span data-stu-id="7d747-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="7d747-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d747-113">Read-only.</span></span>
| <span data-ttu-id="7d747-114">Тенденция</span><span class="sxs-lookup"><span data-stu-id="7d747-114">isTrending</span></span>       | <span data-ttu-id="7d747-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d747-115">Boolean</span></span>                 | <span data-ttu-id="7d747-116">Указывает, является ли элемент "тенденция".</span><span class="sxs-lookup"><span data-stu-id="7d747-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="7d747-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d747-117">Read-only.</span></span>
| <span data-ttu-id="7d747-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7d747-118">startDateTime</span></span>    | <span data-ttu-id="7d747-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d747-119">DateTimeOffset</span></span>          | <span data-ttu-id="7d747-120">Время начала интервала.</span><span class="sxs-lookup"><span data-stu-id="7d747-120">When the interval starts.</span></span> <span data-ttu-id="7d747-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d747-121">Read-only.</span></span>
| <span data-ttu-id="7d747-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7d747-122">endDateTime</span></span>      | <span data-ttu-id="7d747-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d747-123">DateTimeOffset</span></span>          | <span data-ttu-id="7d747-124">По окончании интервала.</span><span class="sxs-lookup"><span data-stu-id="7d747-124">When the interval ends.</span></span> <span data-ttu-id="7d747-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d747-125">Read-only.</span></span>
| <span data-ttu-id="7d747-126">create</span><span class="sxs-lookup"><span data-stu-id="7d747-126">create</span></span>           | <span data-ttu-id="7d747-127">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="7d747-127">[itemActionStat][]</span></span>      | <span data-ttu-id="7d747-128">Статистика по действиям по **созданию** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="7d747-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="7d747-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d747-129">Read-only.</span></span>
| <span data-ttu-id="7d747-130">edit</span><span class="sxs-lookup"><span data-stu-id="7d747-130">edit</span></span>             | <span data-ttu-id="7d747-131">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="7d747-131">[itemActionStat][]</span></span>      | <span data-ttu-id="7d747-132">Статистика действий **редактирования** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="7d747-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="7d747-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d747-133">Read-only.</span></span>
| <span data-ttu-id="7d747-134">delete</span><span class="sxs-lookup"><span data-stu-id="7d747-134">delete</span></span>           | <span data-ttu-id="7d747-135">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="7d747-135">[itemActionStat][]</span></span>      | <span data-ttu-id="7d747-136">Статистика действий **удаления** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="7d747-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="7d747-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d747-137">Read-only.</span></span>
| <span data-ttu-id="7d747-138">move</span><span class="sxs-lookup"><span data-stu-id="7d747-138">move</span></span>             | <span data-ttu-id="7d747-139">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="7d747-139">[itemActionStat][]</span></span>      | <span data-ttu-id="7d747-140">Статистика действий **перемещения** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="7d747-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="7d747-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d747-141">Read-only.</span></span>
| <span data-ttu-id="7d747-142">обращения</span><span class="sxs-lookup"><span data-stu-id="7d747-142">access</span></span>           | <span data-ttu-id="7d747-143">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="7d747-143">[itemActionStat][]</span></span>      | <span data-ttu-id="7d747-144">Статистика действий **доступа** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="7d747-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="7d747-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d747-145">Read-only.</span></span>

[Итемактионстат]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[Инкомплетедата]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="7d747-148">Связи</span><span class="sxs-lookup"><span data-stu-id="7d747-148">Relationships</span></span>

| <span data-ttu-id="7d747-149">Имя связи</span><span class="sxs-lookup"><span data-stu-id="7d747-149">Relationship name</span></span> | <span data-ttu-id="7d747-150">Тип</span><span class="sxs-lookup"><span data-stu-id="7d747-150">Type</span></span>                        | <span data-ttu-id="7d747-151">Описание</span><span class="sxs-lookup"><span data-stu-id="7d747-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="7d747-152">activities</span><span class="sxs-lookup"><span data-stu-id="7d747-152">activities</span></span>        | <span data-ttu-id="7d747-153">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="7d747-153">[itemActivity][] collection</span></span> | <span data-ttu-id="7d747-154">Предоставляет **итемактивитиес** , представленные в этом ресурсе **итемактивитистат** .</span><span class="sxs-lookup"><span data-stu-id="7d747-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="7d747-156">Замечания</span><span class="sxs-lookup"><span data-stu-id="7d747-156">Remarks</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": []
}
-->
