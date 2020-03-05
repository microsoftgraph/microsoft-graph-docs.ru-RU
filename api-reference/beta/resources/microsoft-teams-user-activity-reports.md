---
title: Отчеты о действиях пользователей Microsoft Teams
description: Используйте отчеты об активности пользователей Microsoft Teams, чтобы получить информацию о действиях пользователей Microsoft Teams в вашей организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: c5807af05bda74019ac8b28c53f902ecac6f8e2a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522633"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="0c5bb-103">Отчеты о действиях пользователей Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0c5bb-103">Microsoft Teams user activity reports</span></span>

<span data-ttu-id="0c5bb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0c5bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c5bb-105">Используйте отчеты об активности пользователей Microsoft Teams, чтобы получить информацию о действиях пользователей Microsoft Teams в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="0c5bb-105">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="0c5bb-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0c5bb-106">Methods</span></span>

| <span data-ttu-id="0c5bb-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0c5bb-107">Method</span></span>                                   | <span data-ttu-id="0c5bb-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c5bb-108">Return Type</span></span>                              | <span data-ttu-id="0c5bb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0c5bb-109">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="0c5bb-110">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="0c5bb-110">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="0c5bb-111">теамсусерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="0c5bb-111">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="0c5bb-112">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0c5bb-112">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="0c5bb-113">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="0c5bb-113">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="0c5bb-114">теамсусерактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="0c5bb-114">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="0c5bb-115">Получение количества действий Microsoft Teams по типам.</span><span class="sxs-lookup"><span data-stu-id="0c5bb-115">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="0c5bb-116">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="0c5bb-116">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="0c5bb-117">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="0c5bb-117">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="0c5bb-118">теамсусерактивитюсеркаунтс</span><span class="sxs-lookup"><span data-stu-id="0c5bb-118">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="0c5bb-119">Получение сведений о количестве пользователей по типам действий.</span><span class="sxs-lookup"><span data-stu-id="0c5bb-119">Get the number of users by activity type.</span></span> <span data-ttu-id="0c5bb-120">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="0c5bb-120">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
