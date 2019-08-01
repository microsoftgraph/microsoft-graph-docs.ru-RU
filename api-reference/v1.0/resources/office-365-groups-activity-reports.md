---
title: Отчеты об активности в группах Office 365
description: Эти отчеты позволяют получить представление об активности в группах Office 365 в организации и узнать, сколько групп Office 365 создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: c6733b76626e45673940d235f7b9d33aee899ce3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035954"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="159b5-103">Отчеты об активности в группах Office 365</span><span class="sxs-lookup"><span data-stu-id="159b5-103">Office 365 Groups activity reports</span></span>

<span data-ttu-id="159b5-104">Эти отчеты позволяют получить представление об активности в группах Office 365 в организации и узнать, сколько групп Office 365 создается и используется.</span><span class="sxs-lookup"><span data-stu-id="159b5-104">You can use the Groups activity reports to gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 Groups are being created and used.</span></span>

> <span data-ttu-id="159b5-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="159b5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="159b5-106">Отчеты</span><span class="sxs-lookup"><span data-stu-id="159b5-106">Reports</span></span>

| <span data-ttu-id="159b5-107">Функция</span><span class="sxs-lookup"><span data-stu-id="159b5-107">Function</span></span>                                 | <span data-ttu-id="159b5-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="159b5-108">Return Type</span></span> | <span data-ttu-id="159b5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="159b5-109">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="159b5-110">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="159b5-110">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="159b5-111">Поток</span><span class="sxs-lookup"><span data-stu-id="159b5-111">Stream</span></span>          | <span data-ttu-id="159b5-112">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="159b5-112">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="159b5-113">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="159b5-113">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="159b5-114">Stream</span><span class="sxs-lookup"><span data-stu-id="159b5-114">Stream</span></span>          | <span data-ttu-id="159b5-115">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="159b5-115">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="159b5-116">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="159b5-116">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="159b5-117">Поток</span><span class="sxs-lookup"><span data-stu-id="159b5-117">Stream</span></span>          | <span data-ttu-id="159b5-118">Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.</span><span class="sxs-lookup"><span data-stu-id="159b5-118">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="159b5-119">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="159b5-119">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="159b5-120">Поток</span><span class="sxs-lookup"><span data-stu-id="159b5-120">Stream</span></span>          | <span data-ttu-id="159b5-121">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="159b5-121">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="159b5-122">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="159b5-122">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="159b5-123">Поток</span><span class="sxs-lookup"><span data-stu-id="159b5-123">Stream</span></span>          | <span data-ttu-id="159b5-124">Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны.</span><span class="sxs-lookup"><span data-stu-id="159b5-124">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
