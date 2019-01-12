---
title: Тип ресурса mailboxUsageQuotaStatusMailboxCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921236"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="db0a8-103">Тип ресурса mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="db0a8-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="db0a8-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="db0a8-104">Properties</span></span>

| <span data-ttu-id="db0a8-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="db0a8-105">Property</span></span>              | <span data-ttu-id="db0a8-106">Тип</span><span class="sxs-lookup"><span data-stu-id="db0a8-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="db0a8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="db0a8-107">reportRefreshDate</span></span>     | <span data-ttu-id="db0a8-108">Date</span><span class="sxs-lookup"><span data-stu-id="db0a8-108">Date</span></span>   |
| <span data-ttu-id="db0a8-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="db0a8-109">underLimit</span></span>            | <span data-ttu-id="db0a8-110">Int64</span><span class="sxs-lookup"><span data-stu-id="db0a8-110">Int64</span></span>  |
| <span data-ttu-id="db0a8-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="db0a8-111">warningIssued</span></span>         | <span data-ttu-id="db0a8-112">Int64</span><span class="sxs-lookup"><span data-stu-id="db0a8-112">Int64</span></span>  |
| <span data-ttu-id="db0a8-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="db0a8-113">sendProhibited</span></span>        | <span data-ttu-id="db0a8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="db0a8-114">Int64</span></span>  |
| <span data-ttu-id="db0a8-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="db0a8-115">sendReceiveProhibited</span></span> | <span data-ttu-id="db0a8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="db0a8-116">Int64</span></span>  |
| <span data-ttu-id="db0a8-117">неопределенное</span><span class="sxs-lookup"><span data-stu-id="db0a8-117">indeterminate</span></span>         | <span data-ttu-id="db0a8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="db0a8-118">Int64</span></span>  |
| <span data-ttu-id="db0a8-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="db0a8-119">reportDate</span></span>            | <span data-ttu-id="db0a8-120">Date</span><span class="sxs-lookup"><span data-stu-id="db0a8-120">Date</span></span>   |
| <span data-ttu-id="db0a8-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="db0a8-121">reportPeriod</span></span>          | <span data-ttu-id="db0a8-122">String</span><span class="sxs-lookup"><span data-stu-id="db0a8-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="db0a8-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db0a8-123">JSON representation</span></span>

<span data-ttu-id="db0a8-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db0a8-124">The following is a JSON representation of the resource.</span></span>

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
