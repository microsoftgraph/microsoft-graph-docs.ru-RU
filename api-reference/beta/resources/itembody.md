---
title: Тип ресурса itemBody
description: Представляет свойства основного текста элемента, например сообщения, события или записи группы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: grangeryy
ms.openlocfilehash: 21f2be43bc31d7611cf43ebd228850e3993807fa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952790"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="59561-103">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="59561-103">itemBody resource type</span></span>

<span data-ttu-id="59561-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59561-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59561-105">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="59561-105">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="59561-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="59561-106">Properties</span></span>
| <span data-ttu-id="59561-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="59561-107">Property</span></span>     | <span data-ttu-id="59561-108">Тип</span><span class="sxs-lookup"><span data-stu-id="59561-108">Type</span></span>   |<span data-ttu-id="59561-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59561-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59561-110">content</span><span class="sxs-lookup"><span data-stu-id="59561-110">content</span></span>|<span data-ttu-id="59561-111">String</span><span class="sxs-lookup"><span data-stu-id="59561-111">String</span></span>|<span data-ttu-id="59561-112">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="59561-112">The content of the item.</span></span>|
|<span data-ttu-id="59561-113">contentType</span><span class="sxs-lookup"><span data-stu-id="59561-113">contentType</span></span>|<span data-ttu-id="59561-114">bodyType</span><span class="sxs-lookup"><span data-stu-id="59561-114">bodyType</span></span>|<span data-ttu-id="59561-115">Тип контента.</span><span class="sxs-lookup"><span data-stu-id="59561-115">The type of the content.</span></span> <span data-ttu-id="59561-116">Возможные значения: `text` и `html`.</span><span class="sxs-lookup"><span data-stu-id="59561-116">Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59561-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59561-117">JSON representation</span></span>

<span data-ttu-id="59561-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59561-118">Here is a JSON representation of the resource</span></span>

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


