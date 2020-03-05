---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 02d5f3bcb71b343b0406536d77d80d477cc71223
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519052"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="776d7-104">Отчеты об использовании устройств с Yammer</span><span class="sxs-lookup"><span data-stu-id="776d7-104">Yammer device usage reports</span></span>

<span data-ttu-id="776d7-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="776d7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="776d7-106">Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей.</span><span class="sxs-lookup"><span data-stu-id="776d7-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="776d7-107">Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.</span><span class="sxs-lookup"><span data-stu-id="776d7-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="776d7-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="776d7-108">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="776d7-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="776d7-109">Reports</span></span>

| <span data-ttu-id="776d7-110">Функция</span><span class="sxs-lookup"><span data-stu-id="776d7-110">Function</span></span>                                 | <span data-ttu-id="776d7-111">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="776d7-111">CSV return type</span></span> | <span data-ttu-id="776d7-112">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="776d7-112">JSON return type</span></span>                         | <span data-ttu-id="776d7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="776d7-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="776d7-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="776d7-114">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="776d7-115">Поток</span><span class="sxs-lookup"><span data-stu-id="776d7-115">Stream</span></span>          | [<span data-ttu-id="776d7-116">яммердевицеусажеусердетаил</span><span class="sxs-lookup"><span data-stu-id="776d7-116">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="776d7-117">Получение сведений об использовании устройств с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="776d7-117">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="776d7-118">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="776d7-118">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="776d7-119">Stream</span><span class="sxs-lookup"><span data-stu-id="776d7-119">Stream</span></span>          | [<span data-ttu-id="776d7-120">яммердевицеусажедистрибутионусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="776d7-120">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="776d7-121">Получение сведений о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="776d7-121">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="776d7-122">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="776d7-122">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="776d7-123">Stream</span><span class="sxs-lookup"><span data-stu-id="776d7-123">Stream</span></span>          | [<span data-ttu-id="776d7-124">яммердевицеусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="776d7-124">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="776d7-125">Получение сведений о количестве пользователей в день с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="776d7-125">Get the number of daily users by device type.</span></span> |
