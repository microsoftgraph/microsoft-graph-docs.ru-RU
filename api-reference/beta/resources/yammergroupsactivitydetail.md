---
title: Тип ресурса yammerGroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573265"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="96c5b-103">Тип ресурса yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="96c5b-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="96c5b-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="96c5b-104">Properties</span></span>

| <span data-ttu-id="96c5b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="96c5b-105">Property</span></span>           | <span data-ttu-id="96c5b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="96c5b-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="96c5b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="96c5b-107">reportRefreshDate</span></span>  | <span data-ttu-id="96c5b-108">Date</span><span class="sxs-lookup"><span data-stu-id="96c5b-108">Date</span></span>    |
| <span data-ttu-id="96c5b-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="96c5b-109">groupDisplayName</span></span>   | <span data-ttu-id="96c5b-110">Строка</span><span class="sxs-lookup"><span data-stu-id="96c5b-110">String</span></span>  |
| <span data-ttu-id="96c5b-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="96c5b-111">isDeleted</span></span>          | <span data-ttu-id="96c5b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="96c5b-112">Boolean</span></span> |
| <span data-ttu-id="96c5b-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="96c5b-113">ownerPrincipalName</span></span> | <span data-ttu-id="96c5b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="96c5b-114">String</span></span>  |
| <span data-ttu-id="96c5b-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="96c5b-115">lastActivityDate</span></span>   | <span data-ttu-id="96c5b-116">Date</span><span class="sxs-lookup"><span data-stu-id="96c5b-116">Date</span></span>    |
| <span data-ttu-id="96c5b-117">groupType</span><span class="sxs-lookup"><span data-stu-id="96c5b-117">groupType</span></span>          | <span data-ttu-id="96c5b-118">Строка</span><span class="sxs-lookup"><span data-stu-id="96c5b-118">String</span></span>  |
| <span data-ttu-id="96c5b-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="96c5b-119">office365Connected</span></span> | <span data-ttu-id="96c5b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="96c5b-120">Boolean</span></span> |
| <span data-ttu-id="96c5b-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="96c5b-121">memberCount</span></span>        | <span data-ttu-id="96c5b-122">Int64</span><span class="sxs-lookup"><span data-stu-id="96c5b-122">Int64</span></span>   |
| <span data-ttu-id="96c5b-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="96c5b-123">postedCount</span></span>        | <span data-ttu-id="96c5b-124">Int64</span><span class="sxs-lookup"><span data-stu-id="96c5b-124">Int64</span></span>   |
| <span data-ttu-id="96c5b-125">readCount</span><span class="sxs-lookup"><span data-stu-id="96c5b-125">readCount</span></span>          | <span data-ttu-id="96c5b-126">Int64</span><span class="sxs-lookup"><span data-stu-id="96c5b-126">Int64</span></span>   |
| <span data-ttu-id="96c5b-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="96c5b-127">likedCount</span></span>         | <span data-ttu-id="96c5b-128">Int64</span><span class="sxs-lookup"><span data-stu-id="96c5b-128">Int64</span></span>   |
| <span data-ttu-id="96c5b-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="96c5b-129">reportPeriod</span></span>       | <span data-ttu-id="96c5b-130">String</span><span class="sxs-lookup"><span data-stu-id="96c5b-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="96c5b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96c5b-131">JSON representation</span></span>

<span data-ttu-id="96c5b-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96c5b-132">The following is a JSON representation of the resource.</span></span>

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
