---
title: Тип ресурса Принтмаргин
description: Задает ширину полей, используемую при печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d7399f45138d6ab7d82f33e6577e7d08967ad15
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863700"
---
# <a name="printmargin-complex-type"></a><span data-ttu-id="e32b8-103">сложный тип Принтмаргин</span><span class="sxs-lookup"><span data-stu-id="e32b8-103">printMargin complex type</span></span>

<span data-ttu-id="e32b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e32b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e32b8-105">Задает ширину полей, используемую при печати.</span><span class="sxs-lookup"><span data-stu-id="e32b8-105">Specifies the margin widths to use when printing.</span></span>

## <a name="properties"></a><span data-ttu-id="e32b8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e32b8-106">Properties</span></span>
| <span data-ttu-id="e32b8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e32b8-107">Property</span></span>     | <span data-ttu-id="e32b8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e32b8-108">Type</span></span>        | <span data-ttu-id="e32b8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e32b8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e32b8-110">top</span><span class="sxs-lookup"><span data-stu-id="e32b8-110">top</span></span>|<span data-ttu-id="e32b8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="e32b8-111">Int32</span></span>|<span data-ttu-id="e32b8-112">Маржа в микронах от верхнего края.</span><span class="sxs-lookup"><span data-stu-id="e32b8-112">The margin in microns from the top edge.</span></span>|
|<span data-ttu-id="e32b8-113">bottom</span><span class="sxs-lookup"><span data-stu-id="e32b8-113">bottom</span></span>|<span data-ttu-id="e32b8-114">Int32</span><span class="sxs-lookup"><span data-stu-id="e32b8-114">Int32</span></span>|<span data-ttu-id="e32b8-115">Маржа в микронах от нижнего края.</span><span class="sxs-lookup"><span data-stu-id="e32b8-115">The margin in microns from the bottom edge.</span></span>|
|<span data-ttu-id="e32b8-116">Правильно</span><span class="sxs-lookup"><span data-stu-id="e32b8-116">right</span></span>|<span data-ttu-id="e32b8-117">Int32</span><span class="sxs-lookup"><span data-stu-id="e32b8-117">Int32</span></span>|<span data-ttu-id="e32b8-118">Маржа в микронах от правого края.</span><span class="sxs-lookup"><span data-stu-id="e32b8-118">The margin in microns from the right edge.</span></span>|
|<span data-ttu-id="e32b8-119">left</span><span class="sxs-lookup"><span data-stu-id="e32b8-119">left</span></span>|<span data-ttu-id="e32b8-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e32b8-120">Int32</span></span>|<span data-ttu-id="e32b8-121">Маржа в микронах от левого края.</span><span class="sxs-lookup"><span data-stu-id="e32b8-121">The margin in microns from the left edge.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e32b8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e32b8-122">JSON representation</span></span>

<span data-ttu-id="e32b8-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e32b8-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printMargin"
}-->

```json
{
  "top": 123456,
  "bottom": 123456,
  "right": 123456,
  "left": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printMargin resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
