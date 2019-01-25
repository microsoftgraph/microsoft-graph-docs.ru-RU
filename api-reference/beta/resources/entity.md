---
title: Тип ресурса entity
description: Нет
localization_priority: Normal
ms.openlocfilehash: e1dd9a8d66dd326076c8a7dd534c2210f53d06e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509121"
---
# <a name="entity-resource-type"></a><span data-ttu-id="9cad4-103">Тип ресурса entity</span><span class="sxs-lookup"><span data-stu-id="9cad4-103">entity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="9cad4-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cad4-104">Properties</span></span>
| <span data-ttu-id="9cad4-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cad4-105">Property</span></span> | <span data-ttu-id="9cad4-106">Тип</span><span class="sxs-lookup"><span data-stu-id="9cad4-106">Type</span></span>  | <span data-ttu-id="9cad4-107">Описание</span><span class="sxs-lookup"><span data-stu-id="9cad4-107">Description</span></span> |
|:---------|:------|:------------|
|<span data-ttu-id="9cad4-108">id</span><span class="sxs-lookup"><span data-stu-id="9cad4-108">id</span></span>        |<span data-ttu-id="9cad4-109">String</span><span class="sxs-lookup"><span data-stu-id="9cad4-109">String</span></span> | <span data-ttu-id="9cad4-110">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cad4-110">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="9cad4-111">Отношения</span><span class="sxs-lookup"><span data-stu-id="9cad4-111">Relationships</span></span>
<span data-ttu-id="9cad4-112">Нет</span><span class="sxs-lookup"><span data-stu-id="9cad4-112">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cad4-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cad4-113">JSON representation</span></span>

<span data-ttu-id="9cad4-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cad4-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "abstract": "true",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entity"
}-->
```json
{
  "id": "string (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "entity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/entity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
