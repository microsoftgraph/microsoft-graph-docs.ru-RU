---
title: Тип ресурса Ключзначение
description: Стандартный тип ресурса "ключ — значение".
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: adac348de690b3796399a4276ede4280f35713b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447607"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="2c797-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="2c797-103">keyValue resource type</span></span>

<span data-ttu-id="2c797-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2c797-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c797-105">Представляет собой ключевую строку "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="2c797-105">Represents a key-value pair.</span></span>

## <a name="properties"></a><span data-ttu-id="2c797-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c797-106">Properties</span></span>

| <span data-ttu-id="2c797-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c797-107">Property</span></span>     | <span data-ttu-id="2c797-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2c797-108">Type</span></span>   |<span data-ttu-id="2c797-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2c797-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c797-110">key</span><span class="sxs-lookup"><span data-stu-id="2c797-110">key</span></span>|<span data-ttu-id="2c797-111">string</span><span class="sxs-lookup"><span data-stu-id="2c797-111">string</span></span>| <span data-ttu-id="2c797-112">Ключ для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="2c797-112">Key for the key-value pair.</span></span> |
|<span data-ttu-id="2c797-113">value</span><span class="sxs-lookup"><span data-stu-id="2c797-113">value</span></span>|<span data-ttu-id="2c797-114">строка</span><span class="sxs-lookup"><span data-stu-id="2c797-114">string</span></span>| <span data-ttu-id="2c797-115">Значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="2c797-115">Value for the key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c797-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c797-116">JSON representation</span></span>

<span data-ttu-id="2c797-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c797-117">Here is a JSON representation of the resource.</span></span>

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
