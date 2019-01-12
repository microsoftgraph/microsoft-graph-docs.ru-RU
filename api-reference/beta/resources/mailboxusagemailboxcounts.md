---
title: Тип ресурса mailboxUsageMailboxCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e9da6a72c3c2d79323041e683702a7af2e4699c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941312"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="4ef52-103">Тип ресурса mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="4ef52-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4ef52-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ef52-104">Properties</span></span>

| <span data-ttu-id="4ef52-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ef52-105">Property</span></span>          | <span data-ttu-id="4ef52-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4ef52-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4ef52-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4ef52-107">reportRefreshDate</span></span> | <span data-ttu-id="4ef52-108">Date</span><span class="sxs-lookup"><span data-stu-id="4ef52-108">Date</span></span>   |
| <span data-ttu-id="4ef52-109">total</span><span class="sxs-lookup"><span data-stu-id="4ef52-109">total</span></span>             | <span data-ttu-id="4ef52-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4ef52-110">Int64</span></span>  |
| <span data-ttu-id="4ef52-111">активных</span><span class="sxs-lookup"><span data-stu-id="4ef52-111">active</span></span>            | <span data-ttu-id="4ef52-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4ef52-112">Int64</span></span>  |
| <span data-ttu-id="4ef52-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="4ef52-113">reportDate</span></span>        | <span data-ttu-id="4ef52-114">Date</span><span class="sxs-lookup"><span data-stu-id="4ef52-114">Date</span></span>   |
| <span data-ttu-id="4ef52-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4ef52-115">reportPeriod</span></span>      | <span data-ttu-id="4ef52-116">String</span><span class="sxs-lookup"><span data-stu-id="4ef52-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4ef52-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ef52-117">JSON representation</span></span>

<span data-ttu-id="4ef52-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ef52-118">The following is a JSON representation of the resource.</span></span>

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
