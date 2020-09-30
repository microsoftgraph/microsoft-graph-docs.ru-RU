---
title: Тип ресурса Директорисизекуота
description: Представляет используемую компанией общую квоту каталога.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 8f5f172cb8f090b71b7e0fd3c89151668c167afd
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315603"
---
# <a name="directorysizequota-resource-type"></a><span data-ttu-id="f5ac1-103">Тип ресурса Директорисизекуота</span><span class="sxs-lookup"><span data-stu-id="f5ac1-103">directorySizeQuota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5ac1-104">Представляет используемую компанией общую квоту каталога.</span><span class="sxs-lookup"><span data-stu-id="f5ac1-104">Represents a company's used and total directory quota.</span></span>

## <a name="properties"></a><span data-ttu-id="f5ac1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5ac1-105">Properties</span></span>
| <span data-ttu-id="f5ac1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5ac1-106">Property</span></span>   | <span data-ttu-id="f5ac1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f5ac1-107">Type</span></span>|<span data-ttu-id="f5ac1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f5ac1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5ac1-109">used</span><span class="sxs-lookup"><span data-stu-id="f5ac1-109">used</span></span>|<span data-ttu-id="f5ac1-110">Int32</span><span class="sxs-lookup"><span data-stu-id="f5ac1-110">Int32</span></span>| <span data-ttu-id="f5ac1-111">Использованная сумма квоты каталога.</span><span class="sxs-lookup"><span data-stu-id="f5ac1-111">Used amount of the directory quota.</span></span> |
|<span data-ttu-id="f5ac1-112">total</span><span class="sxs-lookup"><span data-stu-id="f5ac1-112">total</span></span>|<span data-ttu-id="f5ac1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f5ac1-113">Int32</span></span>| <span data-ttu-id="f5ac1-114">Общая сумма квоты каталога.</span><span class="sxs-lookup"><span data-stu-id="f5ac1-114">Total amount of the directory quota.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5ac1-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5ac1-115">JSON representation</span></span>

<span data-ttu-id="f5ac1-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5ac1-116">The following is a JSON representation of the resource.</span></span>

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
