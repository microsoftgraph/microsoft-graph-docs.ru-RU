---
title: Отчеты о действиях в SharePoint
description: Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на SharePoint, в отчетах о действиях с файлами в SharePoint. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 27d7a1ad734bf5d5dbeff59d577232628e531883
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034316"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="c509a-104">Отчеты о действиях в SharePoint</span><span class="sxs-lookup"><span data-stu-id="c509a-104">SharePoint activity reports</span></span>

<span data-ttu-id="c509a-105">Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на SharePoint, в отчетах о действиях с файлами в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c509a-105">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="c509a-106">Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.</span><span class="sxs-lookup"><span data-stu-id="c509a-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="c509a-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="c509a-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="c509a-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="c509a-108">Reports</span></span>

| <span data-ttu-id="c509a-109">Функция</span><span class="sxs-lookup"><span data-stu-id="c509a-109">Function</span></span>                                 | <span data-ttu-id="c509a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c509a-110">Return Type</span></span> | <span data-ttu-id="c509a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c509a-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="c509a-112">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="c509a-112">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="c509a-113">Поток</span><span class="sxs-lookup"><span data-stu-id="c509a-113">Stream</span></span>      | <span data-ttu-id="c509a-114">Получите сведения о действиях в SharePoint с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="c509a-114">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="c509a-115">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="c509a-115">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="c509a-116">Поток</span><span class="sxs-lookup"><span data-stu-id="c509a-116">Stream</span></span>      | <span data-ttu-id="c509a-117">Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c509a-117">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="c509a-118">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="c509a-118">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="c509a-119">Поток</span><span class="sxs-lookup"><span data-stu-id="c509a-119">Stream</span></span>      | <span data-ttu-id="c509a-120">Получение сведений о том, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="c509a-120">Get the trend in the number of active users.</span></span> <span data-ttu-id="c509a-121">Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="c509a-121">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="c509a-122">Получение страниц</span><span class="sxs-lookup"><span data-stu-id="c509a-122">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="c509a-123">Stream</span><span class="sxs-lookup"><span data-stu-id="c509a-123">Stream</span></span>      | <span data-ttu-id="c509a-124">Получите количество уникальных страниц, посещенных пользователями.</span><span class="sxs-lookup"><span data-stu-id="c509a-124">Get the number of unique pages visited by users.</span></span> |
