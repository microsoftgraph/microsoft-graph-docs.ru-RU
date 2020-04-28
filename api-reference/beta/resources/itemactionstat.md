---
author: daspek
description: Ресурс Итемактионстат предоставляет статистические сведения о действии в течение определенного периода времени.
ms.date: 09/14/2017
title: итемактионстат
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6ab31d8a155e0b9fd54b3f2185e7d05969291ec1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523130"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="68b96-103">Тип ресурса Итемактионстат</span><span class="sxs-lookup"><span data-stu-id="68b96-103">itemActionStat resource type</span></span>

<span data-ttu-id="68b96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68b96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68b96-105">Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="68b96-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68b96-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68b96-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="68b96-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="68b96-107">Properties</span></span>

| <span data-ttu-id="68b96-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="68b96-108">Property</span></span>    | <span data-ttu-id="68b96-109">Тип</span><span class="sxs-lookup"><span data-stu-id="68b96-109">Type</span></span>  | <span data-ttu-id="68b96-110">Описание</span><span class="sxs-lookup"><span data-stu-id="68b96-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="68b96-111">актионкаунт</span><span class="sxs-lookup"><span data-stu-id="68b96-111">actionCount</span></span> | <span data-ttu-id="68b96-112">Int32</span><span class="sxs-lookup"><span data-stu-id="68b96-112">Int32</span></span> | <span data-ttu-id="68b96-113">Количество попыток выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="68b96-113">The number of times the action took place.</span></span> <span data-ttu-id="68b96-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68b96-114">Read-only.</span></span>
| <span data-ttu-id="68b96-115">акторкаунт</span><span class="sxs-lookup"><span data-stu-id="68b96-115">actorCount</span></span>  | <span data-ttu-id="68b96-116">Int32</span><span class="sxs-lookup"><span data-stu-id="68b96-116">Int32</span></span> | <span data-ttu-id="68b96-117">Количество уникальных субъектов, которые выполнили действие.</span><span class="sxs-lookup"><span data-stu-id="68b96-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="68b96-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68b96-118">Read-only.</span></span>

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
