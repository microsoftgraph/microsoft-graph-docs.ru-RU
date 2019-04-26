---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: Итемактивитистат
localization_priority: Normal
ms.openlocfilehash: 08bbfd414a32e8eb8a0144d879ede55c71c19b89
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339883"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="edb83-102">Тип ресурса Итемактивитистат</span><span class="sxs-lookup"><span data-stu-id="edb83-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edb83-103">Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="edb83-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="edb83-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edb83-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="edb83-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="edb83-105">Properties</span></span>

| <span data-ttu-id="edb83-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="edb83-106">Property</span></span>         | <span data-ttu-id="edb83-107">Тип</span><span class="sxs-lookup"><span data-stu-id="edb83-107">Type</span></span>                    | <span data-ttu-id="edb83-108">Описание</span><span class="sxs-lookup"><span data-stu-id="edb83-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="edb83-109">Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="edb83-109">incompleteData</span></span>   | <span data-ttu-id="edb83-110">[Инкомплетедата][]</span><span class="sxs-lookup"><span data-stu-id="edb83-110">[incompleteData][]</span></span>      | <span data-ttu-id="edb83-111">Указывает, что статистика в этом интервале основана на неполных данных.</span><span class="sxs-lookup"><span data-stu-id="edb83-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="edb83-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edb83-112">Read-only.</span></span>
| <span data-ttu-id="edb83-113">Тенденция</span><span class="sxs-lookup"><span data-stu-id="edb83-113">isTrending</span></span>       | <span data-ttu-id="edb83-114">Логический</span><span class="sxs-lookup"><span data-stu-id="edb83-114">Boolean</span></span>                 | <span data-ttu-id="edb83-115">Указывает, является ли элемент "тенденция".</span><span class="sxs-lookup"><span data-stu-id="edb83-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="edb83-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edb83-116">Read-only.</span></span>
| <span data-ttu-id="edb83-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="edb83-117">startDateTime</span></span>    | <span data-ttu-id="edb83-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edb83-118">DateTimeOffset</span></span>          | <span data-ttu-id="edb83-119">Время начала интервала.</span><span class="sxs-lookup"><span data-stu-id="edb83-119">When the interval starts.</span></span> <span data-ttu-id="edb83-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edb83-120">Read-only.</span></span>
| <span data-ttu-id="edb83-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="edb83-121">endDateTime</span></span>      | <span data-ttu-id="edb83-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edb83-122">DateTimeOffset</span></span>          | <span data-ttu-id="edb83-123">По окончании интервала.</span><span class="sxs-lookup"><span data-stu-id="edb83-123">When the interval ends.</span></span> <span data-ttu-id="edb83-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edb83-124">Read-only.</span></span>
| <span data-ttu-id="edb83-125">create</span><span class="sxs-lookup"><span data-stu-id="edb83-125">create</span></span>           | <span data-ttu-id="edb83-126">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="edb83-126">[itemActionStat][]</span></span>      | <span data-ttu-id="edb83-127">Статистика по действиям по **созданию** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="edb83-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="edb83-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edb83-128">Read-only.</span></span>
| <span data-ttu-id="edb83-129">edit</span><span class="sxs-lookup"><span data-stu-id="edb83-129">edit</span></span>             | <span data-ttu-id="edb83-130">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="edb83-130">[itemActionStat][]</span></span>      | <span data-ttu-id="edb83-131">Статистика действий **редактирования** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="edb83-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="edb83-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edb83-132">Read-only.</span></span>
| <span data-ttu-id="edb83-133">delete</span><span class="sxs-lookup"><span data-stu-id="edb83-133">delete</span></span>           | <span data-ttu-id="edb83-134">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="edb83-134">[itemActionStat][]</span></span>      | <span data-ttu-id="edb83-135">Статистика действий **удаления** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="edb83-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="edb83-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edb83-136">Read-only.</span></span>
| <span data-ttu-id="edb83-137">move</span><span class="sxs-lookup"><span data-stu-id="edb83-137">move</span></span>             | <span data-ttu-id="edb83-138">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="edb83-138">[itemActionStat][]</span></span>      | <span data-ttu-id="edb83-139">Статистика действий **перемещения** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="edb83-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="edb83-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edb83-140">Read-only.</span></span>
| <span data-ttu-id="edb83-141">обращения</span><span class="sxs-lookup"><span data-stu-id="edb83-141">access</span></span>           | <span data-ttu-id="edb83-142">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="edb83-142">[itemActionStat][]</span></span>      | <span data-ttu-id="edb83-143">Статистика действий **доступа** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="edb83-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="edb83-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edb83-144">Read-only.</span></span>

[Итемактионстат]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[Инкомплетедата]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="edb83-147">Связи</span><span class="sxs-lookup"><span data-stu-id="edb83-147">Relationships</span></span>

| <span data-ttu-id="edb83-148">Имя связи</span><span class="sxs-lookup"><span data-stu-id="edb83-148">Relationship name</span></span> | <span data-ttu-id="edb83-149">Тип</span><span class="sxs-lookup"><span data-stu-id="edb83-149">Type</span></span>                        | <span data-ttu-id="edb83-150">Описание</span><span class="sxs-lookup"><span data-stu-id="edb83-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="edb83-151">activities</span><span class="sxs-lookup"><span data-stu-id="edb83-151">activities</span></span>        | <span data-ttu-id="edb83-152">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="edb83-152">[itemActivity][] collection</span></span> | <span data-ttu-id="edb83-153">Предоставляет **итемактивитиес** , представленные в этом ресурсе **итемактивитистат** .</span><span class="sxs-lookup"><span data-stu-id="edb83-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="edb83-155">Замечания</span><span class="sxs-lookup"><span data-stu-id="edb83-155">Remarks</span></span>

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
