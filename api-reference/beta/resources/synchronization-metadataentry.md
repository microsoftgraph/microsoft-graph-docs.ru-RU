---
title: Тип ресурса metadataEntry
description: Метаданные для данного объекта.
localization_priority: Normal
ms.openlocfilehash: a6b9170144917e4c7b66bb52c1efb17d93167ef0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511781"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="20806-103">Тип ресурса metadataEntry</span><span class="sxs-lookup"><span data-stu-id="20806-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20806-104">Метаданные для данного объекта.</span><span class="sxs-lookup"><span data-stu-id="20806-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="20806-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="20806-105">Properties</span></span>
| <span data-ttu-id="20806-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="20806-106">Property</span></span>     | <span data-ttu-id="20806-107">Тип</span><span class="sxs-lookup"><span data-stu-id="20806-107">Type</span></span>   |<span data-ttu-id="20806-108">Описание</span><span class="sxs-lookup"><span data-stu-id="20806-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20806-109">key</span><span class="sxs-lookup"><span data-stu-id="20806-109">key</span></span>|<span data-ttu-id="20806-110">String</span><span class="sxs-lookup"><span data-stu-id="20806-110">String</span></span>|<span data-ttu-id="20806-111">Имя свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="20806-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="20806-112">value</span><span class="sxs-lookup"><span data-stu-id="20806-112">value</span></span>|<span data-ttu-id="20806-113">String</span><span class="sxs-lookup"><span data-stu-id="20806-113">String</span></span>|<span data-ttu-id="20806-114">Значение свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="20806-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20806-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20806-115">JSON representation</span></span>

<span data-ttu-id="20806-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20806-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
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
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-metadataentry.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
