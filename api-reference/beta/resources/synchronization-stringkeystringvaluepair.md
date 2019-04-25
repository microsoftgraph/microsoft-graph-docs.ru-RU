---
title: Тип ресурса Стрингкэйстрингвалуепаир
description: Представляет собой ключ-значение, в котором ключ является строкой, а значение является строкой.
localization_priority: Normal
ms.openlocfilehash: f91d63ee4b4d3b0328bbb6fbe58c74ec8f78c5b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526274"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="4ed14-103">Тип ресурса Стрингкэйстрингвалуепаир</span><span class="sxs-lookup"><span data-stu-id="4ed14-103">stringKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ed14-104">Представляет собой ключ-значение, в котором ключ является строкой, а значение является строкой.</span><span class="sxs-lookup"><span data-stu-id="4ed14-104">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="4ed14-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ed14-105">Properties</span></span>
| <span data-ttu-id="4ed14-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ed14-106">Property</span></span>     | <span data-ttu-id="4ed14-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4ed14-107">Type</span></span>   |<span data-ttu-id="4ed14-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4ed14-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ed14-109">ключа</span><span class="sxs-lookup"><span data-stu-id="4ed14-109">key</span></span>|<span data-ttu-id="4ed14-110">String</span><span class="sxs-lookup"><span data-stu-id="4ed14-110">String</span></span>|<span data-ttu-id="4ed14-111">Ключ.</span><span class="sxs-lookup"><span data-stu-id="4ed14-111">Key.</span></span>|
|<span data-ttu-id="4ed14-112">value</span><span class="sxs-lookup"><span data-stu-id="4ed14-112">value</span></span>|<span data-ttu-id="4ed14-113">String</span><span class="sxs-lookup"><span data-stu-id="4ed14-113">String</span></span>|<span data-ttu-id="4ed14-114">Значение</span><span class="sxs-lookup"><span data-stu-id="4ed14-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ed14-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4ed14-115">JSON representation</span></span>

<span data-ttu-id="4ed14-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ed14-116">The following is a JSON representation of the resource.</span></span>

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
