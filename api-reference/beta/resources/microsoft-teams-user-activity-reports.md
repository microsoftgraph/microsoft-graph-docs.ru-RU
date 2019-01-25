---
title: Отчеты о действиях пользователей Microsoft Teams
description: Использование отчетов об активности пользователей группами Майкрософт для получения полезные сведения о в действие пользователя группами Майкрософт в вашей организации.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 447aa9d36208ae9c966d86e733e99f81ab01e6ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517703"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="c248e-103">Отчеты о действиях пользователей Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c248e-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c248e-104">Использование отчетов об активности пользователей группами Майкрософт для получения полезные сведения о в действие пользователя группами Майкрософт в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="c248e-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="c248e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c248e-105">Methods</span></span>

| <span data-ttu-id="c248e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="c248e-106">Method</span></span>                                   | <span data-ttu-id="c248e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c248e-107">Return Type</span></span>                              | <span data-ttu-id="c248e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c248e-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="c248e-109">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="c248e-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="c248e-110">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c248e-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="c248e-111">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c248e-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="c248e-112">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="c248e-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="c248e-113">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="c248e-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="c248e-114">Получение количества действий Microsoft Teams по типам.</span><span class="sxs-lookup"><span data-stu-id="c248e-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="c248e-115">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="c248e-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="c248e-116">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="c248e-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="c248e-117">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="c248e-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="c248e-118">Получение сведений о количестве пользователей по типам действий.</span><span class="sxs-lookup"><span data-stu-id="c248e-118">Get the number of users by activity type.</span></span> <span data-ttu-id="c248e-119">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="c248e-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
