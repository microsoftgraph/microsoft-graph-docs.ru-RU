---
title: Отчеты об активности в группах Yammer
description: Эти отчеты позволяют получить представление об активности в группах Yammer в организации и узнать, сколько групп Yammer создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 961072e088d36748d51a4a6081f0ee06c47b6e20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534266"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="b22dc-103">Отчеты об активности в группах Yammer</span><span class="sxs-lookup"><span data-stu-id="b22dc-103">Yammer groups activity reports</span></span>

<span data-ttu-id="b22dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b22dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b22dc-105">Эти отчеты позволяют получить представление об активности в группах Yammer в организации и узнать, сколько групп Yammer создается и используется.</span><span class="sxs-lookup"><span data-stu-id="b22dc-105">You can use the Yammer groups activity reports to gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="b22dc-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="b22dc-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="b22dc-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="b22dc-107">Reports</span></span>

| <span data-ttu-id="b22dc-108">Функция</span><span class="sxs-lookup"><span data-stu-id="b22dc-108">Function</span></span>                                 | <span data-ttu-id="b22dc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b22dc-109">Return Type</span></span> | <span data-ttu-id="b22dc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b22dc-110">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="b22dc-111">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="b22dc-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="b22dc-112">Stream</span><span class="sxs-lookup"><span data-stu-id="b22dc-112">Stream</span></span>      | <span data-ttu-id="b22dc-113">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="b22dc-113">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="b22dc-114">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="b22dc-114">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="b22dc-115">Поток</span><span class="sxs-lookup"><span data-stu-id="b22dc-115">Stream</span></span>      | <span data-ttu-id="b22dc-116">Узнайте, сколько всего существовало групп и в скольких из них была активность.</span><span class="sxs-lookup"><span data-stu-id="b22dc-116">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="b22dc-117">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="b22dc-117">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="b22dc-118">Stream</span><span class="sxs-lookup"><span data-stu-id="b22dc-118">Stream</span></span>      | <span data-ttu-id="b22dc-119">Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах.</span><span class="sxs-lookup"><span data-stu-id="b22dc-119">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
