---
title: Тип ресурса yammerGroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 79ce924fff5d1ce9ca861c3d48589a0ecad149dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939170"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="be3b0-103">Тип ресурса yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="be3b0-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="be3b0-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="be3b0-104">Properties</span></span>

| <span data-ttu-id="be3b0-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="be3b0-105">Property</span></span>           | <span data-ttu-id="be3b0-106">Тип</span><span class="sxs-lookup"><span data-stu-id="be3b0-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="be3b0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="be3b0-107">reportRefreshDate</span></span>  | <span data-ttu-id="be3b0-108">Date</span><span class="sxs-lookup"><span data-stu-id="be3b0-108">Date</span></span>    |
| <span data-ttu-id="be3b0-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="be3b0-109">groupDisplayName</span></span>   | <span data-ttu-id="be3b0-110">Строка</span><span class="sxs-lookup"><span data-stu-id="be3b0-110">String</span></span>  |
| <span data-ttu-id="be3b0-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="be3b0-111">isDeleted</span></span>          | <span data-ttu-id="be3b0-112">Логический</span><span class="sxs-lookup"><span data-stu-id="be3b0-112">Boolean</span></span> |
| <span data-ttu-id="be3b0-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="be3b0-113">ownerPrincipalName</span></span> | <span data-ttu-id="be3b0-114">Строка</span><span class="sxs-lookup"><span data-stu-id="be3b0-114">String</span></span>  |
| <span data-ttu-id="be3b0-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="be3b0-115">lastActivityDate</span></span>   | <span data-ttu-id="be3b0-116">Date</span><span class="sxs-lookup"><span data-stu-id="be3b0-116">Date</span></span>    |
| <span data-ttu-id="be3b0-117">groupType</span><span class="sxs-lookup"><span data-stu-id="be3b0-117">groupType</span></span>          | <span data-ttu-id="be3b0-118">Строка</span><span class="sxs-lookup"><span data-stu-id="be3b0-118">String</span></span>  |
| <span data-ttu-id="be3b0-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="be3b0-119">office365Connected</span></span> | <span data-ttu-id="be3b0-120">Логический</span><span class="sxs-lookup"><span data-stu-id="be3b0-120">Boolean</span></span> |
| <span data-ttu-id="be3b0-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="be3b0-121">memberCount</span></span>        | <span data-ttu-id="be3b0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="be3b0-122">Int64</span></span>   |
| <span data-ttu-id="be3b0-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="be3b0-123">postedCount</span></span>        | <span data-ttu-id="be3b0-124">Int64</span><span class="sxs-lookup"><span data-stu-id="be3b0-124">Int64</span></span>   |
| <span data-ttu-id="be3b0-125">readCount</span><span class="sxs-lookup"><span data-stu-id="be3b0-125">readCount</span></span>          | <span data-ttu-id="be3b0-126">Int64</span><span class="sxs-lookup"><span data-stu-id="be3b0-126">Int64</span></span>   |
| <span data-ttu-id="be3b0-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="be3b0-127">likedCount</span></span>         | <span data-ttu-id="be3b0-128">Int64</span><span class="sxs-lookup"><span data-stu-id="be3b0-128">Int64</span></span>   |
| <span data-ttu-id="be3b0-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="be3b0-129">reportPeriod</span></span>       | <span data-ttu-id="be3b0-130">String</span><span class="sxs-lookup"><span data-stu-id="be3b0-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="be3b0-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be3b0-131">JSON representation</span></span>

<span data-ttu-id="be3b0-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be3b0-132">The following is a JSON representation of the resource.</span></span>

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
