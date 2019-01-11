---
title: Тип ресурса alertTrigger
description: Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).
author: Preetikr
localization_priority: Normal
ms.openlocfilehash: 1dc8bb2b18380da50134aa67e742da89dea3c057
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894343"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="06c9d-103">Тип ресурса alertTrigger</span><span class="sxs-lookup"><span data-stu-id="06c9d-103">alertTrigger resource type</span></span>

<span data-ttu-id="06c9d-104">Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).</span><span class="sxs-lookup"><span data-stu-id="06c9d-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="06c9d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="06c9d-105">Properties</span></span>

| <span data-ttu-id="06c9d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="06c9d-106">Property</span></span>   | <span data-ttu-id="06c9d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="06c9d-107">Type</span></span>|<span data-ttu-id="06c9d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="06c9d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06c9d-109">name</span><span class="sxs-lookup"><span data-stu-id="06c9d-109">name</span></span>|<span data-ttu-id="06c9d-110">Строка</span><span class="sxs-lookup"><span data-stu-id="06c9d-110">String</span></span>|<span data-ttu-id="06c9d-111">Имя свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="06c9d-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="06c9d-112">type</span><span class="sxs-lookup"><span data-stu-id="06c9d-112">type</span></span>|<span data-ttu-id="06c9d-113">Строка</span><span class="sxs-lookup"><span data-stu-id="06c9d-113">String</span></span>|<span data-ttu-id="06c9d-114">Тип свойства в пары "ключ: значение" для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="06c9d-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="06c9d-115">Например String, Boolean, и т.д.</span><span class="sxs-lookup"><span data-stu-id="06c9d-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="06c9d-116">value</span><span class="sxs-lookup"><span data-stu-id="06c9d-116">value</span></span>|<span data-ttu-id="06c9d-117">Строка</span><span class="sxs-lookup"><span data-stu-id="06c9d-117">String</span></span>|<span data-ttu-id="06c9d-118">Значение свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="06c9d-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06c9d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06c9d-119">JSON representation</span></span>

<span data-ttu-id="06c9d-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06c9d-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="06c9d-121">Пример</span><span class="sxs-lookup"><span data-stu-id="06c9d-121">Example</span></span>

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
