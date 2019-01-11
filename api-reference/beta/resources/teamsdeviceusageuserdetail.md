---
title: Тип ресурса teamsDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06e2cea1154c608b61642b07adbd96aae1710903
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807107"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="a9d9a-103">Тип ресурса teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="a9d9a-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a9d9a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9d9a-104">Properties</span></span>

| <span data-ttu-id="a9d9a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9d9a-105">Property</span></span>          | <span data-ttu-id="a9d9a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="a9d9a-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="a9d9a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a9d9a-107">reportRefreshDate</span></span> | <span data-ttu-id="a9d9a-108">Date</span><span class="sxs-lookup"><span data-stu-id="a9d9a-108">Date</span></span>    |
| <span data-ttu-id="a9d9a-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9d9a-109">userPrincipalName</span></span> | <span data-ttu-id="a9d9a-110">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d9a-110">String</span></span>  |
| <span data-ttu-id="a9d9a-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a9d9a-111">lastActivityDate</span></span>  | <span data-ttu-id="a9d9a-112">Date</span><span class="sxs-lookup"><span data-stu-id="a9d9a-112">Date</span></span>    |
| <span data-ttu-id="a9d9a-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a9d9a-113">isDeleted</span></span>         | <span data-ttu-id="a9d9a-114">Логический</span><span class="sxs-lookup"><span data-stu-id="a9d9a-114">Boolean</span></span> |
| <span data-ttu-id="a9d9a-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a9d9a-115">deletedDate</span></span>       | <span data-ttu-id="a9d9a-116">Date</span><span class="sxs-lookup"><span data-stu-id="a9d9a-116">Date</span></span>    |
| <span data-ttu-id="a9d9a-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="a9d9a-117">usedWeb</span></span>           | <span data-ttu-id="a9d9a-118">Логический</span><span class="sxs-lookup"><span data-stu-id="a9d9a-118">Boolean</span></span> |
| <span data-ttu-id="a9d9a-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="a9d9a-119">usedWindowsPhone</span></span>  | <span data-ttu-id="a9d9a-120">Логический</span><span class="sxs-lookup"><span data-stu-id="a9d9a-120">Boolean</span></span> |
| <span data-ttu-id="a9d9a-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="a9d9a-121">usediOS</span></span>           | <span data-ttu-id="a9d9a-122">Логический</span><span class="sxs-lookup"><span data-stu-id="a9d9a-122">Boolean</span></span> |
| <span data-ttu-id="a9d9a-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="a9d9a-123">usedMac</span></span>           | <span data-ttu-id="a9d9a-124">Логический</span><span class="sxs-lookup"><span data-stu-id="a9d9a-124">Boolean</span></span> |
| <span data-ttu-id="a9d9a-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="a9d9a-125">usedAndroidPhone</span></span>  | <span data-ttu-id="a9d9a-126">Логический</span><span class="sxs-lookup"><span data-stu-id="a9d9a-126">Boolean</span></span> |
| <span data-ttu-id="a9d9a-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="a9d9a-127">usedWindows</span></span>       | <span data-ttu-id="a9d9a-128">Логический</span><span class="sxs-lookup"><span data-stu-id="a9d9a-128">Boolean</span></span> |
| <span data-ttu-id="a9d9a-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a9d9a-129">reportPeriod</span></span>      | <span data-ttu-id="a9d9a-130">String</span><span class="sxs-lookup"><span data-stu-id="a9d9a-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a9d9a-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9d9a-131">JSON representation</span></span>

<span data-ttu-id="a9d9a-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9d9a-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
