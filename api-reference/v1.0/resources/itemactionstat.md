---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактионстат
description: Объект Итемактионстат предоставляет статистические сведения о действии в течение определенного периода времени.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1d5531fc969762219f4e2404787190649ecdaf11
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970796"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="1cb3b-103">Тип ресурса Итемактионстат</span><span class="sxs-lookup"><span data-stu-id="1cb3b-103">itemActionStat resource type</span></span>

<span data-ttu-id="1cb3b-104">Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="1cb3b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1cb3b-105">Properties</span></span>

| <span data-ttu-id="1cb3b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cb3b-106">Property</span></span>    | <span data-ttu-id="1cb3b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1cb3b-107">Type</span></span>  | <span data-ttu-id="1cb3b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1cb3b-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="1cb3b-109">Актионкаунт</span><span class="sxs-lookup"><span data-stu-id="1cb3b-109">actionCount</span></span> | <span data-ttu-id="1cb3b-110">Int32</span><span class="sxs-lookup"><span data-stu-id="1cb3b-110">Int32</span></span> | <span data-ttu-id="1cb3b-111">Количество попыток выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-111">The number of times the action took place.</span></span> <span data-ttu-id="1cb3b-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-112">Read-only.</span></span>
| <span data-ttu-id="1cb3b-113">Акторкаунт</span><span class="sxs-lookup"><span data-stu-id="1cb3b-113">actorCount</span></span>  | <span data-ttu-id="1cb3b-114">Int32</span><span class="sxs-lookup"><span data-stu-id="1cb3b-114">Int32</span></span> | <span data-ttu-id="1cb3b-115">Количество уникальных субъектов, которые выполнили действие.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="1cb3b-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cb3b-116">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cb3b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1cb3b-117">JSON representation</span></span>

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
