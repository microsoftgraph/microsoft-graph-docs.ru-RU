---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 57dcba3a91b15b4980d9e76b7aad6251008f5966
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577433"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="5382b-104">Отчеты об использовании устройств с Yammer</span><span class="sxs-lookup"><span data-stu-id="5382b-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5382b-105">Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей.</span><span class="sxs-lookup"><span data-stu-id="5382b-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="5382b-106">Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.</span><span class="sxs-lookup"><span data-stu-id="5382b-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="5382b-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="5382b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="5382b-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="5382b-108">Reports</span></span>

| <span data-ttu-id="5382b-109">Функция</span><span class="sxs-lookup"><span data-stu-id="5382b-109">Function</span></span>                                 | <span data-ttu-id="5382b-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="5382b-110">CSV return type</span></span> | <span data-ttu-id="5382b-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="5382b-111">JSON return type</span></span>                         | <span data-ttu-id="5382b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5382b-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="5382b-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="5382b-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="5382b-114">Stream</span><span class="sxs-lookup"><span data-stu-id="5382b-114">Stream</span></span>          | [<span data-ttu-id="5382b-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="5382b-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="5382b-116">Получение сведений об использовании устройств с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="5382b-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="5382b-117">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="5382b-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="5382b-118">Stream</span><span class="sxs-lookup"><span data-stu-id="5382b-118">Stream</span></span>          | [<span data-ttu-id="5382b-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="5382b-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="5382b-120">Получение сведений о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="5382b-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="5382b-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="5382b-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="5382b-122">Stream</span><span class="sxs-lookup"><span data-stu-id="5382b-122">Stream</span></span>          | [<span data-ttu-id="5382b-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="5382b-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="5382b-124">Получение сведений о количестве пользователей в день с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="5382b-124">Get the number of daily users by device type.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
