---
title: Тип ресурса sizeRange
description: Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.
ms.openlocfilehash: e9ef87063959f320068933a17c1fa8b0a70859da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024795"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="86c54-103">Тип ресурса sizeRange</span><span class="sxs-lookup"><span data-stu-id="86c54-103">sizeRange resource type</span></span>


<span data-ttu-id="86c54-104">Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="86c54-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="86c54-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="86c54-105">Properties</span></span>
| <span data-ttu-id="86c54-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="86c54-106">Property</span></span>     | <span data-ttu-id="86c54-107">Тип</span><span class="sxs-lookup"><span data-stu-id="86c54-107">Type</span></span>   |<span data-ttu-id="86c54-108">Описание</span><span class="sxs-lookup"><span data-stu-id="86c54-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="86c54-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="86c54-109">maximumSize</span></span> | <span data-ttu-id="86c54-110">Int32</span><span class="sxs-lookup"><span data-stu-id="86c54-110">Int32</span></span> | <span data-ttu-id="86c54-111">Максимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="86c54-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="86c54-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="86c54-112">minimumSize</span></span> | <span data-ttu-id="86c54-113">Int32</span><span class="sxs-lookup"><span data-stu-id="86c54-113">Int32</span></span> | <span data-ttu-id="86c54-114">Минимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="86c54-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="86c54-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86c54-115">JSON representation</span></span>
<span data-ttu-id="86c54-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86c54-116">Here is a JSON representation of the resource.</span></span>

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