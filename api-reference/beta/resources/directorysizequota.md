---
title: Тип ресурса directorySizeQuota
description: Представляет используемую компанию и общую квоту каталога.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: davidmu1
ms.openlocfilehash: 3af82a957e152f0edf4d87e6fdf9a7888d4b64e4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133989"
---
# <a name="directorysizequota-resource-type"></a><span data-ttu-id="990c6-103">Тип ресурса directorySizeQuota</span><span class="sxs-lookup"><span data-stu-id="990c6-103">directorySizeQuota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="990c6-104">Представляет используемую компанию и общую квоту каталога.</span><span class="sxs-lookup"><span data-stu-id="990c6-104">Represents a company's used and total directory quota.</span></span>

## <a name="properties"></a><span data-ttu-id="990c6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="990c6-105">Properties</span></span>
| <span data-ttu-id="990c6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="990c6-106">Property</span></span>   | <span data-ttu-id="990c6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="990c6-107">Type</span></span>|<span data-ttu-id="990c6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="990c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="990c6-109">used</span><span class="sxs-lookup"><span data-stu-id="990c6-109">used</span></span>|<span data-ttu-id="990c6-110">Int32</span><span class="sxs-lookup"><span data-stu-id="990c6-110">Int32</span></span>| <span data-ttu-id="990c6-111">Использованная сумма квоты каталога.</span><span class="sxs-lookup"><span data-stu-id="990c6-111">Used amount of the directory quota.</span></span> |
|<span data-ttu-id="990c6-112">total</span><span class="sxs-lookup"><span data-stu-id="990c6-112">total</span></span>|<span data-ttu-id="990c6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="990c6-113">Int32</span></span>| <span data-ttu-id="990c6-114">Общая сумма квоты каталога.</span><span class="sxs-lookup"><span data-stu-id="990c6-114">Total amount of the directory quota.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="990c6-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="990c6-115">JSON representation</span></span>

<span data-ttu-id="990c6-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="990c6-116">The following is a JSON representation of the resource.</span></span>

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
