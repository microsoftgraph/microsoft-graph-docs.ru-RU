---
title: Тип ресурса Теамсдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5bd7443e775a8a9de0dbbc27cf8843331f8f8cb7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007629"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="1ef47-103">Тип ресурса Теамсдевицеусажеусердетаил</span><span class="sxs-lookup"><span data-stu-id="1ef47-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1ef47-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ef47-104">Properties</span></span>

| <span data-ttu-id="1ef47-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ef47-105">Property</span></span>          | <span data-ttu-id="1ef47-106">Тип</span><span class="sxs-lookup"><span data-stu-id="1ef47-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="1ef47-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="1ef47-107">reportRefreshDate</span></span> | <span data-ttu-id="1ef47-108">Дата</span><span class="sxs-lookup"><span data-stu-id="1ef47-108">Date</span></span>    |
| <span data-ttu-id="1ef47-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1ef47-109">userPrincipalName</span></span> | <span data-ttu-id="1ef47-110">String</span><span class="sxs-lookup"><span data-stu-id="1ef47-110">String</span></span>  |
| <span data-ttu-id="1ef47-111">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="1ef47-111">lastActivityDate</span></span>  | <span data-ttu-id="1ef47-112">Дата</span><span class="sxs-lookup"><span data-stu-id="1ef47-112">Date</span></span>    |
| <span data-ttu-id="1ef47-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1ef47-113">isDeleted</span></span>         | <span data-ttu-id="1ef47-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef47-114">Boolean</span></span> |
| <span data-ttu-id="1ef47-115">Делетеддате</span><span class="sxs-lookup"><span data-stu-id="1ef47-115">deletedDate</span></span>       | <span data-ttu-id="1ef47-116">Дата</span><span class="sxs-lookup"><span data-stu-id="1ef47-116">Date</span></span>    |
| <span data-ttu-id="1ef47-117">Уседвеб</span><span class="sxs-lookup"><span data-stu-id="1ef47-117">usedWeb</span></span>           | <span data-ttu-id="1ef47-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef47-118">Boolean</span></span> |
| <span data-ttu-id="1ef47-119">Уседвиндовсфоне</span><span class="sxs-lookup"><span data-stu-id="1ef47-119">usedWindowsPhone</span></span>  | <span data-ttu-id="1ef47-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef47-120">Boolean</span></span> |
| <span data-ttu-id="1ef47-121">Уседиос</span><span class="sxs-lookup"><span data-stu-id="1ef47-121">usediOS</span></span>           | <span data-ttu-id="1ef47-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef47-122">Boolean</span></span> |
| <span data-ttu-id="1ef47-123">Уседмак</span><span class="sxs-lookup"><span data-stu-id="1ef47-123">usedMac</span></span>           | <span data-ttu-id="1ef47-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef47-124">Boolean</span></span> |
| <span data-ttu-id="1ef47-125">Уседандроидфоне</span><span class="sxs-lookup"><span data-stu-id="1ef47-125">usedAndroidPhone</span></span>  | <span data-ttu-id="1ef47-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef47-126">Boolean</span></span> |
| <span data-ttu-id="1ef47-127">Уседвиндовс</span><span class="sxs-lookup"><span data-stu-id="1ef47-127">usedWindows</span></span>       | <span data-ttu-id="1ef47-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef47-128">Boolean</span></span> |
| <span data-ttu-id="1ef47-129">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="1ef47-129">reportPeriod</span></span>      | <span data-ttu-id="1ef47-130">String</span><span class="sxs-lookup"><span data-stu-id="1ef47-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1ef47-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ef47-131">JSON representation</span></span>

<span data-ttu-id="1ef47-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ef47-132">The following is a JSON representation of the resource.</span></span>

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
