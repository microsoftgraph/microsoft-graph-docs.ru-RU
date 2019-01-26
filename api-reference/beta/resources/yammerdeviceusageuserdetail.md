---
title: Тип ресурса yammerDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5fe3aa7fa9da243c9cc8f9b015ee85d779b84eb3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574154"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="a846c-103">Тип ресурса yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="a846c-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a846c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="a846c-104">Properties</span></span>

| <span data-ttu-id="a846c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="a846c-105">Property</span></span>          | <span data-ttu-id="a846c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="a846c-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="a846c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a846c-107">reportRefreshDate</span></span> | <span data-ttu-id="a846c-108">Date</span><span class="sxs-lookup"><span data-stu-id="a846c-108">Date</span></span>    |
| <span data-ttu-id="a846c-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a846c-109">userPrincipalName</span></span> | <span data-ttu-id="a846c-110">Строка</span><span class="sxs-lookup"><span data-stu-id="a846c-110">String</span></span>  |
| <span data-ttu-id="a846c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a846c-111">displayName</span></span>       | <span data-ttu-id="a846c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="a846c-112">String</span></span>  |
| <span data-ttu-id="a846c-113">userState</span><span class="sxs-lookup"><span data-stu-id="a846c-113">userState</span></span>         | <span data-ttu-id="a846c-114">Строка</span><span class="sxs-lookup"><span data-stu-id="a846c-114">String</span></span>  |
| <span data-ttu-id="a846c-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="a846c-115">stateChangeDate</span></span>   | <span data-ttu-id="a846c-116">Date</span><span class="sxs-lookup"><span data-stu-id="a846c-116">Date</span></span>    |
| <span data-ttu-id="a846c-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a846c-117">lastActivityDate</span></span>  | <span data-ttu-id="a846c-118">Date</span><span class="sxs-lookup"><span data-stu-id="a846c-118">Date</span></span>    |
| <span data-ttu-id="a846c-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="a846c-119">usedWeb</span></span>           | <span data-ttu-id="a846c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="a846c-120">Boolean</span></span> |
| <span data-ttu-id="a846c-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="a846c-121">usedWindowsPhone</span></span>  | <span data-ttu-id="a846c-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="a846c-122">Boolean</span></span> |
| <span data-ttu-id="a846c-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="a846c-123">usedAndroidPhone</span></span>  | <span data-ttu-id="a846c-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="a846c-124">Boolean</span></span> |
| <span data-ttu-id="a846c-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="a846c-125">usediPhone</span></span>        | <span data-ttu-id="a846c-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="a846c-126">Boolean</span></span> |
| <span data-ttu-id="a846c-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="a846c-127">usediPad</span></span>          | <span data-ttu-id="a846c-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="a846c-128">Boolean</span></span> |
| <span data-ttu-id="a846c-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="a846c-129">usedOthers</span></span>        | <span data-ttu-id="a846c-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="a846c-130">Boolean</span></span> |
| <span data-ttu-id="a846c-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a846c-131">reportPeriod</span></span>      | <span data-ttu-id="a846c-132">String</span><span class="sxs-lookup"><span data-stu-id="a846c-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a846c-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a846c-133">JSON representation</span></span>

<span data-ttu-id="a846c-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a846c-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```
