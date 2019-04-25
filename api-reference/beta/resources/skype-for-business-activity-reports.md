---
title: Отчеты о работе со Skype для бизнеса
description: Вы можете получить подробные сведения об активности в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3f843efc6834ee59872e7bf750174558cdb0a103
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551906"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="df6d8-104">Отчеты о работе со Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="df6d8-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df6d8-105">Вы можете получить подробные сведения об активности в Организации.</span><span class="sxs-lookup"><span data-stu-id="df6d8-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="df6d8-106">Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.</span><span class="sxs-lookup"><span data-stu-id="df6d8-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="df6d8-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="df6d8-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="df6d8-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="df6d8-108">Reports</span></span>

| <span data-ttu-id="df6d8-109">Функция</span><span class="sxs-lookup"><span data-stu-id="df6d8-109">Function</span></span>                                 | <span data-ttu-id="df6d8-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="df6d8-110">CSV return type</span></span> | <span data-ttu-id="df6d8-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="df6d8-111">JSON return type</span></span>                         | <span data-ttu-id="df6d8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="df6d8-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="df6d8-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="df6d8-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="df6d8-114">Поток</span><span class="sxs-lookup"><span data-stu-id="df6d8-114">Stream</span></span>          | [<span data-ttu-id="df6d8-115">Скипефорбусинессактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="df6d8-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="df6d8-116">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="df6d8-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="df6d8-117">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="df6d8-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="df6d8-118">Stream</span><span class="sxs-lookup"><span data-stu-id="df6d8-118">Stream</span></span>          | [<span data-ttu-id="df6d8-119">Скипефорбусинессактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="df6d8-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="df6d8-120">Отслеживайте, как меняется количество организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="df6d8-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="df6d8-121">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="df6d8-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="df6d8-122">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="df6d8-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="df6d8-123">Поток</span><span class="sxs-lookup"><span data-stu-id="df6d8-123">Stream</span></span>          | [<span data-ttu-id="df6d8-124">Скипефорбусинессактивитюсеркаунтс</span><span class="sxs-lookup"><span data-stu-id="df6d8-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="df6d8-125">Отслеживайте, как меняется количество уникальных организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="df6d8-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="df6d8-126">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="df6d8-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
