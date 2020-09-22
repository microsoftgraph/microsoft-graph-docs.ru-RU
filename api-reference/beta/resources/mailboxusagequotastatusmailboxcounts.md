---
title: Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e09b9d27da4a85dd89f6a09440d56532045573b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029178"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="5e469-103">Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="5e469-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="5e469-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e469-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="5e469-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e469-105">Properties</span></span>

| <span data-ttu-id="5e469-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e469-106">Property</span></span>              | <span data-ttu-id="5e469-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5e469-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="5e469-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="5e469-108">reportRefreshDate</span></span>     | <span data-ttu-id="5e469-109">Дата</span><span class="sxs-lookup"><span data-stu-id="5e469-109">Date</span></span>   |
| <span data-ttu-id="5e469-110">поддельное значение</span><span class="sxs-lookup"><span data-stu-id="5e469-110">underLimit</span></span>            | <span data-ttu-id="5e469-111">Int64</span><span class="sxs-lookup"><span data-stu-id="5e469-111">Int64</span></span>  |
| <span data-ttu-id="5e469-112">варнингиссуед</span><span class="sxs-lookup"><span data-stu-id="5e469-112">warningIssued</span></span>         | <span data-ttu-id="5e469-113">Int64</span><span class="sxs-lookup"><span data-stu-id="5e469-113">Int64</span></span>  |
| <span data-ttu-id="5e469-114">сендпрохибитед</span><span class="sxs-lookup"><span data-stu-id="5e469-114">sendProhibited</span></span>        | <span data-ttu-id="5e469-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5e469-115">Int64</span></span>  |
| <span data-ttu-id="5e469-116">сендрецеивепрохибитед</span><span class="sxs-lookup"><span data-stu-id="5e469-116">sendReceiveProhibited</span></span> | <span data-ttu-id="5e469-117">Int64</span><span class="sxs-lookup"><span data-stu-id="5e469-117">Int64</span></span>  |
| <span data-ttu-id="5e469-118">определен</span><span class="sxs-lookup"><span data-stu-id="5e469-118">indeterminate</span></span>         | <span data-ttu-id="5e469-119">Int64</span><span class="sxs-lookup"><span data-stu-id="5e469-119">Int64</span></span>  |
| <span data-ttu-id="5e469-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="5e469-120">reportDate</span></span>            | <span data-ttu-id="5e469-121">Дата</span><span class="sxs-lookup"><span data-stu-id="5e469-121">Date</span></span>   |
| <span data-ttu-id="5e469-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="5e469-122">reportPeriod</span></span>          | <span data-ttu-id="5e469-123">String</span><span class="sxs-lookup"><span data-stu-id="5e469-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5e469-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e469-124">JSON representation</span></span>

<span data-ttu-id="5e469-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e469-125">The following is a JSON representation of the resource.</span></span>

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


