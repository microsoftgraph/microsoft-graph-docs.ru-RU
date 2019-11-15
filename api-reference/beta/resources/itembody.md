---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: grangeryy
ms.openlocfilehash: 0bba7fce9557c6c249ea9aefced5a198a87f5026
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658809"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="9fed8-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="9fed8-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fed8-104">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="9fed8-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="9fed8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fed8-105">Properties</span></span>
| <span data-ttu-id="9fed8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fed8-106">Property</span></span>     | <span data-ttu-id="9fed8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9fed8-107">Type</span></span>   |<span data-ttu-id="9fed8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9fed8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fed8-109">content</span><span class="sxs-lookup"><span data-stu-id="9fed8-109">content</span></span>|<span data-ttu-id="9fed8-110">String</span><span class="sxs-lookup"><span data-stu-id="9fed8-110">String</span></span>|<span data-ttu-id="9fed8-111">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="9fed8-111">The content of the item.</span></span>|
|<span data-ttu-id="9fed8-112">contentType</span><span class="sxs-lookup"><span data-stu-id="9fed8-112">contentType</span></span>|<span data-ttu-id="9fed8-113">String</span><span class="sxs-lookup"><span data-stu-id="9fed8-113">String</span></span>|<span data-ttu-id="9fed8-p101">Тип контента. Возможные значения: `text` и `html`.</span><span class="sxs-lookup"><span data-stu-id="9fed8-p101">The type of the content. Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fed8-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fed8-116">JSON representation</span></span>

<span data-ttu-id="9fed8-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fed8-117">Here is a JSON representation of the resource</span></span>

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
