---
title: Отчеты об активности в группах Yammer
description: Вы можете получить подробные сведения о действиях в группах Yammer в Организации и узнать, сколько групп Yammer создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 07ec3db93088dd00af1b8595e5d059fc2cede774
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522029"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="52086-103">Отчеты об активности в группах Yammer</span><span class="sxs-lookup"><span data-stu-id="52086-103">Yammer groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52086-104">Вы можете получить подробные сведения о действиях в группах Yammer в Организации и узнать, сколько групп Yammer создается и используется.</span><span class="sxs-lookup"><span data-stu-id="52086-104">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="52086-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="52086-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="52086-106">Отчеты</span><span class="sxs-lookup"><span data-stu-id="52086-106">Reports</span></span>

| <span data-ttu-id="52086-107">Функция</span><span class="sxs-lookup"><span data-stu-id="52086-107">Function</span></span>                                 | <span data-ttu-id="52086-108">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="52086-108">CSV return type</span></span> | <span data-ttu-id="52086-109">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="52086-109">JSON return type</span></span>                         | <span data-ttu-id="52086-110">Описание</span><span class="sxs-lookup"><span data-stu-id="52086-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="52086-111">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="52086-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="52086-112">Поток</span><span class="sxs-lookup"><span data-stu-id="52086-112">Stream</span></span>          | [<span data-ttu-id="52086-113">Яммерграупсактивитидетаил</span><span class="sxs-lookup"><span data-stu-id="52086-113">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="52086-114">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="52086-114">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="52086-115">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="52086-115">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="52086-116">Поток</span><span class="sxs-lookup"><span data-stu-id="52086-116">Stream</span></span>          | [<span data-ttu-id="52086-117">Яммерграупсактивитиграупкаунтс</span><span class="sxs-lookup"><span data-stu-id="52086-117">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="52086-118">Узнайте, сколько всего существовало групп и в скольких из них была активность.</span><span class="sxs-lookup"><span data-stu-id="52086-118">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="52086-119">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="52086-119">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="52086-120">Поток</span><span class="sxs-lookup"><span data-stu-id="52086-120">Stream</span></span>          | [<span data-ttu-id="52086-121">Яммерграупсактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="52086-121">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="52086-122">Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах.</span><span class="sxs-lookup"><span data-stu-id="52086-122">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
