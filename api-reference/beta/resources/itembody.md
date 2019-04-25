---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
ms.openlocfilehash: 1cf79f78caa7b2772bc44b99c6b9bdc526340a87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523492"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="62927-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="62927-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62927-104">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="62927-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="62927-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="62927-105">Properties</span></span>
| <span data-ttu-id="62927-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="62927-106">Property</span></span>     | <span data-ttu-id="62927-107">Тип</span><span class="sxs-lookup"><span data-stu-id="62927-107">Type</span></span>   |<span data-ttu-id="62927-108">Описание</span><span class="sxs-lookup"><span data-stu-id="62927-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62927-109">content</span><span class="sxs-lookup"><span data-stu-id="62927-109">content</span></span>|<span data-ttu-id="62927-110">String</span><span class="sxs-lookup"><span data-stu-id="62927-110">String</span></span>|<span data-ttu-id="62927-111">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="62927-111">The content of the item.</span></span>|
|<span data-ttu-id="62927-112">contentType</span><span class="sxs-lookup"><span data-stu-id="62927-112">contentType</span></span>|<span data-ttu-id="62927-113">Строка</span><span class="sxs-lookup"><span data-stu-id="62927-113">String</span></span>|<span data-ttu-id="62927-p101">Тип контента. Возможные значения: `text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="62927-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62927-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62927-116">JSON representation</span></span>

<span data-ttu-id="62927-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62927-117">Here is a JSON representation of the resource</span></span>

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
