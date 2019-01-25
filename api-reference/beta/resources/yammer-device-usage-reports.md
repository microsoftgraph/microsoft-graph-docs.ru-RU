---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f5b24d6d235a8719f5f4b7df0389b5e5971dd8cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521868"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="ca0c3-104">Отчеты об использовании устройств с Yammer</span><span class="sxs-lookup"><span data-stu-id="ca0c3-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca0c3-105">Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей.</span><span class="sxs-lookup"><span data-stu-id="ca0c3-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="ca0c3-106">Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.</span><span class="sxs-lookup"><span data-stu-id="ca0c3-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="ca0c3-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="ca0c3-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="ca0c3-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="ca0c3-108">Reports</span></span>

| <span data-ttu-id="ca0c3-109">Функция</span><span class="sxs-lookup"><span data-stu-id="ca0c3-109">Function</span></span>                                 | <span data-ttu-id="ca0c3-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="ca0c3-110">CSV return type</span></span> | <span data-ttu-id="ca0c3-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="ca0c3-111">JSON return type</span></span>                         | <span data-ttu-id="ca0c3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ca0c3-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ca0c3-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="ca0c3-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="ca0c3-114">Stream</span><span class="sxs-lookup"><span data-stu-id="ca0c3-114">Stream</span></span>          | [<span data-ttu-id="ca0c3-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="ca0c3-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="ca0c3-116">Получение сведений об использовании устройств с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="ca0c3-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="ca0c3-117">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="ca0c3-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="ca0c3-118">Stream</span><span class="sxs-lookup"><span data-stu-id="ca0c3-118">Stream</span></span>          | [<span data-ttu-id="ca0c3-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ca0c3-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="ca0c3-120">Получение сведений о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="ca0c3-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="ca0c3-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="ca0c3-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="ca0c3-122">Поток</span><span class="sxs-lookup"><span data-stu-id="ca0c3-122">Stream</span></span>          | [<span data-ttu-id="ca0c3-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ca0c3-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="ca0c3-124">Получение сведений о количестве пользователей в день с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="ca0c3-124">Get the number of daily users by device type.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
