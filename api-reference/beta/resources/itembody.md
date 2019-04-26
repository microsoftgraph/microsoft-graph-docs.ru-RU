---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
ms.openlocfilehash: e035c08d5f13d67bfb5871501e5a0f57745b7543
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345612"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="e168a-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="e168a-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e168a-104">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="e168a-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="e168a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e168a-105">Properties</span></span>
| <span data-ttu-id="e168a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e168a-106">Property</span></span>     | <span data-ttu-id="e168a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e168a-107">Type</span></span>   |<span data-ttu-id="e168a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e168a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e168a-109">content</span><span class="sxs-lookup"><span data-stu-id="e168a-109">content</span></span>|<span data-ttu-id="e168a-110">String</span><span class="sxs-lookup"><span data-stu-id="e168a-110">String</span></span>|<span data-ttu-id="e168a-111">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="e168a-111">The content of the item.</span></span>|
|<span data-ttu-id="e168a-112">contentType</span><span class="sxs-lookup"><span data-stu-id="e168a-112">contentType</span></span>|<span data-ttu-id="e168a-113">String</span><span class="sxs-lookup"><span data-stu-id="e168a-113">String</span></span>|<span data-ttu-id="e168a-p101">Тип контента. Возможные значения: `text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="e168a-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e168a-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e168a-116">JSON representation</span></span>

<span data-ttu-id="e168a-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e168a-117">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
