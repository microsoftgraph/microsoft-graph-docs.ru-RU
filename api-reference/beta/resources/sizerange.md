---
title: Тип ресурса sizeRange
description: Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 68fb44ff091720520c5061f0421d3819a8eed176
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965007"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="fcb66-103">Тип ресурса sizeRange</span><span class="sxs-lookup"><span data-stu-id="fcb66-103">sizeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcb66-104">Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="fcb66-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="fcb66-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcb66-105">Properties</span></span>
| <span data-ttu-id="fcb66-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcb66-106">Property</span></span>     | <span data-ttu-id="fcb66-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fcb66-107">Type</span></span>   |<span data-ttu-id="fcb66-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fcb66-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fcb66-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="fcb66-109">maximumSize</span></span> | <span data-ttu-id="fcb66-110">Int32</span><span class="sxs-lookup"><span data-stu-id="fcb66-110">Int32</span></span> | <span data-ttu-id="fcb66-111">Максимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="fcb66-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="fcb66-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="fcb66-112">minimumSize</span></span> | <span data-ttu-id="fcb66-113">Int32</span><span class="sxs-lookup"><span data-stu-id="fcb66-113">Int32</span></span> | <span data-ttu-id="fcb66-114">Минимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="fcb66-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="fcb66-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcb66-115">JSON representation</span></span>
<span data-ttu-id="fcb66-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcb66-116">Here is a JSON representation of the resource.</span></span>

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
