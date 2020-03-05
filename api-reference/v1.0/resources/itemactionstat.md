---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактионстат
description: Объект Итемактионстат предоставляет статистические сведения о действии в течение определенного периода времени.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4207c85185281ec9944aa08dfce088739116bb8e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447684"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="fe48a-103">Тип ресурса Итемактионстат</span><span class="sxs-lookup"><span data-stu-id="fe48a-103">itemActionStat resource type</span></span>

<span data-ttu-id="fe48a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fe48a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe48a-105">Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="fe48a-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="fe48a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe48a-106">Properties</span></span>

| <span data-ttu-id="fe48a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe48a-107">Property</span></span>    | <span data-ttu-id="fe48a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fe48a-108">Type</span></span>  | <span data-ttu-id="fe48a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fe48a-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="fe48a-110">актионкаунт</span><span class="sxs-lookup"><span data-stu-id="fe48a-110">actionCount</span></span> | <span data-ttu-id="fe48a-111">Int32</span><span class="sxs-lookup"><span data-stu-id="fe48a-111">Int32</span></span> | <span data-ttu-id="fe48a-112">Количество попыток выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="fe48a-112">The number of times the action took place.</span></span> <span data-ttu-id="fe48a-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe48a-113">Read-only.</span></span>
| <span data-ttu-id="fe48a-114">акторкаунт</span><span class="sxs-lookup"><span data-stu-id="fe48a-114">actorCount</span></span>  | <span data-ttu-id="fe48a-115">Int32</span><span class="sxs-lookup"><span data-stu-id="fe48a-115">Int32</span></span> | <span data-ttu-id="fe48a-116">Количество уникальных субъектов, которые выполнили действие.</span><span class="sxs-lookup"><span data-stu-id="fe48a-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="fe48a-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe48a-117">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe48a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe48a-118">JSON representation</span></span>

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
