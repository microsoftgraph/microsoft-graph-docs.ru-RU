---
title: Тип ресурса sizeRange
description: Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.
localization_priority: Normal
ms.openlocfilehash: ae754d0666185023272860864ef17f038aecff7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552751"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="95c7d-103">Тип ресурса sizeRange</span><span class="sxs-lookup"><span data-stu-id="95c7d-103">sizeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95c7d-104">Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="95c7d-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="95c7d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="95c7d-105">Properties</span></span>
| <span data-ttu-id="95c7d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="95c7d-106">Property</span></span>     | <span data-ttu-id="95c7d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="95c7d-107">Type</span></span>   |<span data-ttu-id="95c7d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="95c7d-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95c7d-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="95c7d-109">maximumSize</span></span> | <span data-ttu-id="95c7d-110">Int32</span><span class="sxs-lookup"><span data-stu-id="95c7d-110">Int32</span></span> | <span data-ttu-id="95c7d-111">Максимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="95c7d-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="95c7d-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="95c7d-112">minimumSize</span></span> | <span data-ttu-id="95c7d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="95c7d-113">Int32</span></span> | <span data-ttu-id="95c7d-114">Минимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="95c7d-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="95c7d-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="95c7d-115">JSON representation</span></span>
<span data-ttu-id="95c7d-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95c7d-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sizerange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
