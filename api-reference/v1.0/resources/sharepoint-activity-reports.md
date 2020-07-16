---
title: Отчеты о действиях в SharePoint
description: Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на SharePoint, в отчетах о действиях с файлами в SharePoint. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 7d0e323c81ed421c2234bbd78bb3d98a9f21c8bb
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895995"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="373e2-104">Отчеты о действиях в SharePoint</span><span class="sxs-lookup"><span data-stu-id="373e2-104">SharePoint activity reports</span></span>

<span data-ttu-id="373e2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="373e2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="373e2-106">Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на SharePoint, в отчетах о действиях с файлами в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="373e2-106">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="373e2-107">Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.</span><span class="sxs-lookup"><span data-stu-id="373e2-107">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="373e2-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-SharePoint Activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="373e2-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="373e2-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="373e2-109">Reports</span></span>

| <span data-ttu-id="373e2-110">Функция</span><span class="sxs-lookup"><span data-stu-id="373e2-110">Function</span></span>                                 | <span data-ttu-id="373e2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="373e2-111">Return Type</span></span> | <span data-ttu-id="373e2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="373e2-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="373e2-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="373e2-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="373e2-114">Stream</span><span class="sxs-lookup"><span data-stu-id="373e2-114">Stream</span></span>      | <span data-ttu-id="373e2-115">Получите сведения о действиях в SharePoint с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="373e2-115">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="373e2-116">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="373e2-116">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="373e2-117">Stream</span><span class="sxs-lookup"><span data-stu-id="373e2-117">Stream</span></span>      | <span data-ttu-id="373e2-118">Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="373e2-118">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="373e2-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="373e2-119">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="373e2-120">Stream</span><span class="sxs-lookup"><span data-stu-id="373e2-120">Stream</span></span>      | <span data-ttu-id="373e2-121">Получение сведений о том, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="373e2-121">Get the trend in the number of active users.</span></span> <span data-ttu-id="373e2-122">Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="373e2-122">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="373e2-123">Получение страниц</span><span class="sxs-lookup"><span data-stu-id="373e2-123">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="373e2-124">Stream</span><span class="sxs-lookup"><span data-stu-id="373e2-124">Stream</span></span>      | <span data-ttu-id="373e2-125">Получите количество уникальных страниц, посещенных пользователями.</span><span class="sxs-lookup"><span data-stu-id="373e2-125">Get the number of unique pages visited by users.</span></span> |
