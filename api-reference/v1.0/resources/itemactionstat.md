---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактионстат
description: Объект Итемактионстат предоставляет статистические сведения о действии в течение определенного периода времени.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f1be83bef880b967758a803e694b068df9bfaebf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041269"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="a4c37-103">Тип ресурса Итемактионстат</span><span class="sxs-lookup"><span data-stu-id="a4c37-103">itemActionStat resource type</span></span>

<span data-ttu-id="a4c37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4c37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4c37-105">Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="a4c37-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="a4c37-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4c37-106">Properties</span></span>

| <span data-ttu-id="a4c37-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4c37-107">Property</span></span>    | <span data-ttu-id="a4c37-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a4c37-108">Type</span></span>  | <span data-ttu-id="a4c37-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a4c37-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="a4c37-110">актионкаунт</span><span class="sxs-lookup"><span data-stu-id="a4c37-110">actionCount</span></span> | <span data-ttu-id="a4c37-111">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c37-111">Int32</span></span> | <span data-ttu-id="a4c37-112">Количество попыток выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="a4c37-112">The number of times the action took place.</span></span> <span data-ttu-id="a4c37-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4c37-113">Read-only.</span></span>
| <span data-ttu-id="a4c37-114">акторкаунт</span><span class="sxs-lookup"><span data-stu-id="a4c37-114">actorCount</span></span>  | <span data-ttu-id="a4c37-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c37-115">Int32</span></span> | <span data-ttu-id="a4c37-116">Количество уникальных субъектов, которые выполнили действие.</span><span class="sxs-lookup"><span data-stu-id="a4c37-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="a4c37-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4c37-117">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4c37-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4c37-118">JSON representation</span></span>

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

