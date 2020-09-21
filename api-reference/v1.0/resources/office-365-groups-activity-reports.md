---
title: Отчеты об активности в группах Microsoft 365
description: Отчеты об активности групп можно использовать для получения сведений о действиях в группах Microsoft 365 в Организации и о количестве создаваемых и используемых групп Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 52bb3cb71837f049cada3970bdd0faa710f38844
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965423"
---
# <a name="microsoft-365-groups-activity-reports"></a><span data-ttu-id="2d4cc-103">Отчеты об активности в группах Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2d4cc-103">Microsoft 365 groups activity reports</span></span>

<span data-ttu-id="2d4cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d4cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d4cc-105">Отчеты об активности групп можно использовать для получения сведений о действиях в группах Microsoft 365 в Организации и о количестве создаваемых и используемых групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2d4cc-105">You can use the Groups activity reports to gain insights into the activity of Microsoft 365 groups in your organization and see how many Microsoft 365 groups are being created and used.</span></span>

> <span data-ttu-id="2d4cc-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — microsoft 365 Groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="2d4cc-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="2d4cc-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="2d4cc-107">Reports</span></span>

| <span data-ttu-id="2d4cc-108">Функция</span><span class="sxs-lookup"><span data-stu-id="2d4cc-108">Function</span></span>                                 | <span data-ttu-id="2d4cc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2d4cc-109">Return Type</span></span> | <span data-ttu-id="2d4cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2d4cc-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="2d4cc-111">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="2d4cc-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="2d4cc-112">Поток</span><span class="sxs-lookup"><span data-stu-id="2d4cc-112">Stream</span></span>          | <span data-ttu-id="2d4cc-113">Получение сведений о действиях в группах Microsoft 365, сгруппированных по группам.</span><span class="sxs-lookup"><span data-stu-id="2d4cc-113">Get details about Microsoft 365 groups activity by group.</span></span> |
| [<span data-ttu-id="2d4cc-114">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="2d4cc-114">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="2d4cc-115">Stream</span><span class="sxs-lookup"><span data-stu-id="2d4cc-115">Stream</span></span>          | <span data-ttu-id="2d4cc-116">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="2d4cc-116">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="2d4cc-117">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="2d4cc-117">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="2d4cc-118">Поток</span><span class="sxs-lookup"><span data-stu-id="2d4cc-118">Stream</span></span>          | <span data-ttu-id="2d4cc-119">Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.</span><span class="sxs-lookup"><span data-stu-id="2d4cc-119">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="2d4cc-120">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="2d4cc-120">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="2d4cc-121">Поток</span><span class="sxs-lookup"><span data-stu-id="2d4cc-121">Stream</span></span>          | <span data-ttu-id="2d4cc-122">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="2d4cc-122">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="2d4cc-123">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="2d4cc-123">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="2d4cc-124">Stream</span><span class="sxs-lookup"><span data-stu-id="2d4cc-124">Stream</span></span>          | <span data-ttu-id="2d4cc-125">Получите общее количество файлов и их количество, которое было активно на всех сайтах группы, связанных с группой Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2d4cc-125">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span> |

