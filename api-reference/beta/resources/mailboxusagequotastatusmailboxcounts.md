---
title: Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1ebbfe0f134848d78e9c42a159c1c56bdbd21b39
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473427"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="ec96b-103">Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="ec96b-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="ec96b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec96b-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="ec96b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec96b-105">Properties</span></span>

| <span data-ttu-id="ec96b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec96b-106">Property</span></span>              | <span data-ttu-id="ec96b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ec96b-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="ec96b-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="ec96b-108">reportRefreshDate</span></span>     | <span data-ttu-id="ec96b-109">Дата</span><span class="sxs-lookup"><span data-stu-id="ec96b-109">Date</span></span>   |
| <span data-ttu-id="ec96b-110">поддельное значение</span><span class="sxs-lookup"><span data-stu-id="ec96b-110">underLimit</span></span>            | <span data-ttu-id="ec96b-111">Int64</span><span class="sxs-lookup"><span data-stu-id="ec96b-111">Int64</span></span>  |
| <span data-ttu-id="ec96b-112">варнингиссуед</span><span class="sxs-lookup"><span data-stu-id="ec96b-112">warningIssued</span></span>         | <span data-ttu-id="ec96b-113">Int64</span><span class="sxs-lookup"><span data-stu-id="ec96b-113">Int64</span></span>  |
| <span data-ttu-id="ec96b-114">сендпрохибитед</span><span class="sxs-lookup"><span data-stu-id="ec96b-114">sendProhibited</span></span>        | <span data-ttu-id="ec96b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ec96b-115">Int64</span></span>  |
| <span data-ttu-id="ec96b-116">сендрецеивепрохибитед</span><span class="sxs-lookup"><span data-stu-id="ec96b-116">sendReceiveProhibited</span></span> | <span data-ttu-id="ec96b-117">Int64</span><span class="sxs-lookup"><span data-stu-id="ec96b-117">Int64</span></span>  |
| <span data-ttu-id="ec96b-118">определен</span><span class="sxs-lookup"><span data-stu-id="ec96b-118">indeterminate</span></span>         | <span data-ttu-id="ec96b-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ec96b-119">Int64</span></span>  |
| <span data-ttu-id="ec96b-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="ec96b-120">reportDate</span></span>            | <span data-ttu-id="ec96b-121">Дата</span><span class="sxs-lookup"><span data-stu-id="ec96b-121">Date</span></span>   |
| <span data-ttu-id="ec96b-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="ec96b-122">reportPeriod</span></span>          | <span data-ttu-id="ec96b-123">String</span><span class="sxs-lookup"><span data-stu-id="ec96b-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ec96b-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec96b-124">JSON representation</span></span>

<span data-ttu-id="ec96b-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec96b-125">The following is a JSON representation of the resource.</span></span>

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
