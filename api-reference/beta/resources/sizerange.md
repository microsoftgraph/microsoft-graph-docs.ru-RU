---
title: Тип ресурса sizeRange
description: Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.
localization_priority: Normal
ms.openlocfilehash: c2a37c91c968eddffc4aca0c8cf783e5aac1f3eb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343010"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="c1421-103">Тип ресурса sizeRange</span><span class="sxs-lookup"><span data-stu-id="c1421-103">sizeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1421-104">Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="c1421-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="c1421-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1421-105">Properties</span></span>
| <span data-ttu-id="c1421-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1421-106">Property</span></span>     | <span data-ttu-id="c1421-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c1421-107">Type</span></span>   |<span data-ttu-id="c1421-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c1421-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c1421-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="c1421-109">maximumSize</span></span> | <span data-ttu-id="c1421-110">Int32</span><span class="sxs-lookup"><span data-stu-id="c1421-110">Int32</span></span> | <span data-ttu-id="c1421-111">Максимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="c1421-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="c1421-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="c1421-112">minimumSize</span></span> | <span data-ttu-id="c1421-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c1421-113">Int32</span></span> | <span data-ttu-id="c1421-114">Минимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="c1421-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c1421-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1421-115">JSON representation</span></span>
<span data-ttu-id="c1421-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1421-116">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
