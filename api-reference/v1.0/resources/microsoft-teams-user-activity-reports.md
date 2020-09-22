---
title: Отчеты о действиях пользователей Microsoft Teams
description: С помощью отчетов о действиях пользователей Microsoft Teams можно анализировать действия пользователей Microsoft Teams в организации.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f5cdd3f41cf8454a660fc65c10683288a0752923
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083031"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="09770-103">Отчеты о действиях пользователей Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="09770-103">Microsoft Teams user activity reports</span></span>

<span data-ttu-id="09770-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09770-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09770-105">С помощью отчетов о действиях пользователей Microsoft Teams можно анализировать действия пользователей Microsoft Teams в организации.</span><span class="sxs-lookup"><span data-stu-id="09770-105">Use the Microsoft Teams activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="09770-106">Методы</span><span class="sxs-lookup"><span data-stu-id="09770-106">Methods</span></span>

| <span data-ttu-id="09770-107">Метод</span><span class="sxs-lookup"><span data-stu-id="09770-107">Method</span></span>                                   | <span data-ttu-id="09770-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="09770-108">Return Type</span></span> | <span data-ttu-id="09770-109">Описание</span><span class="sxs-lookup"><span data-stu-id="09770-109">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="09770-110">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="09770-110">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | <span data-ttu-id="09770-111">Stream</span><span class="sxs-lookup"><span data-stu-id="09770-111">Stream</span></span>      | <span data-ttu-id="09770-112">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="09770-112">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="09770-113">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="09770-113">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | <span data-ttu-id="09770-114">Stream</span><span class="sxs-lookup"><span data-stu-id="09770-114">Stream</span></span>      | <span data-ttu-id="09770-115">Получение количества действий Microsoft Teams по типам.</span><span class="sxs-lookup"><span data-stu-id="09770-115">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="09770-116">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="09770-116">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="09770-117">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="09770-117">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | <span data-ttu-id="09770-118">Stream</span><span class="sxs-lookup"><span data-stu-id="09770-118">Stream</span></span>      | <span data-ttu-id="09770-119">Получение сведений о количестве пользователей по типам действий.</span><span class="sxs-lookup"><span data-stu-id="09770-119">Get the number of users by activity type.</span></span> <span data-ttu-id="09770-120">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="09770-120">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |

