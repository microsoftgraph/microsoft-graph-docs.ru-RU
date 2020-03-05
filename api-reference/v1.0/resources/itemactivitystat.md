---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактивитистат
description: Объект Итемактивитистат предоставляет сведения о действиях, выполненных с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 11b19e4b953d4353382aec15071c6589b5bb23c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447670"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="8779b-103">Тип ресурса Итемактивитистат</span><span class="sxs-lookup"><span data-stu-id="8779b-103">itemActivityStat resource type</span></span>

<span data-ttu-id="8779b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8779b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8779b-105">Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="8779b-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="8779b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8779b-106">Properties</span></span>

| <span data-ttu-id="8779b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8779b-107">Property</span></span>         | <span data-ttu-id="8779b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8779b-108">Type</span></span>                    | <span data-ttu-id="8779b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8779b-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="8779b-110">инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="8779b-110">incompleteData</span></span>   | <span data-ttu-id="8779b-111">[инкомплетедата][]</span><span class="sxs-lookup"><span data-stu-id="8779b-111">[incompleteData][]</span></span>      | <span data-ttu-id="8779b-112">Указывает, что статистика в этом интервале основана на неполных данных.</span><span class="sxs-lookup"><span data-stu-id="8779b-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="8779b-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8779b-113">Read-only.</span></span>
| <span data-ttu-id="8779b-114">Тенденция</span><span class="sxs-lookup"><span data-stu-id="8779b-114">isTrending</span></span>       | <span data-ttu-id="8779b-115">Логический</span><span class="sxs-lookup"><span data-stu-id="8779b-115">Boolean</span></span>                 | <span data-ttu-id="8779b-116">Указывает, является ли элемент "тенденция".</span><span class="sxs-lookup"><span data-stu-id="8779b-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="8779b-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8779b-117">Read-only.</span></span>
| <span data-ttu-id="8779b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8779b-118">startDateTime</span></span>    | <span data-ttu-id="8779b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8779b-119">DateTimeOffset</span></span>          | <span data-ttu-id="8779b-120">Время начала интервала.</span><span class="sxs-lookup"><span data-stu-id="8779b-120">When the interval starts.</span></span> <span data-ttu-id="8779b-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8779b-121">Read-only.</span></span>
| <span data-ttu-id="8779b-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8779b-122">endDateTime</span></span>      | <span data-ttu-id="8779b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8779b-123">DateTimeOffset</span></span>          | <span data-ttu-id="8779b-124">По окончании интервала.</span><span class="sxs-lookup"><span data-stu-id="8779b-124">When the interval ends.</span></span> <span data-ttu-id="8779b-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8779b-125">Read-only.</span></span>
| <span data-ttu-id="8779b-126">create</span><span class="sxs-lookup"><span data-stu-id="8779b-126">create</span></span>           | <span data-ttu-id="8779b-127">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="8779b-127">[itemActionStat][]</span></span>      | <span data-ttu-id="8779b-128">Статистика по действиям по **созданию** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="8779b-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="8779b-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8779b-129">Read-only.</span></span>
| <span data-ttu-id="8779b-130">edit</span><span class="sxs-lookup"><span data-stu-id="8779b-130">edit</span></span>             | <span data-ttu-id="8779b-131">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="8779b-131">[itemActionStat][]</span></span>      | <span data-ttu-id="8779b-132">Статистика действий **редактирования** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="8779b-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="8779b-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8779b-133">Read-only.</span></span>
| <span data-ttu-id="8779b-134">delete</span><span class="sxs-lookup"><span data-stu-id="8779b-134">delete</span></span>           | <span data-ttu-id="8779b-135">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="8779b-135">[itemActionStat][]</span></span>      | <span data-ttu-id="8779b-136">Статистика действий **удаления** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="8779b-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="8779b-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8779b-137">Read-only.</span></span>
| <span data-ttu-id="8779b-138">move</span><span class="sxs-lookup"><span data-stu-id="8779b-138">move</span></span>             | <span data-ttu-id="8779b-139">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="8779b-139">[itemActionStat][]</span></span>      | <span data-ttu-id="8779b-140">Статистика действий **перемещения** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="8779b-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="8779b-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8779b-141">Read-only.</span></span>
| <span data-ttu-id="8779b-142">обращения</span><span class="sxs-lookup"><span data-stu-id="8779b-142">access</span></span>           | <span data-ttu-id="8779b-143">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="8779b-143">[itemActionStat][]</span></span>      | <span data-ttu-id="8779b-144">Статистика действий **доступа** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="8779b-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="8779b-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8779b-145">Read-only.</span></span>

[итемактионстат]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[инкомплетедата]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="8779b-148">Связи</span><span class="sxs-lookup"><span data-stu-id="8779b-148">Relationships</span></span>

| <span data-ttu-id="8779b-149">Имя связи</span><span class="sxs-lookup"><span data-stu-id="8779b-149">Relationship name</span></span> | <span data-ttu-id="8779b-150">Тип</span><span class="sxs-lookup"><span data-stu-id="8779b-150">Type</span></span>                        | <span data-ttu-id="8779b-151">Описание</span><span class="sxs-lookup"><span data-stu-id="8779b-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="8779b-152">activities</span><span class="sxs-lookup"><span data-stu-id="8779b-152">activities</span></span>        | <span data-ttu-id="8779b-153">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="8779b-153">[itemActivity][] collection</span></span> | <span data-ttu-id="8779b-154">Предоставляет **итемактивитиес** , представленные в этом ресурсе **итемактивитистат** .</span><span class="sxs-lookup"><span data-stu-id="8779b-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8779b-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8779b-156">JSON representation</span></span>

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
