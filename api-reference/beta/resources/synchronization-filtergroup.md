---
title: Тип ресурса filterGroup
description: Определяет набор предложений, которые должны удовлетворяться объектом, чтобы считаться в области.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 6338ae4b02b79d1512d5e9f695a69155197e2f4a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131917"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="89c4a-103">Тип ресурса filterGroup</span><span class="sxs-lookup"><span data-stu-id="89c4a-103">filterGroup resource type</span></span>

<span data-ttu-id="89c4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89c4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89c4a-105">Определяет набор предложений, которые должны удовлетворяться объектом, чтобы считаться в области.</span><span class="sxs-lookup"><span data-stu-id="89c4a-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="89c4a-106">Объект рассматривается в области для группы (группа оценивается как ) только в том случае, если все предложения группы `true` оцениваются как `true` .</span><span class="sxs-lookup"><span data-stu-id="89c4a-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="89c4a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="89c4a-107">Properties</span></span>
| <span data-ttu-id="89c4a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="89c4a-108">Property</span></span>     | <span data-ttu-id="89c4a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="89c4a-109">Type</span></span>   |<span data-ttu-id="89c4a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="89c4a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89c4a-111">clauses</span><span class="sxs-lookup"><span data-stu-id="89c4a-111">clauses</span></span>|<span data-ttu-id="89c4a-112">[Коллекция filterClause](synchronization-filterclause.md)</span><span class="sxs-lookup"><span data-stu-id="89c4a-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="89c4a-113">Условия фильтра для этой группы.</span><span class="sxs-lookup"><span data-stu-id="89c4a-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="89c4a-114">Все предложения в группе должны быть выполнены, чтобы группа фильтров оценивалась как `true` .</span><span class="sxs-lookup"><span data-stu-id="89c4a-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="89c4a-115">name</span><span class="sxs-lookup"><span data-stu-id="89c4a-115">name</span></span>|<span data-ttu-id="89c4a-116">String</span><span class="sxs-lookup"><span data-stu-id="89c4a-116">String</span></span>|<span data-ttu-id="89c4a-117">Понятное для человека имя группы фильтров.</span><span class="sxs-lookup"><span data-stu-id="89c4a-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89c4a-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="89c4a-118">JSON representation</span></span>

<span data-ttu-id="89c4a-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89c4a-119">The following is a JSON representation of the resource.</span></span>

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


