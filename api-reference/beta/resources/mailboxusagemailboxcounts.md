---
title: Тип ресурса mailboxUsageMailboxCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 8f5b5080255a12c474cb8ab5c078c4f991089c31
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081807"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="b8aae-103">Тип ресурса mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="b8aae-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b8aae-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8aae-104">Properties</span></span>

| <span data-ttu-id="b8aae-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8aae-105">Property</span></span>          | <span data-ttu-id="b8aae-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b8aae-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b8aae-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b8aae-107">reportRefreshDate</span></span> | <span data-ttu-id="b8aae-108">Date</span><span class="sxs-lookup"><span data-stu-id="b8aae-108">Date</span></span>   |
| <span data-ttu-id="b8aae-109">total</span><span class="sxs-lookup"><span data-stu-id="b8aae-109">total</span></span>             | <span data-ttu-id="b8aae-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b8aae-110">Int64</span></span>  |
| <span data-ttu-id="b8aae-111">активных</span><span class="sxs-lookup"><span data-stu-id="b8aae-111">active</span></span>            | <span data-ttu-id="b8aae-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b8aae-112">Int64</span></span>  |
| <span data-ttu-id="b8aae-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="b8aae-113">reportDate</span></span>        | <span data-ttu-id="b8aae-114">Date</span><span class="sxs-lookup"><span data-stu-id="b8aae-114">Date</span></span>   |
| <span data-ttu-id="b8aae-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b8aae-115">reportPeriod</span></span>      | <span data-ttu-id="b8aae-116">String</span><span class="sxs-lookup"><span data-stu-id="b8aae-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b8aae-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8aae-117">JSON representation</span></span>

<span data-ttu-id="b8aae-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8aae-118">The following is a JSON representation of the resource.</span></span>

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
