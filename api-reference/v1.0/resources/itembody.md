---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6cf87c803ec957b42cc55cf1523a708b145af117
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38657490"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="2fb9e-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="2fb9e-103">itemBody resource type</span></span>

<span data-ttu-id="2fb9e-104">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="2fb9e-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="2fb9e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2fb9e-105">Properties</span></span>
| <span data-ttu-id="2fb9e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fb9e-106">Property</span></span>     | <span data-ttu-id="2fb9e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2fb9e-107">Type</span></span>   |<span data-ttu-id="2fb9e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2fb9e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fb9e-109">content</span><span class="sxs-lookup"><span data-stu-id="2fb9e-109">content</span></span>|<span data-ttu-id="2fb9e-110">String</span><span class="sxs-lookup"><span data-stu-id="2fb9e-110">String</span></span>|<span data-ttu-id="2fb9e-111">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="2fb9e-111">The content of the item.</span></span>|
|<span data-ttu-id="2fb9e-112">contentType</span><span class="sxs-lookup"><span data-stu-id="2fb9e-112">contentType</span></span>|<span data-ttu-id="2fb9e-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="2fb9e-113">bodyType</span></span>|<span data-ttu-id="2fb9e-114">Тип контента.</span><span class="sxs-lookup"><span data-stu-id="2fb9e-114">The type of the content.</span></span> <span data-ttu-id="2fb9e-115">Возможные значения: `text` и `html`.</span><span class="sxs-lookup"><span data-stu-id="2fb9e-115">Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2fb9e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2fb9e-116">JSON representation</span></span>

<span data-ttu-id="2fb9e-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fb9e-117">Here is a JSON representation of the resource</span></span>

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
