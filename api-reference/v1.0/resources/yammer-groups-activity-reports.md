---
title: Отчеты об активности в группах Yammer
description: Эти отчеты позволяют получить представление об активности в группах Yammer в организации и узнать, сколько групп Yammer создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 07b5521efb3b89eedc480101f107a421452918a2
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897647"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="9f940-103">Отчеты об активности в группах Yammer</span><span class="sxs-lookup"><span data-stu-id="9f940-103">Yammer groups activity reports</span></span>

<span data-ttu-id="9f940-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f940-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f940-105">Эти отчеты позволяют получить представление об активности в группах Yammer в организации и узнать, сколько групп Yammer создается и используется.</span><span class="sxs-lookup"><span data-stu-id="9f940-105">You can use the Yammer groups activity reports to gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="9f940-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports: активность групп Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="9f940-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="9f940-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="9f940-107">Reports</span></span>

| <span data-ttu-id="9f940-108">Функция</span><span class="sxs-lookup"><span data-stu-id="9f940-108">Function</span></span>                                 | <span data-ttu-id="9f940-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9f940-109">Return Type</span></span> | <span data-ttu-id="9f940-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9f940-110">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="9f940-111">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="9f940-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="9f940-112">Stream</span><span class="sxs-lookup"><span data-stu-id="9f940-112">Stream</span></span>      | <span data-ttu-id="9f940-113">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="9f940-113">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="9f940-114">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="9f940-114">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="9f940-115">Поток</span><span class="sxs-lookup"><span data-stu-id="9f940-115">Stream</span></span>      | <span data-ttu-id="9f940-116">Узнайте, сколько всего существовало групп и в скольких из них была активность.</span><span class="sxs-lookup"><span data-stu-id="9f940-116">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="9f940-117">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="9f940-117">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="9f940-118">Stream</span><span class="sxs-lookup"><span data-stu-id="9f940-118">Stream</span></span>      | <span data-ttu-id="9f940-119">Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах.</span><span class="sxs-lookup"><span data-stu-id="9f940-119">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
