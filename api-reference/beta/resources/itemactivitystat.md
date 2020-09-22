---
author: daspek
description: Ресурс Итемактивитистат предоставляет сведения о действиях, которые выполнялись в течение интервала времени.
ms.date: 09/14/2017
title: итемактивитистат
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c21183911e111b2070d463f4552f913d93780493
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075664"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="f4e53-103">Тип ресурса Итемактивитистат</span><span class="sxs-lookup"><span data-stu-id="f4e53-103">itemActivityStat resource type</span></span>

<span data-ttu-id="f4e53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4e53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4e53-105">Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="f4e53-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4e53-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4e53-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f4e53-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4e53-107">Properties</span></span>

| <span data-ttu-id="f4e53-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4e53-108">Property</span></span>         | <span data-ttu-id="f4e53-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f4e53-109">Type</span></span>                    | <span data-ttu-id="f4e53-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f4e53-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="f4e53-111">инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="f4e53-111">incompleteData</span></span>   | <span data-ttu-id="f4e53-112">[инкомплетедата][]</span><span class="sxs-lookup"><span data-stu-id="f4e53-112">[incompleteData][]</span></span>      | <span data-ttu-id="f4e53-113">Указывает, что статистика в этом интервале основана на неполных данных.</span><span class="sxs-lookup"><span data-stu-id="f4e53-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="f4e53-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4e53-114">Read-only.</span></span>
| <span data-ttu-id="f4e53-115">Тенденция</span><span class="sxs-lookup"><span data-stu-id="f4e53-115">isTrending</span></span>       | <span data-ttu-id="f4e53-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4e53-116">Boolean</span></span>                 | <span data-ttu-id="f4e53-117">Указывает, является ли элемент "тенденция".</span><span class="sxs-lookup"><span data-stu-id="f4e53-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="f4e53-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4e53-118">Read-only.</span></span>
| <span data-ttu-id="f4e53-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f4e53-119">startDateTime</span></span>    | <span data-ttu-id="f4e53-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4e53-120">DateTimeOffset</span></span>          | <span data-ttu-id="f4e53-121">Время начала интервала.</span><span class="sxs-lookup"><span data-stu-id="f4e53-121">When the interval starts.</span></span> <span data-ttu-id="f4e53-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4e53-122">Read-only.</span></span>
| <span data-ttu-id="f4e53-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f4e53-123">endDateTime</span></span>      | <span data-ttu-id="f4e53-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4e53-124">DateTimeOffset</span></span>          | <span data-ttu-id="f4e53-125">По окончании интервала.</span><span class="sxs-lookup"><span data-stu-id="f4e53-125">When the interval ends.</span></span> <span data-ttu-id="f4e53-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4e53-126">Read-only.</span></span>
| <span data-ttu-id="f4e53-127">create</span><span class="sxs-lookup"><span data-stu-id="f4e53-127">create</span></span>           | <span data-ttu-id="f4e53-128">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="f4e53-128">[itemActionStat][]</span></span>      | <span data-ttu-id="f4e53-129">Статистика по действиям по **созданию** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="f4e53-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="f4e53-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4e53-130">Read-only.</span></span>
| <span data-ttu-id="f4e53-131">edit</span><span class="sxs-lookup"><span data-stu-id="f4e53-131">edit</span></span>             | <span data-ttu-id="f4e53-132">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="f4e53-132">[itemActionStat][]</span></span>      | <span data-ttu-id="f4e53-133">Статистика действий **редактирования** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="f4e53-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="f4e53-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4e53-134">Read-only.</span></span>
| <span data-ttu-id="f4e53-135">delete</span><span class="sxs-lookup"><span data-stu-id="f4e53-135">delete</span></span>           | <span data-ttu-id="f4e53-136">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="f4e53-136">[itemActionStat][]</span></span>      | <span data-ttu-id="f4e53-137">Статистика действий **удаления** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="f4e53-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="f4e53-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4e53-138">Read-only.</span></span>
| <span data-ttu-id="f4e53-139">move</span><span class="sxs-lookup"><span data-stu-id="f4e53-139">move</span></span>             | <span data-ttu-id="f4e53-140">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="f4e53-140">[itemActionStat][]</span></span>      | <span data-ttu-id="f4e53-141">Статистика действий **перемещения** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="f4e53-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="f4e53-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4e53-142">Read-only.</span></span>
| <span data-ttu-id="f4e53-143">обращения</span><span class="sxs-lookup"><span data-stu-id="f4e53-143">access</span></span>           | <span data-ttu-id="f4e53-144">[итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="f4e53-144">[itemActionStat][]</span></span>      | <span data-ttu-id="f4e53-145">Статистика действий **доступа** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="f4e53-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="f4e53-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4e53-146">Read-only.</span></span>

[итемактионстат]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[инкомплетедата]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="f4e53-149">Связи</span><span class="sxs-lookup"><span data-stu-id="f4e53-149">Relationships</span></span>

| <span data-ttu-id="f4e53-150">Имя связи</span><span class="sxs-lookup"><span data-stu-id="f4e53-150">Relationship name</span></span> | <span data-ttu-id="f4e53-151">Тип</span><span class="sxs-lookup"><span data-stu-id="f4e53-151">Type</span></span>                        | <span data-ttu-id="f4e53-152">Описание</span><span class="sxs-lookup"><span data-stu-id="f4e53-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="f4e53-153">activities</span><span class="sxs-lookup"><span data-stu-id="f4e53-153">activities</span></span>        | <span data-ttu-id="f4e53-154">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="f4e53-154">[itemActivity][] collection</span></span> | <span data-ttu-id="f4e53-155">Предоставляет **итемактивитиес** , представленные в этом ресурсе **итемактивитистат** .</span><span class="sxs-lookup"><span data-stu-id="f4e53-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="f4e53-157">Замечания</span><span class="sxs-lookup"><span data-stu-id="f4e53-157">Remarks</span></span>

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


