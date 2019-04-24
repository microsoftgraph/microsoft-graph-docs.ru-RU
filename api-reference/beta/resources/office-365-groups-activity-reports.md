---
title: Отчеты об активности в группах Office 365
description: Вы можете получить представление об активности групп Office 365 в Организации и узнать, сколько групп Office 365 создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e698a1096d244b864bbb15cf06c16e8cf79ff1f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505579"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="23bc5-103">Отчеты об активности в группах Office 365</span><span class="sxs-lookup"><span data-stu-id="23bc5-103">Office 365 Groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23bc5-104">Вы можете получить представление об активности групп Office 365 в Организации и узнать, сколько групп Office 365 создается и используется.</span><span class="sxs-lookup"><span data-stu-id="23bc5-104">You can gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 groups are being created and used.</span></span>

> <span data-ttu-id="23bc5-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="23bc5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="23bc5-106">Отчеты</span><span class="sxs-lookup"><span data-stu-id="23bc5-106">Reports</span></span>

| <span data-ttu-id="23bc5-107">Функция</span><span class="sxs-lookup"><span data-stu-id="23bc5-107">Function</span></span>                                 | <span data-ttu-id="23bc5-108">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="23bc5-108">CSV return type</span></span> | <span data-ttu-id="23bc5-109">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="23bc5-109">JSON return type</span></span>                         | <span data-ttu-id="23bc5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="23bc5-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="23bc5-111">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="23bc5-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="23bc5-112">Stream</span><span class="sxs-lookup"><span data-stu-id="23bc5-112">Stream</span></span>          | [<span data-ttu-id="23bc5-113">office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="23bc5-113">office365GroupsActivityDetail</span></span>](../resources/office365groupsactivitydetail.md) | <span data-ttu-id="23bc5-114">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="23bc5-114">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="23bc5-115">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="23bc5-115">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="23bc5-116">Stream</span><span class="sxs-lookup"><span data-stu-id="23bc5-116">Stream</span></span>          | [<span data-ttu-id="23bc5-117">office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="23bc5-117">office365GroupsActivityCounts</span></span>](../resources/office365groupsactivitycounts.md) | <span data-ttu-id="23bc5-118">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="23bc5-118">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="23bc5-119">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="23bc5-119">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="23bc5-120">Stream</span><span class="sxs-lookup"><span data-stu-id="23bc5-120">Stream</span></span>          | [<span data-ttu-id="23bc5-121">office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="23bc5-121">office365GroupsActivityGroupCounts</span></span>](../resources/office365groupsactivitygroupcounts.md) | <span data-ttu-id="23bc5-122">Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.</span><span class="sxs-lookup"><span data-stu-id="23bc5-122">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="23bc5-123">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="23bc5-123">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="23bc5-124">Stream</span><span class="sxs-lookup"><span data-stu-id="23bc5-124">Stream</span></span>          | [<span data-ttu-id="23bc5-125">office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="23bc5-125">office365GroupsActivityStorage</span></span>](../resources/office365groupsactivitystorage.md) | <span data-ttu-id="23bc5-126">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="23bc5-126">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="23bc5-127">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="23bc5-127">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="23bc5-128">Поток</span><span class="sxs-lookup"><span data-stu-id="23bc5-128">Stream</span></span>          | [<span data-ttu-id="23bc5-129">office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="23bc5-129">office365GroupsActivityFileCounts</span></span>](../resources/office365groupsactivityfilecounts.md) | <span data-ttu-id="23bc5-130">Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны.</span><span class="sxs-lookup"><span data-stu-id="23bc5-130">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
