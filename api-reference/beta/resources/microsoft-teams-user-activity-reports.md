---
title: Отчеты о действиях пользователей Microsoft Teams
description: Используйте отчеты о действиях пользователей Microsoft Teams, чтобы получить представление о действиях пользователей Microsoft Teams в вашей организации.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: e249998d8c4481c7e3ef0b2fe31072fe59c84378
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980799"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="b36d1-103">Отчеты о действиях пользователей Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b36d1-103">Microsoft Teams user activity reports</span></span>

<span data-ttu-id="b36d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b36d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b36d1-105">Используйте отчеты о действиях пользователей Microsoft Teams, чтобы получить представление о действиях пользователей Microsoft Teams в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="b36d1-105">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="b36d1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b36d1-106">Methods</span></span>

| <span data-ttu-id="b36d1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b36d1-107">Method</span></span>                                   | <span data-ttu-id="b36d1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b36d1-108">Return Type</span></span>                              | <span data-ttu-id="b36d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b36d1-109">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="b36d1-110">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="b36d1-110">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="b36d1-111">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b36d1-111">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="b36d1-112">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b36d1-112">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="b36d1-113">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="b36d1-113">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="b36d1-114">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="b36d1-114">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="b36d1-115">Получение количества действий Microsoft Teams по типам.</span><span class="sxs-lookup"><span data-stu-id="b36d1-115">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="b36d1-116">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="b36d1-116">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="b36d1-117">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="b36d1-117">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="b36d1-118">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="b36d1-118">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="b36d1-119">Получение сведений о количестве пользователей по типам действий.</span><span class="sxs-lookup"><span data-stu-id="b36d1-119">Get the number of users by activity type.</span></span> <span data-ttu-id="b36d1-120">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="b36d1-120">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |


