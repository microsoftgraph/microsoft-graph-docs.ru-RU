---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
ms.openlocfilehash: 067cf88773b5f5d69b2b3538a2ddeab6741631a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075135"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="dc556-102">Тип ресурса itemActivityStat</span><span class="sxs-lookup"><span data-stu-id="dc556-102">itemActivityStat resource type</span></span>

> <span data-ttu-id="dc556-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc556-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc556-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc556-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc556-105">Ресурс **itemActivityStat** содержит сведения о действиях, выполняемых в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="dc556-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc556-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc556-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="dc556-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc556-107">Properties</span></span>

| <span data-ttu-id="dc556-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc556-108">Property</span></span>         | <span data-ttu-id="dc556-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dc556-109">Type</span></span>                    | <span data-ttu-id="dc556-110">Description</span><span class="sxs-lookup"><span data-stu-id="dc556-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="dc556-111">incompleteData</span><span class="sxs-lookup"><span data-stu-id="dc556-111">incompleteData</span></span>   | <span data-ttu-id="dc556-112">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="dc556-112">[incompleteData][]</span></span>      | <span data-ttu-id="dc556-113">Указывает, что Статистика ожидания основаны на неполные данные.</span><span class="sxs-lookup"><span data-stu-id="dc556-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="dc556-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc556-114">Read-only.</span></span>
| <span data-ttu-id="dc556-115">isTrending</span><span class="sxs-lookup"><span data-stu-id="dc556-115">isTrending</span></span>       | <span data-ttu-id="dc556-116">Логический</span><span class="sxs-lookup"><span data-stu-id="dc556-116">Boolean</span></span>                 | <span data-ttu-id="dc556-117">Указывает, является ли элемент «прибора.»</span><span class="sxs-lookup"><span data-stu-id="dc556-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="dc556-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc556-118">Read-only.</span></span>
| <span data-ttu-id="dc556-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dc556-119">startDateTime</span></span>    | <span data-ttu-id="dc556-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc556-120">DateTimeOffset</span></span>          | <span data-ttu-id="dc556-121">При запуске интервала.</span><span class="sxs-lookup"><span data-stu-id="dc556-121">When the interval starts.</span></span> <span data-ttu-id="dc556-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc556-122">Read-only.</span></span>
| <span data-ttu-id="dc556-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="dc556-123">endDateTime</span></span>      | <span data-ttu-id="dc556-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc556-124">DateTimeOffset</span></span>          | <span data-ttu-id="dc556-125">Окончания интервала.</span><span class="sxs-lookup"><span data-stu-id="dc556-125">When the interval ends.</span></span> <span data-ttu-id="dc556-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc556-126">Read-only.</span></span>
| <span data-ttu-id="dc556-127">create</span><span class="sxs-lookup"><span data-stu-id="dc556-127">create</span></span>           | <span data-ttu-id="dc556-128">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="dc556-128">[itemActionStat][]</span></span>      | <span data-ttu-id="dc556-129">Сведения о действия **Создание** ожидания.</span><span class="sxs-lookup"><span data-stu-id="dc556-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="dc556-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc556-130">Read-only.</span></span>
| <span data-ttu-id="dc556-131">edit</span><span class="sxs-lookup"><span data-stu-id="dc556-131">edit</span></span>             | <span data-ttu-id="dc556-132">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="dc556-132">[itemActionStat][]</span></span>      | <span data-ttu-id="dc556-133">Сведения о действия **редактирования** в этот интервал.</span><span class="sxs-lookup"><span data-stu-id="dc556-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="dc556-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc556-134">Read-only.</span></span>
| <span data-ttu-id="dc556-135">delete</span><span class="sxs-lookup"><span data-stu-id="dc556-135">delete</span></span>           | <span data-ttu-id="dc556-136">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="dc556-136">[itemActionStat][]</span></span>      | <span data-ttu-id="dc556-137">Сведения о действиям **удаления** ожидания.</span><span class="sxs-lookup"><span data-stu-id="dc556-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="dc556-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc556-138">Read-only.</span></span>
| <span data-ttu-id="dc556-139">move</span><span class="sxs-lookup"><span data-stu-id="dc556-139">move</span></span>             | <span data-ttu-id="dc556-140">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="dc556-140">[itemActionStat][]</span></span>      | <span data-ttu-id="dc556-141">Сведения о действия **переместить** в этот интервал.</span><span class="sxs-lookup"><span data-stu-id="dc556-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="dc556-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc556-142">Read-only.</span></span>
| <span data-ttu-id="dc556-143">Access</span><span class="sxs-lookup"><span data-stu-id="dc556-143">access</span></span>           | <span data-ttu-id="dc556-144">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="dc556-144">[itemActionStat][]</span></span>      | <span data-ttu-id="dc556-145">Сведения о действия **клиента** в этот интервал.</span><span class="sxs-lookup"><span data-stu-id="dc556-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="dc556-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc556-146">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="dc556-149">Связи</span><span class="sxs-lookup"><span data-stu-id="dc556-149">Relationships</span></span>

| <span data-ttu-id="dc556-150">Имя связи</span><span class="sxs-lookup"><span data-stu-id="dc556-150">Relationship name</span></span> | <span data-ttu-id="dc556-151">Тип</span><span class="sxs-lookup"><span data-stu-id="dc556-151">Type</span></span>                        | <span data-ttu-id="dc556-152">Описание</span><span class="sxs-lookup"><span data-stu-id="dc556-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="dc556-153">activities</span><span class="sxs-lookup"><span data-stu-id="dc556-153">activities</span></span>        | <span data-ttu-id="dc556-154">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="dc556-154">[itemActivity][] collection</span></span> | <span data-ttu-id="dc556-155">Предоставляет **itemActivities** , представленного в этом **itemActivityStat** ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc556-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="dc556-157">Примечания</span><span class="sxs-lookup"><span data-stu-id="dc556-157">Remarks</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->
