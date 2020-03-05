---
title: Тип ресурса Филтерграуп
description: Определяет набор предложений, которым должен удовлетворять объект, чтобы рассматриваться в области. Объект рассматривается в области для группы (Группа оценивается как `true`) только в `true`том случае, если все предложения группы оцениваются.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 433528d9d663a3dc19cecaa5c2dad68e362dc882
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520186"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="7fecd-104">Тип ресурса Филтерграуп</span><span class="sxs-lookup"><span data-stu-id="7fecd-104">filterGroup resource type</span></span>

<span data-ttu-id="7fecd-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7fecd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fecd-106">Определяет набор предложений, которым должен удовлетворять объект, чтобы рассматриваться в области.</span><span class="sxs-lookup"><span data-stu-id="7fecd-106">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="7fecd-107">Объект рассматривается в области для группы (Группа оценивается как `true`) только в `true`том случае, если все предложения группы оцениваются.</span><span class="sxs-lookup"><span data-stu-id="7fecd-107">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="7fecd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7fecd-108">Properties</span></span>
| <span data-ttu-id="7fecd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fecd-109">Property</span></span>     | <span data-ttu-id="7fecd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7fecd-110">Type</span></span>   |<span data-ttu-id="7fecd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7fecd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fecd-112">предложения</span><span class="sxs-lookup"><span data-stu-id="7fecd-112">clauses</span></span>|<span data-ttu-id="7fecd-113">Коллекция [филтерклаусе](synchronization-filterclause.md)</span><span class="sxs-lookup"><span data-stu-id="7fecd-113">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="7fecd-114">Предложения фильтра (условия) этой группы.</span><span class="sxs-lookup"><span data-stu-id="7fecd-114">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="7fecd-115">Все предложения в группе должны быть удовлетворены для того, чтобы `true`Группа фильтров вычислить значение.</span><span class="sxs-lookup"><span data-stu-id="7fecd-115">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="7fecd-116">name</span><span class="sxs-lookup"><span data-stu-id="7fecd-116">name</span></span>|<span data-ttu-id="7fecd-117">String</span><span class="sxs-lookup"><span data-stu-id="7fecd-117">String</span></span>|<span data-ttu-id="7fecd-118">Понятное имя группы фильтров.</span><span class="sxs-lookup"><span data-stu-id="7fecd-118">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7fecd-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7fecd-119">JSON representation</span></span>

<span data-ttu-id="7fecd-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fecd-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterGroup"
}-->

```json
{
  "clauses": [{"@odata.type": "microsoft.graph.filterClause"}],
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
