---
title: Тип ресурса Филтероперанд
description: Содержит коллекцию значений для операнда.
localization_priority: Normal
ms.openlocfilehash: ab62477889cc92954ed308c508e18a638cd59375
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581809"
---
# <a name="filteroperand-resource-type"></a><span data-ttu-id="5755a-103">Тип ресурса Филтероперанд</span><span class="sxs-lookup"><span data-stu-id="5755a-103">filterOperand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5755a-104">Содержит коллекцию значений для операнда.</span><span class="sxs-lookup"><span data-stu-id="5755a-104">Contains a collection of values for the operand.</span></span>

## <a name="properties"></a><span data-ttu-id="5755a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5755a-105">Properties</span></span>
| <span data-ttu-id="5755a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5755a-106">Property</span></span>     | <span data-ttu-id="5755a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5755a-107">Type</span></span>   |<span data-ttu-id="5755a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5755a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5755a-109">values</span><span class="sxs-lookup"><span data-stu-id="5755a-109">values</span></span>|<span data-ttu-id="5755a-110">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5755a-110">String collection</span></span>|<span data-ttu-id="5755a-111">Коллекция значений.</span><span class="sxs-lookup"><span data-stu-id="5755a-111">Collection of values.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5755a-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5755a-112">JSON representation</span></span>

<span data-ttu-id="5755a-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5755a-113">The following is a JSON representation of the resource.</span></span>

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
