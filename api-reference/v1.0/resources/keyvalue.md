---
title: Тип ресурса Ключзначение
description: Стандартный тип ресурса "ключ — значение".
localization_priority: Normal
author: dougeby
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 94de9529f53fc018633c9fb5a361b45ad0067e73
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811310"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="883d1-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="883d1-103">keyValue resource type</span></span>

<span data-ttu-id="883d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="883d1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="883d1-105">Представляет собой ключевую строку "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="883d1-105">Represents a key-value pair.</span></span>

## <a name="properties"></a><span data-ttu-id="883d1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="883d1-106">Properties</span></span>

| <span data-ttu-id="883d1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="883d1-107">Property</span></span>     | <span data-ttu-id="883d1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="883d1-108">Type</span></span>   |<span data-ttu-id="883d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="883d1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="883d1-110">key</span><span class="sxs-lookup"><span data-stu-id="883d1-110">key</span></span>|<span data-ttu-id="883d1-111">string</span><span class="sxs-lookup"><span data-stu-id="883d1-111">string</span></span>| <span data-ttu-id="883d1-112">Ключ для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="883d1-112">Key for the key-value pair.</span></span> |
|<span data-ttu-id="883d1-113">value</span><span class="sxs-lookup"><span data-stu-id="883d1-113">value</span></span>|<span data-ttu-id="883d1-114">string</span><span class="sxs-lookup"><span data-stu-id="883d1-114">string</span></span>| <span data-ttu-id="883d1-115">Значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="883d1-115">Value for the key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="883d1-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="883d1-116">JSON representation</span></span>

<span data-ttu-id="883d1-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="883d1-117">Here is a JSON representation of the resource.</span></span>

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
