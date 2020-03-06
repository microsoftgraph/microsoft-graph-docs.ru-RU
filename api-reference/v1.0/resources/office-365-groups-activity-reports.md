---
title: Отчеты об активности в группах Office 365
description: Эти отчеты позволяют получить представление об активности в группах Office 365 в организации и узнать, сколько групп Office 365 создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 57749ca15e4eaf4aad14f3f914426d861ea45eeb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534179"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="2e598-103">Отчеты об активности в группах Office 365</span><span class="sxs-lookup"><span data-stu-id="2e598-103">Office 365 Groups activity reports</span></span>

<span data-ttu-id="2e598-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e598-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e598-105">Эти отчеты позволяют получить представление об активности в группах Office 365 в организации и узнать, сколько групп Office 365 создается и используется.</span><span class="sxs-lookup"><span data-stu-id="2e598-105">You can use the Groups activity reports to gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 Groups are being created and used.</span></span>

> <span data-ttu-id="2e598-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="2e598-106">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="2e598-107">Отчеты</span><span class="sxs-lookup"><span data-stu-id="2e598-107">Reports</span></span>

| <span data-ttu-id="2e598-108">Функция</span><span class="sxs-lookup"><span data-stu-id="2e598-108">Function</span></span>                                 | <span data-ttu-id="2e598-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2e598-109">Return Type</span></span> | <span data-ttu-id="2e598-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e598-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="2e598-111">Получение сведений о группах</span><span class="sxs-lookup"><span data-stu-id="2e598-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="2e598-112">Stream</span><span class="sxs-lookup"><span data-stu-id="2e598-112">Stream</span></span>          | <span data-ttu-id="2e598-113">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="2e598-113">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="2e598-114">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="2e598-114">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="2e598-115">Stream</span><span class="sxs-lookup"><span data-stu-id="2e598-115">Stream</span></span>          | <span data-ttu-id="2e598-116">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="2e598-116">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="2e598-117">Получение количества групп</span><span class="sxs-lookup"><span data-stu-id="2e598-117">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="2e598-118">Stream</span><span class="sxs-lookup"><span data-stu-id="2e598-118">Stream</span></span>          | <span data-ttu-id="2e598-119">Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.</span><span class="sxs-lookup"><span data-stu-id="2e598-119">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="2e598-120">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="2e598-120">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="2e598-121">Поток</span><span class="sxs-lookup"><span data-stu-id="2e598-121">Stream</span></span>          | <span data-ttu-id="2e598-122">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="2e598-122">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="2e598-123">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="2e598-123">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="2e598-124">Поток</span><span class="sxs-lookup"><span data-stu-id="2e598-124">Stream</span></span>          | <span data-ttu-id="2e598-125">Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны.</span><span class="sxs-lookup"><span data-stu-id="2e598-125">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
