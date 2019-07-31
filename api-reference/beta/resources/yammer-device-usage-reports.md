---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f36ed78805bc664adfbbd4ced9bc86b1444ab262
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007006"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="eebd1-104">Отчеты об использовании устройств с Yammer</span><span class="sxs-lookup"><span data-stu-id="eebd1-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eebd1-105">Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей.</span><span class="sxs-lookup"><span data-stu-id="eebd1-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="eebd1-106">Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.</span><span class="sxs-lookup"><span data-stu-id="eebd1-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="eebd1-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="eebd1-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="eebd1-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="eebd1-108">Reports</span></span>

| <span data-ttu-id="eebd1-109">Функция</span><span class="sxs-lookup"><span data-stu-id="eebd1-109">Function</span></span>                                 | <span data-ttu-id="eebd1-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="eebd1-110">CSV return type</span></span> | <span data-ttu-id="eebd1-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="eebd1-111">JSON return type</span></span>                         | <span data-ttu-id="eebd1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="eebd1-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="eebd1-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="eebd1-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="eebd1-114">Поток</span><span class="sxs-lookup"><span data-stu-id="eebd1-114">Stream</span></span>          | [<span data-ttu-id="eebd1-115">Яммердевицеусажеусердетаил</span><span class="sxs-lookup"><span data-stu-id="eebd1-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="eebd1-116">Получение сведений об использовании устройств с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="eebd1-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="eebd1-117">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="eebd1-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="eebd1-118">Stream</span><span class="sxs-lookup"><span data-stu-id="eebd1-118">Stream</span></span>          | [<span data-ttu-id="eebd1-119">Яммердевицеусажедистрибутионусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="eebd1-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="eebd1-120">Получение сведений о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="eebd1-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="eebd1-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="eebd1-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="eebd1-122">Поток</span><span class="sxs-lookup"><span data-stu-id="eebd1-122">Stream</span></span>          | [<span data-ttu-id="eebd1-123">Яммердевицеусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="eebd1-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="eebd1-124">Получение сведений о количестве пользователей в день с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="eebd1-124">Get the number of daily users by device type.</span></span> |
