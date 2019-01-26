---
title: Отчеты о действиях в SharePoint
description: Можно получить активности каждый пользователь с лицензии на использование SharePoint, посмотрев их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 98d0393545963a73852197f5bd78241cfb958a22
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577118"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="e1b43-104">Отчеты о действиях в SharePoint</span><span class="sxs-lookup"><span data-stu-id="e1b43-104">SharePoint activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1b43-105">Можно получить активности каждый пользователь с лицензии на использование SharePoint, посмотрев их взаимодействие с файлами.</span><span class="sxs-lookup"><span data-stu-id="e1b43-105">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="e1b43-106">Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.</span><span class="sxs-lookup"><span data-stu-id="e1b43-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="e1b43-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="e1b43-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="e1b43-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="e1b43-108">Reports</span></span>

| <span data-ttu-id="e1b43-109">Функция</span><span class="sxs-lookup"><span data-stu-id="e1b43-109">Function</span></span>                                 | <span data-ttu-id="e1b43-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="e1b43-110">CSV Return Type</span></span> | <span data-ttu-id="e1b43-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="e1b43-111">JSON Return Type</span></span>                         | <span data-ttu-id="e1b43-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e1b43-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e1b43-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="e1b43-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="e1b43-114">Stream</span><span class="sxs-lookup"><span data-stu-id="e1b43-114">Stream</span></span>          | [<span data-ttu-id="e1b43-115">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e1b43-115">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="e1b43-116">Получите сведения о действиях в SharePoint с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="e1b43-116">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="e1b43-117">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="e1b43-117">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="e1b43-118">Stream</span><span class="sxs-lookup"><span data-stu-id="e1b43-118">Stream</span></span>          | [<span data-ttu-id="e1b43-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e1b43-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="e1b43-120">Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e1b43-120">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="e1b43-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="e1b43-121">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="e1b43-122">Stream</span><span class="sxs-lookup"><span data-stu-id="e1b43-122">Stream</span></span>          | [<span data-ttu-id="e1b43-123">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="e1b43-123">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="e1b43-124">Отслеживайте, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="e1b43-124">Get the trend in the number of active users.</span></span> <span data-ttu-id="e1b43-125">Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="e1b43-125">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="e1b43-126">Получение страниц</span><span class="sxs-lookup"><span data-stu-id="e1b43-126">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="e1b43-127">Stream</span><span class="sxs-lookup"><span data-stu-id="e1b43-127">Stream</span></span>          | [<span data-ttu-id="e1b43-128">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="e1b43-128">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="e1b43-129">Получите количество уникальных страниц, посещенных пользователями.</span><span class="sxs-lookup"><span data-stu-id="e1b43-129">Get the number of unique pages visited by users.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
