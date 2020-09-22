---
title: Тип ресурса Филтерграуп
description: Определяет набор предложений, которым должен удовлетворять объект, чтобы рассматриваться в области.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4dd174442cedf8f194bb9faf87d8e844b8c73163
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079767"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="41384-103">Тип ресурса Филтерграуп</span><span class="sxs-lookup"><span data-stu-id="41384-103">filterGroup resource type</span></span>

<span data-ttu-id="41384-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41384-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41384-105">Определяет набор предложений, которым должен удовлетворять объект, чтобы рассматриваться в области.</span><span class="sxs-lookup"><span data-stu-id="41384-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="41384-106">Объект рассматривается в области для группы (Группа оценивается как `true` ) только в том случае, если все предложения группы оцениваются `true` .</span><span class="sxs-lookup"><span data-stu-id="41384-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="41384-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="41384-107">Properties</span></span>
| <span data-ttu-id="41384-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="41384-108">Property</span></span>     | <span data-ttu-id="41384-109">Тип</span><span class="sxs-lookup"><span data-stu-id="41384-109">Type</span></span>   |<span data-ttu-id="41384-110">Описание</span><span class="sxs-lookup"><span data-stu-id="41384-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41384-111">предложения</span><span class="sxs-lookup"><span data-stu-id="41384-111">clauses</span></span>|<span data-ttu-id="41384-112">Коллекция [филтерклаусе](synchronization-filterclause.md)</span><span class="sxs-lookup"><span data-stu-id="41384-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="41384-113">Предложения фильтра (условия) этой группы.</span><span class="sxs-lookup"><span data-stu-id="41384-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="41384-114">Все предложения в группе должны быть удовлетворены для того, чтобы Группа фильтров вычислить значение `true` .</span><span class="sxs-lookup"><span data-stu-id="41384-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="41384-115">name</span><span class="sxs-lookup"><span data-stu-id="41384-115">name</span></span>|<span data-ttu-id="41384-116">String</span><span class="sxs-lookup"><span data-stu-id="41384-116">String</span></span>|<span data-ttu-id="41384-117">Понятное имя группы фильтров.</span><span class="sxs-lookup"><span data-stu-id="41384-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41384-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41384-118">JSON representation</span></span>

<span data-ttu-id="41384-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41384-119">The following is a JSON representation of the resource.</span></span>

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


