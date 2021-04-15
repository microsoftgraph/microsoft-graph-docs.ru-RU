---
title: тип ресурса teamsDeviceUsageUserCounts
description: Представляет число ежедневных пользователей по типу устройства.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d7b813727a5ac9b2f7547e108bad8ee455d206b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766576"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="e0bd6-103">тип ресурса teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="e0bd6-103">teamsDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="e0bd6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0bd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0bd6-105">Представляет число ежедневных пользователей по типу устройства.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-105">Represents number of daily users by device type.</span></span>

## <a name="properties"></a><span data-ttu-id="e0bd6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0bd6-106">Properties</span></span>

| <span data-ttu-id="e0bd6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0bd6-107">Property</span></span>          | <span data-ttu-id="e0bd6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e0bd6-108">Type</span></span>   | <span data-ttu-id="e0bd6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e0bd6-109">Description</span></span>                                                  |
| :---------------- | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="e0bd6-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e0bd6-110">reportRefreshDate</span></span> | <span data-ttu-id="e0bd6-111">Дата</span><span class="sxs-lookup"><span data-stu-id="e0bd6-111">Date</span></span>   | <span data-ttu-id="e0bd6-112">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="e0bd6-113">web</span><span class="sxs-lookup"><span data-stu-id="e0bd6-113">web</span></span>               | <span data-ttu-id="e0bd6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e0bd6-114">Int64</span></span>  | <span data-ttu-id="e0bd6-115">Количество пользователей, активных в веб-клиенте Teams на устройствах.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-115">The number of users who were active in the Teams web client on devices.</span></span> |
| <span data-ttu-id="e0bd6-116">WindowsPhone</span><span class="sxs-lookup"><span data-stu-id="e0bd6-116">windowsPhone</span></span>      | <span data-ttu-id="e0bd6-117">Int64</span><span class="sxs-lookup"><span data-stu-id="e0bd6-117">Int64</span></span>  | <span data-ttu-id="e0bd6-118">Количество пользователей, активных в мобильном клиенте Teams для телефона Windows.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-118">The number of users who were active on the Teams mobile client for Windows phone.</span></span> |
| <span data-ttu-id="e0bd6-119">AndroidPhone</span><span class="sxs-lookup"><span data-stu-id="e0bd6-119">androidPhone</span></span>      | <span data-ttu-id="e0bd6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e0bd6-120">Int64</span></span>  | <span data-ttu-id="e0bd6-121">Количество пользователей, активных в мобильном клиенте Teams для Android.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-121">The number of users who were active on the Teams mobile client for Android.</span></span> |
| <span data-ttu-id="e0bd6-122">ios</span><span class="sxs-lookup"><span data-stu-id="e0bd6-122">ios</span></span>               | <span data-ttu-id="e0bd6-123">Int64</span><span class="sxs-lookup"><span data-stu-id="e0bd6-123">Int64</span></span>  | <span data-ttu-id="e0bd6-124">Количество пользователей, активных в мобильном клиенте Teams для iOS.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-124">The number of users who were active on the Teams mobile client for iOS.</span></span> |
| <span data-ttu-id="e0bd6-125">mac</span><span class="sxs-lookup"><span data-stu-id="e0bd6-125">mac</span></span>               | <span data-ttu-id="e0bd6-126">Int64</span><span class="sxs-lookup"><span data-stu-id="e0bd6-126">Int64</span></span>  | <span data-ttu-id="e0bd6-127">Число пользователей, активных в клиенте Teams на компьютере macOS.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-127">The number of users who were active in the Teams desktop client on a macOS computer.</span></span> |
| <span data-ttu-id="e0bd6-128">Windows</span><span class="sxs-lookup"><span data-stu-id="e0bd6-128">windows</span></span>           | <span data-ttu-id="e0bd6-129">Int64</span><span class="sxs-lookup"><span data-stu-id="e0bd6-129">Int64</span></span>  | <span data-ttu-id="e0bd6-130">Количество пользователей, активных в клиенте teams на компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-130">The number of users who were active in the Teams desktop client on a Windows-based computer.</span></span> |
| <span data-ttu-id="e0bd6-131">chromeOS</span><span class="sxs-lookup"><span data-stu-id="e0bd6-131">chromeOS</span></span>          | <span data-ttu-id="e0bd6-132">Int64</span><span class="sxs-lookup"><span data-stu-id="e0bd6-132">Int64</span></span>  | <span data-ttu-id="e0bd6-133">Количество пользователей, активных в клиенте teams на компьютере ChromeOS.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-133">The number of users who were active in the Teams desktop client on a ChromeOS computer.</span></span> |
| <span data-ttu-id="e0bd6-134">Linux</span><span class="sxs-lookup"><span data-stu-id="e0bd6-134">linux</span></span>             | <span data-ttu-id="e0bd6-135">Int64</span><span class="sxs-lookup"><span data-stu-id="e0bd6-135">Int64</span></span>  | <span data-ttu-id="e0bd6-136">Количество пользователей, которые были активны в клиенте настольных компьютеров Teams на компьютере Linux.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-136">The number of users who were active in the Teams desktop client on a Linux computer.</span></span> |
| <span data-ttu-id="e0bd6-137">reportDate</span><span class="sxs-lookup"><span data-stu-id="e0bd6-137">reportDate</span></span>        | <span data-ttu-id="e0bd6-138">Дата</span><span class="sxs-lookup"><span data-stu-id="e0bd6-138">Date</span></span>   | <span data-ttu-id="e0bd6-139">Дата выполнения пользователями действий.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-139">The date on which the users performed the activities.</span></span>        |
| <span data-ttu-id="e0bd6-140">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e0bd6-140">reportPeriod</span></span>      | <span data-ttu-id="e0bd6-141">String</span><span class="sxs-lookup"><span data-stu-id="e0bd6-141">String</span></span> | <span data-ttu-id="e0bd6-142">Количество дней, которые охватывает отчет.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-142">The number of days the report covers.</span></span>                        |

## <a name="representation"></a><span data-ttu-id="e0bd6-143">представление</span><span class="sxs-lookup"><span data-stu-id="e0bd6-143">representation</span></span>

<span data-ttu-id="e0bd6-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0bd6-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "chromeOS": 1024, 
  "linux": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


