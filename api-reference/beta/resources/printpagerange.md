---
title: Тип ресурса Принтпажеранже
description: Указывает диапазон страниц для печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 65e2455438dbdb8c7bef3ef3439f846e737ebba0
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895987"
---
# <a name="printpagerange-resource-type"></a><span data-ttu-id="e5067-103">Тип ресурса Принтпажеранже</span><span class="sxs-lookup"><span data-stu-id="e5067-103">printPageRange resource type</span></span>

<span data-ttu-id="e5067-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5067-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5067-105">Указывает диапазон страниц для печати.</span><span class="sxs-lookup"><span data-stu-id="e5067-105">Specifies the range of pages to be printed.</span></span>

## <a name="properties"></a><span data-ttu-id="e5067-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5067-106">Properties</span></span>
| <span data-ttu-id="e5067-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5067-107">Property</span></span>     | <span data-ttu-id="e5067-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e5067-108">Type</span></span>        | <span data-ttu-id="e5067-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e5067-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e5067-110">startPage</span><span class="sxs-lookup"><span data-stu-id="e5067-110">startPage</span></span>|<span data-ttu-id="e5067-111">Int32</span><span class="sxs-lookup"><span data-stu-id="e5067-111">Int32</span></span>|<span data-ttu-id="e5067-112">Начальная страница диапазона (включающая).</span><span class="sxs-lookup"><span data-stu-id="e5067-112">The start page (inclusive) for the range.</span></span> <span data-ttu-id="e5067-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5067-113">Read-only.</span></span>|
|<span data-ttu-id="e5067-114">ендпаже</span><span class="sxs-lookup"><span data-stu-id="e5067-114">endPage</span></span>|<span data-ttu-id="e5067-115">Int32</span><span class="sxs-lookup"><span data-stu-id="e5067-115">Int32</span></span>|<span data-ttu-id="e5067-116">Конечная страница диапазона (включающая).</span><span class="sxs-lookup"><span data-stu-id="e5067-116">The end page (inclusive) for the range.</span></span> <span data-ttu-id="e5067-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5067-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5067-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5067-118">JSON representation</span></span>

<span data-ttu-id="e5067-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5067-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printPageRange"
}-->

```json
{
  "startPage": 123456,
  "endPage": 123456
}
```
