---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактивитистат
description: Объект Итемактивитистат предоставляет сведения о действиях, выполненных с элементом.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3af10bba565585341d04cdc47702e18e71d8accd
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970800"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="5e163-103">Тип ресурса Итемактивитистат</span><span class="sxs-lookup"><span data-stu-id="5e163-103">itemActivityStat resource type</span></span>

<span data-ttu-id="5e163-104">Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="5e163-104">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="5e163-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e163-105">Properties</span></span>

| <span data-ttu-id="5e163-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e163-106">Property</span></span>         | <span data-ttu-id="5e163-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5e163-107">Type</span></span>                    | <span data-ttu-id="5e163-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5e163-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="5e163-109">Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="5e163-109">incompleteData</span></span>   | <span data-ttu-id="5e163-110">[Инкомплетедата][]</span><span class="sxs-lookup"><span data-stu-id="5e163-110">[incompleteData][]</span></span>      | <span data-ttu-id="5e163-111">Указывает, что статистика в этом интервале основана на неполных данных.</span><span class="sxs-lookup"><span data-stu-id="5e163-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="5e163-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e163-112">Read-only.</span></span>
| <span data-ttu-id="5e163-113">Тенденция</span><span class="sxs-lookup"><span data-stu-id="5e163-113">isTrending</span></span>       | <span data-ttu-id="5e163-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e163-114">Boolean</span></span>                 | <span data-ttu-id="5e163-115">Указывает, является ли элемент "тенденция".</span><span class="sxs-lookup"><span data-stu-id="5e163-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="5e163-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e163-116">Read-only.</span></span>
| <span data-ttu-id="5e163-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5e163-117">startDateTime</span></span>    | <span data-ttu-id="5e163-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e163-118">DateTimeOffset</span></span>          | <span data-ttu-id="5e163-119">Время начала интервала.</span><span class="sxs-lookup"><span data-stu-id="5e163-119">When the interval starts.</span></span> <span data-ttu-id="5e163-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e163-120">Read-only.</span></span>
| <span data-ttu-id="5e163-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5e163-121">endDateTime</span></span>      | <span data-ttu-id="5e163-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e163-122">DateTimeOffset</span></span>          | <span data-ttu-id="5e163-123">По окончании интервала.</span><span class="sxs-lookup"><span data-stu-id="5e163-123">When the interval ends.</span></span> <span data-ttu-id="5e163-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e163-124">Read-only.</span></span>
| <span data-ttu-id="5e163-125">create</span><span class="sxs-lookup"><span data-stu-id="5e163-125">create</span></span>           | <span data-ttu-id="5e163-126">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="5e163-126">[itemActionStat][]</span></span>      | <span data-ttu-id="5e163-127">Статистика по действиям по **созданию** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="5e163-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="5e163-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e163-128">Read-only.</span></span>
| <span data-ttu-id="5e163-129">edit</span><span class="sxs-lookup"><span data-stu-id="5e163-129">edit</span></span>             | <span data-ttu-id="5e163-130">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="5e163-130">[itemActionStat][]</span></span>      | <span data-ttu-id="5e163-131">Статистика действий **редактирования** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="5e163-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="5e163-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e163-132">Read-only.</span></span>
| <span data-ttu-id="5e163-133">delete</span><span class="sxs-lookup"><span data-stu-id="5e163-133">delete</span></span>           | <span data-ttu-id="5e163-134">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="5e163-134">[itemActionStat][]</span></span>      | <span data-ttu-id="5e163-135">Статистика действий **удаления** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="5e163-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="5e163-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e163-136">Read-only.</span></span>
| <span data-ttu-id="5e163-137">move</span><span class="sxs-lookup"><span data-stu-id="5e163-137">move</span></span>             | <span data-ttu-id="5e163-138">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="5e163-138">[itemActionStat][]</span></span>      | <span data-ttu-id="5e163-139">Статистика действий **перемещения** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="5e163-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="5e163-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e163-140">Read-only.</span></span>
| <span data-ttu-id="5e163-141">обращения</span><span class="sxs-lookup"><span data-stu-id="5e163-141">access</span></span>           | <span data-ttu-id="5e163-142">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="5e163-142">[itemActionStat][]</span></span>      | <span data-ttu-id="5e163-143">Статистика действий **доступа** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="5e163-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="5e163-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e163-144">Read-only.</span></span>

[Итемактионстат]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[Инкомплетедата]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="5e163-147">Связи</span><span class="sxs-lookup"><span data-stu-id="5e163-147">Relationships</span></span>

| <span data-ttu-id="5e163-148">Имя связи</span><span class="sxs-lookup"><span data-stu-id="5e163-148">Relationship name</span></span> | <span data-ttu-id="5e163-149">Тип</span><span class="sxs-lookup"><span data-stu-id="5e163-149">Type</span></span>                        | <span data-ttu-id="5e163-150">Описание</span><span class="sxs-lookup"><span data-stu-id="5e163-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="5e163-151">activities</span><span class="sxs-lookup"><span data-stu-id="5e163-151">activities</span></span>        | <span data-ttu-id="5e163-152">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="5e163-152">[itemActivity][] collection</span></span> | <span data-ttu-id="5e163-153">Предоставляет **итемактивитиес** , представленные в этом ресурсе **итемактивитистат** .</span><span class="sxs-lookup"><span data-stu-id="5e163-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="5e163-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e163-155">JSON representation</span></span>

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
