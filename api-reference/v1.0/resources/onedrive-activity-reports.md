---
title: Отчеты о действиях в OneDrive
description: Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на OneDrive, в отчетах действий с файлами в OneDrive. Эти отчеты позволят оценить уровень взаимодействия благодаря данным о количестве файлов, к которым предоставлен общий доступ.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 5a40e194b7ac315639842432ca279ce309248ed8
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980985"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="bbba4-104">Отчеты о действиях в OneDrive</span><span class="sxs-lookup"><span data-stu-id="bbba4-104">OneDrive activity reports</span></span>

<span data-ttu-id="bbba4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbba4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bbba4-106">Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на OneDrive, в отчетах действий с файлами в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bbba4-106">Use the OneDrive activity reports to get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="bbba4-107">Эти отчеты позволят оценить уровень взаимодействия благодаря данным о количестве файлов, к которым предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="bbba4-107">These reports can help you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="bbba4-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365: действия в OneDrive для бизнеса.](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)</span><span class="sxs-lookup"><span data-stu-id="bbba4-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="bbba4-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="bbba4-109">Reports</span></span>

| <span data-ttu-id="bbba4-110">Функция</span><span class="sxs-lookup"><span data-stu-id="bbba4-110">Function</span></span>                                 | <span data-ttu-id="bbba4-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bbba4-111">Return Type</span></span> | <span data-ttu-id="bbba4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bbba4-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="bbba4-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="bbba4-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="bbba4-114">Stream</span><span class="sxs-lookup"><span data-stu-id="bbba4-114">Stream</span></span>      | <span data-ttu-id="bbba4-115">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="bbba4-115">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="bbba4-116">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="bbba4-116">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="bbba4-117">Stream</span><span class="sxs-lookup"><span data-stu-id="bbba4-117">Stream</span></span>      | <span data-ttu-id="bbba4-118">Получение тренда в отношении количества активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bbba4-118">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="bbba4-119">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="bbba4-119">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="bbba4-120">Stream</span><span class="sxs-lookup"><span data-stu-id="bbba4-120">Stream</span></span>      | <span data-ttu-id="bbba4-121">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bbba4-121">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |


