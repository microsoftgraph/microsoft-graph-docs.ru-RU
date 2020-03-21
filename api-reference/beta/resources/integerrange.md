---
title: Тип ресурса Интежерранже
description: Представляет включающий диапазон целых чисел, который описывается двумя границами Int64.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c7c3a14e8b8772a0bc319d8415046f3e10871f52
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896038"
---
# <a name="integerrange-resource-type"></a><span data-ttu-id="db49a-103">Тип ресурса Интежерранже</span><span class="sxs-lookup"><span data-stu-id="db49a-103">integerRange resource type</span></span>

<span data-ttu-id="db49a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db49a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db49a-105">Представляет включающий диапазон целых чисел, который описывается двумя границами Int64.</span><span class="sxs-lookup"><span data-stu-id="db49a-105">Represents an inclusive range of integers described by two Int64 boundaries.</span></span>

## <a name="properties"></a><span data-ttu-id="db49a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="db49a-106">Properties</span></span>
| <span data-ttu-id="db49a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="db49a-107">Property</span></span>     | <span data-ttu-id="db49a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="db49a-108">Type</span></span>        | <span data-ttu-id="db49a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="db49a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="db49a-110">minimum</span><span class="sxs-lookup"><span data-stu-id="db49a-110">minimum</span></span>|<span data-ttu-id="db49a-111">Int64</span><span class="sxs-lookup"><span data-stu-id="db49a-111">Int64</span></span>|<span data-ttu-id="db49a-112">Инклюзивная Нижняя граница диапазона целых чисел.</span><span class="sxs-lookup"><span data-stu-id="db49a-112">The inclusive lower bound of the integer range.</span></span>|
|<span data-ttu-id="db49a-113">maximum</span><span class="sxs-lookup"><span data-stu-id="db49a-113">maximum</span></span>|<span data-ttu-id="db49a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="db49a-114">Int64</span></span>|<span data-ttu-id="db49a-115">Включающая верхняя граница диапазона целых чисел.</span><span class="sxs-lookup"><span data-stu-id="db49a-115">The inclusive upper bound of the integer range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db49a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db49a-116">JSON representation</span></span>

<span data-ttu-id="db49a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db49a-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.integerRange"
}-->

```json
{
    "minimum": 12345,
    "maximum": 12345
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