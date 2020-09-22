---
author: daspek
description: Ресурс Итемактионстат предоставляет статистические сведения о действии в течение определенного периода времени.
ms.date: 09/14/2017
title: итемактионстат
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8316239a7e00cdc74921c42b70431eba60cdc2d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075680"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="bb8c6-103">Тип ресурса Итемактионстат</span><span class="sxs-lookup"><span data-stu-id="bb8c6-103">itemActionStat resource type</span></span>

<span data-ttu-id="bb8c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb8c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb8c6-105">Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="bb8c6-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb8c6-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb8c6-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bb8c6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb8c6-107">Properties</span></span>

| <span data-ttu-id="bb8c6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb8c6-108">Property</span></span>    | <span data-ttu-id="bb8c6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bb8c6-109">Type</span></span>  | <span data-ttu-id="bb8c6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb8c6-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="bb8c6-111">актионкаунт</span><span class="sxs-lookup"><span data-stu-id="bb8c6-111">actionCount</span></span> | <span data-ttu-id="bb8c6-112">Int32</span><span class="sxs-lookup"><span data-stu-id="bb8c6-112">Int32</span></span> | <span data-ttu-id="bb8c6-113">Количество попыток выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="bb8c6-113">The number of times the action took place.</span></span> <span data-ttu-id="bb8c6-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb8c6-114">Read-only.</span></span>
| <span data-ttu-id="bb8c6-115">акторкаунт</span><span class="sxs-lookup"><span data-stu-id="bb8c6-115">actorCount</span></span>  | <span data-ttu-id="bb8c6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="bb8c6-116">Int32</span></span> | <span data-ttu-id="bb8c6-117">Количество уникальных субъектов, которые выполнили действие.</span><span class="sxs-lookup"><span data-stu-id="bb8c6-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="bb8c6-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb8c6-118">Read-only.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": []
}
-->


