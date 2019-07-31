---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0fa0360e3fe6c05e18446640900ca8840731219c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010065"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="9778d-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="9778d-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9778d-104">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="9778d-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="9778d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9778d-105">Properties</span></span>
| <span data-ttu-id="9778d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9778d-106">Property</span></span>     | <span data-ttu-id="9778d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9778d-107">Type</span></span>   |<span data-ttu-id="9778d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9778d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9778d-109">content</span><span class="sxs-lookup"><span data-stu-id="9778d-109">content</span></span>|<span data-ttu-id="9778d-110">String</span><span class="sxs-lookup"><span data-stu-id="9778d-110">String</span></span>|<span data-ttu-id="9778d-111">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="9778d-111">The content of the item.</span></span>|
|<span data-ttu-id="9778d-112">contentType</span><span class="sxs-lookup"><span data-stu-id="9778d-112">contentType</span></span>|<span data-ttu-id="9778d-113">String</span><span class="sxs-lookup"><span data-stu-id="9778d-113">String</span></span>|<span data-ttu-id="9778d-p101">Тип контента. Возможные значения: `text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="9778d-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9778d-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9778d-116">JSON representation</span></span>

<span data-ttu-id="9778d-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9778d-117">Here is a JSON representation of the resource</span></span>

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
