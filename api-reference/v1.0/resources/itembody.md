---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
ms.openlocfilehash: df2e7e8cea9e1b2e6a6d1011029a1898e2794f45
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585309"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="722e6-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="722e6-103">itemBody resource type</span></span>

<span data-ttu-id="722e6-104">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="722e6-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="722e6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="722e6-105">Properties</span></span>
| <span data-ttu-id="722e6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="722e6-106">Property</span></span>     | <span data-ttu-id="722e6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="722e6-107">Type</span></span>   |<span data-ttu-id="722e6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="722e6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="722e6-109">content</span><span class="sxs-lookup"><span data-stu-id="722e6-109">content</span></span>|<span data-ttu-id="722e6-110">String</span><span class="sxs-lookup"><span data-stu-id="722e6-110">String</span></span>|<span data-ttu-id="722e6-111">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="722e6-111">The content of the item.</span></span>|
|<span data-ttu-id="722e6-112">contentType</span><span class="sxs-lookup"><span data-stu-id="722e6-112">contentType</span></span>|<span data-ttu-id="722e6-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="722e6-113">bodyType</span></span>|<span data-ttu-id="722e6-114">Тип контента.</span><span class="sxs-lookup"><span data-stu-id="722e6-114">The type of the content.</span></span> <span data-ttu-id="722e6-115">Возможные значения: `text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="722e6-115">Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="722e6-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="722e6-116">JSON representation</span></span>

<span data-ttu-id="722e6-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="722e6-117">Here is a JSON representation of the resource</span></span>

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
