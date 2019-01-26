---
title: Отчеты об активности в группах Office 365
description: Можно воспользоваться сведениями в действие группы Office 365 в вашей организации и видеть, сколько групп Office 365 создаются и используются.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e698a1096d244b864bbb15cf06c16e8cf79ff1f2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572201"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="a1861-103">Отчеты об активности в группах Office 365</span><span class="sxs-lookup"><span data-stu-id="a1861-103">Office 365 Groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1861-104">Можно воспользоваться сведениями в действие группы Office 365 в вашей организации и видеть, сколько групп Office 365 создаются и используются.</span><span class="sxs-lookup"><span data-stu-id="a1861-104">You can gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 groups are being created and used.</span></span>

> <span data-ttu-id="a1861-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="a1861-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="a1861-106">Отчеты</span><span class="sxs-lookup"><span data-stu-id="a1861-106">Reports</span></span>

| <span data-ttu-id="a1861-107">Функция</span><span class="sxs-lookup"><span data-stu-id="a1861-107">Function</span></span>                                 | <span data-ttu-id="a1861-108">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="a1861-108">CSV return type</span></span> | <span data-ttu-id="a1861-109">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="a1861-109">JSON return type</span></span>                         | <span data-ttu-id="a1861-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a1861-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="a1861-111">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="a1861-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="a1861-112">Поток</span><span class="sxs-lookup"><span data-stu-id="a1861-112">Stream</span></span>          | [<span data-ttu-id="a1861-113">office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="a1861-113">office365GroupsActivityDetail</span></span>](../resources/office365groupsactivitydetail.md) | <span data-ttu-id="a1861-114">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="a1861-114">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="a1861-115">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="a1861-115">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="a1861-116">Stream</span><span class="sxs-lookup"><span data-stu-id="a1861-116">Stream</span></span>          | [<span data-ttu-id="a1861-117">office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="a1861-117">office365GroupsActivityCounts</span></span>](../resources/office365groupsactivitycounts.md) | <span data-ttu-id="a1861-118">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="a1861-118">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="a1861-119">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="a1861-119">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="a1861-120">Поток</span><span class="sxs-lookup"><span data-stu-id="a1861-120">Stream</span></span>          | [<span data-ttu-id="a1861-121">office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="a1861-121">office365GroupsActivityGroupCounts</span></span>](../resources/office365groupsactivitygroupcounts.md) | <span data-ttu-id="a1861-122">Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.</span><span class="sxs-lookup"><span data-stu-id="a1861-122">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="a1861-123">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="a1861-123">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="a1861-124">Stream</span><span class="sxs-lookup"><span data-stu-id="a1861-124">Stream</span></span>          | [<span data-ttu-id="a1861-125">office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="a1861-125">office365GroupsActivityStorage</span></span>](../resources/office365groupsactivitystorage.md) | <span data-ttu-id="a1861-126">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="a1861-126">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="a1861-127">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="a1861-127">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="a1861-128">Stream</span><span class="sxs-lookup"><span data-stu-id="a1861-128">Stream</span></span>          | [<span data-ttu-id="a1861-129">office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="a1861-129">office365GroupsActivityFileCounts</span></span>](../resources/office365groupsactivityfilecounts.md) | <span data-ttu-id="a1861-130">Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны.</span><span class="sxs-lookup"><span data-stu-id="a1861-130">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
