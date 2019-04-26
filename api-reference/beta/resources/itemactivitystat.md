---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: Итемактивитистат
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561910"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="62db4-102">Тип ресурса Итемактивитистат</span><span class="sxs-lookup"><span data-stu-id="62db4-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62db4-103">Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="62db4-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62db4-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62db4-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="62db4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="62db4-105">Properties</span></span>

| <span data-ttu-id="62db4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="62db4-106">Property</span></span>         | <span data-ttu-id="62db4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="62db4-107">Type</span></span>                    | <span data-ttu-id="62db4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="62db4-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="62db4-109">Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="62db4-109">incompleteData</span></span>   | <span data-ttu-id="62db4-110">[Инкомплетедата][]</span><span class="sxs-lookup"><span data-stu-id="62db4-110">[incompleteData][]</span></span>      | <span data-ttu-id="62db4-111">Указывает, что статистика в этом интервале основана на неполных данных.</span><span class="sxs-lookup"><span data-stu-id="62db4-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="62db4-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62db4-112">Read-only.</span></span>
| <span data-ttu-id="62db4-113">Тенденция</span><span class="sxs-lookup"><span data-stu-id="62db4-113">isTrending</span></span>       | <span data-ttu-id="62db4-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="62db4-114">Boolean</span></span>                 | <span data-ttu-id="62db4-115">Указывает, является ли элемент "тенденция".</span><span class="sxs-lookup"><span data-stu-id="62db4-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="62db4-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62db4-116">Read-only.</span></span>
| <span data-ttu-id="62db4-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="62db4-117">startDateTime</span></span>    | <span data-ttu-id="62db4-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62db4-118">DateTimeOffset</span></span>          | <span data-ttu-id="62db4-119">Время начала интервала.</span><span class="sxs-lookup"><span data-stu-id="62db4-119">When the interval starts.</span></span> <span data-ttu-id="62db4-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62db4-120">Read-only.</span></span>
| <span data-ttu-id="62db4-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="62db4-121">endDateTime</span></span>      | <span data-ttu-id="62db4-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62db4-122">DateTimeOffset</span></span>          | <span data-ttu-id="62db4-123">По окончании интервала.</span><span class="sxs-lookup"><span data-stu-id="62db4-123">When the interval ends.</span></span> <span data-ttu-id="62db4-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62db4-124">Read-only.</span></span>
| <span data-ttu-id="62db4-125">create</span><span class="sxs-lookup"><span data-stu-id="62db4-125">create</span></span>           | <span data-ttu-id="62db4-126">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="62db4-126">[itemActionStat][]</span></span>      | <span data-ttu-id="62db4-127">Статистика по действиям по **созданию** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="62db4-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="62db4-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62db4-128">Read-only.</span></span>
| <span data-ttu-id="62db4-129">edit</span><span class="sxs-lookup"><span data-stu-id="62db4-129">edit</span></span>             | <span data-ttu-id="62db4-130">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="62db4-130">[itemActionStat][]</span></span>      | <span data-ttu-id="62db4-131">Статистика действий **редактирования** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="62db4-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="62db4-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62db4-132">Read-only.</span></span>
| <span data-ttu-id="62db4-133">delete</span><span class="sxs-lookup"><span data-stu-id="62db4-133">delete</span></span>           | <span data-ttu-id="62db4-134">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="62db4-134">[itemActionStat][]</span></span>      | <span data-ttu-id="62db4-135">Статистика действий **удаления** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="62db4-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="62db4-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62db4-136">Read-only.</span></span>
| <span data-ttu-id="62db4-137">move</span><span class="sxs-lookup"><span data-stu-id="62db4-137">move</span></span>             | <span data-ttu-id="62db4-138">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="62db4-138">[itemActionStat][]</span></span>      | <span data-ttu-id="62db4-139">Статистика действий **перемещения** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="62db4-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="62db4-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62db4-140">Read-only.</span></span>
| <span data-ttu-id="62db4-141">обращения</span><span class="sxs-lookup"><span data-stu-id="62db4-141">access</span></span>           | <span data-ttu-id="62db4-142">[Итемактионстат][]</span><span class="sxs-lookup"><span data-stu-id="62db4-142">[itemActionStat][]</span></span>      | <span data-ttu-id="62db4-143">Статистика действий **доступа** в этом интервале.</span><span class="sxs-lookup"><span data-stu-id="62db4-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="62db4-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62db4-144">Read-only.</span></span>

[Итемактионстат]: itemactionstat.md
[itemActionStat]: itemactionstat.md
[Инкомплетедата]: incompletedata.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="62db4-147">Связи</span><span class="sxs-lookup"><span data-stu-id="62db4-147">Relationships</span></span>

| <span data-ttu-id="62db4-148">Имя связи</span><span class="sxs-lookup"><span data-stu-id="62db4-148">Relationship name</span></span> | <span data-ttu-id="62db4-149">Тип</span><span class="sxs-lookup"><span data-stu-id="62db4-149">Type</span></span>                        | <span data-ttu-id="62db4-150">Описание</span><span class="sxs-lookup"><span data-stu-id="62db4-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="62db4-151">activities</span><span class="sxs-lookup"><span data-stu-id="62db4-151">activities</span></span>        | <span data-ttu-id="62db4-152">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="62db4-152">[itemActivity][] collection</span></span> | <span data-ttu-id="62db4-153">Предоставляет **итемактивитиес** , представленные в этом ресурсе **итемактивитистат** .</span><span class="sxs-lookup"><span data-stu-id="62db4-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="62db4-155">Замечания</span><span class="sxs-lookup"><span data-stu-id="62db4-155">Remarks</span></span>

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
