---
title: Тип ресурса skypeForBusinessDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: b62920d124fd52e0f653c128eeb0956cdfe0c680
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076382"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="8e966-103">Тип ресурса skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="8e966-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8e966-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e966-104">Properties</span></span>

| <span data-ttu-id="8e966-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e966-105">Property</span></span>          | <span data-ttu-id="8e966-106">Тип</span><span class="sxs-lookup"><span data-stu-id="8e966-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="8e966-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8e966-107">reportRefreshDate</span></span> | <span data-ttu-id="8e966-108">Date</span><span class="sxs-lookup"><span data-stu-id="8e966-108">Date</span></span>    |
| <span data-ttu-id="8e966-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8e966-109">userPrincipalName</span></span> | <span data-ttu-id="8e966-110">String</span><span class="sxs-lookup"><span data-stu-id="8e966-110">String</span></span>  |
| <span data-ttu-id="8e966-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8e966-111">lastActivityDate</span></span>  | <span data-ttu-id="8e966-112">Date</span><span class="sxs-lookup"><span data-stu-id="8e966-112">Date</span></span>    |
| <span data-ttu-id="8e966-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="8e966-113">usedWindows</span></span>       | <span data-ttu-id="8e966-114">Логический</span><span class="sxs-lookup"><span data-stu-id="8e966-114">Boolean</span></span> |
| <span data-ttu-id="8e966-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="8e966-115">usedWindowsPhone</span></span>  | <span data-ttu-id="8e966-116">Логический</span><span class="sxs-lookup"><span data-stu-id="8e966-116">Boolean</span></span> |
| <span data-ttu-id="8e966-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="8e966-117">usedAndroidPhone</span></span>  | <span data-ttu-id="8e966-118">Логический</span><span class="sxs-lookup"><span data-stu-id="8e966-118">Boolean</span></span> |
| <span data-ttu-id="8e966-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="8e966-119">usediPhone</span></span>        | <span data-ttu-id="8e966-120">Логический</span><span class="sxs-lookup"><span data-stu-id="8e966-120">Boolean</span></span> |
| <span data-ttu-id="8e966-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="8e966-121">usediPad</span></span>          | <span data-ttu-id="8e966-122">Логический</span><span class="sxs-lookup"><span data-stu-id="8e966-122">Boolean</span></span> |
| <span data-ttu-id="8e966-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8e966-123">reportPeriod</span></span>      | <span data-ttu-id="8e966-124">String</span><span class="sxs-lookup"><span data-stu-id="8e966-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8e966-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e966-125">JSON representation</span></span>

<span data-ttu-id="8e966-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e966-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
