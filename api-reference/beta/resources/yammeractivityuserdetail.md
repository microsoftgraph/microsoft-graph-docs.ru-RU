---
title: Тип ресурса yammerActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: d7869869466dc785b92db23f8b574eb2e77dd786
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816403"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="a4df1-103">Тип ресурса yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="a4df1-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a4df1-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4df1-104">Properties</span></span>

| <span data-ttu-id="a4df1-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4df1-105">Property</span></span>          | <span data-ttu-id="a4df1-106">Тип</span><span class="sxs-lookup"><span data-stu-id="a4df1-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="a4df1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a4df1-107">reportRefreshDate</span></span> | <span data-ttu-id="a4df1-108">Date</span><span class="sxs-lookup"><span data-stu-id="a4df1-108">Date</span></span>              |
| <span data-ttu-id="a4df1-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4df1-109">userPrincipalName</span></span> | <span data-ttu-id="a4df1-110">Строка</span><span class="sxs-lookup"><span data-stu-id="a4df1-110">String</span></span>            |
| <span data-ttu-id="a4df1-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a4df1-111">displayName</span></span>       | <span data-ttu-id="a4df1-112">Строка</span><span class="sxs-lookup"><span data-stu-id="a4df1-112">String</span></span>            |
| <span data-ttu-id="a4df1-113">userState</span><span class="sxs-lookup"><span data-stu-id="a4df1-113">userState</span></span>         | <span data-ttu-id="a4df1-114">Строка</span><span class="sxs-lookup"><span data-stu-id="a4df1-114">String</span></span>            |
| <span data-ttu-id="a4df1-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="a4df1-115">stateChangeDate</span></span>   | <span data-ttu-id="a4df1-116">Date</span><span class="sxs-lookup"><span data-stu-id="a4df1-116">Date</span></span>              |
| <span data-ttu-id="a4df1-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a4df1-117">lastActivityDate</span></span>  | <span data-ttu-id="a4df1-118">Date</span><span class="sxs-lookup"><span data-stu-id="a4df1-118">Date</span></span>              |
| <span data-ttu-id="a4df1-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="a4df1-119">postedCount</span></span>       | <span data-ttu-id="a4df1-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a4df1-120">Int64</span></span>             |
| <span data-ttu-id="a4df1-121">readCount</span><span class="sxs-lookup"><span data-stu-id="a4df1-121">readCount</span></span>         | <span data-ttu-id="a4df1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a4df1-122">Int64</span></span>             |
| <span data-ttu-id="a4df1-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="a4df1-123">likedCount</span></span>        | <span data-ttu-id="a4df1-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a4df1-124">Int64</span></span>             |
| <span data-ttu-id="a4df1-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="a4df1-125">assignedProducts</span></span>  | <span data-ttu-id="a4df1-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a4df1-126">String collection</span></span> |
| <span data-ttu-id="a4df1-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a4df1-127">reportPeriod</span></span>      | <span data-ttu-id="a4df1-128">String</span><span class="sxs-lookup"><span data-stu-id="a4df1-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="a4df1-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4df1-129">JSON representation</span></span>

<span data-ttu-id="a4df1-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4df1-130">The following is a JSON representation of the resource.</span></span>

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
