---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: Итемактионстат
localization_priority: Normal
ms.openlocfilehash: a0e3bc3f217308d96eaadf6ab367431c7f1b8c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345454"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="b79b6-102">Тип ресурса Итемактионстат</span><span class="sxs-lookup"><span data-stu-id="b79b6-102">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b79b6-103">Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="b79b6-103">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b79b6-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b79b6-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b79b6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b79b6-105">Properties</span></span>

| <span data-ttu-id="b79b6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b79b6-106">Property</span></span>    | <span data-ttu-id="b79b6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b79b6-107">Type</span></span>  | <span data-ttu-id="b79b6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b79b6-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="b79b6-109">Актионкаунт</span><span class="sxs-lookup"><span data-stu-id="b79b6-109">actionCount</span></span> | <span data-ttu-id="b79b6-110">Int32</span><span class="sxs-lookup"><span data-stu-id="b79b6-110">Int32</span></span> | <span data-ttu-id="b79b6-111">Количество попыток выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="b79b6-111">The number of times the action took place.</span></span> <span data-ttu-id="b79b6-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b79b6-112">Read-only.</span></span>
| <span data-ttu-id="b79b6-113">Акторкаунт</span><span class="sxs-lookup"><span data-stu-id="b79b6-113">actorCount</span></span>  | <span data-ttu-id="b79b6-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b79b6-114">Int32</span></span> | <span data-ttu-id="b79b6-115">Количество уникальных субъектов, которые выполнили действие.</span><span class="sxs-lookup"><span data-stu-id="b79b6-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="b79b6-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b79b6-116">Read-only.</span></span>

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
