---
title: Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1e8fafe9a3cdce4519cf5755337b016fa587cd06
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966904"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="7d91a-103">Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="7d91a-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7d91a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d91a-104">Properties</span></span>

| <span data-ttu-id="7d91a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d91a-105">Property</span></span>              | <span data-ttu-id="7d91a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7d91a-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="7d91a-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="7d91a-107">reportRefreshDate</span></span>     | <span data-ttu-id="7d91a-108">Дата</span><span class="sxs-lookup"><span data-stu-id="7d91a-108">Date</span></span>   |
| <span data-ttu-id="7d91a-109">поддельное значение</span><span class="sxs-lookup"><span data-stu-id="7d91a-109">underLimit</span></span>            | <span data-ttu-id="7d91a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7d91a-110">Int64</span></span>  |
| <span data-ttu-id="7d91a-111">Варнингиссуед</span><span class="sxs-lookup"><span data-stu-id="7d91a-111">warningIssued</span></span>         | <span data-ttu-id="7d91a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7d91a-112">Int64</span></span>  |
| <span data-ttu-id="7d91a-113">Сендпрохибитед</span><span class="sxs-lookup"><span data-stu-id="7d91a-113">sendProhibited</span></span>        | <span data-ttu-id="7d91a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7d91a-114">Int64</span></span>  |
| <span data-ttu-id="7d91a-115">Сендрецеивепрохибитед</span><span class="sxs-lookup"><span data-stu-id="7d91a-115">sendReceiveProhibited</span></span> | <span data-ttu-id="7d91a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7d91a-116">Int64</span></span>  |
| <span data-ttu-id="7d91a-117">определен</span><span class="sxs-lookup"><span data-stu-id="7d91a-117">indeterminate</span></span>         | <span data-ttu-id="7d91a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="7d91a-118">Int64</span></span>  |
| <span data-ttu-id="7d91a-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="7d91a-119">reportDate</span></span>            | <span data-ttu-id="7d91a-120">Дата</span><span class="sxs-lookup"><span data-stu-id="7d91a-120">Date</span></span>   |
| <span data-ttu-id="7d91a-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="7d91a-121">reportPeriod</span></span>          | <span data-ttu-id="7d91a-122">String</span><span class="sxs-lookup"><span data-stu-id="7d91a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7d91a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d91a-123">JSON representation</span></span>

<span data-ttu-id="7d91a-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d91a-124">The following is a JSON representation of the resource.</span></span>

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
