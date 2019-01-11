---
title: Тип ресурса yammerGroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 9e4ac61f2af69b4229c2e9c3df7c653428cc2033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832034"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="357ac-103">Тип ресурса yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="357ac-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="357ac-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="357ac-104">Properties</span></span>

| <span data-ttu-id="357ac-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="357ac-105">Property</span></span>           | <span data-ttu-id="357ac-106">Тип</span><span class="sxs-lookup"><span data-stu-id="357ac-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="357ac-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="357ac-107">reportRefreshDate</span></span>  | <span data-ttu-id="357ac-108">Date</span><span class="sxs-lookup"><span data-stu-id="357ac-108">Date</span></span>    |
| <span data-ttu-id="357ac-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="357ac-109">groupDisplayName</span></span>   | <span data-ttu-id="357ac-110">Строка</span><span class="sxs-lookup"><span data-stu-id="357ac-110">String</span></span>  |
| <span data-ttu-id="357ac-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="357ac-111">isDeleted</span></span>          | <span data-ttu-id="357ac-112">Логический</span><span class="sxs-lookup"><span data-stu-id="357ac-112">Boolean</span></span> |
| <span data-ttu-id="357ac-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="357ac-113">ownerPrincipalName</span></span> | <span data-ttu-id="357ac-114">Строка</span><span class="sxs-lookup"><span data-stu-id="357ac-114">String</span></span>  |
| <span data-ttu-id="357ac-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="357ac-115">lastActivityDate</span></span>   | <span data-ttu-id="357ac-116">Date</span><span class="sxs-lookup"><span data-stu-id="357ac-116">Date</span></span>    |
| <span data-ttu-id="357ac-117">groupType</span><span class="sxs-lookup"><span data-stu-id="357ac-117">groupType</span></span>          | <span data-ttu-id="357ac-118">Строка</span><span class="sxs-lookup"><span data-stu-id="357ac-118">String</span></span>  |
| <span data-ttu-id="357ac-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="357ac-119">office365Connected</span></span> | <span data-ttu-id="357ac-120">Логический</span><span class="sxs-lookup"><span data-stu-id="357ac-120">Boolean</span></span> |
| <span data-ttu-id="357ac-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="357ac-121">memberCount</span></span>        | <span data-ttu-id="357ac-122">Int64</span><span class="sxs-lookup"><span data-stu-id="357ac-122">Int64</span></span>   |
| <span data-ttu-id="357ac-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="357ac-123">postedCount</span></span>        | <span data-ttu-id="357ac-124">Int64</span><span class="sxs-lookup"><span data-stu-id="357ac-124">Int64</span></span>   |
| <span data-ttu-id="357ac-125">readCount</span><span class="sxs-lookup"><span data-stu-id="357ac-125">readCount</span></span>          | <span data-ttu-id="357ac-126">Int64</span><span class="sxs-lookup"><span data-stu-id="357ac-126">Int64</span></span>   |
| <span data-ttu-id="357ac-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="357ac-127">likedCount</span></span>         | <span data-ttu-id="357ac-128">Int64</span><span class="sxs-lookup"><span data-stu-id="357ac-128">Int64</span></span>   |
| <span data-ttu-id="357ac-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="357ac-129">reportPeriod</span></span>       | <span data-ttu-id="357ac-130">String</span><span class="sxs-lookup"><span data-stu-id="357ac-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="357ac-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="357ac-131">JSON representation</span></span>

<span data-ttu-id="357ac-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="357ac-132">The following is a JSON representation of the resource.</span></span>

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
