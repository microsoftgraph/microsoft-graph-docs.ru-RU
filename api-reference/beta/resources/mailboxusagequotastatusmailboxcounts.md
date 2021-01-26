---
title: Тип ресурса mailboxUsageQuotaStatusMailboxCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 10ce05121ec900f5475a082191f4192974f980b4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983547"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="d8245-103">Тип ресурса mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="d8245-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="d8245-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8245-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d8245-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8245-105">Properties</span></span>

| <span data-ttu-id="d8245-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8245-106">Property</span></span>              | <span data-ttu-id="d8245-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d8245-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="d8245-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d8245-108">reportRefreshDate</span></span>     | <span data-ttu-id="d8245-109">Дата</span><span class="sxs-lookup"><span data-stu-id="d8245-109">Date</span></span>   |
| <span data-ttu-id="d8245-110">underLimit</span><span class="sxs-lookup"><span data-stu-id="d8245-110">underLimit</span></span>            | <span data-ttu-id="d8245-111">Int64</span><span class="sxs-lookup"><span data-stu-id="d8245-111">Int64</span></span>  |
| <span data-ttu-id="d8245-112">warningIssued</span><span class="sxs-lookup"><span data-stu-id="d8245-112">warningIssued</span></span>         | <span data-ttu-id="d8245-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d8245-113">Int64</span></span>  |
| <span data-ttu-id="d8245-114">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="d8245-114">sendProhibited</span></span>        | <span data-ttu-id="d8245-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d8245-115">Int64</span></span>  |
| <span data-ttu-id="d8245-116">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="d8245-116">sendReceiveProhibited</span></span> | <span data-ttu-id="d8245-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d8245-117">Int64</span></span>  |
| <span data-ttu-id="d8245-118">indeterminate</span><span class="sxs-lookup"><span data-stu-id="d8245-118">indeterminate</span></span>         | <span data-ttu-id="d8245-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d8245-119">Int64</span></span>  |
| <span data-ttu-id="d8245-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="d8245-120">reportDate</span></span>            | <span data-ttu-id="d8245-121">Дата</span><span class="sxs-lookup"><span data-stu-id="d8245-121">Date</span></span>   |
| <span data-ttu-id="d8245-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d8245-122">reportPeriod</span></span>          | <span data-ttu-id="d8245-123">String</span><span class="sxs-lookup"><span data-stu-id="d8245-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8245-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8245-124">JSON representation</span></span>

<span data-ttu-id="d8245-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8245-125">The following is a JSON representation of the resource.</span></span>

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


