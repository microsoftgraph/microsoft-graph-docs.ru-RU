---
title: Тип ресурса Принтпажеранже
description: Указывает диапазон страниц для печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a8bbf452c337cb5c2ade7302eb29cff4bdb73d23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052544"
---
# <a name="printpagerange-resource-type"></a><span data-ttu-id="10271-103">Тип ресурса Принтпажеранже</span><span class="sxs-lookup"><span data-stu-id="10271-103">printPageRange resource type</span></span>

<span data-ttu-id="10271-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10271-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10271-105">Указывает диапазон страниц для печати.</span><span class="sxs-lookup"><span data-stu-id="10271-105">Specifies the range of pages to be printed.</span></span>

## <a name="properties"></a><span data-ttu-id="10271-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="10271-106">Properties</span></span>
| <span data-ttu-id="10271-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="10271-107">Property</span></span>     | <span data-ttu-id="10271-108">Тип</span><span class="sxs-lookup"><span data-stu-id="10271-108">Type</span></span>        | <span data-ttu-id="10271-109">Описание</span><span class="sxs-lookup"><span data-stu-id="10271-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10271-110">startPage</span><span class="sxs-lookup"><span data-stu-id="10271-110">startPage</span></span>|<span data-ttu-id="10271-111">Int32</span><span class="sxs-lookup"><span data-stu-id="10271-111">Int32</span></span>|<span data-ttu-id="10271-112">Начальная страница диапазона (включающая).</span><span class="sxs-lookup"><span data-stu-id="10271-112">The start page (inclusive) for the range.</span></span> <span data-ttu-id="10271-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="10271-113">Read-only.</span></span>|
|<span data-ttu-id="10271-114">ендпаже</span><span class="sxs-lookup"><span data-stu-id="10271-114">endPage</span></span>|<span data-ttu-id="10271-115">Int32</span><span class="sxs-lookup"><span data-stu-id="10271-115">Int32</span></span>|<span data-ttu-id="10271-116">Конечная страница диапазона (включающая).</span><span class="sxs-lookup"><span data-stu-id="10271-116">The end page (inclusive) for the range.</span></span> <span data-ttu-id="10271-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="10271-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10271-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10271-118">JSON representation</span></span>

<span data-ttu-id="10271-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10271-119">The following is a JSON representation of the resource.</span></span>

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


