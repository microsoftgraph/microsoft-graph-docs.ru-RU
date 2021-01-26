---
title: Отчеты о действиях в Yammer
description: Вы можете понять уровень взаимодействия вашей организации с Yammer по уровню активности в организации и количеству уникальных пользователей, которые читают и читают сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: c0009949b5eb429f15155059768365b201078134
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982469"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="e9e67-103">Отчеты о действиях в Yammer</span><span class="sxs-lookup"><span data-stu-id="e9e67-103">Yammer activity reports</span></span>

<span data-ttu-id="e9e67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9e67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9e67-105">Вы можете понять уровень взаимодействия вашей организации с Yammer по уровню активности в организации и количеству уникальных пользователей, которые читают и читают сообщения в Yammer.</span><span class="sxs-lookup"><span data-stu-id="e9e67-105">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="e9e67-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 - Yammer Activity.](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)</span><span class="sxs-lookup"><span data-stu-id="e9e67-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="e9e67-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="e9e67-107">Reports</span></span>

| <span data-ttu-id="e9e67-108">Функция</span><span class="sxs-lookup"><span data-stu-id="e9e67-108">Function</span></span>                                 | <span data-ttu-id="e9e67-109">Тип возврата CSV</span><span class="sxs-lookup"><span data-stu-id="e9e67-109">CSV return type</span></span> | <span data-ttu-id="e9e67-110">Тип возврата JSON</span><span class="sxs-lookup"><span data-stu-id="e9e67-110">JSON return type</span></span>                         | <span data-ttu-id="e9e67-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e9e67-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e9e67-112">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="e9e67-112">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="e9e67-113">Stream</span><span class="sxs-lookup"><span data-stu-id="e9e67-113">Stream</span></span>          | [<span data-ttu-id="e9e67-114">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e9e67-114">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="e9e67-115">Получение сведений о действиях в Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="e9e67-115">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="e9e67-116">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="e9e67-116">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="e9e67-117">Stream</span><span class="sxs-lookup"><span data-stu-id="e9e67-117">Stream</span></span>          | [<span data-ttu-id="e9e67-118">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e9e67-118">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="e9e67-119">Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="e9e67-119">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="e9e67-120">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="e9e67-120">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="e9e67-121">Stream</span><span class="sxs-lookup"><span data-stu-id="e9e67-121">Stream</span></span>          | [<span data-ttu-id="e9e67-122">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e9e67-122">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="e9e67-123">Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.</span><span class="sxs-lookup"><span data-stu-id="e9e67-123">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |


