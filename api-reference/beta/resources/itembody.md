---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
ms.openlocfilehash: 1cf79f78caa7b2772bc44b99c6b9bdc526340a87
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643194"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="f3403-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="f3403-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3403-104">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="f3403-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="f3403-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3403-105">Properties</span></span>
| <span data-ttu-id="f3403-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3403-106">Property</span></span>     | <span data-ttu-id="f3403-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f3403-107">Type</span></span>   |<span data-ttu-id="f3403-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f3403-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3403-109">content</span><span class="sxs-lookup"><span data-stu-id="f3403-109">content</span></span>|<span data-ttu-id="f3403-110">String</span><span class="sxs-lookup"><span data-stu-id="f3403-110">String</span></span>|<span data-ttu-id="f3403-111">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="f3403-111">The content of the item.</span></span>|
|<span data-ttu-id="f3403-112">contentType</span><span class="sxs-lookup"><span data-stu-id="f3403-112">contentType</span></span>|<span data-ttu-id="f3403-113">String</span><span class="sxs-lookup"><span data-stu-id="f3403-113">String</span></span>|<span data-ttu-id="f3403-p101">Тип контента. Возможные значения: `text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="f3403-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3403-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3403-116">JSON representation</span></span>

<span data-ttu-id="f3403-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3403-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/itembody.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
