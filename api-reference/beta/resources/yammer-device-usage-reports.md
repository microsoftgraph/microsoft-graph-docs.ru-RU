---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 47dcdabb2230645ce2575fc573a99c37868c1919
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982434"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="1f6d3-104">Отчеты об использовании устройств с Yammer</span><span class="sxs-lookup"><span data-stu-id="1f6d3-104">Yammer device usage reports</span></span>

<span data-ttu-id="1f6d3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f6d3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f6d3-106">Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей.</span><span class="sxs-lookup"><span data-stu-id="1f6d3-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="1f6d3-107">Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.</span><span class="sxs-lookup"><span data-stu-id="1f6d3-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="1f6d3-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании устройств Yammer.](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)</span><span class="sxs-lookup"><span data-stu-id="1f6d3-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="1f6d3-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="1f6d3-109">Reports</span></span>

| <span data-ttu-id="1f6d3-110">Функция</span><span class="sxs-lookup"><span data-stu-id="1f6d3-110">Function</span></span>                                 | <span data-ttu-id="1f6d3-111">Тип возврата CSV</span><span class="sxs-lookup"><span data-stu-id="1f6d3-111">CSV return type</span></span> | <span data-ttu-id="1f6d3-112">Тип возврата JSON</span><span class="sxs-lookup"><span data-stu-id="1f6d3-112">JSON return type</span></span>                         | <span data-ttu-id="1f6d3-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1f6d3-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="1f6d3-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="1f6d3-114">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="1f6d3-115">Stream</span><span class="sxs-lookup"><span data-stu-id="1f6d3-115">Stream</span></span>          | [<span data-ttu-id="1f6d3-116">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="1f6d3-116">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="1f6d3-117">Получение сведений об использовании устройств с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="1f6d3-117">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="1f6d3-118">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="1f6d3-118">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="1f6d3-119">Stream</span><span class="sxs-lookup"><span data-stu-id="1f6d3-119">Stream</span></span>          | [<span data-ttu-id="1f6d3-120">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="1f6d3-120">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="1f6d3-121">Получение сведений о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="1f6d3-121">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="1f6d3-122">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="1f6d3-122">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="1f6d3-123">Stream</span><span class="sxs-lookup"><span data-stu-id="1f6d3-123">Stream</span></span>          | [<span data-ttu-id="1f6d3-124">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="1f6d3-124">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="1f6d3-125">Получение сведений о количестве пользователей в день с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="1f6d3-125">Get the number of daily users by device type.</span></span> |


