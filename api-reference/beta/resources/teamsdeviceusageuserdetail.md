---
title: Тип ресурса teamsDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953787"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="493fc-103">Тип ресурса teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="493fc-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="493fc-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="493fc-104">Properties</span></span>

| <span data-ttu-id="493fc-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="493fc-105">Property</span></span>          | <span data-ttu-id="493fc-106">Тип</span><span class="sxs-lookup"><span data-stu-id="493fc-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="493fc-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="493fc-107">reportRefreshDate</span></span> | <span data-ttu-id="493fc-108">Date</span><span class="sxs-lookup"><span data-stu-id="493fc-108">Date</span></span>    |
| <span data-ttu-id="493fc-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="493fc-109">userPrincipalName</span></span> | <span data-ttu-id="493fc-110">Строка</span><span class="sxs-lookup"><span data-stu-id="493fc-110">String</span></span>  |
| <span data-ttu-id="493fc-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="493fc-111">lastActivityDate</span></span>  | <span data-ttu-id="493fc-112">Date</span><span class="sxs-lookup"><span data-stu-id="493fc-112">Date</span></span>    |
| <span data-ttu-id="493fc-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="493fc-113">isDeleted</span></span>         | <span data-ttu-id="493fc-114">Логический</span><span class="sxs-lookup"><span data-stu-id="493fc-114">Boolean</span></span> |
| <span data-ttu-id="493fc-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="493fc-115">deletedDate</span></span>       | <span data-ttu-id="493fc-116">Date</span><span class="sxs-lookup"><span data-stu-id="493fc-116">Date</span></span>    |
| <span data-ttu-id="493fc-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="493fc-117">usedWeb</span></span>           | <span data-ttu-id="493fc-118">Логический</span><span class="sxs-lookup"><span data-stu-id="493fc-118">Boolean</span></span> |
| <span data-ttu-id="493fc-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="493fc-119">usedWindowsPhone</span></span>  | <span data-ttu-id="493fc-120">Логический</span><span class="sxs-lookup"><span data-stu-id="493fc-120">Boolean</span></span> |
| <span data-ttu-id="493fc-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="493fc-121">usediOS</span></span>           | <span data-ttu-id="493fc-122">Логический</span><span class="sxs-lookup"><span data-stu-id="493fc-122">Boolean</span></span> |
| <span data-ttu-id="493fc-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="493fc-123">usedMac</span></span>           | <span data-ttu-id="493fc-124">Логический</span><span class="sxs-lookup"><span data-stu-id="493fc-124">Boolean</span></span> |
| <span data-ttu-id="493fc-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="493fc-125">usedAndroidPhone</span></span>  | <span data-ttu-id="493fc-126">Логический</span><span class="sxs-lookup"><span data-stu-id="493fc-126">Boolean</span></span> |
| <span data-ttu-id="493fc-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="493fc-127">usedWindows</span></span>       | <span data-ttu-id="493fc-128">Логический</span><span class="sxs-lookup"><span data-stu-id="493fc-128">Boolean</span></span> |
| <span data-ttu-id="493fc-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="493fc-129">reportPeriod</span></span>      | <span data-ttu-id="493fc-130">String</span><span class="sxs-lookup"><span data-stu-id="493fc-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="493fc-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="493fc-131">JSON representation</span></span>

<span data-ttu-id="493fc-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="493fc-132">The following is a JSON representation of the resource.</span></span>

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
