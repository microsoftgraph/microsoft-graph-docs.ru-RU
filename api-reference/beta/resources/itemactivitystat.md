---
author: daspek
description: Ресурс Итемактивитистат предоставляет сведения о действиях, которые выполнялись в течение интервала времени.
ms.date: 09/14/2017
title: итемактивитистат
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 612acf6ef619f13b0c334dd2046041b25020f450
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523116"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="1f47a-103">Тип ресурса Итемактивитистат</span><span class="sxs-lookup"><span data-stu-id="1f47a-103">itemActivityStat resource type</span></span>

<span data-ttu-id="1f47a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1f47a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f47a-105">Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="1f47a-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f47a-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f47a-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1f47a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f47a-107">Properties</span></span>

| <span data-ttu-id="1f47a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f47a-108">Property</span></span>         | <span data-ttu-id="1f47a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1f47a-109">Type</span></span>                    | <span data-ttu-id="1f47a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1f47a-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="1f47a-111">инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="1f47a-111">incompleteData</span></span>   | <span data-ttu-id="1f47a-112">[инкомплетедата][]</span><span class="sxs-lookup"><span data-stu-id="1f47a-112">[incompleteData][]</span></span>      | <span data-ttu-id="1f47a-113">Указывает, что статистика в этом интервале основана на неполных данных.</span><span class="sxs-lookup"><span data-stu-id="1f47a-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="1f47a-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f47a-114">Read-only.</span></span>
| <span data-ttu-id="1f47a-115">Тенденция</span><span class="sxs-lookup"><span data-stu-id="1f47a-115">isTrending</span></span>       | <span data-ttu-id="1f47a-116">Логический</span><span class="sxs-lookup"><span data-stu-id="1f47a-116">Boolean</span></span>                 | <span data-ttu-id="1f47a-117">Указывает, является ли элемент "тенденция".</span><span class="sxs-lookup"><span data-stu-id="1f47a-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="1f47a-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f47a-118">Read-only.</span></span>
| <span data-ttu-id="1f47a-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1f47a-119">startDateTime</span></span>    | <span data-ttu-id="1f47a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f47a-120">DateTimeOffset</span></span>          | <span data-ttu-id="1f47a-121">Время начала интервала.</span><span class="sxs-lookup"><span data-stu-id="1f47a-121">When the interval starts.</span></span> <span data-ttu-id="1f47a-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f47a-122">Read-only.</span></span>
| <span data-ttu-id="1f47a-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1f47a-123">endDateTime</span></span>      | <span data-ttu-id="1f47a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f47a-124">DateTimeOffset</span></span>          | <span data-ttu-id="1f47a-125">По окончании интервала.</span><span class="sxs-lookup"><span data-stu-id="1f47a-125">When the interval ends.</span></span> <span data-ttu-id="1f47a-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f47a-126">Read-only.</span></span>
| <span data-ttu-id="1f47a-127">create</span><span class="sxs-lookup"><span data-stu-id="1f47a-127">create</span></span>           | <span data-ttu-id="1f47a-128">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="1f47a-128">[itemActionStat][]</span></span>      | <span data-ttu-id="1f47a-129">Статистика по действиям по **созданию** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="1f47a-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="1f47a-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f47a-130">Read-only.</span></span>
| <span data-ttu-id="1f47a-131">edit</span><span class="sxs-lookup"><span data-stu-id="1f47a-131">edit</span></span>             | <span data-ttu-id="1f47a-132">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="1f47a-132">[itemActionStat][]</span></span>      | <span data-ttu-id="1f47a-133">Статистика действий **редактирования** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="1f47a-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="1f47a-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f47a-134">Read-only.</span></span>
| <span data-ttu-id="1f47a-135">delete</span><span class="sxs-lookup"><span data-stu-id="1f47a-135">delete</span></span>           | <span data-ttu-id="1f47a-136">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="1f47a-136">[itemActionStat][]</span></span>      | <span data-ttu-id="1f47a-137">Статистика действий **удаления** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="1f47a-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="1f47a-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f47a-138">Read-only.</span></span>
| <span data-ttu-id="1f47a-139">move</span><span class="sxs-lookup"><span data-stu-id="1f47a-139">move</span></span>             | <span data-ttu-id="1f47a-140">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="1f47a-140">[itemActionStat][]</span></span>      | <span data-ttu-id="1f47a-141">Статистика действий **перемещения** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="1f47a-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="1f47a-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f47a-142">Read-only.</span></span>
| <span data-ttu-id="1f47a-143">обращения</span><span class="sxs-lookup"><span data-stu-id="1f47a-143">access</span></span>           | <span data-ttu-id="1f47a-144">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="1f47a-144">[itemActionStat][]</span></span>      | <span data-ttu-id="1f47a-145">Статистика действий **доступа** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="1f47a-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="1f47a-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f47a-146">Read-only.</span></span>

[итемактионстат]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[инкомплетедата]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="1f47a-149">Связи</span><span class="sxs-lookup"><span data-stu-id="1f47a-149">Relationships</span></span>

| <span data-ttu-id="1f47a-150">Имя связи</span><span class="sxs-lookup"><span data-stu-id="1f47a-150">Relationship name</span></span> | <span data-ttu-id="1f47a-151">Тип</span><span class="sxs-lookup"><span data-stu-id="1f47a-151">Type</span></span>                        | <span data-ttu-id="1f47a-152">Описание</span><span class="sxs-lookup"><span data-stu-id="1f47a-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="1f47a-153">activities</span><span class="sxs-lookup"><span data-stu-id="1f47a-153">activities</span></span>        | <span data-ttu-id="1f47a-154">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="1f47a-154">[itemActivity][] collection</span></span> | <span data-ttu-id="1f47a-155">Предоставляет **итемактивитиес** , представленные в этом ресурсе **итемактивитистат** .</span><span class="sxs-lookup"><span data-stu-id="1f47a-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="1f47a-157">Замечания</span><span class="sxs-lookup"><span data-stu-id="1f47a-157">Remarks</span></span>

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
