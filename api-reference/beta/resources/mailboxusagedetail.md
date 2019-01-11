---
title: Тип ресурса mailboxUsageDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 25cb41e38138a677bfc6636b035003bb8fc5858c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818013"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="6b541-103">Тип ресурса mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="6b541-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6b541-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b541-104">Properties</span></span>

| <span data-ttu-id="6b541-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b541-105">Property</span></span>                        | <span data-ttu-id="6b541-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6b541-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="6b541-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6b541-107">reportRefreshDate</span></span>               | <span data-ttu-id="6b541-108">Date</span><span class="sxs-lookup"><span data-stu-id="6b541-108">Date</span></span>    |
| <span data-ttu-id="6b541-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6b541-109">userPrincipalName</span></span>               | <span data-ttu-id="6b541-110">Строка</span><span class="sxs-lookup"><span data-stu-id="6b541-110">String</span></span>  |
| <span data-ttu-id="6b541-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6b541-111">displayName</span></span>                     | <span data-ttu-id="6b541-112">Строка</span><span class="sxs-lookup"><span data-stu-id="6b541-112">String</span></span>  |
| <span data-ttu-id="6b541-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6b541-113">isDeleted</span></span>                       | <span data-ttu-id="6b541-114">Логический</span><span class="sxs-lookup"><span data-stu-id="6b541-114">Boolean</span></span> |
| <span data-ttu-id="6b541-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="6b541-115">deletedDate</span></span>                     | <span data-ttu-id="6b541-116">Date</span><span class="sxs-lookup"><span data-stu-id="6b541-116">Date</span></span>    |
| <span data-ttu-id="6b541-117">Дата создания</span><span class="sxs-lookup"><span data-stu-id="6b541-117">createdDate</span></span>                     | <span data-ttu-id="6b541-118">Date</span><span class="sxs-lookup"><span data-stu-id="6b541-118">Date</span></span>    |
| <span data-ttu-id="6b541-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6b541-119">lastActivityDate</span></span>                | <span data-ttu-id="6b541-120">Date</span><span class="sxs-lookup"><span data-stu-id="6b541-120">Date</span></span>    |
| <span data-ttu-id="6b541-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="6b541-121">itemCount</span></span>                       | <span data-ttu-id="6b541-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6b541-122">Int64</span></span>   |
| <span data-ttu-id="6b541-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="6b541-123">storageUsedInBytes</span></span>              | <span data-ttu-id="6b541-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6b541-124">Int64</span></span>   |
| <span data-ttu-id="6b541-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="6b541-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="6b541-126">Int64</span><span class="sxs-lookup"><span data-stu-id="6b541-126">Int64</span></span>   |
| <span data-ttu-id="6b541-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="6b541-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="6b541-128">Int64</span><span class="sxs-lookup"><span data-stu-id="6b541-128">Int64</span></span>   |
| <span data-ttu-id="6b541-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="6b541-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="6b541-130">Int64</span><span class="sxs-lookup"><span data-stu-id="6b541-130">Int64</span></span>   |
| <span data-ttu-id="6b541-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6b541-131">reportPeriod</span></span>                    | <span data-ttu-id="6b541-132">String</span><span class="sxs-lookup"><span data-stu-id="6b541-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6b541-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b541-133">JSON representation</span></span>

<span data-ttu-id="6b541-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b541-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
