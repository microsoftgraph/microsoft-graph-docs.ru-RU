---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактионстат
description: Объект Итемактионстат предоставляет статистические сведения о действии в течение определенного периода времени.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 7eda0f6ddbed16dadf1eac4a3ea737cdd7fd2c89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036759"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="89f30-103">Тип ресурса Итемактионстат</span><span class="sxs-lookup"><span data-stu-id="89f30-103">itemActionStat resource type</span></span>

<span data-ttu-id="89f30-104">Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="89f30-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="89f30-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="89f30-105">Properties</span></span>

| <span data-ttu-id="89f30-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="89f30-106">Property</span></span>    | <span data-ttu-id="89f30-107">Тип</span><span class="sxs-lookup"><span data-stu-id="89f30-107">Type</span></span>  | <span data-ttu-id="89f30-108">Описание</span><span class="sxs-lookup"><span data-stu-id="89f30-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="89f30-109">Актионкаунт</span><span class="sxs-lookup"><span data-stu-id="89f30-109">actionCount</span></span> | <span data-ttu-id="89f30-110">Int32</span><span class="sxs-lookup"><span data-stu-id="89f30-110">Int32</span></span> | <span data-ttu-id="89f30-111">Количество попыток выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="89f30-111">The number of times the action took place.</span></span> <span data-ttu-id="89f30-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89f30-112">Read-only.</span></span>
| <span data-ttu-id="89f30-113">Акторкаунт</span><span class="sxs-lookup"><span data-stu-id="89f30-113">actorCount</span></span>  | <span data-ttu-id="89f30-114">Int32</span><span class="sxs-lookup"><span data-stu-id="89f30-114">Int32</span></span> | <span data-ttu-id="89f30-115">Количество уникальных субъектов, которые выполнили действие.</span><span class="sxs-lookup"><span data-stu-id="89f30-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="89f30-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89f30-116">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89f30-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89f30-117">JSON representation</span></span>

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
