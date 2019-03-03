---
title: Тип ресурса keyValuePair
description: Ключевое значение для параметров Action.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 86a5415c20721f717947238838341345ec9a4250
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366940"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="8427e-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="8427e-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8427e-104">Ключевое значение для параметров Action.</span><span class="sxs-lookup"><span data-stu-id="8427e-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="8427e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8427e-105">Properties</span></span>

| <span data-ttu-id="8427e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8427e-106">Property</span></span>     | <span data-ttu-id="8427e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8427e-107">Type</span></span>        | <span data-ttu-id="8427e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8427e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8427e-109">name</span><span class="sxs-lookup"><span data-stu-id="8427e-109">name</span></span>|<span data-ttu-id="8427e-110">String</span><span class="sxs-lookup"><span data-stu-id="8427e-110">String</span></span>|<span data-ttu-id="8427e-111">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="8427e-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="8427e-112">value</span><span class="sxs-lookup"><span data-stu-id="8427e-112">value</span></span>|<span data-ttu-id="8427e-113">String</span><span class="sxs-lookup"><span data-stu-id="8427e-113">String</span></span>|<span data-ttu-id="8427e-114">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="8427e-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8427e-115">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8427e-115">JSON representation</span></span>

<span data-ttu-id="8427e-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8427e-116">The following is a JSON representation of the resource.</span></span>

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