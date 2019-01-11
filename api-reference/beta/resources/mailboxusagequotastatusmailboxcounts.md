---
title: Тип ресурса mailboxUsageQuotaStatusMailboxCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: b87bb1ce91626f9151d294e2243bba72ba72346b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835225"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="87b04-103">Тип ресурса mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="87b04-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="87b04-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="87b04-104">Properties</span></span>

| <span data-ttu-id="87b04-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="87b04-105">Property</span></span>              | <span data-ttu-id="87b04-106">Тип</span><span class="sxs-lookup"><span data-stu-id="87b04-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="87b04-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="87b04-107">reportRefreshDate</span></span>     | <span data-ttu-id="87b04-108">Date</span><span class="sxs-lookup"><span data-stu-id="87b04-108">Date</span></span>   |
| <span data-ttu-id="87b04-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="87b04-109">underLimit</span></span>            | <span data-ttu-id="87b04-110">Int64</span><span class="sxs-lookup"><span data-stu-id="87b04-110">Int64</span></span>  |
| <span data-ttu-id="87b04-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="87b04-111">warningIssued</span></span>         | <span data-ttu-id="87b04-112">Int64</span><span class="sxs-lookup"><span data-stu-id="87b04-112">Int64</span></span>  |
| <span data-ttu-id="87b04-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="87b04-113">sendProhibited</span></span>        | <span data-ttu-id="87b04-114">Int64</span><span class="sxs-lookup"><span data-stu-id="87b04-114">Int64</span></span>  |
| <span data-ttu-id="87b04-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="87b04-115">sendReceiveProhibited</span></span> | <span data-ttu-id="87b04-116">Int64</span><span class="sxs-lookup"><span data-stu-id="87b04-116">Int64</span></span>  |
| <span data-ttu-id="87b04-117">неопределенное</span><span class="sxs-lookup"><span data-stu-id="87b04-117">indeterminate</span></span>         | <span data-ttu-id="87b04-118">Int64</span><span class="sxs-lookup"><span data-stu-id="87b04-118">Int64</span></span>  |
| <span data-ttu-id="87b04-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="87b04-119">reportDate</span></span>            | <span data-ttu-id="87b04-120">Date</span><span class="sxs-lookup"><span data-stu-id="87b04-120">Date</span></span>   |
| <span data-ttu-id="87b04-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="87b04-121">reportPeriod</span></span>          | <span data-ttu-id="87b04-122">String</span><span class="sxs-lookup"><span data-stu-id="87b04-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87b04-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87b04-123">JSON representation</span></span>

<span data-ttu-id="87b04-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87b04-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "underLimit": 1024, 
  "warningIssued": 1024, 
  "sendProhibited": 1024, 
  "sendReceiveProhibited": 1024, 
  "indeterminate": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
