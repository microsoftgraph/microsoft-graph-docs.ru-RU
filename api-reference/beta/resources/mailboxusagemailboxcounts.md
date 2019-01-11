---
title: Тип ресурса mailboxUsageMailboxCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 4e18993590d6de893b78db511037eb28ec1cc0cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814814"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="feeb3-103">Тип ресурса mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="feeb3-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="feeb3-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="feeb3-104">Properties</span></span>

| <span data-ttu-id="feeb3-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="feeb3-105">Property</span></span>          | <span data-ttu-id="feeb3-106">Тип</span><span class="sxs-lookup"><span data-stu-id="feeb3-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="feeb3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="feeb3-107">reportRefreshDate</span></span> | <span data-ttu-id="feeb3-108">Date</span><span class="sxs-lookup"><span data-stu-id="feeb3-108">Date</span></span>   |
| <span data-ttu-id="feeb3-109">total</span><span class="sxs-lookup"><span data-stu-id="feeb3-109">total</span></span>             | <span data-ttu-id="feeb3-110">Int64</span><span class="sxs-lookup"><span data-stu-id="feeb3-110">Int64</span></span>  |
| <span data-ttu-id="feeb3-111">активных</span><span class="sxs-lookup"><span data-stu-id="feeb3-111">active</span></span>            | <span data-ttu-id="feeb3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="feeb3-112">Int64</span></span>  |
| <span data-ttu-id="feeb3-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="feeb3-113">reportDate</span></span>        | <span data-ttu-id="feeb3-114">Date</span><span class="sxs-lookup"><span data-stu-id="feeb3-114">Date</span></span>   |
| <span data-ttu-id="feeb3-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="feeb3-115">reportPeriod</span></span>      | <span data-ttu-id="feeb3-116">String</span><span class="sxs-lookup"><span data-stu-id="feeb3-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="feeb3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="feeb3-117">JSON representation</span></span>

<span data-ttu-id="feeb3-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="feeb3-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
