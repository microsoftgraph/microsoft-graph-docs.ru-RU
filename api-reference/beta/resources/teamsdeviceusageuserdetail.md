---
title: Тип ресурса teamsDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
ms.openlocfilehash: 1947b66a59190945e5a6b823b47ef8df7d02683a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329003"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="f48a6-103">Тип ресурса teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="f48a6-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f48a6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f48a6-104">Properties</span></span>

| <span data-ttu-id="f48a6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f48a6-105">Property</span></span>          | <span data-ttu-id="f48a6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f48a6-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="f48a6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f48a6-107">reportRefreshDate</span></span> | <span data-ttu-id="f48a6-108">Date</span><span class="sxs-lookup"><span data-stu-id="f48a6-108">Date</span></span>    |
| <span data-ttu-id="f48a6-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f48a6-109">userPrincipalName</span></span> | <span data-ttu-id="f48a6-110">Строка</span><span class="sxs-lookup"><span data-stu-id="f48a6-110">String</span></span>  |
| <span data-ttu-id="f48a6-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f48a6-111">lastActivityDate</span></span>  | <span data-ttu-id="f48a6-112">Date</span><span class="sxs-lookup"><span data-stu-id="f48a6-112">Date</span></span>    |
| <span data-ttu-id="f48a6-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f48a6-113">isDeleted</span></span>         | <span data-ttu-id="f48a6-114">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f48a6-114">Boolean</span></span> |
| <span data-ttu-id="f48a6-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="f48a6-115">deletedDate</span></span>       | <span data-ttu-id="f48a6-116">Date</span><span class="sxs-lookup"><span data-stu-id="f48a6-116">Date</span></span>    |
| <span data-ttu-id="f48a6-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="f48a6-117">usedWeb</span></span>           | <span data-ttu-id="f48a6-118">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f48a6-118">Boolean</span></span> |
| <span data-ttu-id="f48a6-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="f48a6-119">usedWindowsPhone</span></span>  | <span data-ttu-id="f48a6-120">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f48a6-120">Boolean</span></span> |
| <span data-ttu-id="f48a6-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="f48a6-121">usediOS</span></span>           | <span data-ttu-id="f48a6-122">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f48a6-122">Boolean</span></span> |
| <span data-ttu-id="f48a6-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="f48a6-123">usedMac</span></span>           | <span data-ttu-id="f48a6-124">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f48a6-124">Boolean</span></span> |
| <span data-ttu-id="f48a6-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="f48a6-125">usedAndroidPhone</span></span>  | <span data-ttu-id="f48a6-126">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f48a6-126">Boolean</span></span> |
| <span data-ttu-id="f48a6-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="f48a6-127">usedWindows</span></span>       | <span data-ttu-id="f48a6-128">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f48a6-128">Boolean</span></span> |
| <span data-ttu-id="f48a6-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f48a6-129">reportPeriod</span></span>      | <span data-ttu-id="f48a6-130">String</span><span class="sxs-lookup"><span data-stu-id="f48a6-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f48a6-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f48a6-131">JSON representation</span></span>

<span data-ttu-id="f48a6-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f48a6-132">The following is a JSON representation of the resource.</span></span>

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
