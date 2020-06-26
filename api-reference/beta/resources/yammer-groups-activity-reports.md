---
title: Отчеты об активности в группах Yammer
description: Вы можете получить подробные сведения о действиях в группах Yammer в Организации и узнать, сколько групп Yammer создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: cdeb94c9b5b687ab9584a236daaafb7c018a809c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897472"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="e93da-103">Отчеты об активности в группах Yammer</span><span class="sxs-lookup"><span data-stu-id="e93da-103">Yammer groups activity reports</span></span>

<span data-ttu-id="e93da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e93da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e93da-105">Вы можете получить подробные сведения о действиях в группах Yammer в Организации и узнать, сколько групп Yammer создается и используется.</span><span class="sxs-lookup"><span data-stu-id="e93da-105">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="e93da-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports: активность групп Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="e93da-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="e93da-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="e93da-107">Reports</span></span>

| <span data-ttu-id="e93da-108">Функция</span><span class="sxs-lookup"><span data-stu-id="e93da-108">Function</span></span>                                 | <span data-ttu-id="e93da-109">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="e93da-109">CSV return type</span></span> | <span data-ttu-id="e93da-110">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="e93da-110">JSON return type</span></span>                         | <span data-ttu-id="e93da-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e93da-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e93da-112">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="e93da-112">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="e93da-113">Stream</span><span class="sxs-lookup"><span data-stu-id="e93da-113">Stream</span></span>          | [<span data-ttu-id="e93da-114">яммерграупсактивитидетаил</span><span class="sxs-lookup"><span data-stu-id="e93da-114">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="e93da-115">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="e93da-115">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="e93da-116">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="e93da-116">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="e93da-117">Поток</span><span class="sxs-lookup"><span data-stu-id="e93da-117">Stream</span></span>          | [<span data-ttu-id="e93da-118">яммерграупсактивитиграупкаунтс</span><span class="sxs-lookup"><span data-stu-id="e93da-118">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="e93da-119">Узнайте, сколько всего существовало групп и в скольких из них была активность.</span><span class="sxs-lookup"><span data-stu-id="e93da-119">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="e93da-120">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="e93da-120">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="e93da-121">Stream</span><span class="sxs-lookup"><span data-stu-id="e93da-121">Stream</span></span>          | [<span data-ttu-id="e93da-122">яммерграупсактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="e93da-122">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="e93da-123">Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах.</span><span class="sxs-lookup"><span data-stu-id="e93da-123">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
