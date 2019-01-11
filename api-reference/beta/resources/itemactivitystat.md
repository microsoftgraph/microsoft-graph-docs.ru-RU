---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: d0917d0100d33abee1095e2a7d06a4732d382937
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854252"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="f3242-102">Тип ресурса itemActivityStat</span><span class="sxs-lookup"><span data-stu-id="f3242-102">itemActivityStat resource type</span></span>

> <span data-ttu-id="f3242-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f3242-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3242-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3242-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3242-105">Ресурс **itemActivityStat** содержит сведения о действиях, выполняемых в течение интервала времени.</span><span class="sxs-lookup"><span data-stu-id="f3242-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3242-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3242-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f3242-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3242-107">Properties</span></span>

| <span data-ttu-id="f3242-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3242-108">Property</span></span>         | <span data-ttu-id="f3242-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3242-109">Type</span></span>                    | <span data-ttu-id="f3242-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f3242-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="f3242-111">incompleteData</span><span class="sxs-lookup"><span data-stu-id="f3242-111">incompleteData</span></span>   | <span data-ttu-id="f3242-112">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="f3242-112">[incompleteData][]</span></span>      | <span data-ttu-id="f3242-113">Указывает, что Статистика ожидания основаны на неполные данные.</span><span class="sxs-lookup"><span data-stu-id="f3242-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="f3242-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3242-114">Read-only.</span></span>
| <span data-ttu-id="f3242-115">isTrending</span><span class="sxs-lookup"><span data-stu-id="f3242-115">isTrending</span></span>       | <span data-ttu-id="f3242-116">Логический</span><span class="sxs-lookup"><span data-stu-id="f3242-116">Boolean</span></span>                 | <span data-ttu-id="f3242-117">Указывает, является ли элемент «прибора.»</span><span class="sxs-lookup"><span data-stu-id="f3242-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="f3242-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3242-118">Read-only.</span></span>
| <span data-ttu-id="f3242-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f3242-119">startDateTime</span></span>    | <span data-ttu-id="f3242-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3242-120">DateTimeOffset</span></span>          | <span data-ttu-id="f3242-121">При запуске интервала.</span><span class="sxs-lookup"><span data-stu-id="f3242-121">When the interval starts.</span></span> <span data-ttu-id="f3242-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3242-122">Read-only.</span></span>
| <span data-ttu-id="f3242-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f3242-123">endDateTime</span></span>      | <span data-ttu-id="f3242-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3242-124">DateTimeOffset</span></span>          | <span data-ttu-id="f3242-125">Окончания интервала.</span><span class="sxs-lookup"><span data-stu-id="f3242-125">When the interval ends.</span></span> <span data-ttu-id="f3242-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3242-126">Read-only.</span></span>
| <span data-ttu-id="f3242-127">create</span><span class="sxs-lookup"><span data-stu-id="f3242-127">create</span></span>           | <span data-ttu-id="f3242-128">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="f3242-128">[itemActionStat][]</span></span>      | <span data-ttu-id="f3242-129">Сведения о действия **Создание** ожидания.</span><span class="sxs-lookup"><span data-stu-id="f3242-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="f3242-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3242-130">Read-only.</span></span>
| <span data-ttu-id="f3242-131">edit</span><span class="sxs-lookup"><span data-stu-id="f3242-131">edit</span></span>             | <span data-ttu-id="f3242-132">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="f3242-132">[itemActionStat][]</span></span>      | <span data-ttu-id="f3242-133">Сведения о действия **редактирования** в этот интервал.</span><span class="sxs-lookup"><span data-stu-id="f3242-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="f3242-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3242-134">Read-only.</span></span>
| <span data-ttu-id="f3242-135">delete</span><span class="sxs-lookup"><span data-stu-id="f3242-135">delete</span></span>           | <span data-ttu-id="f3242-136">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="f3242-136">[itemActionStat][]</span></span>      | <span data-ttu-id="f3242-137">Сведения о действиям **удаления** ожидания.</span><span class="sxs-lookup"><span data-stu-id="f3242-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="f3242-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3242-138">Read-only.</span></span>
| <span data-ttu-id="f3242-139">move</span><span class="sxs-lookup"><span data-stu-id="f3242-139">move</span></span>             | <span data-ttu-id="f3242-140">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="f3242-140">[itemActionStat][]</span></span>      | <span data-ttu-id="f3242-141">Сведения о действия **переместить** в этот интервал.</span><span class="sxs-lookup"><span data-stu-id="f3242-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="f3242-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3242-142">Read-only.</span></span>
| <span data-ttu-id="f3242-143">Access</span><span class="sxs-lookup"><span data-stu-id="f3242-143">access</span></span>           | <span data-ttu-id="f3242-144">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="f3242-144">[itemActionStat][]</span></span>      | <span data-ttu-id="f3242-145">Сведения о действия **клиента** в этот интервал.</span><span class="sxs-lookup"><span data-stu-id="f3242-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="f3242-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3242-146">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="f3242-149">Связи</span><span class="sxs-lookup"><span data-stu-id="f3242-149">Relationships</span></span>

| <span data-ttu-id="f3242-150">Имя связи</span><span class="sxs-lookup"><span data-stu-id="f3242-150">Relationship name</span></span> | <span data-ttu-id="f3242-151">Тип</span><span class="sxs-lookup"><span data-stu-id="f3242-151">Type</span></span>                        | <span data-ttu-id="f3242-152">Описание</span><span class="sxs-lookup"><span data-stu-id="f3242-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="f3242-153">activities</span><span class="sxs-lookup"><span data-stu-id="f3242-153">activities</span></span>        | <span data-ttu-id="f3242-154">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="f3242-154">[itemActivity][] collection</span></span> | <span data-ttu-id="f3242-155">Предоставляет **itemActivities** , представленного в этом **itemActivityStat** ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f3242-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="f3242-157">Примечания</span><span class="sxs-lookup"><span data-stu-id="f3242-157">Remarks</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->
