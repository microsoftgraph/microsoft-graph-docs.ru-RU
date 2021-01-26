---
title: Отчеты об активности групп Microsoft 365
description: Вы можете использовать отчеты о действиях в группах, чтобы получить представление об активности групп Microsoft 365 в организации и узнать, сколько групп Microsoft 365 создается и используется.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7470eff43c2c77a63206cf24e0484360bf3371b6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980999"
---
# <a name="microsoft-365-groups-activity-reports"></a><span data-ttu-id="6b2a5-103">Отчеты об активности групп Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6b2a5-103">Microsoft 365 groups activity reports</span></span>

<span data-ttu-id="6b2a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b2a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b2a5-105">Вы можете использовать отчеты о действиях в группах, чтобы получить представление об активности групп Microsoft 365 в организации и узнать, сколько групп Microsoft 365 создается и используется.</span><span class="sxs-lookup"><span data-stu-id="6b2a5-105">You can use the Groups activity reports to gain insights into the activity of Microsoft 365 groups in your organization and see how many Microsoft 365 groups are being created and used.</span></span>

> <span data-ttu-id="6b2a5-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 — группы Microsoft 365.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)</span><span class="sxs-lookup"><span data-stu-id="6b2a5-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="6b2a5-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="6b2a5-107">Reports</span></span>

| <span data-ttu-id="6b2a5-108">Функция</span><span class="sxs-lookup"><span data-stu-id="6b2a5-108">Function</span></span>                                 | <span data-ttu-id="6b2a5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6b2a5-109">Return Type</span></span> | <span data-ttu-id="6b2a5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6b2a5-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="6b2a5-111">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="6b2a5-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="6b2a5-112">Поток</span><span class="sxs-lookup"><span data-stu-id="6b2a5-112">Stream</span></span>          | <span data-ttu-id="6b2a5-113">Получите сведения об активности групп Microsoft 365 по группам.</span><span class="sxs-lookup"><span data-stu-id="6b2a5-113">Get details about Microsoft 365 groups activity by group.</span></span> |
| [<span data-ttu-id="6b2a5-114">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="6b2a5-114">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="6b2a5-115">Stream</span><span class="sxs-lookup"><span data-stu-id="6b2a5-115">Stream</span></span>          | <span data-ttu-id="6b2a5-116">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="6b2a5-116">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="6b2a5-117">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="6b2a5-117">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="6b2a5-118">Поток</span><span class="sxs-lookup"><span data-stu-id="6b2a5-118">Stream</span></span>          | <span data-ttu-id="6b2a5-119">Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.</span><span class="sxs-lookup"><span data-stu-id="6b2a5-119">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="6b2a5-120">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="6b2a5-120">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="6b2a5-121">Поток</span><span class="sxs-lookup"><span data-stu-id="6b2a5-121">Stream</span></span>          | <span data-ttu-id="6b2a5-122">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="6b2a5-122">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="6b2a5-123">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="6b2a5-123">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="6b2a5-124">Stream</span><span class="sxs-lookup"><span data-stu-id="6b2a5-124">Stream</span></span>          | <span data-ttu-id="6b2a5-125">Получите общее количество файлов и их количество на всех сайтах групп, связанных с группой Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6b2a5-125">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span> |

