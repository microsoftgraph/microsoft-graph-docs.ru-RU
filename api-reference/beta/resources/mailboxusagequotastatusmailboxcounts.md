---
title: Тип ресурса mailboxUsageQuotaStatusMailboxCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: ac6c597cad9d28f985da97d6f55a5726ebbf491e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077708"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="318ab-103">Тип ресурса mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="318ab-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="318ab-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="318ab-104">Properties</span></span>

| <span data-ttu-id="318ab-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="318ab-105">Property</span></span>              | <span data-ttu-id="318ab-106">Тип</span><span class="sxs-lookup"><span data-stu-id="318ab-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="318ab-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="318ab-107">reportRefreshDate</span></span>     | <span data-ttu-id="318ab-108">Date</span><span class="sxs-lookup"><span data-stu-id="318ab-108">Date</span></span>   |
| <span data-ttu-id="318ab-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="318ab-109">underLimit</span></span>            | <span data-ttu-id="318ab-110">Int64</span><span class="sxs-lookup"><span data-stu-id="318ab-110">Int64</span></span>  |
| <span data-ttu-id="318ab-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="318ab-111">warningIssued</span></span>         | <span data-ttu-id="318ab-112">Int64</span><span class="sxs-lookup"><span data-stu-id="318ab-112">Int64</span></span>  |
| <span data-ttu-id="318ab-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="318ab-113">sendProhibited</span></span>        | <span data-ttu-id="318ab-114">Int64</span><span class="sxs-lookup"><span data-stu-id="318ab-114">Int64</span></span>  |
| <span data-ttu-id="318ab-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="318ab-115">sendReceiveProhibited</span></span> | <span data-ttu-id="318ab-116">Int64</span><span class="sxs-lookup"><span data-stu-id="318ab-116">Int64</span></span>  |
| <span data-ttu-id="318ab-117">неопределенное</span><span class="sxs-lookup"><span data-stu-id="318ab-117">indeterminate</span></span>         | <span data-ttu-id="318ab-118">Int64</span><span class="sxs-lookup"><span data-stu-id="318ab-118">Int64</span></span>  |
| <span data-ttu-id="318ab-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="318ab-119">reportDate</span></span>            | <span data-ttu-id="318ab-120">Date</span><span class="sxs-lookup"><span data-stu-id="318ab-120">Date</span></span>   |
| <span data-ttu-id="318ab-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="318ab-121">reportPeriod</span></span>          | <span data-ttu-id="318ab-122">String</span><span class="sxs-lookup"><span data-stu-id="318ab-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="318ab-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="318ab-123">JSON representation</span></span>

<span data-ttu-id="318ab-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="318ab-124">The following is a JSON representation of the resource.</span></span>

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
