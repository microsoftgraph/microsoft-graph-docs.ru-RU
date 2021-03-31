---
title: тип ресурса directorySizeQuota
description: Представляет используемую и общую квоту каталогов компании.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: 54e2280fdb416e5ccfd0853ee77a2ef3f90ddf37
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469376"
---
# <a name="directorysizequota-resource-type"></a><span data-ttu-id="5e889-103">тип ресурса directorySizeQuota</span><span class="sxs-lookup"><span data-stu-id="5e889-103">directorySizeQuota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e889-104">Представляет используемую и общую квоту каталогов компании.</span><span class="sxs-lookup"><span data-stu-id="5e889-104">Represents a company's used and total directory quota.</span></span>

## <a name="properties"></a><span data-ttu-id="5e889-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e889-105">Properties</span></span>
| <span data-ttu-id="5e889-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e889-106">Property</span></span>   | <span data-ttu-id="5e889-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5e889-107">Type</span></span>|<span data-ttu-id="5e889-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5e889-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e889-109">used</span><span class="sxs-lookup"><span data-stu-id="5e889-109">used</span></span>|<span data-ttu-id="5e889-110">Int32</span><span class="sxs-lookup"><span data-stu-id="5e889-110">Int32</span></span>| <span data-ttu-id="5e889-111">Используемая сумма квоты каталога.</span><span class="sxs-lookup"><span data-stu-id="5e889-111">Used amount of the directory quota.</span></span> |
|<span data-ttu-id="5e889-112">total</span><span class="sxs-lookup"><span data-stu-id="5e889-112">total</span></span>|<span data-ttu-id="5e889-113">Int32</span><span class="sxs-lookup"><span data-stu-id="5e889-113">Int32</span></span>| <span data-ttu-id="5e889-114">Общая сумма квоты каталога.</span><span class="sxs-lookup"><span data-stu-id="5e889-114">Total amount of the directory quota.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e889-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e889-115">JSON representation</span></span>

<span data-ttu-id="5e889-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e889-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySizeQuota"
}-->

```json
{
  "used": 123,
  "total": 1234
}
```
