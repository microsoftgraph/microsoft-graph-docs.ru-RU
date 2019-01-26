---
title: Тип ресурса stringKeyObjectValuePair
description: Представляет пару ключ значение, где ключ — это строка, а значение — это произвольный объект JSON. Это открытого типа OData, который будет использовать свойство с именем `value` то есть допустимый объект JSON.
localization_priority: Normal
ms.openlocfilehash: 819a2e004ee712f1250652ce0b3811940545e643
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572173"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="08c5a-104">Тип ресурса stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="08c5a-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08c5a-105">Представляет пару ключ значение, где ключ — это строка, а значение — это произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="08c5a-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="08c5a-106">Это открытого типа OData, который будет использовать свойство с именем `value` то есть допустимый объект JSON.</span><span class="sxs-lookup"><span data-stu-id="08c5a-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="08c5a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08c5a-107">Properties</span></span>
| <span data-ttu-id="08c5a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08c5a-108">Property</span></span>     | <span data-ttu-id="08c5a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08c5a-109">Type</span></span>   |<span data-ttu-id="08c5a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="08c5a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08c5a-111">key</span><span class="sxs-lookup"><span data-stu-id="08c5a-111">key</span></span>|<span data-ttu-id="08c5a-112">Строка</span><span class="sxs-lookup"><span data-stu-id="08c5a-112">String</span></span>|<span data-ttu-id="08c5a-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="08c5a-113">Key.</span></span>|
|<span data-ttu-id="08c5a-114">value</span><span class="sxs-lookup"><span data-stu-id="08c5a-114">value</span></span>|<span data-ttu-id="08c5a-115">Json</span><span class="sxs-lookup"><span data-stu-id="08c5a-115">Json</span></span>|<span data-ttu-id="08c5a-116">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="08c5a-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08c5a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08c5a-117">JSON representation</span></span>

<span data-ttu-id="08c5a-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08c5a-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value":"Json"
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
