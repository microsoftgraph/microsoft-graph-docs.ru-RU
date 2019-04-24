---
title: Отчеты об активности в группах Office 365
description: Эти отчеты позволяют получить представление об активности в группах Office 365 в организации и узнать, сколько групп Office 365 создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5d8c414034a110db64b770a72fe2e3540806acdd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462951"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="1a04f-103">Отчеты об активности в группах Office 365</span><span class="sxs-lookup"><span data-stu-id="1a04f-103">Office 365 Groups activity reports</span></span>

<span data-ttu-id="1a04f-104">Эти отчеты позволяют получить представление об активности в группах Office 365 в организации и узнать, сколько групп Office 365 создается и используется.</span><span class="sxs-lookup"><span data-stu-id="1a04f-104">You can use the Groups activity reports to gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 Groups are being created and used.</span></span>

> <span data-ttu-id="1a04f-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="1a04f-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="1a04f-106">Отчеты</span><span class="sxs-lookup"><span data-stu-id="1a04f-106">Reports</span></span>

| <span data-ttu-id="1a04f-107">Функция</span><span class="sxs-lookup"><span data-stu-id="1a04f-107">Function</span></span>                                 | <span data-ttu-id="1a04f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1a04f-108">Return Type</span></span> | <span data-ttu-id="1a04f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1a04f-109">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="1a04f-110">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="1a04f-110">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="1a04f-111">Stream</span><span class="sxs-lookup"><span data-stu-id="1a04f-111">Stream</span></span>          | <span data-ttu-id="1a04f-112">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="1a04f-112">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="1a04f-113">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="1a04f-113">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="1a04f-114">Stream</span><span class="sxs-lookup"><span data-stu-id="1a04f-114">Stream</span></span>          | <span data-ttu-id="1a04f-115">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="1a04f-115">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="1a04f-116">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="1a04f-116">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="1a04f-117">Stream</span><span class="sxs-lookup"><span data-stu-id="1a04f-117">Stream</span></span>          | <span data-ttu-id="1a04f-118">Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.</span><span class="sxs-lookup"><span data-stu-id="1a04f-118">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="1a04f-119">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="1a04f-119">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="1a04f-120">Stream</span><span class="sxs-lookup"><span data-stu-id="1a04f-120">Stream</span></span>          | <span data-ttu-id="1a04f-121">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="1a04f-121">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="1a04f-122">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="1a04f-122">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="1a04f-123">Поток</span><span class="sxs-lookup"><span data-stu-id="1a04f-123">Stream</span></span>          | <span data-ttu-id="1a04f-124">Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны.</span><span class="sxs-lookup"><span data-stu-id="1a04f-124">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
