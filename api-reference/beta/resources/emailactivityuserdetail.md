---
title: Тип ресурса emailActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938309"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="6d119-103">Тип ресурса emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="6d119-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6d119-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d119-104">Properties</span></span>

| <span data-ttu-id="6d119-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d119-105">Property</span></span>          | <span data-ttu-id="6d119-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6d119-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="6d119-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6d119-107">reportRefreshDate</span></span> | <span data-ttu-id="6d119-108">Date</span><span class="sxs-lookup"><span data-stu-id="6d119-108">Date</span></span>              |
| <span data-ttu-id="6d119-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6d119-109">userPrincipalName</span></span> | <span data-ttu-id="6d119-110">Строка</span><span class="sxs-lookup"><span data-stu-id="6d119-110">String</span></span>            |
| <span data-ttu-id="6d119-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6d119-111">displayName</span></span>       | <span data-ttu-id="6d119-112">Строка</span><span class="sxs-lookup"><span data-stu-id="6d119-112">String</span></span>            |
| <span data-ttu-id="6d119-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6d119-113">isDeleted</span></span>         | <span data-ttu-id="6d119-114">Логический</span><span class="sxs-lookup"><span data-stu-id="6d119-114">Boolean</span></span>           |
| <span data-ttu-id="6d119-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="6d119-115">deletedDate</span></span>       | <span data-ttu-id="6d119-116">Date</span><span class="sxs-lookup"><span data-stu-id="6d119-116">Date</span></span>              |
| <span data-ttu-id="6d119-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6d119-117">lastActivityDate</span></span>  | <span data-ttu-id="6d119-118">Date</span><span class="sxs-lookup"><span data-stu-id="6d119-118">Date</span></span>              |
| <span data-ttu-id="6d119-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="6d119-119">sendCount</span></span>         | <span data-ttu-id="6d119-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6d119-120">Int64</span></span>             |
| <span data-ttu-id="6d119-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="6d119-121">receiveCount</span></span>      | <span data-ttu-id="6d119-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6d119-122">Int64</span></span>             |
| <span data-ttu-id="6d119-123">readCount</span><span class="sxs-lookup"><span data-stu-id="6d119-123">readCount</span></span>         | <span data-ttu-id="6d119-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6d119-124">Int64</span></span>             |
| <span data-ttu-id="6d119-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="6d119-125">assignedProducts</span></span>  | <span data-ttu-id="6d119-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6d119-126">String collection</span></span> |
| <span data-ttu-id="6d119-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6d119-127">reportPeriod</span></span>      | <span data-ttu-id="6d119-128">String</span><span class="sxs-lookup"><span data-stu-id="6d119-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="6d119-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d119-129">JSON representation</span></span>

<span data-ttu-id="6d119-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d119-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
