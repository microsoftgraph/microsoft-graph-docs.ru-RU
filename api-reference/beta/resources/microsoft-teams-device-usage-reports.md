---
title: Отчеты об использовании устройств Microsoft Teams
description: 'Используйте отчеты об использовании устройств Microsoft Teams, чтобы получить сведения об использовании устройств Microsoft Teams в вашей организации. '
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: b9a4d2ab3034281970a3e342aa0a2d78e53678e5
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766114"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="acf6d-103">Отчеты об использовании устройств Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="acf6d-103">Microsoft Teams device usage reports</span></span>

<span data-ttu-id="acf6d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acf6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acf6d-105">Используйте отчеты об использовании устройств Microsoft Teams, чтобы получить сведения об использовании устройств Microsoft Teams в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="acf6d-105">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="acf6d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="acf6d-106">Methods</span></span>

| <span data-ttu-id="acf6d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="acf6d-107">Method</span></span>                                                       | <span data-ttu-id="acf6d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="acf6d-108">Return Type</span></span>                                                  | <span data-ttu-id="acf6d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="acf6d-109">Description</span></span>                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| [<span data-ttu-id="acf6d-110">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="acf6d-110">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="acf6d-111">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="acf6d-111">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="acf6d-112">Получение сведений об использовании устройств Microsoft Teams отдельными пользователями.</span><span class="sxs-lookup"><span data-stu-id="acf6d-112">Get details about Microsoft Teams device usage by user.</span></span>      |
| [<span data-ttu-id="acf6d-113">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="acf6d-113">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="acf6d-114">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="acf6d-114">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="acf6d-115">Получите количество ежедневных уникальных пользователей Microsoft Teams, лицензированных по типу устройства.</span><span class="sxs-lookup"><span data-stu-id="acf6d-115">Get the number of daily unique Microsoft Teams licensed users by device type.</span></span> |
| [<span data-ttu-id="acf6d-116">Общее количество пользователей</span><span class="sxs-lookup"><span data-stu-id="acf6d-116">Get total user counts</span></span>](../api/reportroot-getteamsdeviceusagetotalusercounts.md) | [<span data-ttu-id="acf6d-117">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="acf6d-117">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="acf6d-118">Получите число ежедневных уникальных пользователей Microsoft Teams, лицензированных или не лицензированных по типу устройства.</span><span class="sxs-lookup"><span data-stu-id="acf6d-118">Get the number of daily unique Microsoft Teams licensed or non-licensed users by device type.</span></span> |
| [<span data-ttu-id="acf6d-119">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="acf6d-119">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="acf6d-120">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="acf6d-120">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="acf6d-121">Получите количество уникальных лицензированных пользователей Microsoft Teams по типу устройства за выбранный период времени.</span><span class="sxs-lookup"><span data-stu-id="acf6d-121">Get the number of unique Microsoft Teams licensed users by device type over the selected time period.</span></span> |
| [<span data-ttu-id="acf6d-122">Общее количество пользователей в распределении</span><span class="sxs-lookup"><span data-stu-id="acf6d-122">Get distribution total user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributiontotalusercounts.md) | [<span data-ttu-id="acf6d-123">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="acf6d-123">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="acf6d-124">Получите число уникальных пользователей Microsoft Teams, лицензированных или не лицензированных по типу устройства за выбранный период времени.</span><span class="sxs-lookup"><span data-stu-id="acf6d-124">Get the number of unique Microsoft Teams licensed or non-licensed users by device type over the selected time period.</span></span> |


