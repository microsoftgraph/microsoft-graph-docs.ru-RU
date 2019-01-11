---
title: Тип ресурса skypeForBusinessDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858382"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="f23af-103">Тип ресурса skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="f23af-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f23af-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f23af-104">Properties</span></span>

| <span data-ttu-id="f23af-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f23af-105">Property</span></span>          | <span data-ttu-id="f23af-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f23af-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="f23af-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f23af-107">reportRefreshDate</span></span> | <span data-ttu-id="f23af-108">Date</span><span class="sxs-lookup"><span data-stu-id="f23af-108">Date</span></span>    |
| <span data-ttu-id="f23af-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f23af-109">userPrincipalName</span></span> | <span data-ttu-id="f23af-110">Строка</span><span class="sxs-lookup"><span data-stu-id="f23af-110">String</span></span>  |
| <span data-ttu-id="f23af-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f23af-111">lastActivityDate</span></span>  | <span data-ttu-id="f23af-112">Date</span><span class="sxs-lookup"><span data-stu-id="f23af-112">Date</span></span>    |
| <span data-ttu-id="f23af-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="f23af-113">usedWindows</span></span>       | <span data-ttu-id="f23af-114">Логический</span><span class="sxs-lookup"><span data-stu-id="f23af-114">Boolean</span></span> |
| <span data-ttu-id="f23af-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="f23af-115">usedWindowsPhone</span></span>  | <span data-ttu-id="f23af-116">Логический</span><span class="sxs-lookup"><span data-stu-id="f23af-116">Boolean</span></span> |
| <span data-ttu-id="f23af-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="f23af-117">usedAndroidPhone</span></span>  | <span data-ttu-id="f23af-118">Логический</span><span class="sxs-lookup"><span data-stu-id="f23af-118">Boolean</span></span> |
| <span data-ttu-id="f23af-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="f23af-119">usediPhone</span></span>        | <span data-ttu-id="f23af-120">Логический</span><span class="sxs-lookup"><span data-stu-id="f23af-120">Boolean</span></span> |
| <span data-ttu-id="f23af-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="f23af-121">usediPad</span></span>          | <span data-ttu-id="f23af-122">Логический</span><span class="sxs-lookup"><span data-stu-id="f23af-122">Boolean</span></span> |
| <span data-ttu-id="f23af-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f23af-123">reportPeriod</span></span>      | <span data-ttu-id="f23af-124">String</span><span class="sxs-lookup"><span data-stu-id="f23af-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f23af-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f23af-125">JSON representation</span></span>

<span data-ttu-id="f23af-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f23af-126">The following is a JSON representation of the resource.</span></span>

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
