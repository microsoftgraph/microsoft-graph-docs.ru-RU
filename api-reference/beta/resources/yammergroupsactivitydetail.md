---
title: Тип ресурса yammerGroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 9a4bb00aecb2ae1d14b68a5388e0dedc7c41b1cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075778"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="c38d6-103">Тип ресурса yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="c38d6-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c38d6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c38d6-104">Properties</span></span>

| <span data-ttu-id="c38d6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c38d6-105">Property</span></span>           | <span data-ttu-id="c38d6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c38d6-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="c38d6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c38d6-107">reportRefreshDate</span></span>  | <span data-ttu-id="c38d6-108">Date</span><span class="sxs-lookup"><span data-stu-id="c38d6-108">Date</span></span>    |
| <span data-ttu-id="c38d6-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="c38d6-109">groupDisplayName</span></span>   | <span data-ttu-id="c38d6-110">String</span><span class="sxs-lookup"><span data-stu-id="c38d6-110">String</span></span>  |
| <span data-ttu-id="c38d6-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c38d6-111">isDeleted</span></span>          | <span data-ttu-id="c38d6-112">Логический</span><span class="sxs-lookup"><span data-stu-id="c38d6-112">Boolean</span></span> |
| <span data-ttu-id="c38d6-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c38d6-113">ownerPrincipalName</span></span> | <span data-ttu-id="c38d6-114">String</span><span class="sxs-lookup"><span data-stu-id="c38d6-114">String</span></span>  |
| <span data-ttu-id="c38d6-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c38d6-115">lastActivityDate</span></span>   | <span data-ttu-id="c38d6-116">Date</span><span class="sxs-lookup"><span data-stu-id="c38d6-116">Date</span></span>    |
| <span data-ttu-id="c38d6-117">groupType</span><span class="sxs-lookup"><span data-stu-id="c38d6-117">groupType</span></span>          | <span data-ttu-id="c38d6-118">String</span><span class="sxs-lookup"><span data-stu-id="c38d6-118">String</span></span>  |
| <span data-ttu-id="c38d6-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="c38d6-119">office365Connected</span></span> | <span data-ttu-id="c38d6-120">Логический</span><span class="sxs-lookup"><span data-stu-id="c38d6-120">Boolean</span></span> |
| <span data-ttu-id="c38d6-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="c38d6-121">memberCount</span></span>        | <span data-ttu-id="c38d6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c38d6-122">Int64</span></span>   |
| <span data-ttu-id="c38d6-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="c38d6-123">postedCount</span></span>        | <span data-ttu-id="c38d6-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c38d6-124">Int64</span></span>   |
| <span data-ttu-id="c38d6-125">readCount</span><span class="sxs-lookup"><span data-stu-id="c38d6-125">readCount</span></span>          | <span data-ttu-id="c38d6-126">Int64</span><span class="sxs-lookup"><span data-stu-id="c38d6-126">Int64</span></span>   |
| <span data-ttu-id="c38d6-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="c38d6-127">likedCount</span></span>         | <span data-ttu-id="c38d6-128">Int64</span><span class="sxs-lookup"><span data-stu-id="c38d6-128">Int64</span></span>   |
| <span data-ttu-id="c38d6-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c38d6-129">reportPeriod</span></span>       | <span data-ttu-id="c38d6-130">String</span><span class="sxs-lookup"><span data-stu-id="c38d6-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c38d6-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c38d6-131">JSON representation</span></span>

<span data-ttu-id="c38d6-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c38d6-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "office365Connected": true, 
  "memberCount": 1024, 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "reportPeriod": "String"
}
```
