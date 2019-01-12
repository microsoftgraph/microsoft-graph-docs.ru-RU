---
title: Тип ресурса yammerActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d24e21c9525d49b7af5f8c4efaddd606c20c162b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923035"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="3eb49-103">Тип ресурса yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="3eb49-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3eb49-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="3eb49-104">Properties</span></span>

| <span data-ttu-id="3eb49-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="3eb49-105">Property</span></span>          | <span data-ttu-id="3eb49-106">Тип</span><span class="sxs-lookup"><span data-stu-id="3eb49-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="3eb49-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3eb49-107">reportRefreshDate</span></span> | <span data-ttu-id="3eb49-108">Date</span><span class="sxs-lookup"><span data-stu-id="3eb49-108">Date</span></span>              |
| <span data-ttu-id="3eb49-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3eb49-109">userPrincipalName</span></span> | <span data-ttu-id="3eb49-110">String</span><span class="sxs-lookup"><span data-stu-id="3eb49-110">String</span></span>            |
| <span data-ttu-id="3eb49-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3eb49-111">displayName</span></span>       | <span data-ttu-id="3eb49-112">String</span><span class="sxs-lookup"><span data-stu-id="3eb49-112">String</span></span>            |
| <span data-ttu-id="3eb49-113">userState</span><span class="sxs-lookup"><span data-stu-id="3eb49-113">userState</span></span>         | <span data-ttu-id="3eb49-114">String</span><span class="sxs-lookup"><span data-stu-id="3eb49-114">String</span></span>            |
| <span data-ttu-id="3eb49-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="3eb49-115">stateChangeDate</span></span>   | <span data-ttu-id="3eb49-116">Date</span><span class="sxs-lookup"><span data-stu-id="3eb49-116">Date</span></span>              |
| <span data-ttu-id="3eb49-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="3eb49-117">lastActivityDate</span></span>  | <span data-ttu-id="3eb49-118">Date</span><span class="sxs-lookup"><span data-stu-id="3eb49-118">Date</span></span>              |
| <span data-ttu-id="3eb49-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="3eb49-119">postedCount</span></span>       | <span data-ttu-id="3eb49-120">Int64</span><span class="sxs-lookup"><span data-stu-id="3eb49-120">Int64</span></span>             |
| <span data-ttu-id="3eb49-121">readCount</span><span class="sxs-lookup"><span data-stu-id="3eb49-121">readCount</span></span>         | <span data-ttu-id="3eb49-122">Int64</span><span class="sxs-lookup"><span data-stu-id="3eb49-122">Int64</span></span>             |
| <span data-ttu-id="3eb49-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="3eb49-123">likedCount</span></span>        | <span data-ttu-id="3eb49-124">Int64</span><span class="sxs-lookup"><span data-stu-id="3eb49-124">Int64</span></span>             |
| <span data-ttu-id="3eb49-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="3eb49-125">assignedProducts</span></span>  | <span data-ttu-id="3eb49-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3eb49-126">String collection</span></span> |
| <span data-ttu-id="3eb49-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3eb49-127">reportPeriod</span></span>      | <span data-ttu-id="3eb49-128">String</span><span class="sxs-lookup"><span data-stu-id="3eb49-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="3eb49-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3eb49-129">JSON representation</span></span>

<span data-ttu-id="3eb49-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3eb49-130">The following is a JSON representation of the resource.</span></span>

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
