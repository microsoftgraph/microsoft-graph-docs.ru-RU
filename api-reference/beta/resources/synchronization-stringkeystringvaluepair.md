---
title: Тип ресурса stringKeyStringValuePair
description: Представляет пару ключ значение, где ключ — это строка, а значение — это строка.
localization_priority: Normal
ms.openlocfilehash: f91d63ee4b4d3b0328bbb6fbe58c74ec8f78c5b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520223"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="ecb30-103">Тип ресурса stringKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="ecb30-103">stringKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecb30-104">Представляет пару ключ значение, где ключ — это строка, а значение — это строка.</span><span class="sxs-lookup"><span data-stu-id="ecb30-104">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="ecb30-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ecb30-105">Properties</span></span>
| <span data-ttu-id="ecb30-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecb30-106">Property</span></span>     | <span data-ttu-id="ecb30-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ecb30-107">Type</span></span>   |<span data-ttu-id="ecb30-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ecb30-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecb30-109">key</span><span class="sxs-lookup"><span data-stu-id="ecb30-109">key</span></span>|<span data-ttu-id="ecb30-110">String</span><span class="sxs-lookup"><span data-stu-id="ecb30-110">String</span></span>|<span data-ttu-id="ecb30-111">Ключ.</span><span class="sxs-lookup"><span data-stu-id="ecb30-111">Key.</span></span>|
|<span data-ttu-id="ecb30-112">value</span><span class="sxs-lookup"><span data-stu-id="ecb30-112">value</span></span>|<span data-ttu-id="ecb30-113">String</span><span class="sxs-lookup"><span data-stu-id="ecb30-113">String</span></span>|<span data-ttu-id="ecb30-114">Значение</span><span class="sxs-lookup"><span data-stu-id="ecb30-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ecb30-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ecb30-115">JSON representation</span></span>

<span data-ttu-id="ecb30-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecb30-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeystringvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
