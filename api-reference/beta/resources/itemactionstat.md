---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
ms.openlocfilehash: f7e9351bc4a394005cffc712aa444c999a51b363
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081602"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="c2b82-102">Тип ресурса itemActionStat</span><span class="sxs-lookup"><span data-stu-id="c2b82-102">itemActionStat resource type</span></span>

> <span data-ttu-id="c2b82-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2b82-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2b82-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b82-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2b82-105">Ресурс **itemActionStat** статистические сведения о действия за период времени.</span><span class="sxs-lookup"><span data-stu-id="c2b82-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2b82-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2b82-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c2b82-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2b82-107">Properties</span></span>

| <span data-ttu-id="c2b82-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2b82-108">Property</span></span>    | <span data-ttu-id="c2b82-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c2b82-109">Type</span></span>  | <span data-ttu-id="c2b82-110">Description</span><span class="sxs-lookup"><span data-stu-id="c2b82-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="c2b82-111">actionCount</span><span class="sxs-lookup"><span data-stu-id="c2b82-111">actionCount</span></span> | <span data-ttu-id="c2b82-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c2b82-112">Int32</span></span> | <span data-ttu-id="c2b82-113">Количество раз, когда действие, когда был выполнен.</span><span class="sxs-lookup"><span data-stu-id="c2b82-113">The number of times the action took place.</span></span> <span data-ttu-id="c2b82-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2b82-114">Read-only.</span></span>
| <span data-ttu-id="c2b82-115">actorCount</span><span class="sxs-lookup"><span data-stu-id="c2b82-115">actorCount</span></span>  | <span data-ttu-id="c2b82-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c2b82-116">Int32</span></span> | <span data-ttu-id="c2b82-117">Количество уникальных субъекты, выполнившего действия.</span><span class="sxs-lookup"><span data-stu-id="c2b82-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="c2b82-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2b82-118">Read-only.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat"
} -->
