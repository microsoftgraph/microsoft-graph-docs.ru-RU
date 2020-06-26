---
title: Отчеты о действиях в OneDrive
description: Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на OneDrive, в отчетах действий с файлами в OneDrive. Эти отчеты позволят оценить уровень взаимодействия благодаря данным о количестве файлов, к которым предоставлен общий доступ.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 24a2e74e9e117c13fa49efc6fba4323f75716ffe
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898151"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="74471-104">Отчеты о действиях в OneDrive</span><span class="sxs-lookup"><span data-stu-id="74471-104">OneDrive activity reports</span></span>

<span data-ttu-id="74471-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74471-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74471-106">Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на OneDrive, в отчетах действий с файлами в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="74471-106">Use the OneDrive activity reports to get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="74471-107">Эти отчеты позволят оценить уровень взаимодействия благодаря данным о количестве файлов, к которым предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="74471-107">These reports can help you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="74471-108">**Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-Activity for OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="74471-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="74471-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="74471-109">Reports</span></span>

| <span data-ttu-id="74471-110">Функция</span><span class="sxs-lookup"><span data-stu-id="74471-110">Function</span></span>                                 | <span data-ttu-id="74471-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74471-111">Return Type</span></span> | <span data-ttu-id="74471-112">Описание</span><span class="sxs-lookup"><span data-stu-id="74471-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="74471-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="74471-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="74471-114">Stream</span><span class="sxs-lookup"><span data-stu-id="74471-114">Stream</span></span>      | <span data-ttu-id="74471-115">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="74471-115">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="74471-116">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="74471-116">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="74471-117">Stream</span><span class="sxs-lookup"><span data-stu-id="74471-117">Stream</span></span>      | <span data-ttu-id="74471-118">Получение тренда в отношении количества активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="74471-118">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="74471-119">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="74471-119">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="74471-120">Stream</span><span class="sxs-lookup"><span data-stu-id="74471-120">Stream</span></span>      | <span data-ttu-id="74471-121">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="74471-121">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |

