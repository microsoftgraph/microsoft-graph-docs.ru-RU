---
title: Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ce215e0eae3a13aa0c2d27f54338efc57c0c5486
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522843"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="f4340-103">Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="f4340-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="f4340-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f4340-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f4340-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4340-105">Properties</span></span>

| <span data-ttu-id="f4340-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4340-106">Property</span></span>              | <span data-ttu-id="f4340-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f4340-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="f4340-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="f4340-108">reportRefreshDate</span></span>     | <span data-ttu-id="f4340-109">Дата</span><span class="sxs-lookup"><span data-stu-id="f4340-109">Date</span></span>   |
| <span data-ttu-id="f4340-110">поддельное значение</span><span class="sxs-lookup"><span data-stu-id="f4340-110">underLimit</span></span>            | <span data-ttu-id="f4340-111">Int64</span><span class="sxs-lookup"><span data-stu-id="f4340-111">Int64</span></span>  |
| <span data-ttu-id="f4340-112">варнингиссуед</span><span class="sxs-lookup"><span data-stu-id="f4340-112">warningIssued</span></span>         | <span data-ttu-id="f4340-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f4340-113">Int64</span></span>  |
| <span data-ttu-id="f4340-114">сендпрохибитед</span><span class="sxs-lookup"><span data-stu-id="f4340-114">sendProhibited</span></span>        | <span data-ttu-id="f4340-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f4340-115">Int64</span></span>  |
| <span data-ttu-id="f4340-116">сендрецеивепрохибитед</span><span class="sxs-lookup"><span data-stu-id="f4340-116">sendReceiveProhibited</span></span> | <span data-ttu-id="f4340-117">Int64</span><span class="sxs-lookup"><span data-stu-id="f4340-117">Int64</span></span>  |
| <span data-ttu-id="f4340-118">определен</span><span class="sxs-lookup"><span data-stu-id="f4340-118">indeterminate</span></span>         | <span data-ttu-id="f4340-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f4340-119">Int64</span></span>  |
| <span data-ttu-id="f4340-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="f4340-120">reportDate</span></span>            | <span data-ttu-id="f4340-121">Дата</span><span class="sxs-lookup"><span data-stu-id="f4340-121">Date</span></span>   |
| <span data-ttu-id="f4340-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="f4340-122">reportPeriod</span></span>          | <span data-ttu-id="f4340-123">String</span><span class="sxs-lookup"><span data-stu-id="f4340-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f4340-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4340-124">JSON representation</span></span>

<span data-ttu-id="f4340-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4340-125">The following is a JSON representation of the resource.</span></span>

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
