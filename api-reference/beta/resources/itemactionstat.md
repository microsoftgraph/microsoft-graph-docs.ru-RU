---
author: daspek
description: Ресурс Итемактионстат предоставляет статистические сведения о действии в течение определенного периода времени.
ms.date: 09/14/2017
title: Итемактионстат
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 719a443af65fd9642feee3bc8ddbc832eb3964c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010114"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="6e315-103">Тип ресурса Итемактионстат</span><span class="sxs-lookup"><span data-stu-id="6e315-103">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e315-104">Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="6e315-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e315-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e315-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6e315-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e315-106">Properties</span></span>

| <span data-ttu-id="6e315-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e315-107">Property</span></span>    | <span data-ttu-id="6e315-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6e315-108">Type</span></span>  | <span data-ttu-id="6e315-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6e315-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="6e315-110">Актионкаунт</span><span class="sxs-lookup"><span data-stu-id="6e315-110">actionCount</span></span> | <span data-ttu-id="6e315-111">Int32</span><span class="sxs-lookup"><span data-stu-id="6e315-111">Int32</span></span> | <span data-ttu-id="6e315-112">Количество попыток выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="6e315-112">The number of times the action took place.</span></span> <span data-ttu-id="6e315-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e315-113">Read-only.</span></span>
| <span data-ttu-id="6e315-114">Акторкаунт</span><span class="sxs-lookup"><span data-stu-id="6e315-114">actorCount</span></span>  | <span data-ttu-id="6e315-115">Int32</span><span class="sxs-lookup"><span data-stu-id="6e315-115">Int32</span></span> | <span data-ttu-id="6e315-116">Количество уникальных субъектов, которые выполнили действие.</span><span class="sxs-lookup"><span data-stu-id="6e315-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="6e315-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e315-117">Read-only.</span></span>

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
