---
title: Тип ресурса yammerActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575830"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="21ef6-103">Тип ресурса yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="21ef6-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="21ef6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="21ef6-104">Properties</span></span>

| <span data-ttu-id="21ef6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="21ef6-105">Property</span></span>          | <span data-ttu-id="21ef6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="21ef6-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="21ef6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="21ef6-107">reportRefreshDate</span></span> | <span data-ttu-id="21ef6-108">Date</span><span class="sxs-lookup"><span data-stu-id="21ef6-108">Date</span></span>              |
| <span data-ttu-id="21ef6-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21ef6-109">userPrincipalName</span></span> | <span data-ttu-id="21ef6-110">Строка</span><span class="sxs-lookup"><span data-stu-id="21ef6-110">String</span></span>            |
| <span data-ttu-id="21ef6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="21ef6-111">displayName</span></span>       | <span data-ttu-id="21ef6-112">Строка</span><span class="sxs-lookup"><span data-stu-id="21ef6-112">String</span></span>            |
| <span data-ttu-id="21ef6-113">userState</span><span class="sxs-lookup"><span data-stu-id="21ef6-113">userState</span></span>         | <span data-ttu-id="21ef6-114">Строка</span><span class="sxs-lookup"><span data-stu-id="21ef6-114">String</span></span>            |
| <span data-ttu-id="21ef6-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="21ef6-115">stateChangeDate</span></span>   | <span data-ttu-id="21ef6-116">Date</span><span class="sxs-lookup"><span data-stu-id="21ef6-116">Date</span></span>              |
| <span data-ttu-id="21ef6-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="21ef6-117">lastActivityDate</span></span>  | <span data-ttu-id="21ef6-118">Date</span><span class="sxs-lookup"><span data-stu-id="21ef6-118">Date</span></span>              |
| <span data-ttu-id="21ef6-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="21ef6-119">postedCount</span></span>       | <span data-ttu-id="21ef6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="21ef6-120">Int64</span></span>             |
| <span data-ttu-id="21ef6-121">readCount</span><span class="sxs-lookup"><span data-stu-id="21ef6-121">readCount</span></span>         | <span data-ttu-id="21ef6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="21ef6-122">Int64</span></span>             |
| <span data-ttu-id="21ef6-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="21ef6-123">likedCount</span></span>        | <span data-ttu-id="21ef6-124">Int64</span><span class="sxs-lookup"><span data-stu-id="21ef6-124">Int64</span></span>             |
| <span data-ttu-id="21ef6-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="21ef6-125">assignedProducts</span></span>  | <span data-ttu-id="21ef6-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="21ef6-126">String collection</span></span> |
| <span data-ttu-id="21ef6-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="21ef6-127">reportPeriod</span></span>      | <span data-ttu-id="21ef6-128">String</span><span class="sxs-lookup"><span data-stu-id="21ef6-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="21ef6-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21ef6-129">JSON representation</span></span>

<span data-ttu-id="21ef6-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21ef6-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
