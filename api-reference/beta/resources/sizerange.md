---
title: Тип ресурса sizeRange
description: Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: db90f040eef98af1136be7a80323dbedfe0acb92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520515"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="152f8-103">Тип ресурса sizeRange</span><span class="sxs-lookup"><span data-stu-id="152f8-103">sizeRange resource type</span></span>

<span data-ttu-id="152f8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="152f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="152f8-105">Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="152f8-105">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="152f8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="152f8-106">Properties</span></span>
| <span data-ttu-id="152f8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="152f8-107">Property</span></span>     | <span data-ttu-id="152f8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="152f8-108">Type</span></span>   |<span data-ttu-id="152f8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="152f8-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="152f8-110">maximumSize</span><span class="sxs-lookup"><span data-stu-id="152f8-110">maximumSize</span></span> | <span data-ttu-id="152f8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="152f8-111">Int32</span></span> | <span data-ttu-id="152f8-112">Максимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="152f8-112">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="152f8-113">minimumSize</span><span class="sxs-lookup"><span data-stu-id="152f8-113">minimumSize</span></span> | <span data-ttu-id="152f8-114">Int32</span><span class="sxs-lookup"><span data-stu-id="152f8-114">Int32</span></span> | <span data-ttu-id="152f8-115">Минимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="152f8-115">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="152f8-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="152f8-116">JSON representation</span></span>
<span data-ttu-id="152f8-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="152f8-117">Here is a JSON representation of the resource.</span></span>

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
