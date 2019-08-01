---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактивитистат
description: Объект Итемактивитистат предоставляет сведения о действиях, выполненных с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bf4396e6da5c56b19d33d7a914d864cb6dd54592
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036675"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="8e0da-103">Тип ресурса Итемактивитистат</span><span class="sxs-lookup"><span data-stu-id="8e0da-103">itemActivityStat resource type</span></span>

<span data-ttu-id="8e0da-104">Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="8e0da-104">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="8e0da-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e0da-105">Properties</span></span>

| <span data-ttu-id="8e0da-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e0da-106">Property</span></span>         | <span data-ttu-id="8e0da-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8e0da-107">Type</span></span>                    | <span data-ttu-id="8e0da-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8e0da-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="8e0da-109">Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="8e0da-109">incompleteData</span></span>   | <span data-ttu-id="8e0da-110">[Инкомплетедата][]</span><span class="sxs-lookup"><span data-stu-id="8e0da-110">[incompleteData][]</span></span>      | <span data-ttu-id="8e0da-111">Указывает, что статистика в этом интервале основана на неполных данных.</span><span class="sxs-lookup"><span data-stu-id="8e0da-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="8e0da-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0da-112">Read-only.</span></span>
| <span data-ttu-id="8e0da-113">Тенденция</span><span class="sxs-lookup"><span data-stu-id="8e0da-113">isTrending</span></span>       | <span data-ttu-id="8e0da-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e0da-114">Boolean</span></span>                 | <span data-ttu-id="8e0da-115">Указывает, является ли элемент "тенденция".</span><span class="sxs-lookup"><span data-stu-id="8e0da-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="8e0da-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0da-116">Read-only.</span></span>
| <span data-ttu-id="8e0da-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8e0da-117">startDateTime</span></span>    | <span data-ttu-id="8e0da-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e0da-118">DateTimeOffset</span></span>          | <span data-ttu-id="8e0da-119">Время начала интервала.</span><span class="sxs-lookup"><span data-stu-id="8e0da-119">When the interval starts.</span></span> <span data-ttu-id="8e0da-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0da-120">Read-only.</span></span>
| <span data-ttu-id="8e0da-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8e0da-121">endDateTime</span></span>      | <span data-ttu-id="8e0da-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e0da-122">DateTimeOffset</span></span>          | <span data-ttu-id="8e0da-123">По окончании интервала.</span><span class="sxs-lookup"><span data-stu-id="8e0da-123">When the interval ends.</span></span> <span data-ttu-id="8e0da-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0da-124">Read-only.</span></span>
| <span data-ttu-id="8e0da-125">create</span><span class="sxs-lookup"><span data-stu-id="8e0da-125">create</span></span>           | <span data-ttu-id="8e0da-126">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="8e0da-126">[itemActionStat][]</span></span>      | <span data-ttu-id="8e0da-127">Статистика по действиям по **созданию** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="8e0da-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="8e0da-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0da-128">Read-only.</span></span>
| <span data-ttu-id="8e0da-129">edit</span><span class="sxs-lookup"><span data-stu-id="8e0da-129">edit</span></span>             | <span data-ttu-id="8e0da-130">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="8e0da-130">[itemActionStat][]</span></span>      | <span data-ttu-id="8e0da-131">Статистика действий **редактирования** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="8e0da-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="8e0da-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0da-132">Read-only.</span></span>
| <span data-ttu-id="8e0da-133">delete</span><span class="sxs-lookup"><span data-stu-id="8e0da-133">delete</span></span>           | <span data-ttu-id="8e0da-134">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="8e0da-134">[itemActionStat][]</span></span>      | <span data-ttu-id="8e0da-135">Статистика действий **удаления** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="8e0da-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="8e0da-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0da-136">Read-only.</span></span>
| <span data-ttu-id="8e0da-137">move</span><span class="sxs-lookup"><span data-stu-id="8e0da-137">move</span></span>             | <span data-ttu-id="8e0da-138">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="8e0da-138">[itemActionStat][]</span></span>      | <span data-ttu-id="8e0da-139">Статистика действий **перемещения** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="8e0da-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="8e0da-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0da-140">Read-only.</span></span>
| <span data-ttu-id="8e0da-141">обращения</span><span class="sxs-lookup"><span data-stu-id="8e0da-141">access</span></span>           | <span data-ttu-id="8e0da-142">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="8e0da-142">[itemActionStat][]</span></span>      | <span data-ttu-id="8e0da-143">Статистика действий **доступа** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="8e0da-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="8e0da-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0da-144">Read-only.</span></span>

[Итемактионстат]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[Инкомплетедата]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="8e0da-147">Связи</span><span class="sxs-lookup"><span data-stu-id="8e0da-147">Relationships</span></span>

| <span data-ttu-id="8e0da-148">Имя связи</span><span class="sxs-lookup"><span data-stu-id="8e0da-148">Relationship name</span></span> | <span data-ttu-id="8e0da-149">Тип</span><span class="sxs-lookup"><span data-stu-id="8e0da-149">Type</span></span>                        | <span data-ttu-id="8e0da-150">Описание</span><span class="sxs-lookup"><span data-stu-id="8e0da-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="8e0da-151">activities</span><span class="sxs-lookup"><span data-stu-id="8e0da-151">activities</span></span>        | <span data-ttu-id="8e0da-152">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="8e0da-152">[itemActivity][] collection</span></span> | <span data-ttu-id="8e0da-153">Предоставляет **итемактивитиес** , представленные в этом ресурсе **итемактивитистат** .</span><span class="sxs-lookup"><span data-stu-id="8e0da-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8e0da-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e0da-155">JSON representation</span></span>

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
