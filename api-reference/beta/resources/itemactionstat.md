---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: Итемактионстат
localization_priority: Normal
ms.openlocfilehash: 39209671b63b991a8fb3ccf1c830c8557fce27c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569986"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="d26f2-102">Тип ресурса Итемактионстат</span><span class="sxs-lookup"><span data-stu-id="d26f2-102">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d26f2-103">Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="d26f2-103">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d26f2-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d26f2-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d26f2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d26f2-105">Properties</span></span>

| <span data-ttu-id="d26f2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d26f2-106">Property</span></span>    | <span data-ttu-id="d26f2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d26f2-107">Type</span></span>  | <span data-ttu-id="d26f2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d26f2-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="d26f2-109">Актионкаунт</span><span class="sxs-lookup"><span data-stu-id="d26f2-109">actionCount</span></span> | <span data-ttu-id="d26f2-110">Int32</span><span class="sxs-lookup"><span data-stu-id="d26f2-110">Int32</span></span> | <span data-ttu-id="d26f2-111">Количество попыток выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="d26f2-111">The number of times the action took place.</span></span> <span data-ttu-id="d26f2-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d26f2-112">Read-only.</span></span>
| <span data-ttu-id="d26f2-113">Акторкаунт</span><span class="sxs-lookup"><span data-stu-id="d26f2-113">actorCount</span></span>  | <span data-ttu-id="d26f2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="d26f2-114">Int32</span></span> | <span data-ttu-id="d26f2-115">Количество уникальных субъектов, которые выполнили действие.</span><span class="sxs-lookup"><span data-stu-id="d26f2-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="d26f2-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d26f2-116">Read-only.</span></span>

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
