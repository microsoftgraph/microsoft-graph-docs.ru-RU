---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
ms.openlocfilehash: 791906c8442250d05d1b94b9eb9b19320f45e9c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872144"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="9bbe9-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="9bbe9-103">itemBody resource type</span></span>

> <span data-ttu-id="9bbe9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9bbe9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bbe9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bbe9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bbe9-106">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="9bbe9-106">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="9bbe9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9bbe9-107">Properties</span></span>
| <span data-ttu-id="9bbe9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bbe9-108">Property</span></span>     | <span data-ttu-id="9bbe9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9bbe9-109">Type</span></span>   |<span data-ttu-id="9bbe9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9bbe9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bbe9-111">content</span><span class="sxs-lookup"><span data-stu-id="9bbe9-111">content</span></span>|<span data-ttu-id="9bbe9-112">String</span><span class="sxs-lookup"><span data-stu-id="9bbe9-112">String</span></span>|<span data-ttu-id="9bbe9-113">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="9bbe9-113">The content of the item.</span></span>|
|<span data-ttu-id="9bbe9-114">contentType</span><span class="sxs-lookup"><span data-stu-id="9bbe9-114">contentType</span></span>|<span data-ttu-id="9bbe9-115">String</span><span class="sxs-lookup"><span data-stu-id="9bbe9-115">String</span></span>|<span data-ttu-id="9bbe9-p102">Тип контента. Возможные значения: `Text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="9bbe9-p102">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9bbe9-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9bbe9-118">JSON representation</span></span>

<span data-ttu-id="9bbe9-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bbe9-119">Here is a JSON representation of the resource</span></span>

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
