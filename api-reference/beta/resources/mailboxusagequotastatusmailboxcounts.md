---
title: Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457132"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="d81d8-103">Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="d81d8-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d81d8-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d81d8-104">Properties</span></span>

| <span data-ttu-id="d81d8-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d81d8-105">Property</span></span>              | <span data-ttu-id="d81d8-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d81d8-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="d81d8-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="d81d8-107">reportRefreshDate</span></span>     | <span data-ttu-id="d81d8-108">Дата</span><span class="sxs-lookup"><span data-stu-id="d81d8-108">Date</span></span>   |
| <span data-ttu-id="d81d8-109">подДельное значение</span><span class="sxs-lookup"><span data-stu-id="d81d8-109">underLimit</span></span>            | <span data-ttu-id="d81d8-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d81d8-110">Int64</span></span>  |
| <span data-ttu-id="d81d8-111">Варнингиссуед</span><span class="sxs-lookup"><span data-stu-id="d81d8-111">warningIssued</span></span>         | <span data-ttu-id="d81d8-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d81d8-112">Int64</span></span>  |
| <span data-ttu-id="d81d8-113">Сендпрохибитед</span><span class="sxs-lookup"><span data-stu-id="d81d8-113">sendProhibited</span></span>        | <span data-ttu-id="d81d8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d81d8-114">Int64</span></span>  |
| <span data-ttu-id="d81d8-115">Сендрецеивепрохибитед</span><span class="sxs-lookup"><span data-stu-id="d81d8-115">sendReceiveProhibited</span></span> | <span data-ttu-id="d81d8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d81d8-116">Int64</span></span>  |
| <span data-ttu-id="d81d8-117">определен</span><span class="sxs-lookup"><span data-stu-id="d81d8-117">indeterminate</span></span>         | <span data-ttu-id="d81d8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d81d8-118">Int64</span></span>  |
| <span data-ttu-id="d81d8-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="d81d8-119">reportDate</span></span>            | <span data-ttu-id="d81d8-120">Дата</span><span class="sxs-lookup"><span data-stu-id="d81d8-120">Date</span></span>   |
| <span data-ttu-id="d81d8-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="d81d8-121">reportPeriod</span></span>          | <span data-ttu-id="d81d8-122">Строка</span><span class="sxs-lookup"><span data-stu-id="d81d8-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d81d8-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d81d8-123">JSON representation</span></span>

<span data-ttu-id="d81d8-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d81d8-124">The following is a JSON representation of the resource.</span></span>

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
