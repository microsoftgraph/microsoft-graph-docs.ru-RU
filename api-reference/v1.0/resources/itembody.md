---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
ms.openlocfilehash: ebcc2797052ac3a5a73547332e37c5e9c1bd3a41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027052"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="263b8-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="263b8-103">itemBody resource type</span></span>

<span data-ttu-id="263b8-104">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="263b8-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="263b8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="263b8-105">Properties</span></span>
| <span data-ttu-id="263b8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="263b8-106">Property</span></span>     | <span data-ttu-id="263b8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="263b8-107">Type</span></span>   |<span data-ttu-id="263b8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="263b8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="263b8-109">content</span><span class="sxs-lookup"><span data-stu-id="263b8-109">content</span></span>|<span data-ttu-id="263b8-110">String</span><span class="sxs-lookup"><span data-stu-id="263b8-110">String</span></span>|<span data-ttu-id="263b8-111">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="263b8-111">The content of the item.</span></span>|
|<span data-ttu-id="263b8-112">contentType</span><span class="sxs-lookup"><span data-stu-id="263b8-112">contentType</span></span>|<span data-ttu-id="263b8-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="263b8-113">bodyType</span></span>|<span data-ttu-id="263b8-p101">Тип контента. Возможные значения: `Text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="263b8-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="263b8-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="263b8-116">JSON representation</span></span>

<span data-ttu-id="263b8-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="263b8-117">Here is a JSON representation of the resource</span></span>

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
