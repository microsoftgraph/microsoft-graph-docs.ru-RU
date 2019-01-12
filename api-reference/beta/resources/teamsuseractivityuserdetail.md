---
title: Тип ресурса teamsUserActivityUserDetail
description: Ниже приведен representaion JSON ресурса.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913431"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="db808-103">Тип ресурса teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="db808-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="db808-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="db808-104">Properties</span></span>

| <span data-ttu-id="db808-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="db808-105">Property</span></span>                | <span data-ttu-id="db808-106">Тип</span><span class="sxs-lookup"><span data-stu-id="db808-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="db808-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="db808-107">reportRefreshDate</span></span>       | <span data-ttu-id="db808-108">Date</span><span class="sxs-lookup"><span data-stu-id="db808-108">Date</span></span>              |
| <span data-ttu-id="db808-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="db808-109">userPrincipalName</span></span>       | <span data-ttu-id="db808-110">Строка</span><span class="sxs-lookup"><span data-stu-id="db808-110">String</span></span>            |
| <span data-ttu-id="db808-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="db808-111">lastActivityDate</span></span>        | <span data-ttu-id="db808-112">Date</span><span class="sxs-lookup"><span data-stu-id="db808-112">Date</span></span>              |
| <span data-ttu-id="db808-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="db808-113">isDeleted</span></span>               | <span data-ttu-id="db808-114">Логический</span><span class="sxs-lookup"><span data-stu-id="db808-114">Boolean</span></span>           |
| <span data-ttu-id="db808-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="db808-115">deletedDate</span></span>             | <span data-ttu-id="db808-116">Date</span><span class="sxs-lookup"><span data-stu-id="db808-116">Date</span></span>              |
| <span data-ttu-id="db808-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="db808-117">assignedProducts</span></span>        | <span data-ttu-id="db808-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="db808-118">String collection</span></span> |
| <span data-ttu-id="db808-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="db808-119">teamChatMessageCount</span></span>    | <span data-ttu-id="db808-120">Int64</span><span class="sxs-lookup"><span data-stu-id="db808-120">Int64</span></span>             |
| <span data-ttu-id="db808-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="db808-121">privateChatMessageCount</span></span> | <span data-ttu-id="db808-122">Int64</span><span class="sxs-lookup"><span data-stu-id="db808-122">Int64</span></span>             |
| <span data-ttu-id="db808-123">callCount</span><span class="sxs-lookup"><span data-stu-id="db808-123">callCount</span></span>               | <span data-ttu-id="db808-124">Int64</span><span class="sxs-lookup"><span data-stu-id="db808-124">Int64</span></span>             |
| <span data-ttu-id="db808-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="db808-125">meetingCount</span></span>            | <span data-ttu-id="db808-126">Int64</span><span class="sxs-lookup"><span data-stu-id="db808-126">Int64</span></span>             |
| <span data-ttu-id="db808-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="db808-127">hasOtherAction</span></span>          | <span data-ttu-id="db808-128">Логический</span><span class="sxs-lookup"><span data-stu-id="db808-128">Boolean</span></span>           |
| <span data-ttu-id="db808-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="db808-129">reportPeriod</span></span>            | <span data-ttu-id="db808-130">String</span><span class="sxs-lookup"><span data-stu-id="db808-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="db808-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db808-131">JSON representation</span></span>

<span data-ttu-id="db808-132">Ниже приведен representaion JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="db808-132">The following is a JSON representaion of the resource.</span></span>

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
