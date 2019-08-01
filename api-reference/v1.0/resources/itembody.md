---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 406a753ef8b58ba5ff19f7669239c3d9abb860c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036556"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="fc2cb-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="fc2cb-103">itemBody resource type</span></span>

<span data-ttu-id="fc2cb-104">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="fc2cb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc2cb-105">Properties</span></span>
| <span data-ttu-id="fc2cb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc2cb-106">Property</span></span>     | <span data-ttu-id="fc2cb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fc2cb-107">Type</span></span>   |<span data-ttu-id="fc2cb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fc2cb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc2cb-109">content</span><span class="sxs-lookup"><span data-stu-id="fc2cb-109">content</span></span>|<span data-ttu-id="fc2cb-110">String</span><span class="sxs-lookup"><span data-stu-id="fc2cb-110">String</span></span>|<span data-ttu-id="fc2cb-111">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-111">The content of the item.</span></span>|
|<span data-ttu-id="fc2cb-112">contentType</span><span class="sxs-lookup"><span data-stu-id="fc2cb-112">contentType</span></span>|<span data-ttu-id="fc2cb-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="fc2cb-113">bodyType</span></span>|<span data-ttu-id="fc2cb-114">Тип контента.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-114">The type of the content.</span></span> <span data-ttu-id="fc2cb-115">Возможные значения: `text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-115">Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc2cb-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc2cb-116">JSON representation</span></span>

<span data-ttu-id="fc2cb-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-117">Here is a JSON representation of the resource</span></span>

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
