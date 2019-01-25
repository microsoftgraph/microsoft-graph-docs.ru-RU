---
title: Тип ресурса keyValue
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 4223df85f9f120ba6477480f943d65a2511b6f2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528531"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="c3992-103">Тип ресурса keyValue</span><span class="sxs-lookup"><span data-stu-id="c3992-103">keyValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="c3992-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3992-104">JSON representation</span></span>

<span data-ttu-id="c3992-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3992-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyvalue"
}-->

```json
{
  "key": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="c3992-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3992-106">Properties</span></span>
| <span data-ttu-id="c3992-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3992-107">Property</span></span>     | <span data-ttu-id="c3992-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c3992-108">Type</span></span>   |<span data-ttu-id="c3992-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c3992-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3992-110">key</span><span class="sxs-lookup"><span data-stu-id="c3992-110">key</span></span>|<span data-ttu-id="c3992-111">string</span><span class="sxs-lookup"><span data-stu-id="c3992-111">string</span></span>||
|<span data-ttu-id="c3992-112">value</span><span class="sxs-lookup"><span data-stu-id="c3992-112">value</span></span>|<span data-ttu-id="c3992-113">строка</span><span class="sxs-lookup"><span data-stu-id="c3992-113">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/keyvalue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
