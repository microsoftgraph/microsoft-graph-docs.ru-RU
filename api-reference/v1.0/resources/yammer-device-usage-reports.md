---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f4736d92a990c94d2017cc8a26396a3cc4f6e04f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897752"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="61fbc-104">Отчеты об использовании устройств с Yammer</span><span class="sxs-lookup"><span data-stu-id="61fbc-104">Yammer device usage reports</span></span>

<span data-ttu-id="61fbc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61fbc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61fbc-106">Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей.</span><span class="sxs-lookup"><span data-stu-id="61fbc-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="61fbc-107">Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.</span><span class="sxs-lookup"><span data-stu-id="61fbc-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="61fbc-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Device Device Usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="61fbc-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="61fbc-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="61fbc-109">Reports</span></span>

| <span data-ttu-id="61fbc-110">Функция</span><span class="sxs-lookup"><span data-stu-id="61fbc-110">Function</span></span>                                 | <span data-ttu-id="61fbc-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="61fbc-111">Return Type</span></span> | <span data-ttu-id="61fbc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="61fbc-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="61fbc-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="61fbc-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="61fbc-114">Поток</span><span class="sxs-lookup"><span data-stu-id="61fbc-114">Stream</span></span>      | <span data-ttu-id="61fbc-115">Получение сведений об использовании устройств с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="61fbc-115">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="61fbc-116">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="61fbc-116">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="61fbc-117">Stream</span><span class="sxs-lookup"><span data-stu-id="61fbc-117">Stream</span></span>      | <span data-ttu-id="61fbc-118">Получение сведений о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="61fbc-118">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="61fbc-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="61fbc-119">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="61fbc-120">Stream</span><span class="sxs-lookup"><span data-stu-id="61fbc-120">Stream</span></span>      | <span data-ttu-id="61fbc-121">Получение сведений о количестве пользователей в день с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="61fbc-121">Get the number of daily users by device type.</span></span> |
