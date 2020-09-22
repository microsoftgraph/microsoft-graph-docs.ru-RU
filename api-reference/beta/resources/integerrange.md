---
title: Тип ресурса Интежерранже
description: Представляет включающий диапазон целых чисел, который описывается двумя границами Int64.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ee879104878189ddcaf51f65e4e127a61798c811
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986058"
---
# <a name="integerrange-resource-type"></a><span data-ttu-id="e65f8-103">Тип ресурса Интежерранже</span><span class="sxs-lookup"><span data-stu-id="e65f8-103">integerRange resource type</span></span>

<span data-ttu-id="e65f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e65f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e65f8-105">Представляет включающий диапазон целых чисел, который описывается двумя границами Int64.</span><span class="sxs-lookup"><span data-stu-id="e65f8-105">Represents an inclusive range of integers described by two Int64 boundaries.</span></span>

## <a name="properties"></a><span data-ttu-id="e65f8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e65f8-106">Properties</span></span>
| <span data-ttu-id="e65f8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e65f8-107">Property</span></span>     | <span data-ttu-id="e65f8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e65f8-108">Type</span></span>        | <span data-ttu-id="e65f8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e65f8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e65f8-110">start</span><span class="sxs-lookup"><span data-stu-id="e65f8-110">start</span></span>|<span data-ttu-id="e65f8-111">Int64</span><span class="sxs-lookup"><span data-stu-id="e65f8-111">Int64</span></span>|<span data-ttu-id="e65f8-112">Инклюзивная Нижняя граница диапазона целых чисел.</span><span class="sxs-lookup"><span data-stu-id="e65f8-112">The inclusive lower bound of the integer range.</span></span>|
|<span data-ttu-id="e65f8-113">end</span><span class="sxs-lookup"><span data-stu-id="e65f8-113">end</span></span>|<span data-ttu-id="e65f8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e65f8-114">Int64</span></span>|<span data-ttu-id="e65f8-115">Включающая верхняя граница диапазона целых чисел.</span><span class="sxs-lookup"><span data-stu-id="e65f8-115">The inclusive upper bound of the integer range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e65f8-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e65f8-116">JSON representation</span></span>

<span data-ttu-id="e65f8-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e65f8-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.integerRange"
}-->

```json
{
    "start": 12345,
    "end": 12345
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "integerRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

