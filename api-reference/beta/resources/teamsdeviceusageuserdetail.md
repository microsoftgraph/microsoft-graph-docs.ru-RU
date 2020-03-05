---
title: Тип ресурса Теамсдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c5c3815b2418f414aa552f211bbeed5f643eb0d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519864"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="a72ff-103">Тип ресурса Теамсдевицеусажеусердетаил</span><span class="sxs-lookup"><span data-stu-id="a72ff-103">teamsDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="a72ff-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a72ff-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a72ff-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a72ff-105">Properties</span></span>

| <span data-ttu-id="a72ff-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a72ff-106">Property</span></span>          | <span data-ttu-id="a72ff-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a72ff-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="a72ff-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="a72ff-108">reportRefreshDate</span></span> | <span data-ttu-id="a72ff-109">Дата</span><span class="sxs-lookup"><span data-stu-id="a72ff-109">Date</span></span>    |
| <span data-ttu-id="a72ff-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a72ff-110">userPrincipalName</span></span> | <span data-ttu-id="a72ff-111">String</span><span class="sxs-lookup"><span data-stu-id="a72ff-111">String</span></span>  |
| <span data-ttu-id="a72ff-112">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="a72ff-112">lastActivityDate</span></span>  | <span data-ttu-id="a72ff-113">Дата</span><span class="sxs-lookup"><span data-stu-id="a72ff-113">Date</span></span>    |
| <span data-ttu-id="a72ff-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a72ff-114">isDeleted</span></span>         | <span data-ttu-id="a72ff-115">Логический</span><span class="sxs-lookup"><span data-stu-id="a72ff-115">Boolean</span></span> |
| <span data-ttu-id="a72ff-116">делетеддате</span><span class="sxs-lookup"><span data-stu-id="a72ff-116">deletedDate</span></span>       | <span data-ttu-id="a72ff-117">Дата</span><span class="sxs-lookup"><span data-stu-id="a72ff-117">Date</span></span>    |
| <span data-ttu-id="a72ff-118">уседвеб</span><span class="sxs-lookup"><span data-stu-id="a72ff-118">usedWeb</span></span>           | <span data-ttu-id="a72ff-119">Логический</span><span class="sxs-lookup"><span data-stu-id="a72ff-119">Boolean</span></span> |
| <span data-ttu-id="a72ff-120">уседвиндовсфоне</span><span class="sxs-lookup"><span data-stu-id="a72ff-120">usedWindowsPhone</span></span>  | <span data-ttu-id="a72ff-121">Логический</span><span class="sxs-lookup"><span data-stu-id="a72ff-121">Boolean</span></span> |
| <span data-ttu-id="a72ff-122">уседиос</span><span class="sxs-lookup"><span data-stu-id="a72ff-122">usediOS</span></span>           | <span data-ttu-id="a72ff-123">Логический</span><span class="sxs-lookup"><span data-stu-id="a72ff-123">Boolean</span></span> |
| <span data-ttu-id="a72ff-124">уседмак</span><span class="sxs-lookup"><span data-stu-id="a72ff-124">usedMac</span></span>           | <span data-ttu-id="a72ff-125">Логический</span><span class="sxs-lookup"><span data-stu-id="a72ff-125">Boolean</span></span> |
| <span data-ttu-id="a72ff-126">уседандроидфоне</span><span class="sxs-lookup"><span data-stu-id="a72ff-126">usedAndroidPhone</span></span>  | <span data-ttu-id="a72ff-127">Логический</span><span class="sxs-lookup"><span data-stu-id="a72ff-127">Boolean</span></span> |
| <span data-ttu-id="a72ff-128">уседвиндовс</span><span class="sxs-lookup"><span data-stu-id="a72ff-128">usedWindows</span></span>       | <span data-ttu-id="a72ff-129">Логический</span><span class="sxs-lookup"><span data-stu-id="a72ff-129">Boolean</span></span> |
| <span data-ttu-id="a72ff-130">репортпериод</span><span class="sxs-lookup"><span data-stu-id="a72ff-130">reportPeriod</span></span>      | <span data-ttu-id="a72ff-131">String</span><span class="sxs-lookup"><span data-stu-id="a72ff-131">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a72ff-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a72ff-132">JSON representation</span></span>

<span data-ttu-id="a72ff-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a72ff-133">The following is a JSON representation of the resource.</span></span>

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
