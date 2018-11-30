---
title: Тип ресурса teamsUserActivityUserDetail
description: Ниже приведен representaion JSON ресурса.
ms.openlocfilehash: 4e40ea4adf07450e6b51555df47579955a2a0286
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081479"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="6674c-103">Тип ресурса teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="6674c-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6674c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6674c-104">Properties</span></span>

| <span data-ttu-id="6674c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6674c-105">Property</span></span>                | <span data-ttu-id="6674c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6674c-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="6674c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6674c-107">reportRefreshDate</span></span>       | <span data-ttu-id="6674c-108">Date</span><span class="sxs-lookup"><span data-stu-id="6674c-108">Date</span></span>              |
| <span data-ttu-id="6674c-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6674c-109">userPrincipalName</span></span>       | <span data-ttu-id="6674c-110">String</span><span class="sxs-lookup"><span data-stu-id="6674c-110">String</span></span>            |
| <span data-ttu-id="6674c-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6674c-111">lastActivityDate</span></span>        | <span data-ttu-id="6674c-112">Date</span><span class="sxs-lookup"><span data-stu-id="6674c-112">Date</span></span>              |
| <span data-ttu-id="6674c-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6674c-113">isDeleted</span></span>               | <span data-ttu-id="6674c-114">Логический</span><span class="sxs-lookup"><span data-stu-id="6674c-114">Boolean</span></span>           |
| <span data-ttu-id="6674c-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="6674c-115">deletedDate</span></span>             | <span data-ttu-id="6674c-116">Date</span><span class="sxs-lookup"><span data-stu-id="6674c-116">Date</span></span>              |
| <span data-ttu-id="6674c-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="6674c-117">assignedProducts</span></span>        | <span data-ttu-id="6674c-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6674c-118">String collection</span></span> |
| <span data-ttu-id="6674c-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="6674c-119">teamChatMessageCount</span></span>    | <span data-ttu-id="6674c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6674c-120">Int64</span></span>             |
| <span data-ttu-id="6674c-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="6674c-121">privateChatMessageCount</span></span> | <span data-ttu-id="6674c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6674c-122">Int64</span></span>             |
| <span data-ttu-id="6674c-123">callCount</span><span class="sxs-lookup"><span data-stu-id="6674c-123">callCount</span></span>               | <span data-ttu-id="6674c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6674c-124">Int64</span></span>             |
| <span data-ttu-id="6674c-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="6674c-125">meetingCount</span></span>            | <span data-ttu-id="6674c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="6674c-126">Int64</span></span>             |
| <span data-ttu-id="6674c-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="6674c-127">hasOtherAction</span></span>          | <span data-ttu-id="6674c-128">Логический</span><span class="sxs-lookup"><span data-stu-id="6674c-128">Boolean</span></span>           |
| <span data-ttu-id="6674c-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6674c-129">reportPeriod</span></span>            | <span data-ttu-id="6674c-130">String</span><span class="sxs-lookup"><span data-stu-id="6674c-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="6674c-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6674c-131">JSON representation</span></span>

<span data-ttu-id="6674c-132">Ниже приведен representaion JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6674c-132">The following is a JSON representaion of the resource.</span></span>

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
