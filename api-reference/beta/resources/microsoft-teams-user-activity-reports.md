---
title: Отчеты о действиях пользователей Microsoft Teams
description: Использование отчетов об активности пользователей группами Майкрософт для получения полезные сведения о в действие пользователя группами Майкрософт в вашей организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4a071fb38ce9fd76aff4ccdc648201f91a600f24
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574721"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="cdc43-103">Отчеты о действиях пользователей Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cdc43-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdc43-104">Использование отчетов об активности пользователей группами Майкрософт для получения полезные сведения о в действие пользователя группами Майкрософт в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="cdc43-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="cdc43-105">Методы</span><span class="sxs-lookup"><span data-stu-id="cdc43-105">Methods</span></span>

| <span data-ttu-id="cdc43-106">Метод</span><span class="sxs-lookup"><span data-stu-id="cdc43-106">Method</span></span>                                   | <span data-ttu-id="cdc43-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cdc43-107">Return Type</span></span>                              | <span data-ttu-id="cdc43-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cdc43-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="cdc43-109">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="cdc43-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="cdc43-110">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="cdc43-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="cdc43-111">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="cdc43-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="cdc43-112">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="cdc43-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="cdc43-113">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="cdc43-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="cdc43-114">Получение количества действий Microsoft Teams по типам.</span><span class="sxs-lookup"><span data-stu-id="cdc43-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="cdc43-115">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="cdc43-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="cdc43-116">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="cdc43-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="cdc43-117">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="cdc43-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="cdc43-118">Получение сведений о количестве пользователей по типам действий.</span><span class="sxs-lookup"><span data-stu-id="cdc43-118">Get the number of users by activity type.</span></span> <span data-ttu-id="cdc43-119">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="cdc43-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
