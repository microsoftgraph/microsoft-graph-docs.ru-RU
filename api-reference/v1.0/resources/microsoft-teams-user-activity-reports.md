---
title: Отчеты о действиях пользователей Microsoft Teams
description: С помощью отчетов о действиях пользователей Microsoft Teams можно анализировать действия пользователей Microsoft Teams в организации.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: adde0eecbfe468b5eac45bf0c0d496d430947284
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447390"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="b0dc5-103">Отчеты о действиях пользователей Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b0dc5-103">Microsoft Teams user activity reports</span></span>

<span data-ttu-id="b0dc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0dc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0dc5-105">С помощью отчетов о действиях пользователей Microsoft Teams можно анализировать действия пользователей Microsoft Teams в организации.</span><span class="sxs-lookup"><span data-stu-id="b0dc5-105">Use the Microsoft Teams activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="b0dc5-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b0dc5-106">Methods</span></span>

| <span data-ttu-id="b0dc5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b0dc5-107">Method</span></span>                                   | <span data-ttu-id="b0dc5-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b0dc5-108">Return Type</span></span> | <span data-ttu-id="b0dc5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b0dc5-109">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="b0dc5-110">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="b0dc5-110">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | <span data-ttu-id="b0dc5-111">Stream</span><span class="sxs-lookup"><span data-stu-id="b0dc5-111">Stream</span></span>      | <span data-ttu-id="b0dc5-112">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b0dc5-112">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="b0dc5-113">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="b0dc5-113">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | <span data-ttu-id="b0dc5-114">Stream</span><span class="sxs-lookup"><span data-stu-id="b0dc5-114">Stream</span></span>      | <span data-ttu-id="b0dc5-115">Получение количества действий Microsoft Teams по типам.</span><span class="sxs-lookup"><span data-stu-id="b0dc5-115">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="b0dc5-116">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="b0dc5-116">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="b0dc5-117">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="b0dc5-117">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | <span data-ttu-id="b0dc5-118">Stream</span><span class="sxs-lookup"><span data-stu-id="b0dc5-118">Stream</span></span>      | <span data-ttu-id="b0dc5-119">Получение сведений о количестве пользователей по типам действий.</span><span class="sxs-lookup"><span data-stu-id="b0dc5-119">Get the number of users by activity type.</span></span> <span data-ttu-id="b0dc5-120">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="b0dc5-120">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
