---
title: Тип ресурса Ключзначение
description: Стандартный тип ресурса "ключ — значение".
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a3008b328337e4dd4d816f4b0d7432b7e24c08d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036493"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="50287-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="50287-103">keyValue resource type</span></span>

<span data-ttu-id="50287-104">Представляет собой ключевую строку "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="50287-104">Represents a key-value pair.</span></span>

## <a name="properties"></a><span data-ttu-id="50287-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="50287-105">Properties</span></span>

| <span data-ttu-id="50287-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="50287-106">Property</span></span>     | <span data-ttu-id="50287-107">Тип</span><span class="sxs-lookup"><span data-stu-id="50287-107">Type</span></span>   |<span data-ttu-id="50287-108">Описание</span><span class="sxs-lookup"><span data-stu-id="50287-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50287-109">key</span><span class="sxs-lookup"><span data-stu-id="50287-109">key</span></span>|<span data-ttu-id="50287-110">string</span><span class="sxs-lookup"><span data-stu-id="50287-110">string</span></span>| <span data-ttu-id="50287-111">Ключ для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="50287-111">Key for the key-value pair.</span></span> |
|<span data-ttu-id="50287-112">value</span><span class="sxs-lookup"><span data-stu-id="50287-112">value</span></span>|<span data-ttu-id="50287-113">string</span><span class="sxs-lookup"><span data-stu-id="50287-113">string</span></span>| <span data-ttu-id="50287-114">Значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="50287-114">Value for the key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50287-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50287-115">JSON representation</span></span>

<span data-ttu-id="50287-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50287-116">Here is a JSON representation of the resource.</span></span>

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
