---
author: daspek
title: Тип ресурса itemActionStat
description: Объект itemActionStat предоставляет сводные сведения о действии за период времени.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 13bc306a1b14d7d59ec8eddda5b02a5cba84e649
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238528"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="df833-103">Тип ресурса itemActionStat</span><span class="sxs-lookup"><span data-stu-id="df833-103">itemActionStat resource type</span></span>

<span data-ttu-id="df833-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df833-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df833-105">Ресурс **itemActionStat** предоставляет сводную информацию о действии за период времени.</span><span class="sxs-lookup"><span data-stu-id="df833-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="df833-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="df833-106">Properties</span></span>

| <span data-ttu-id="df833-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="df833-107">Property</span></span>    | <span data-ttu-id="df833-108">Тип</span><span class="sxs-lookup"><span data-stu-id="df833-108">Type</span></span>  | <span data-ttu-id="df833-109">Описание</span><span class="sxs-lookup"><span data-stu-id="df833-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="df833-110">actionCount</span><span class="sxs-lookup"><span data-stu-id="df833-110">actionCount</span></span> | <span data-ttu-id="df833-111">Int32</span><span class="sxs-lookup"><span data-stu-id="df833-111">Int32</span></span> | <span data-ttu-id="df833-112">Количество действий.</span><span class="sxs-lookup"><span data-stu-id="df833-112">The number of times the action took place.</span></span> <span data-ttu-id="df833-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="df833-113">Read-only.</span></span>
| <span data-ttu-id="df833-114">actorCount</span><span class="sxs-lookup"><span data-stu-id="df833-114">actorCount</span></span>  | <span data-ttu-id="df833-115">Int32</span><span class="sxs-lookup"><span data-stu-id="df833-115">Int32</span></span> | <span data-ttu-id="df833-116">Количество отдельных субъектов, которые выполнили действие.</span><span class="sxs-lookup"><span data-stu-id="df833-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="df833-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="df833-117">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df833-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df833-118">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/itemActionStat",
  "suppressions": []
}
-->

