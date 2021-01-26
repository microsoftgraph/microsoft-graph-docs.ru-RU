---
title: Отчеты о работе со Skype для бизнеса
description: Вы можете получить сведения о действиях в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 0fe3236fc8c4f29357e2ae3fae45c80969c353db
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980649"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="89e2a-104">Отчеты о работе со Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="89e2a-104">Skype for Business activity reports</span></span>

<span data-ttu-id="89e2a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89e2a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89e2a-106">Вы можете получить сведения о действиях в организации.</span><span class="sxs-lookup"><span data-stu-id="89e2a-106">You can get details on activity across your organization.</span></span> <span data-ttu-id="89e2a-107">Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.</span><span class="sxs-lookup"><span data-stu-id="89e2a-107">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="89e2a-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Microsoft 365: действия в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="89e2a-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="89e2a-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="89e2a-109">Reports</span></span>

| <span data-ttu-id="89e2a-110">Функция</span><span class="sxs-lookup"><span data-stu-id="89e2a-110">Function</span></span>                                 | <span data-ttu-id="89e2a-111">Тип возврата CSV</span><span class="sxs-lookup"><span data-stu-id="89e2a-111">CSV return type</span></span> | <span data-ttu-id="89e2a-112">Тип возврата JSON</span><span class="sxs-lookup"><span data-stu-id="89e2a-112">JSON return type</span></span>                         | <span data-ttu-id="89e2a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="89e2a-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="89e2a-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="89e2a-114">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="89e2a-115">Stream</span><span class="sxs-lookup"><span data-stu-id="89e2a-115">Stream</span></span>          | [<span data-ttu-id="89e2a-116">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="89e2a-116">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="89e2a-117">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="89e2a-117">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="89e2a-118">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="89e2a-118">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="89e2a-119">Stream</span><span class="sxs-lookup"><span data-stu-id="89e2a-119">Stream</span></span>          | [<span data-ttu-id="89e2a-120">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="89e2a-120">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="89e2a-121">Отслеживайте, как меняется количество организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="89e2a-121">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="89e2a-122">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="89e2a-122">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="89e2a-123">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="89e2a-123">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="89e2a-124">Stream</span><span class="sxs-lookup"><span data-stu-id="89e2a-124">Stream</span></span>          | [<span data-ttu-id="89e2a-125">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="89e2a-125">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="89e2a-126">Отслеживайте, как меняется количество уникальных организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="89e2a-126">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="89e2a-127">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="89e2a-127">The report also includes the number of peer-to-peer sessions.</span></span> |


