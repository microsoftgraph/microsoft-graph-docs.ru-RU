---
title: Тип ресурса teamsDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 4eeec5f07a0a604249617ac87a62ea12b4052395
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082098"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="c31d8-103">Тип ресурса teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="c31d8-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c31d8-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c31d8-104">Properties</span></span>

| <span data-ttu-id="c31d8-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c31d8-105">Property</span></span>          | <span data-ttu-id="c31d8-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c31d8-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="c31d8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c31d8-107">reportRefreshDate</span></span> | <span data-ttu-id="c31d8-108">Date</span><span class="sxs-lookup"><span data-stu-id="c31d8-108">Date</span></span>    |
| <span data-ttu-id="c31d8-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c31d8-109">userPrincipalName</span></span> | <span data-ttu-id="c31d8-110">String</span><span class="sxs-lookup"><span data-stu-id="c31d8-110">String</span></span>  |
| <span data-ttu-id="c31d8-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c31d8-111">lastActivityDate</span></span>  | <span data-ttu-id="c31d8-112">Date</span><span class="sxs-lookup"><span data-stu-id="c31d8-112">Date</span></span>    |
| <span data-ttu-id="c31d8-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c31d8-113">isDeleted</span></span>         | <span data-ttu-id="c31d8-114">Логический</span><span class="sxs-lookup"><span data-stu-id="c31d8-114">Boolean</span></span> |
| <span data-ttu-id="c31d8-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="c31d8-115">deletedDate</span></span>       | <span data-ttu-id="c31d8-116">Date</span><span class="sxs-lookup"><span data-stu-id="c31d8-116">Date</span></span>    |
| <span data-ttu-id="c31d8-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="c31d8-117">usedWeb</span></span>           | <span data-ttu-id="c31d8-118">Логический</span><span class="sxs-lookup"><span data-stu-id="c31d8-118">Boolean</span></span> |
| <span data-ttu-id="c31d8-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="c31d8-119">usedWindowsPhone</span></span>  | <span data-ttu-id="c31d8-120">Логический</span><span class="sxs-lookup"><span data-stu-id="c31d8-120">Boolean</span></span> |
| <span data-ttu-id="c31d8-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="c31d8-121">usediOS</span></span>           | <span data-ttu-id="c31d8-122">Логический</span><span class="sxs-lookup"><span data-stu-id="c31d8-122">Boolean</span></span> |
| <span data-ttu-id="c31d8-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="c31d8-123">usedMac</span></span>           | <span data-ttu-id="c31d8-124">Логический</span><span class="sxs-lookup"><span data-stu-id="c31d8-124">Boolean</span></span> |
| <span data-ttu-id="c31d8-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="c31d8-125">usedAndroidPhone</span></span>  | <span data-ttu-id="c31d8-126">Логический</span><span class="sxs-lookup"><span data-stu-id="c31d8-126">Boolean</span></span> |
| <span data-ttu-id="c31d8-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="c31d8-127">usedWindows</span></span>       | <span data-ttu-id="c31d8-128">Логический</span><span class="sxs-lookup"><span data-stu-id="c31d8-128">Boolean</span></span> |
| <span data-ttu-id="c31d8-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c31d8-129">reportPeriod</span></span>      | <span data-ttu-id="c31d8-130">String</span><span class="sxs-lookup"><span data-stu-id="c31d8-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c31d8-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c31d8-131">JSON representation</span></span>

<span data-ttu-id="c31d8-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c31d8-132">The following is a JSON representation of the resource.</span></span>

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
