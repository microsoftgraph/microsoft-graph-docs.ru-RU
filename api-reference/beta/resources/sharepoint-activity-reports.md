---
title: Отчеты о действиях в SharePoint
description: Вы можете получить действия каждого пользователя с лицензией на использование SharePoint, изусмотрив их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 2e7b834f9bd4e1a440f0fd5167679ce0074668cd
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983787"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="22446-104">Отчеты о действиях в SharePoint</span><span class="sxs-lookup"><span data-stu-id="22446-104">SharePoint activity reports</span></span>

<span data-ttu-id="22446-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22446-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22446-106">Вы можете получить действия каждого пользователя с лицензией на использование SharePoint, изусмотрив их взаимодействие с файлами.</span><span class="sxs-lookup"><span data-stu-id="22446-106">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="22446-107">Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.</span><span class="sxs-lookup"><span data-stu-id="22446-107">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="22446-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 : действия в SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="22446-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="22446-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="22446-109">Reports</span></span>

| <span data-ttu-id="22446-110">Функция</span><span class="sxs-lookup"><span data-stu-id="22446-110">Function</span></span>                                 | <span data-ttu-id="22446-111">Тип возврата CSV</span><span class="sxs-lookup"><span data-stu-id="22446-111">CSV Return Type</span></span> | <span data-ttu-id="22446-112">Тип возвращаемого JSON</span><span class="sxs-lookup"><span data-stu-id="22446-112">JSON Return Type</span></span>                         | <span data-ttu-id="22446-113">Описание</span><span class="sxs-lookup"><span data-stu-id="22446-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="22446-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="22446-114">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="22446-115">Stream</span><span class="sxs-lookup"><span data-stu-id="22446-115">Stream</span></span>          | [<span data-ttu-id="22446-116">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="22446-116">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="22446-117">Получите сведения о действиях в SharePoint с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="22446-117">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="22446-118">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="22446-118">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="22446-119">Stream</span><span class="sxs-lookup"><span data-stu-id="22446-119">Stream</span></span>          | [<span data-ttu-id="22446-120">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="22446-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="22446-121">Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="22446-121">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="22446-122">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="22446-122">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="22446-123">Stream</span><span class="sxs-lookup"><span data-stu-id="22446-123">Stream</span></span>          | [<span data-ttu-id="22446-124">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="22446-124">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="22446-125">Получение сведений о том, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="22446-125">Get the trend in the number of active users.</span></span> <span data-ttu-id="22446-126">Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="22446-126">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="22446-127">Получение страниц</span><span class="sxs-lookup"><span data-stu-id="22446-127">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="22446-128">Stream</span><span class="sxs-lookup"><span data-stu-id="22446-128">Stream</span></span>          | [<span data-ttu-id="22446-129">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="22446-129">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="22446-130">Получите количество уникальных страниц, посещенных пользователями.</span><span class="sxs-lookup"><span data-stu-id="22446-130">Get the number of unique pages visited by users.</span></span> |


