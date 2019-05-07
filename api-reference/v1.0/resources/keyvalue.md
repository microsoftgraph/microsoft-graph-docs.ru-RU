---
title: Тип ресурса Ключзначение
description: Стандартный тип ресурса "ключ — значение".
localization_priority: Normal
ms.openlocfilehash: aa026f36d69e894e056f21ba19865c730ec5b643
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629273"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="b689a-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="b689a-103">keyValue resource type</span></span>

<span data-ttu-id="b689a-104">Представляет собой ключевую строку "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="b689a-104">Represents a key-value pair.</span></span>

## <a name="properties"></a><span data-ttu-id="b689a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b689a-105">Properties</span></span>

| <span data-ttu-id="b689a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b689a-106">Property</span></span>     | <span data-ttu-id="b689a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b689a-107">Type</span></span>   |<span data-ttu-id="b689a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b689a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b689a-109">key</span><span class="sxs-lookup"><span data-stu-id="b689a-109">key</span></span>|<span data-ttu-id="b689a-110">string</span><span class="sxs-lookup"><span data-stu-id="b689a-110">string</span></span>| <span data-ttu-id="b689a-111">Ключ для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="b689a-111">Key for the key-value pair.</span></span> |
|<span data-ttu-id="b689a-112">value</span><span class="sxs-lookup"><span data-stu-id="b689a-112">value</span></span>|<span data-ttu-id="b689a-113">string</span><span class="sxs-lookup"><span data-stu-id="b689a-113">string</span></span>| <span data-ttu-id="b689a-114">Значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="b689a-114">Value for the key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b689a-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b689a-115">JSON representation</span></span>

<span data-ttu-id="b689a-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b689a-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue"
}-->

```json
{
  "key": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
