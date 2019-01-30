---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
ms.openlocfilehash: df2e7e8cea9e1b2e6a6d1011029a1898e2794f45
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642564"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="e82b1-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="e82b1-103">itemBody resource type</span></span>

<span data-ttu-id="e82b1-104">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="e82b1-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="e82b1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e82b1-105">Properties</span></span>
| <span data-ttu-id="e82b1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e82b1-106">Property</span></span>     | <span data-ttu-id="e82b1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e82b1-107">Type</span></span>   |<span data-ttu-id="e82b1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e82b1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e82b1-109">content</span><span class="sxs-lookup"><span data-stu-id="e82b1-109">content</span></span>|<span data-ttu-id="e82b1-110">String</span><span class="sxs-lookup"><span data-stu-id="e82b1-110">String</span></span>|<span data-ttu-id="e82b1-111">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="e82b1-111">The content of the item.</span></span>|
|<span data-ttu-id="e82b1-112">contentType</span><span class="sxs-lookup"><span data-stu-id="e82b1-112">contentType</span></span>|<span data-ttu-id="e82b1-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="e82b1-113">bodyType</span></span>|<span data-ttu-id="e82b1-p101">Тип контента. Возможные значения: `text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="e82b1-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e82b1-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e82b1-116">JSON representation</span></span>

<span data-ttu-id="e82b1-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e82b1-117">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
