---
title: тип ресурса alertTrigger
description: Содержит сведения о свойствах, которые вызвали обнаружение (свойства существуют в объекте оповещений).
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6bdee4ee550b44694a572e3611652b19c7ff574c
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129441"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="a2e35-103">тип ресурса alertTrigger</span><span class="sxs-lookup"><span data-stu-id="a2e35-103">alertTrigger resource type</span></span>

<span data-ttu-id="a2e35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2e35-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2e35-105">Содержит сведения о свойствах, которые вызвали обнаружение (свойства существуют в объекте оповещений).</span><span class="sxs-lookup"><span data-stu-id="a2e35-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="a2e35-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2e35-106">Properties</span></span>

| <span data-ttu-id="a2e35-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2e35-107">Property</span></span>   | <span data-ttu-id="a2e35-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a2e35-108">Type</span></span>|<span data-ttu-id="a2e35-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a2e35-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2e35-110">name</span><span class="sxs-lookup"><span data-stu-id="a2e35-110">name</span></span>|<span data-ttu-id="a2e35-111">String</span><span class="sxs-lookup"><span data-stu-id="a2e35-111">String</span></span>|<span data-ttu-id="a2e35-112">Имя свойства, которое служит спусковым крючком обнаружения.</span><span class="sxs-lookup"><span data-stu-id="a2e35-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="a2e35-113">type</span><span class="sxs-lookup"><span data-stu-id="a2e35-113">type</span></span>|<span data-ttu-id="a2e35-114">String</span><span class="sxs-lookup"><span data-stu-id="a2e35-114">String</span></span>|<span data-ttu-id="a2e35-115">Тип свойства в паре key:value для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="a2e35-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="a2e35-116">Например, String, Boolean и т.д.</span><span class="sxs-lookup"><span data-stu-id="a2e35-116">For example, String, Boolean etc.</span></span>|
|<span data-ttu-id="a2e35-117">value</span><span class="sxs-lookup"><span data-stu-id="a2e35-117">value</span></span>|<span data-ttu-id="a2e35-118">String</span><span class="sxs-lookup"><span data-stu-id="a2e35-118">String</span></span>|<span data-ttu-id="a2e35-119">Значение свойства, служащая в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="a2e35-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2e35-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2e35-120">JSON representation</span></span>

<span data-ttu-id="a2e35-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2e35-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}
```

## <a name="example"></a><span data-ttu-id="a2e35-122">Пример</span><span class="sxs-lookup"><span data-stu-id="a2e35-122">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

