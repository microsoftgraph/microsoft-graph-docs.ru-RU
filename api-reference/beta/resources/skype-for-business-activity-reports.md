---
title: Отчеты о работе со Skype для бизнеса
description: Вы можете получить подробные сведения об активности в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: a66780b54239ab6bb87e8c910734a0c1a4ca32fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520494"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="5f29c-104">Отчеты о работе со Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="5f29c-104">Skype for Business activity reports</span></span>

<span data-ttu-id="5f29c-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5f29c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f29c-106">Вы можете получить подробные сведения об активности в Организации.</span><span class="sxs-lookup"><span data-stu-id="5f29c-106">You can get details on activity across your organization.</span></span> <span data-ttu-id="5f29c-107">Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.</span><span class="sxs-lookup"><span data-stu-id="5f29c-107">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="5f29c-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="5f29c-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="5f29c-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="5f29c-109">Reports</span></span>

| <span data-ttu-id="5f29c-110">Функция</span><span class="sxs-lookup"><span data-stu-id="5f29c-110">Function</span></span>                                 | <span data-ttu-id="5f29c-111">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="5f29c-111">CSV return type</span></span> | <span data-ttu-id="5f29c-112">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="5f29c-112">JSON return type</span></span>                         | <span data-ttu-id="5f29c-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5f29c-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="5f29c-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="5f29c-114">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="5f29c-115">Stream</span><span class="sxs-lookup"><span data-stu-id="5f29c-115">Stream</span></span>          | [<span data-ttu-id="5f29c-116">скипефорбусинессактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="5f29c-116">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="5f29c-117">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5f29c-117">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="5f29c-118">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="5f29c-118">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="5f29c-119">Stream</span><span class="sxs-lookup"><span data-stu-id="5f29c-119">Stream</span></span>          | [<span data-ttu-id="5f29c-120">скипефорбусинессактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="5f29c-120">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="5f29c-121">Отслеживайте, как меняется количество организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5f29c-121">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="5f29c-122">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="5f29c-122">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="5f29c-123">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="5f29c-123">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="5f29c-124">Stream</span><span class="sxs-lookup"><span data-stu-id="5f29c-124">Stream</span></span>          | [<span data-ttu-id="5f29c-125">скипефорбусинессактивитюсеркаунтс</span><span class="sxs-lookup"><span data-stu-id="5f29c-125">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="5f29c-126">Отслеживайте, как меняется количество уникальных организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5f29c-126">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="5f29c-127">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="5f29c-127">The report also includes the number of peer-to-peer sessions.</span></span> |
