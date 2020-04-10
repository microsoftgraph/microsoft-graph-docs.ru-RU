---
title: Тип ресурса Филтерграуп
description: Определяет набор предложений, которым должен удовлетворять объект, чтобы рассматриваться в области.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6e7933bf2fef6240dd0dc53d7da975074225aa30
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217892"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="b2ddb-103">Тип ресурса Филтерграуп</span><span class="sxs-lookup"><span data-stu-id="b2ddb-103">filterGroup resource type</span></span>

<span data-ttu-id="b2ddb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2ddb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2ddb-105">Определяет набор предложений, которым должен удовлетворять объект, чтобы рассматриваться в области.</span><span class="sxs-lookup"><span data-stu-id="b2ddb-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="b2ddb-106">Объект рассматривается в области для группы (Группа оценивается как `true`) только в `true`том случае, если все предложения группы оцениваются.</span><span class="sxs-lookup"><span data-stu-id="b2ddb-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="b2ddb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2ddb-107">Properties</span></span>
| <span data-ttu-id="b2ddb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2ddb-108">Property</span></span>     | <span data-ttu-id="b2ddb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b2ddb-109">Type</span></span>   |<span data-ttu-id="b2ddb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b2ddb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2ddb-111">предложения</span><span class="sxs-lookup"><span data-stu-id="b2ddb-111">clauses</span></span>|<span data-ttu-id="b2ddb-112">Коллекция [филтерклаусе](synchronization-filterclause.md)</span><span class="sxs-lookup"><span data-stu-id="b2ddb-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="b2ddb-113">Предложения фильтра (условия) этой группы.</span><span class="sxs-lookup"><span data-stu-id="b2ddb-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="b2ddb-114">Все предложения в группе должны быть удовлетворены для того, чтобы `true`Группа фильтров вычислить значение.</span><span class="sxs-lookup"><span data-stu-id="b2ddb-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="b2ddb-115">name</span><span class="sxs-lookup"><span data-stu-id="b2ddb-115">name</span></span>|<span data-ttu-id="b2ddb-116">String</span><span class="sxs-lookup"><span data-stu-id="b2ddb-116">String</span></span>|<span data-ttu-id="b2ddb-117">Понятное имя группы фильтров.</span><span class="sxs-lookup"><span data-stu-id="b2ddb-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2ddb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2ddb-118">JSON representation</span></span>

<span data-ttu-id="b2ddb-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2ddb-119">The following is a JSON representation of the resource.</span></span>

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
