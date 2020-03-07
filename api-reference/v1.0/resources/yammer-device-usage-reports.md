---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 3e2c91db77fbd57118c340d2d51a3bcd67ac0641
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446641"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="b2808-104">Отчеты об использовании устройств с Yammer</span><span class="sxs-lookup"><span data-stu-id="b2808-104">Yammer device usage reports</span></span>

<span data-ttu-id="b2808-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2808-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2808-106">Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей.</span><span class="sxs-lookup"><span data-stu-id="b2808-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="b2808-107">Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.</span><span class="sxs-lookup"><span data-stu-id="b2808-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="b2808-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="b2808-108">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="b2808-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="b2808-109">Reports</span></span>

| <span data-ttu-id="b2808-110">Функция</span><span class="sxs-lookup"><span data-stu-id="b2808-110">Function</span></span>                                 | <span data-ttu-id="b2808-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b2808-111">Return Type</span></span> | <span data-ttu-id="b2808-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b2808-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="b2808-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="b2808-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="b2808-114">Поток</span><span class="sxs-lookup"><span data-stu-id="b2808-114">Stream</span></span>      | <span data-ttu-id="b2808-115">Получение сведений об использовании устройств с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="b2808-115">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="b2808-116">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="b2808-116">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="b2808-117">Stream</span><span class="sxs-lookup"><span data-stu-id="b2808-117">Stream</span></span>      | <span data-ttu-id="b2808-118">Получение сведений о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="b2808-118">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="b2808-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="b2808-119">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="b2808-120">Stream</span><span class="sxs-lookup"><span data-stu-id="b2808-120">Stream</span></span>      | <span data-ttu-id="b2808-121">Получение сведений о количестве пользователей в день с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="b2808-121">Get the number of daily users by device type.</span></span> |
