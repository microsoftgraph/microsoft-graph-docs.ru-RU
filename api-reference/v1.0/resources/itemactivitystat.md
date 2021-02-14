---
author: daspek
title: Тип ресурса itemActivityStat
description: Объект ItemActivityStat предоставляет сведения о действиях, которые произошли с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a33453fc884fc6dba7bd5b8fbcf4edc0261c11cb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238682"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="716cf-103">Тип ресурса itemActivityStat</span><span class="sxs-lookup"><span data-stu-id="716cf-103">itemActivityStat resource type</span></span>

<span data-ttu-id="716cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="716cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="716cf-105">Ресурс **itemActivityStat** предоставляет сведения о действиях, которые произошли в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="716cf-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="716cf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="716cf-106">Properties</span></span>

| <span data-ttu-id="716cf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="716cf-107">Property</span></span>         | <span data-ttu-id="716cf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="716cf-108">Type</span></span>                    | <span data-ttu-id="716cf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="716cf-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="716cf-110">incompleteData</span><span class="sxs-lookup"><span data-stu-id="716cf-110">incompleteData</span></span>   | <span data-ttu-id="716cf-111">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="716cf-111">[incompleteData][]</span></span>      | <span data-ttu-id="716cf-112">Указывает, что статистика за этот интервал основана на неполных данных.</span><span class="sxs-lookup"><span data-stu-id="716cf-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="716cf-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="716cf-113">Read-only.</span></span>
| <span data-ttu-id="716cf-114">isTrending</span><span class="sxs-lookup"><span data-stu-id="716cf-114">isTrending</span></span>       | <span data-ttu-id="716cf-115">Логическое</span><span class="sxs-lookup"><span data-stu-id="716cf-115">Boolean</span></span>                 | <span data-ttu-id="716cf-116">Указывает, является ли элемент "трендом".</span><span class="sxs-lookup"><span data-stu-id="716cf-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="716cf-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="716cf-117">Read-only.</span></span>
| <span data-ttu-id="716cf-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="716cf-118">startDateTime</span></span>    | <span data-ttu-id="716cf-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="716cf-119">DateTimeOffset</span></span>          | <span data-ttu-id="716cf-120">Когда начинается интервал.</span><span class="sxs-lookup"><span data-stu-id="716cf-120">When the interval starts.</span></span> <span data-ttu-id="716cf-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="716cf-121">Read-only.</span></span>
| <span data-ttu-id="716cf-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="716cf-122">endDateTime</span></span>      | <span data-ttu-id="716cf-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="716cf-123">DateTimeOffset</span></span>          | <span data-ttu-id="716cf-124">Когда интервал заканчивается.</span><span class="sxs-lookup"><span data-stu-id="716cf-124">When the interval ends.</span></span> <span data-ttu-id="716cf-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="716cf-125">Read-only.</span></span>
| <span data-ttu-id="716cf-126">create</span><span class="sxs-lookup"><span data-stu-id="716cf-126">create</span></span>           | <span data-ttu-id="716cf-127">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="716cf-127">[itemActionStat][]</span></span>      | <span data-ttu-id="716cf-128">Статистика о действиях **создания** за этот интервал.</span><span class="sxs-lookup"><span data-stu-id="716cf-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="716cf-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="716cf-129">Read-only.</span></span>
| <span data-ttu-id="716cf-130">edit</span><span class="sxs-lookup"><span data-stu-id="716cf-130">edit</span></span>             | <span data-ttu-id="716cf-131">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="716cf-131">[itemActionStat][]</span></span>      | <span data-ttu-id="716cf-132">Статистика о действиях **редактирования** за этот интервал.</span><span class="sxs-lookup"><span data-stu-id="716cf-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="716cf-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="716cf-133">Read-only.</span></span>
| <span data-ttu-id="716cf-134">delete</span><span class="sxs-lookup"><span data-stu-id="716cf-134">delete</span></span>           | <span data-ttu-id="716cf-135">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="716cf-135">[itemActionStat][]</span></span>      | <span data-ttu-id="716cf-136">Статистика о действиях **удаления** за этот интервал.</span><span class="sxs-lookup"><span data-stu-id="716cf-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="716cf-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="716cf-137">Read-only.</span></span>
| <span data-ttu-id="716cf-138">move</span><span class="sxs-lookup"><span data-stu-id="716cf-138">move</span></span>             | <span data-ttu-id="716cf-139">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="716cf-139">[itemActionStat][]</span></span>      | <span data-ttu-id="716cf-140">Статистика о действиях **перемещения** за этот интервал.</span><span class="sxs-lookup"><span data-stu-id="716cf-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="716cf-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="716cf-141">Read-only.</span></span>
| <span data-ttu-id="716cf-142">access</span><span class="sxs-lookup"><span data-stu-id="716cf-142">access</span></span>           | <span data-ttu-id="716cf-143">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="716cf-143">[itemActionStat][]</span></span>      | <span data-ttu-id="716cf-144">Статистика о действиях **доступа** за этот интервал.</span><span class="sxs-lookup"><span data-stu-id="716cf-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="716cf-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="716cf-145">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="716cf-148">Связи</span><span class="sxs-lookup"><span data-stu-id="716cf-148">Relationships</span></span>

| <span data-ttu-id="716cf-149">Имя связи</span><span class="sxs-lookup"><span data-stu-id="716cf-149">Relationship name</span></span> | <span data-ttu-id="716cf-150">Тип</span><span class="sxs-lookup"><span data-stu-id="716cf-150">Type</span></span>                        | <span data-ttu-id="716cf-151">Описание</span><span class="sxs-lookup"><span data-stu-id="716cf-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="716cf-152">activities</span><span class="sxs-lookup"><span data-stu-id="716cf-152">activities</span></span>        | <span data-ttu-id="716cf-153">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="716cf-153">[itemActivity][] collection</span></span> | <span data-ttu-id="716cf-154">Предоставляет объект **itemActivities,** представленный в **ресурсе itemActivityStat.**</span><span class="sxs-lookup"><span data-stu-id="716cf-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="716cf-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="716cf-156">JSON representation</span></span>

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

