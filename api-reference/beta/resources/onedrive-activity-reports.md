---
title: Отчеты о действиях в OneDrive
description: Вы можете получить действия каждого пользователя, у кого есть лицензия на использование OneDrive, изусмотрив их взаимодействие с файлами в OneDrive. Кроме того, это помогает понять, каков уровень совместной работы, показывая количество общих файлов.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7d0c069d2787b30f37e634757127b6141843a9ed
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983603"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="f27d8-104">Отчеты о действиях в OneDrive</span><span class="sxs-lookup"><span data-stu-id="f27d8-104">OneDrive activity reports</span></span>

<span data-ttu-id="f27d8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f27d8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f27d8-106">Вы можете получить действия каждого пользователя, у кого есть лицензия на использование OneDrive, изусмотрив их взаимодействие с файлами в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f27d8-106">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="f27d8-107">Кроме того, это помогает понять, каков уровень совместной работы, показывая количество общих файлов.</span><span class="sxs-lookup"><span data-stu-id="f27d8-107">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="f27d8-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365: действия в OneDrive для бизнеса.](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)</span><span class="sxs-lookup"><span data-stu-id="f27d8-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="f27d8-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="f27d8-109">Reports</span></span>

| <span data-ttu-id="f27d8-110">Функция</span><span class="sxs-lookup"><span data-stu-id="f27d8-110">Function</span></span>                                 | <span data-ttu-id="f27d8-111">Тип возврата CSV</span><span class="sxs-lookup"><span data-stu-id="f27d8-111">CSV return type</span></span> | <span data-ttu-id="f27d8-112">Тип возврата JSON</span><span class="sxs-lookup"><span data-stu-id="f27d8-112">JSON return type</span></span>                         | <span data-ttu-id="f27d8-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f27d8-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="f27d8-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="f27d8-114">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="f27d8-115">Stream</span><span class="sxs-lookup"><span data-stu-id="f27d8-115">Stream</span></span>          | [<span data-ttu-id="f27d8-116">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f27d8-116">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="f27d8-117">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="f27d8-117">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="f27d8-118">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="f27d8-118">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="f27d8-119">Stream</span><span class="sxs-lookup"><span data-stu-id="f27d8-119">Stream</span></span>          | [<span data-ttu-id="f27d8-120">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="f27d8-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="f27d8-121">Получение тренда в отношении количества активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f27d8-121">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="f27d8-122">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="f27d8-122">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="f27d8-123">Stream</span><span class="sxs-lookup"><span data-stu-id="f27d8-123">Stream</span></span>          | [<span data-ttu-id="f27d8-124">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="f27d8-124">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="f27d8-125">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f27d8-125">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |


