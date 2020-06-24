---
title: Тип ресурса Интежерранже
description: Представляет включающий диапазон целых чисел, который описывается двумя границами Int64.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bef2bd71d3ac039165146bcc5783eef7ba67a785
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863707"
---
# <a name="integerrange-resource-type"></a><span data-ttu-id="70810-103">Тип ресурса Интежерранже</span><span class="sxs-lookup"><span data-stu-id="70810-103">integerRange resource type</span></span>

<span data-ttu-id="70810-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70810-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70810-105">Представляет включающий диапазон целых чисел, который описывается двумя границами Int64.</span><span class="sxs-lookup"><span data-stu-id="70810-105">Represents an inclusive range of integers described by two Int64 boundaries.</span></span>

## <a name="properties"></a><span data-ttu-id="70810-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="70810-106">Properties</span></span>
| <span data-ttu-id="70810-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="70810-107">Property</span></span>     | <span data-ttu-id="70810-108">Тип</span><span class="sxs-lookup"><span data-stu-id="70810-108">Type</span></span>        | <span data-ttu-id="70810-109">Описание</span><span class="sxs-lookup"><span data-stu-id="70810-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="70810-110">начать</span><span class="sxs-lookup"><span data-stu-id="70810-110">start</span></span>|<span data-ttu-id="70810-111">Int64</span><span class="sxs-lookup"><span data-stu-id="70810-111">Int64</span></span>|<span data-ttu-id="70810-112">Инклюзивная Нижняя граница диапазона целых чисел.</span><span class="sxs-lookup"><span data-stu-id="70810-112">The inclusive lower bound of the integer range.</span></span>|
|<span data-ttu-id="70810-113">end</span><span class="sxs-lookup"><span data-stu-id="70810-113">end</span></span>|<span data-ttu-id="70810-114">Int64</span><span class="sxs-lookup"><span data-stu-id="70810-114">Int64</span></span>|<span data-ttu-id="70810-115">Включающая верхняя граница диапазона целых чисел.</span><span class="sxs-lookup"><span data-stu-id="70810-115">The inclusive upper bound of the integer range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70810-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70810-116">JSON representation</span></span>

<span data-ttu-id="70810-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70810-117">The following is a JSON representation of the resource.</span></span>

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