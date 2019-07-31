---
title: Тип ресурса keyValuePair
description: Ключевое значение для параметров Action.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: db8d3b14ceaa0ff05181894af803b8b6feea77c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967037"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="67ffe-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="67ffe-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67ffe-104">Ключевое значение для параметров Action.</span><span class="sxs-lookup"><span data-stu-id="67ffe-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="67ffe-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="67ffe-105">Properties</span></span>

| <span data-ttu-id="67ffe-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="67ffe-106">Property</span></span>     | <span data-ttu-id="67ffe-107">Тип</span><span class="sxs-lookup"><span data-stu-id="67ffe-107">Type</span></span>        | <span data-ttu-id="67ffe-108">Описание</span><span class="sxs-lookup"><span data-stu-id="67ffe-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="67ffe-109">name</span><span class="sxs-lookup"><span data-stu-id="67ffe-109">name</span></span>|<span data-ttu-id="67ffe-110">String</span><span class="sxs-lookup"><span data-stu-id="67ffe-110">String</span></span>|<span data-ttu-id="67ffe-111">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="67ffe-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="67ffe-112">value</span><span class="sxs-lookup"><span data-stu-id="67ffe-112">value</span></span>|<span data-ttu-id="67ffe-113">String</span><span class="sxs-lookup"><span data-stu-id="67ffe-113">String</span></span>|<span data-ttu-id="67ffe-114">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="67ffe-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67ffe-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67ffe-115">JSON representation</span></span>

<span data-ttu-id="67ffe-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67ffe-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->