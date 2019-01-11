---
title: Тип ресурса sizeRange
description: Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.
localization_priority: Normal
ms.openlocfilehash: 14dd86502feb0a5082d3af142202f77ec9eac75c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876407"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="f2c4a-103">Тип ресурса sizeRange</span><span class="sxs-lookup"><span data-stu-id="f2c4a-103">sizeRange resource type</span></span>

> <span data-ttu-id="f2c4a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2c4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2c4a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2c4a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2c4a-106">Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="f2c4a-106">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="f2c4a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2c4a-107">Properties</span></span>
| <span data-ttu-id="f2c4a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2c4a-108">Property</span></span>     | <span data-ttu-id="f2c4a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f2c4a-109">Type</span></span>   |<span data-ttu-id="f2c4a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f2c4a-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f2c4a-111">maximumSize</span><span class="sxs-lookup"><span data-stu-id="f2c4a-111">maximumSize</span></span> | <span data-ttu-id="f2c4a-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f2c4a-112">Int32</span></span> | <span data-ttu-id="f2c4a-113">Максимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="f2c4a-113">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="f2c4a-114">minimumSize</span><span class="sxs-lookup"><span data-stu-id="f2c4a-114">minimumSize</span></span> | <span data-ttu-id="f2c4a-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f2c4a-115">Int32</span></span> | <span data-ttu-id="f2c4a-116">Минимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="f2c4a-116">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f2c4a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2c4a-117">JSON representation</span></span>
<span data-ttu-id="f2c4a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2c4a-118">Here is a JSON representation of the resource.</span></span>

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
