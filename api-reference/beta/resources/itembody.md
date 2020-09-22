---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: grangeryy
ms.openlocfilehash: 8ee076b96df14b4d4c4958b4c1d6bdf36fecdde2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075618"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="31567-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="31567-103">itemBody resource type</span></span>

<span data-ttu-id="31567-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31567-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31567-105">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="31567-105">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="31567-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="31567-106">Properties</span></span>
| <span data-ttu-id="31567-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="31567-107">Property</span></span>     | <span data-ttu-id="31567-108">Тип</span><span class="sxs-lookup"><span data-stu-id="31567-108">Type</span></span>   |<span data-ttu-id="31567-109">Описание</span><span class="sxs-lookup"><span data-stu-id="31567-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31567-110">content</span><span class="sxs-lookup"><span data-stu-id="31567-110">content</span></span>|<span data-ttu-id="31567-111">String</span><span class="sxs-lookup"><span data-stu-id="31567-111">String</span></span>|<span data-ttu-id="31567-112">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="31567-112">The content of the item.</span></span>|
|<span data-ttu-id="31567-113">contentType</span><span class="sxs-lookup"><span data-stu-id="31567-113">contentType</span></span>|<span data-ttu-id="31567-114">String</span><span class="sxs-lookup"><span data-stu-id="31567-114">String</span></span>|<span data-ttu-id="31567-p101">Тип контента. Возможные значения: `text` и `html`.</span><span class="sxs-lookup"><span data-stu-id="31567-p101">The type of the content. Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31567-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31567-117">JSON representation</span></span>

<span data-ttu-id="31567-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31567-118">Here is a JSON representation of the resource</span></span>

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


