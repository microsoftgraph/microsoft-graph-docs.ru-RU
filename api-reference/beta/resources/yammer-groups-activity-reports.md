---
title: Отчеты об активности в группах Yammer
description: Можно воспользоваться сведениями в действие группы Yammer в вашей организации и видеть, сколько групп Yammer создаются и используются.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 05e5826a85e7d2e37af82cdf6277857746b1b922
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514161"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="54fa9-103">Отчеты об активности в группах Yammer</span><span class="sxs-lookup"><span data-stu-id="54fa9-103">Yammer groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54fa9-104">Можно воспользоваться сведениями в действие группы Yammer в вашей организации и видеть, сколько групп Yammer создаются и используются.</span><span class="sxs-lookup"><span data-stu-id="54fa9-104">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="54fa9-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="54fa9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="54fa9-106">Отчеты</span><span class="sxs-lookup"><span data-stu-id="54fa9-106">Reports</span></span>

| <span data-ttu-id="54fa9-107">Функция</span><span class="sxs-lookup"><span data-stu-id="54fa9-107">Function</span></span>                                 | <span data-ttu-id="54fa9-108">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="54fa9-108">CSV return type</span></span> | <span data-ttu-id="54fa9-109">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="54fa9-109">JSON return type</span></span>                         | <span data-ttu-id="54fa9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54fa9-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="54fa9-111">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="54fa9-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="54fa9-112">Stream</span><span class="sxs-lookup"><span data-stu-id="54fa9-112">Stream</span></span>          | [<span data-ttu-id="54fa9-113">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="54fa9-113">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="54fa9-114">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="54fa9-114">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="54fa9-115">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="54fa9-115">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="54fa9-116">Stream</span><span class="sxs-lookup"><span data-stu-id="54fa9-116">Stream</span></span>          | [<span data-ttu-id="54fa9-117">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="54fa9-117">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="54fa9-118">Узнайте, сколько всего существовало групп и в скольких из них была активность.</span><span class="sxs-lookup"><span data-stu-id="54fa9-118">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="54fa9-119">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="54fa9-119">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="54fa9-120">Stream</span><span class="sxs-lookup"><span data-stu-id="54fa9-120">Stream</span></span>          | [<span data-ttu-id="54fa9-121">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="54fa9-121">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="54fa9-122">Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах.</span><span class="sxs-lookup"><span data-stu-id="54fa9-122">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
