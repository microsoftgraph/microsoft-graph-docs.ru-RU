---
title: Тип ресурса extension
description: Абстрактный тип для поддержки открытого типа openTypeExtension в OData 4-й версии.
localization_priority: Normal
ms.openlocfilehash: b261ceeff4639b8a602edbb411b34ab19d46ea8e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512747"
---
# <a name="extension-resource-type"></a><span data-ttu-id="2ba02-103">Тип ресурса extension</span><span class="sxs-lookup"><span data-stu-id="2ba02-103">extension resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ba02-104">Абстрактный тип для поддержки открытого типа [openTypeExtension](opentypeextension.md) в OData 4-й версии.</span><span class="sxs-lookup"><span data-stu-id="2ba02-104">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ba02-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ba02-105">JSON representation</span></span>

<span data-ttu-id="2ba02-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="2ba02-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="2ba02-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ba02-107">Properties</span></span>
| <span data-ttu-id="2ba02-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ba02-108">Property</span></span>     | <span data-ttu-id="2ba02-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2ba02-109">Type</span></span>   |<span data-ttu-id="2ba02-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2ba02-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ba02-111">id</span><span class="sxs-lookup"><span data-stu-id="2ba02-111">id</span></span>|<span data-ttu-id="2ba02-112">String</span><span class="sxs-lookup"><span data-stu-id="2ba02-112">String</span></span>| <span data-ttu-id="2ba02-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ba02-113">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ba02-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="2ba02-114">Relationships</span></span>
<span data-ttu-id="2ba02-115">Нет</span><span class="sxs-lookup"><span data-stu-id="2ba02-115">None</span></span>


## <a name="methods"></a><span data-ttu-id="2ba02-116">Методы</span><span class="sxs-lookup"><span data-stu-id="2ba02-116">Methods</span></span>

<span data-ttu-id="2ba02-117">Фактически поддерживаемые методы указаны в описании производного типа [openTypeExtension](opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="2ba02-117">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/extension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
