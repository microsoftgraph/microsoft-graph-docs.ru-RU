---
title: teamsDeviceUsageDistributionUserCounts resource type
description: Представляет число пользователей по типу устройства за выбранный период времени.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d1c716a4be9ab6ffac7b37484d7cb8bc8f01ee9
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766569"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="21718-103">teamsDeviceUsageDistributionUserCounts resource type</span><span class="sxs-lookup"><span data-stu-id="21718-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="21718-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21718-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21718-105">Представляет число пользователей по типу устройства за выбранный период времени.</span><span class="sxs-lookup"><span data-stu-id="21718-105">Represents number of users by device type over the selected time period.</span></span>

## <a name="properties"></a><span data-ttu-id="21718-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="21718-106">Properties</span></span>

| <span data-ttu-id="21718-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="21718-107">Property</span></span>          | <span data-ttu-id="21718-108">Тип</span><span class="sxs-lookup"><span data-stu-id="21718-108">Type</span></span>   | <span data-ttu-id="21718-109">Описание</span><span class="sxs-lookup"><span data-stu-id="21718-109">Description</span></span>                                                  |
| :---------------- | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="21718-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="21718-110">reportRefreshDate</span></span> | <span data-ttu-id="21718-111">Дата</span><span class="sxs-lookup"><span data-stu-id="21718-111">Date</span></span>   | <span data-ttu-id="21718-112">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="21718-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="21718-113">web</span><span class="sxs-lookup"><span data-stu-id="21718-113">web</span></span>               | <span data-ttu-id="21718-114">Int64</span><span class="sxs-lookup"><span data-stu-id="21718-114">Int64</span></span>  | <span data-ttu-id="21718-115">Количество пользователей, активных в веб-клиенте Teams на устройствах.</span><span class="sxs-lookup"><span data-stu-id="21718-115">The number of users who were active in the Teams web client on devices.</span></span> |
| <span data-ttu-id="21718-116">WindowsPhone</span><span class="sxs-lookup"><span data-stu-id="21718-116">windowsPhone</span></span>      | <span data-ttu-id="21718-117">Int64</span><span class="sxs-lookup"><span data-stu-id="21718-117">Int64</span></span>  | <span data-ttu-id="21718-118">Количество пользователей, активных в мобильном клиенте Teams для телефона Windows.</span><span class="sxs-lookup"><span data-stu-id="21718-118">The number of users who were active on the Teams mobile client for Windows phone.</span></span> |
| <span data-ttu-id="21718-119">AndroidPhone</span><span class="sxs-lookup"><span data-stu-id="21718-119">androidPhone</span></span>      | <span data-ttu-id="21718-120">Int64</span><span class="sxs-lookup"><span data-stu-id="21718-120">Int64</span></span>  | <span data-ttu-id="21718-121">Количество пользователей, активных в мобильном клиенте Teams для Android.</span><span class="sxs-lookup"><span data-stu-id="21718-121">The number of users who were active on the Teams mobile client for Android.</span></span> |
| <span data-ttu-id="21718-122">ios</span><span class="sxs-lookup"><span data-stu-id="21718-122">ios</span></span>               | <span data-ttu-id="21718-123">Int64</span><span class="sxs-lookup"><span data-stu-id="21718-123">Int64</span></span>  | <span data-ttu-id="21718-124">Количество пользователей, активных в мобильном клиенте Teams для iOS.</span><span class="sxs-lookup"><span data-stu-id="21718-124">The number of users who were active on the Teams mobile client for iOS.</span></span> |
| <span data-ttu-id="21718-125">mac</span><span class="sxs-lookup"><span data-stu-id="21718-125">mac</span></span>               | <span data-ttu-id="21718-126">Int64</span><span class="sxs-lookup"><span data-stu-id="21718-126">Int64</span></span>  | <span data-ttu-id="21718-127">Число пользователей, активных в клиенте Teams на компьютере macOS.</span><span class="sxs-lookup"><span data-stu-id="21718-127">The number of users who were active in the Teams desktop client on a macOS computer.</span></span> |
| <span data-ttu-id="21718-128">Windows</span><span class="sxs-lookup"><span data-stu-id="21718-128">windows</span></span>           | <span data-ttu-id="21718-129">Int64</span><span class="sxs-lookup"><span data-stu-id="21718-129">Int64</span></span>  | <span data-ttu-id="21718-130">Количество пользователей, активных в клиенте teams на компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="21718-130">The number of users who were active in the Teams desktop client on a Windows-based computer.</span></span> |
| <span data-ttu-id="21718-131">chromeOS</span><span class="sxs-lookup"><span data-stu-id="21718-131">chromeOS</span></span>          | <span data-ttu-id="21718-132">Int64</span><span class="sxs-lookup"><span data-stu-id="21718-132">Int64</span></span>  | <span data-ttu-id="21718-133">Количество пользователей, активных в клиенте teams на компьютере ChromeOS.</span><span class="sxs-lookup"><span data-stu-id="21718-133">The number of users who were active in the Teams desktop client on a ChromeOS computer.</span></span> |
| <span data-ttu-id="21718-134">Linux</span><span class="sxs-lookup"><span data-stu-id="21718-134">linux</span></span>             | <span data-ttu-id="21718-135">Int64</span><span class="sxs-lookup"><span data-stu-id="21718-135">Int64</span></span>  | <span data-ttu-id="21718-136">Количество пользователей, которые были активны в клиенте настольных компьютеров Teams на компьютере Linux.</span><span class="sxs-lookup"><span data-stu-id="21718-136">The number of users who were active in the Teams desktop client on a Linux computer.</span></span> |
| <span data-ttu-id="21718-137">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="21718-137">reportPeriod</span></span>      | <span data-ttu-id="21718-138">String</span><span class="sxs-lookup"><span data-stu-id="21718-138">String</span></span> | <span data-ttu-id="21718-139">Количество дней, которые охватывает отчет.</span><span class="sxs-lookup"><span data-stu-id="21718-139">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="21718-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21718-140">JSON representation</span></span>

<span data-ttu-id="21718-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21718-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```


