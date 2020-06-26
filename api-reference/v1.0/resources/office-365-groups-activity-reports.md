---
title: Отчеты об активности в группах Microsoft 365
description: Отчеты об активности групп можно использовать для получения сведений о действиях в группах Microsoft 365 в Организации и о количестве создаваемых и используемых групп Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0cd0dfc07813714d376a38125835917c712e7ebe
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898158"
---
# <a name="microsoft-365-groups-activity-reports"></a><span data-ttu-id="a71f5-103">Отчеты об активности в группах Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a71f5-103">Microsoft 365 groups activity reports</span></span>

<span data-ttu-id="a71f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a71f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a71f5-105">Отчеты об активности групп можно использовать для получения сведений о действиях в группах Microsoft 365 в Организации и о количестве создаваемых и используемых групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a71f5-105">You can use the Groups activity reports to gain insights into the activity of Microsoft 365 groups in your organization and see how many Microsoft 365 groups are being created and used.</span></span>

> <span data-ttu-id="a71f5-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — microsoft 365 Groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="a71f5-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="a71f5-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="a71f5-107">Reports</span></span>

| <span data-ttu-id="a71f5-108">Функция</span><span class="sxs-lookup"><span data-stu-id="a71f5-108">Function</span></span>                                 | <span data-ttu-id="a71f5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a71f5-109">Return Type</span></span> | <span data-ttu-id="a71f5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a71f5-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="a71f5-111">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="a71f5-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="a71f5-112">Stream</span><span class="sxs-lookup"><span data-stu-id="a71f5-112">Stream</span></span>          | <span data-ttu-id="a71f5-113">Получение сведений о действиях в группах Microsoft 365, сгруппированных по группам.</span><span class="sxs-lookup"><span data-stu-id="a71f5-113">Get details about Microsoft 365 groups activity by group.</span></span> |
| [<span data-ttu-id="a71f5-114">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="a71f5-114">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="a71f5-115">Stream</span><span class="sxs-lookup"><span data-stu-id="a71f5-115">Stream</span></span>          | <span data-ttu-id="a71f5-116">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="a71f5-116">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="a71f5-117">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="a71f5-117">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="a71f5-118">Поток</span><span class="sxs-lookup"><span data-stu-id="a71f5-118">Stream</span></span>          | <span data-ttu-id="a71f5-119">Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.</span><span class="sxs-lookup"><span data-stu-id="a71f5-119">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="a71f5-120">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="a71f5-120">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="a71f5-121">Поток</span><span class="sxs-lookup"><span data-stu-id="a71f5-121">Stream</span></span>          | <span data-ttu-id="a71f5-122">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="a71f5-122">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="a71f5-123">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="a71f5-123">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="a71f5-124">Stream</span><span class="sxs-lookup"><span data-stu-id="a71f5-124">Stream</span></span>          | <span data-ttu-id="a71f5-125">Получите общее количество файлов и их количество, которое было активно на всех сайтах группы, связанных с группой Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a71f5-125">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span> |
