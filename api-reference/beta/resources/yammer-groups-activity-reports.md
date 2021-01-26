---
title: Отчеты об активности в группах Yammer
description: Вы можете получить представление об активности групп Yammer в организации и узнать, сколько групп Yammer создается и используется.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 09c8aa8476886f8bbf7266817449195b4c07aa05
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982427"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="49212-103">Отчеты об активности в группах Yammer</span><span class="sxs-lookup"><span data-stu-id="49212-103">Yammer groups activity reports</span></span>

<span data-ttu-id="49212-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49212-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49212-105">Вы можете получить представление об активности групп Yammer в вашей организации и узнать, сколько групп Yammer создается и используется.</span><span class="sxs-lookup"><span data-stu-id="49212-105">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="49212-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 о](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)действиях в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="49212-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="49212-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="49212-107">Reports</span></span>

| <span data-ttu-id="49212-108">Функция</span><span class="sxs-lookup"><span data-stu-id="49212-108">Function</span></span>                                 | <span data-ttu-id="49212-109">Тип возврата CSV</span><span class="sxs-lookup"><span data-stu-id="49212-109">CSV return type</span></span> | <span data-ttu-id="49212-110">Тип возврата JSON</span><span class="sxs-lookup"><span data-stu-id="49212-110">JSON return type</span></span>                         | <span data-ttu-id="49212-111">Описание</span><span class="sxs-lookup"><span data-stu-id="49212-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="49212-112">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="49212-112">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="49212-113">Поток</span><span class="sxs-lookup"><span data-stu-id="49212-113">Stream</span></span>          | [<span data-ttu-id="49212-114">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="49212-114">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="49212-115">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="49212-115">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="49212-116">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="49212-116">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="49212-117">Поток</span><span class="sxs-lookup"><span data-stu-id="49212-117">Stream</span></span>          | [<span data-ttu-id="49212-118">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="49212-118">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="49212-119">Узнайте, сколько всего существовало групп и в скольких из них была активность.</span><span class="sxs-lookup"><span data-stu-id="49212-119">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="49212-120">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="49212-120">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="49212-121">Stream</span><span class="sxs-lookup"><span data-stu-id="49212-121">Stream</span></span>          | [<span data-ttu-id="49212-122">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="49212-122">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="49212-123">Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах.</span><span class="sxs-lookup"><span data-stu-id="49212-123">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |


