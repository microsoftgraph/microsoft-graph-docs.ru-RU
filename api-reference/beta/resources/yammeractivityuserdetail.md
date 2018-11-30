---
title: Тип ресурса yammerActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: a1ca33efe8327b1c1e52de25714df9c0bd45ee05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080800"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="ee106-103">Тип ресурса yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ee106-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ee106-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee106-104">Properties</span></span>

| <span data-ttu-id="ee106-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee106-105">Property</span></span>          | <span data-ttu-id="ee106-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ee106-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="ee106-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ee106-107">reportRefreshDate</span></span> | <span data-ttu-id="ee106-108">Date</span><span class="sxs-lookup"><span data-stu-id="ee106-108">Date</span></span>              |
| <span data-ttu-id="ee106-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee106-109">userPrincipalName</span></span> | <span data-ttu-id="ee106-110">String</span><span class="sxs-lookup"><span data-stu-id="ee106-110">String</span></span>            |
| <span data-ttu-id="ee106-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ee106-111">displayName</span></span>       | <span data-ttu-id="ee106-112">String</span><span class="sxs-lookup"><span data-stu-id="ee106-112">String</span></span>            |
| <span data-ttu-id="ee106-113">userState</span><span class="sxs-lookup"><span data-stu-id="ee106-113">userState</span></span>         | <span data-ttu-id="ee106-114">String</span><span class="sxs-lookup"><span data-stu-id="ee106-114">String</span></span>            |
| <span data-ttu-id="ee106-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="ee106-115">stateChangeDate</span></span>   | <span data-ttu-id="ee106-116">Date</span><span class="sxs-lookup"><span data-stu-id="ee106-116">Date</span></span>              |
| <span data-ttu-id="ee106-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ee106-117">lastActivityDate</span></span>  | <span data-ttu-id="ee106-118">Date</span><span class="sxs-lookup"><span data-stu-id="ee106-118">Date</span></span>              |
| <span data-ttu-id="ee106-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="ee106-119">postedCount</span></span>       | <span data-ttu-id="ee106-120">Int64</span><span class="sxs-lookup"><span data-stu-id="ee106-120">Int64</span></span>             |
| <span data-ttu-id="ee106-121">readCount</span><span class="sxs-lookup"><span data-stu-id="ee106-121">readCount</span></span>         | <span data-ttu-id="ee106-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ee106-122">Int64</span></span>             |
| <span data-ttu-id="ee106-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="ee106-123">likedCount</span></span>        | <span data-ttu-id="ee106-124">Int64</span><span class="sxs-lookup"><span data-stu-id="ee106-124">Int64</span></span>             |
| <span data-ttu-id="ee106-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="ee106-125">assignedProducts</span></span>  | <span data-ttu-id="ee106-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ee106-126">String collection</span></span> |
| <span data-ttu-id="ee106-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ee106-127">reportPeriod</span></span>      | <span data-ttu-id="ee106-128">String</span><span class="sxs-lookup"><span data-stu-id="ee106-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="ee106-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee106-129">JSON representation</span></span>

<span data-ttu-id="ee106-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee106-130">The following is a JSON representation of the resource.</span></span>

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
