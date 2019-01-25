---
title: Тип ресурса stringKeyAttributeMappingSourceValuePair
description: Представляет пару ключ значение, где ключ — это строка, а значение — attributeMappingSource.
localization_priority: Normal
ms.openlocfilehash: ff914c23a238356a821d2902bf18900cf9957548
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516219"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="9c17a-103">Тип ресурса stringKeyAttributeMappingSourceValuePair</span><span class="sxs-lookup"><span data-stu-id="9c17a-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c17a-104">Представляет пару ключ значение, где ключ — это строка, а значение — [attributeMappingSource](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="9c17a-104">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9c17a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c17a-105">Properties</span></span>
| <span data-ttu-id="9c17a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c17a-106">Property</span></span>     | <span data-ttu-id="9c17a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9c17a-107">Type</span></span>   |<span data-ttu-id="9c17a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9c17a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c17a-109">key</span><span class="sxs-lookup"><span data-stu-id="9c17a-109">key</span></span>|<span data-ttu-id="9c17a-110">String</span><span class="sxs-lookup"><span data-stu-id="9c17a-110">String</span></span>|<span data-ttu-id="9c17a-111">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="9c17a-111">The name of the parameter.</span></span>|
|<span data-ttu-id="9c17a-112">value</span><span class="sxs-lookup"><span data-stu-id="9c17a-112">value</span></span>|[<span data-ttu-id="9c17a-113">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="9c17a-113">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="9c17a-114">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="9c17a-114">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c17a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c17a-115">JSON representation</span></span>

<span data-ttu-id="9c17a-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c17a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyattributemappingsourcevaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
