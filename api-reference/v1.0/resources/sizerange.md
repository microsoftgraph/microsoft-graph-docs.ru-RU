---
title: Тип ресурса sizeRange
description: Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e9c174216508679373c607dc9a2acd95df9096c9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034148"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="bfd2b-103">Тип ресурса sizeRange</span><span class="sxs-lookup"><span data-stu-id="bfd2b-103">sizeRange resource type</span></span>


<span data-ttu-id="bfd2b-104">Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="bfd2b-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="bfd2b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfd2b-105">Properties</span></span>
| <span data-ttu-id="bfd2b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfd2b-106">Property</span></span>     | <span data-ttu-id="bfd2b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="bfd2b-107">Type</span></span>   |<span data-ttu-id="bfd2b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bfd2b-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bfd2b-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="bfd2b-109">maximumSize</span></span> | <span data-ttu-id="bfd2b-110">Int32</span><span class="sxs-lookup"><span data-stu-id="bfd2b-110">Int32</span></span> | <span data-ttu-id="bfd2b-111">Максимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="bfd2b-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="bfd2b-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="bfd2b-112">minimumSize</span></span> | <span data-ttu-id="bfd2b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="bfd2b-113">Int32</span></span> | <span data-ttu-id="bfd2b-114">Минимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="bfd2b-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="bfd2b-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfd2b-115">JSON representation</span></span>
<span data-ttu-id="bfd2b-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfd2b-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
