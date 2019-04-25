---
title: Отчеты о действиях в SharePoint
description: Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию на использование SharePoint, изучив их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 98d0393545963a73852197f5bd78241cfb958a22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584105"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="c9537-104">Отчеты о действиях в SharePoint</span><span class="sxs-lookup"><span data-stu-id="c9537-104">SharePoint activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9537-105">Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию на использование SharePoint, изучив их взаимодействие с файлами.</span><span class="sxs-lookup"><span data-stu-id="c9537-105">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="c9537-106">Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.</span><span class="sxs-lookup"><span data-stu-id="c9537-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="c9537-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="c9537-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="c9537-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="c9537-108">Reports</span></span>

| <span data-ttu-id="c9537-109">Функция</span><span class="sxs-lookup"><span data-stu-id="c9537-109">Function</span></span>                                 | <span data-ttu-id="c9537-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="c9537-110">CSV Return Type</span></span> | <span data-ttu-id="c9537-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="c9537-111">JSON Return Type</span></span>                         | <span data-ttu-id="c9537-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c9537-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="c9537-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="c9537-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="c9537-114">Поток</span><span class="sxs-lookup"><span data-stu-id="c9537-114">Stream</span></span>          | [<span data-ttu-id="c9537-115">Шарепоинтактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="c9537-115">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="c9537-116">Получите сведения о действиях в SharePoint с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="c9537-116">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="c9537-117">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="c9537-117">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="c9537-118">Поток</span><span class="sxs-lookup"><span data-stu-id="c9537-118">Stream</span></span>          | [<span data-ttu-id="c9537-119">Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="c9537-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="c9537-120">Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c9537-120">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="c9537-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="c9537-121">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="c9537-122">Поток</span><span class="sxs-lookup"><span data-stu-id="c9537-122">Stream</span></span>          | [<span data-ttu-id="c9537-123">Шарепоинтактивитюсеркаунтс</span><span class="sxs-lookup"><span data-stu-id="c9537-123">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="c9537-124">Получение сведений о том, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="c9537-124">Get the trend in the number of active users.</span></span> <span data-ttu-id="c9537-125">Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="c9537-125">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="c9537-126">Получение страниц</span><span class="sxs-lookup"><span data-stu-id="c9537-126">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="c9537-127">Stream</span><span class="sxs-lookup"><span data-stu-id="c9537-127">Stream</span></span>          | [<span data-ttu-id="c9537-128">Шарепоинтактивитипажес</span><span class="sxs-lookup"><span data-stu-id="c9537-128">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="c9537-129">Получите количество уникальных страниц, посещенных пользователями.</span><span class="sxs-lookup"><span data-stu-id="c9537-129">Get the number of unique pages visited by users.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
