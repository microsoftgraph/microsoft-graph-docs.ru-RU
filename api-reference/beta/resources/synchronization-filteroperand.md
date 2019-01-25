---
title: Тип ресурса filterOperand
description: Содержит коллекцию значений для операнда.
localization_priority: Normal
ms.openlocfilehash: ab62477889cc92954ed308c508e18a638cd59375
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515379"
---
# <a name="filteroperand-resource-type"></a><span data-ttu-id="93a30-103">Тип ресурса filterOperand</span><span class="sxs-lookup"><span data-stu-id="93a30-103">filterOperand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93a30-104">Содержит коллекцию значений для операнда.</span><span class="sxs-lookup"><span data-stu-id="93a30-104">Contains a collection of values for the operand.</span></span>

## <a name="properties"></a><span data-ttu-id="93a30-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="93a30-105">Properties</span></span>
| <span data-ttu-id="93a30-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="93a30-106">Property</span></span>     | <span data-ttu-id="93a30-107">Тип</span><span class="sxs-lookup"><span data-stu-id="93a30-107">Type</span></span>   |<span data-ttu-id="93a30-108">Описание</span><span class="sxs-lookup"><span data-stu-id="93a30-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93a30-109">values</span><span class="sxs-lookup"><span data-stu-id="93a30-109">values</span></span>|<span data-ttu-id="93a30-110">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="93a30-110">String collection</span></span>|<span data-ttu-id="93a30-111">Коллекция значений.</span><span class="sxs-lookup"><span data-stu-id="93a30-111">Collection of values.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93a30-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93a30-112">JSON representation</span></span>

<span data-ttu-id="93a30-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93a30-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperand"
}-->

```json
{
  "values": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterOperand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperand.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
