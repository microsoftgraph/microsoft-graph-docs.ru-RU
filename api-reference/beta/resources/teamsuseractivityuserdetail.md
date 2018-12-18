---
title: Тип ресурса teamsUserActivityUserDetail
description: Ниже приведен representaion JSON ресурса.
author: nkramer
ms.openlocfilehash: a1f47bc52c2a0a613598ce663f16023dce208c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331943"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="ce678-103">Тип ресурса teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ce678-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ce678-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce678-104">Properties</span></span>

| <span data-ttu-id="ce678-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce678-105">Property</span></span>                | <span data-ttu-id="ce678-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ce678-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="ce678-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ce678-107">reportRefreshDate</span></span>       | <span data-ttu-id="ce678-108">Date</span><span class="sxs-lookup"><span data-stu-id="ce678-108">Date</span></span>              |
| <span data-ttu-id="ce678-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ce678-109">userPrincipalName</span></span>       | <span data-ttu-id="ce678-110">Строка</span><span class="sxs-lookup"><span data-stu-id="ce678-110">String</span></span>            |
| <span data-ttu-id="ce678-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ce678-111">lastActivityDate</span></span>        | <span data-ttu-id="ce678-112">Date</span><span class="sxs-lookup"><span data-stu-id="ce678-112">Date</span></span>              |
| <span data-ttu-id="ce678-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ce678-113">isDeleted</span></span>               | <span data-ttu-id="ce678-114">Boolean.</span><span class="sxs-lookup"><span data-stu-id="ce678-114">Boolean</span></span>           |
| <span data-ttu-id="ce678-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="ce678-115">deletedDate</span></span>             | <span data-ttu-id="ce678-116">Date</span><span class="sxs-lookup"><span data-stu-id="ce678-116">Date</span></span>              |
| <span data-ttu-id="ce678-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="ce678-117">assignedProducts</span></span>        | <span data-ttu-id="ce678-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ce678-118">String collection</span></span> |
| <span data-ttu-id="ce678-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="ce678-119">teamChatMessageCount</span></span>    | <span data-ttu-id="ce678-120">Int64</span><span class="sxs-lookup"><span data-stu-id="ce678-120">Int64</span></span>             |
| <span data-ttu-id="ce678-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="ce678-121">privateChatMessageCount</span></span> | <span data-ttu-id="ce678-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ce678-122">Int64</span></span>             |
| <span data-ttu-id="ce678-123">callCount</span><span class="sxs-lookup"><span data-stu-id="ce678-123">callCount</span></span>               | <span data-ttu-id="ce678-124">Int64</span><span class="sxs-lookup"><span data-stu-id="ce678-124">Int64</span></span>             |
| <span data-ttu-id="ce678-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="ce678-125">meetingCount</span></span>            | <span data-ttu-id="ce678-126">Int64</span><span class="sxs-lookup"><span data-stu-id="ce678-126">Int64</span></span>             |
| <span data-ttu-id="ce678-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="ce678-127">hasOtherAction</span></span>          | <span data-ttu-id="ce678-128">Boolean.</span><span class="sxs-lookup"><span data-stu-id="ce678-128">Boolean</span></span>           |
| <span data-ttu-id="ce678-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ce678-129">reportPeriod</span></span>            | <span data-ttu-id="ce678-130">String</span><span class="sxs-lookup"><span data-stu-id="ce678-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="ce678-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce678-131">JSON representation</span></span>

<span data-ttu-id="ce678-132">Ниже приведен representaion JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ce678-132">The following is a JSON representaion of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
