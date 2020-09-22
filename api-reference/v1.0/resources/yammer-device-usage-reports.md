---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: fccfdddef78ffb75ff79c6c8088035277a7fb2c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074827"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="08c91-104">Отчеты об использовании устройств с Yammer</span><span class="sxs-lookup"><span data-stu-id="08c91-104">Yammer device usage reports</span></span>

<span data-ttu-id="08c91-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08c91-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08c91-106">Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей.</span><span class="sxs-lookup"><span data-stu-id="08c91-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="08c91-107">Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.</span><span class="sxs-lookup"><span data-stu-id="08c91-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="08c91-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Device Device Usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="08c91-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="08c91-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="08c91-109">Reports</span></span>

| <span data-ttu-id="08c91-110">Функция</span><span class="sxs-lookup"><span data-stu-id="08c91-110">Function</span></span>                                 | <span data-ttu-id="08c91-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="08c91-111">Return Type</span></span> | <span data-ttu-id="08c91-112">Описание</span><span class="sxs-lookup"><span data-stu-id="08c91-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="08c91-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="08c91-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="08c91-114">Stream</span><span class="sxs-lookup"><span data-stu-id="08c91-114">Stream</span></span>      | <span data-ttu-id="08c91-115">Получение сведений об использовании устройств с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="08c91-115">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="08c91-116">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="08c91-116">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="08c91-117">Stream</span><span class="sxs-lookup"><span data-stu-id="08c91-117">Stream</span></span>      | <span data-ttu-id="08c91-118">Получение сведений о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="08c91-118">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="08c91-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="08c91-119">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="08c91-120">Stream</span><span class="sxs-lookup"><span data-stu-id="08c91-120">Stream</span></span>      | <span data-ttu-id="08c91-121">Получение сведений о количестве пользователей в день с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="08c91-121">Get the number of daily users by device type.</span></span> |

