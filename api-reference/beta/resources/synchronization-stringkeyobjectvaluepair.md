---
title: Тип ресурса stringKeyObjectValuePair
description: Представляет пару ключ значение, где ключ — это строка, а значение — это произвольный объект JSON. Это открытого типа OData, который будет использовать свойство с именем `value` то есть допустимый объект JSON.
localization_priority: Normal
ms.openlocfilehash: 8f939c177f2130813c6080d46ad78664f6118857
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642928"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="9d5d4-104">Тип ресурса stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="9d5d4-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d5d4-105">Представляет пару ключ значение, где ключ — это строка, а значение — это произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="9d5d4-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="9d5d4-106">Это открытого типа OData, который будет использовать свойство с именем `value` то есть допустимый объект JSON.</span><span class="sxs-lookup"><span data-stu-id="9d5d4-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="9d5d4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d5d4-107">Properties</span></span>
| <span data-ttu-id="9d5d4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d5d4-108">Property</span></span>     | <span data-ttu-id="9d5d4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9d5d4-109">Type</span></span>   |<span data-ttu-id="9d5d4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d5d4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d5d4-111">key</span><span class="sxs-lookup"><span data-stu-id="9d5d4-111">key</span></span>|<span data-ttu-id="9d5d4-112">String</span><span class="sxs-lookup"><span data-stu-id="9d5d4-112">String</span></span>|<span data-ttu-id="9d5d4-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="9d5d4-113">Key.</span></span>|
|<span data-ttu-id="9d5d4-114">value</span><span class="sxs-lookup"><span data-stu-id="9d5d4-114">value</span></span>|<span data-ttu-id="9d5d4-115">Любой</span><span class="sxs-lookup"><span data-stu-id="9d5d4-115">Any</span></span>|<span data-ttu-id="9d5d4-116">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="9d5d4-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d5d4-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d5d4-117">JSON representation</span></span>

<span data-ttu-id="9d5d4-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d5d4-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyobjectvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
