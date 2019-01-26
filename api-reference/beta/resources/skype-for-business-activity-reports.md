---
title: Отчеты о работе со Skype для бизнеса
description: Можно получить подробные сведения об активности внутри организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3f843efc6834ee59872e7bf750174558cdb0a103
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577384"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="fe928-104">Отчеты о работе со Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="fe928-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe928-105">Можно получить подробные сведения об активности внутри организации.</span><span class="sxs-lookup"><span data-stu-id="fe928-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="fe928-106">Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.</span><span class="sxs-lookup"><span data-stu-id="fe928-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="fe928-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="fe928-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="fe928-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="fe928-108">Reports</span></span>

| <span data-ttu-id="fe928-109">Функция</span><span class="sxs-lookup"><span data-stu-id="fe928-109">Function</span></span>                                 | <span data-ttu-id="fe928-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="fe928-110">CSV return type</span></span> | <span data-ttu-id="fe928-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="fe928-111">JSON return type</span></span>                         | <span data-ttu-id="fe928-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fe928-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="fe928-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="fe928-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="fe928-114">Stream</span><span class="sxs-lookup"><span data-stu-id="fe928-114">Stream</span></span>          | [<span data-ttu-id="fe928-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="fe928-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="fe928-116">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fe928-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="fe928-117">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="fe928-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="fe928-118">Stream</span><span class="sxs-lookup"><span data-stu-id="fe928-118">Stream</span></span>          | [<span data-ttu-id="fe928-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="fe928-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="fe928-120">Узнайте, как меняется количество организаторов и участников сеансов конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fe928-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="fe928-121">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="fe928-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="fe928-122">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="fe928-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="fe928-123">Stream</span><span class="sxs-lookup"><span data-stu-id="fe928-123">Stream</span></span>          | [<span data-ttu-id="fe928-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="fe928-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="fe928-125">Отследите, как меняется количество уникальных организаторов и участников сеансов конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fe928-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="fe928-126">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="fe928-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
