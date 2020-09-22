---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактивитистат
description: Объект Итемактивитистат предоставляет сведения о действиях, выполненных с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 80cc78486415f809082a2e9631dee86293e3389e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009326"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="0c68f-103">Тип ресурса Итемактивитистат</span><span class="sxs-lookup"><span data-stu-id="0c68f-103">itemActivityStat resource type</span></span>

<span data-ttu-id="0c68f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c68f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c68f-105">Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="0c68f-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="0c68f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c68f-106">Properties</span></span>

| <span data-ttu-id="0c68f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c68f-107">Property</span></span>         | <span data-ttu-id="0c68f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0c68f-108">Type</span></span>                    | <span data-ttu-id="0c68f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0c68f-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="0c68f-110">инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="0c68f-110">incompleteData</span></span>   | <span data-ttu-id="0c68f-111">[инкомплетедата][]</span><span class="sxs-lookup"><span data-stu-id="0c68f-111">[incompleteData][]</span></span>      | <span data-ttu-id="0c68f-112">Указывает, что статистика в этом интервале основана на неполных данных.</span><span class="sxs-lookup"><span data-stu-id="0c68f-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="0c68f-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c68f-113">Read-only.</span></span>
| <span data-ttu-id="0c68f-114">Тенденция</span><span class="sxs-lookup"><span data-stu-id="0c68f-114">isTrending</span></span>       | <span data-ttu-id="0c68f-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c68f-115">Boolean</span></span>                 | <span data-ttu-id="0c68f-116">Указывает, является ли элемент "тенденция".</span><span class="sxs-lookup"><span data-stu-id="0c68f-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="0c68f-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c68f-117">Read-only.</span></span>
| <span data-ttu-id="0c68f-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0c68f-118">startDateTime</span></span>    | <span data-ttu-id="0c68f-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c68f-119">DateTimeOffset</span></span>          | <span data-ttu-id="0c68f-120">Время начала интервала.</span><span class="sxs-lookup"><span data-stu-id="0c68f-120">When the interval starts.</span></span> <span data-ttu-id="0c68f-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c68f-121">Read-only.</span></span>
| <span data-ttu-id="0c68f-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0c68f-122">endDateTime</span></span>      | <span data-ttu-id="0c68f-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c68f-123">DateTimeOffset</span></span>          | <span data-ttu-id="0c68f-124">По окончании интервала.</span><span class="sxs-lookup"><span data-stu-id="0c68f-124">When the interval ends.</span></span> <span data-ttu-id="0c68f-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c68f-125">Read-only.</span></span>
| <span data-ttu-id="0c68f-126">create</span><span class="sxs-lookup"><span data-stu-id="0c68f-126">create</span></span>           | <span data-ttu-id="0c68f-127">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="0c68f-127">[itemActionStat][]</span></span>      | <span data-ttu-id="0c68f-128">Статистика по действиям по **созданию** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="0c68f-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="0c68f-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c68f-129">Read-only.</span></span>
| <span data-ttu-id="0c68f-130">edit</span><span class="sxs-lookup"><span data-stu-id="0c68f-130">edit</span></span>             | <span data-ttu-id="0c68f-131">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="0c68f-131">[itemActionStat][]</span></span>      | <span data-ttu-id="0c68f-132">Статистика действий **редактирования** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="0c68f-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="0c68f-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c68f-133">Read-only.</span></span>
| <span data-ttu-id="0c68f-134">delete</span><span class="sxs-lookup"><span data-stu-id="0c68f-134">delete</span></span>           | <span data-ttu-id="0c68f-135">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="0c68f-135">[itemActionStat][]</span></span>      | <span data-ttu-id="0c68f-136">Статистика действий **удаления** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="0c68f-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="0c68f-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c68f-137">Read-only.</span></span>
| <span data-ttu-id="0c68f-138">move</span><span class="sxs-lookup"><span data-stu-id="0c68f-138">move</span></span>             | <span data-ttu-id="0c68f-139">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="0c68f-139">[itemActionStat][]</span></span>      | <span data-ttu-id="0c68f-140">Статистика действий **перемещения** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="0c68f-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="0c68f-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c68f-141">Read-only.</span></span>
| <span data-ttu-id="0c68f-142">обращения</span><span class="sxs-lookup"><span data-stu-id="0c68f-142">access</span></span>           | <span data-ttu-id="0c68f-143">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="0c68f-143">[itemActionStat][]</span></span>      | <span data-ttu-id="0c68f-144">Статистика действий **доступа** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="0c68f-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="0c68f-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c68f-145">Read-only.</span></span>

[итемактионстат]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[инкомплетедата]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="0c68f-148">Связи</span><span class="sxs-lookup"><span data-stu-id="0c68f-148">Relationships</span></span>

| <span data-ttu-id="0c68f-149">Имя связи</span><span class="sxs-lookup"><span data-stu-id="0c68f-149">Relationship name</span></span> | <span data-ttu-id="0c68f-150">Тип</span><span class="sxs-lookup"><span data-stu-id="0c68f-150">Type</span></span>                        | <span data-ttu-id="0c68f-151">Описание</span><span class="sxs-lookup"><span data-stu-id="0c68f-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="0c68f-152">activities</span><span class="sxs-lookup"><span data-stu-id="0c68f-152">activities</span></span>        | <span data-ttu-id="0c68f-153">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="0c68f-153">[itemActivity][] collection</span></span> | <span data-ttu-id="0c68f-154">Предоставляет **итемактивитиес** , представленные в этом ресурсе **итемактивитистат** .</span><span class="sxs-lookup"><span data-stu-id="0c68f-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="0c68f-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c68f-156">JSON representation</span></span>

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

