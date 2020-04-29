---
title: Отчеты о действиях в SharePoint
description: Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на SharePoint, в отчетах о действиях с файлами в SharePoint. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: defa0efa39a9eea57f9304663e42d0214b4305b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446886"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="cacd2-104">Отчеты о действиях в SharePoint</span><span class="sxs-lookup"><span data-stu-id="cacd2-104">SharePoint activity reports</span></span>

<span data-ttu-id="cacd2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cacd2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cacd2-106">Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на SharePoint, в отчетах о действиях с файлами в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cacd2-106">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="cacd2-107">Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.</span><span class="sxs-lookup"><span data-stu-id="cacd2-107">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="cacd2-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="cacd2-108">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="cacd2-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="cacd2-109">Reports</span></span>

| <span data-ttu-id="cacd2-110">Функция</span><span class="sxs-lookup"><span data-stu-id="cacd2-110">Function</span></span>                                 | <span data-ttu-id="cacd2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cacd2-111">Return Type</span></span> | <span data-ttu-id="cacd2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cacd2-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="cacd2-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="cacd2-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="cacd2-114">Stream</span><span class="sxs-lookup"><span data-stu-id="cacd2-114">Stream</span></span>      | <span data-ttu-id="cacd2-115">Получите сведения о действиях в SharePoint с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="cacd2-115">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="cacd2-116">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="cacd2-116">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="cacd2-117">Stream</span><span class="sxs-lookup"><span data-stu-id="cacd2-117">Stream</span></span>      | <span data-ttu-id="cacd2-118">Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cacd2-118">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="cacd2-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="cacd2-119">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="cacd2-120">Stream</span><span class="sxs-lookup"><span data-stu-id="cacd2-120">Stream</span></span>      | <span data-ttu-id="cacd2-121">Получение сведений о том, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="cacd2-121">Get the trend in the number of active users.</span></span> <span data-ttu-id="cacd2-122">Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="cacd2-122">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="cacd2-123">Получение страниц</span><span class="sxs-lookup"><span data-stu-id="cacd2-123">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="cacd2-124">Stream</span><span class="sxs-lookup"><span data-stu-id="cacd2-124">Stream</span></span>      | <span data-ttu-id="cacd2-125">Получите количество уникальных страниц, посещенных пользователями.</span><span class="sxs-lookup"><span data-stu-id="cacd2-125">Get the number of unique pages visited by users.</span></span> |
