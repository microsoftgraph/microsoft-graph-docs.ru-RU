---
title: Отчеты о действиях в OneDrive
description: Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на OneDrive, в отчетах действий с файлами в OneDrive. Эти отчеты позволят оценить уровень взаимодействия благодаря данным о количестве файлов, к которым предоставлен общий доступ.
localization_priority: Normal
ms.openlocfilehash: bda056970d9147645926dc8753a747f3e6a38662
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878738"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="78b26-104">Отчеты о действиях в OneDrive</span><span class="sxs-lookup"><span data-stu-id="78b26-104">OneDrive activity reports</span></span>

<span data-ttu-id="78b26-105">Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на OneDrive, в отчетах действий с файлами в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="78b26-105">Use the OneDrive activity reports to get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="78b26-106">Эти отчеты позволят оценить уровень взаимодействия благодаря данным о количестве файлов, к которым предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="78b26-106">These reports can help you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="78b26-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="78b26-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="78b26-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="78b26-108">Reports</span></span>

| <span data-ttu-id="78b26-109">Функция</span><span class="sxs-lookup"><span data-stu-id="78b26-109">Function</span></span>                                 | <span data-ttu-id="78b26-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="78b26-110">Return Type</span></span> | <span data-ttu-id="78b26-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78b26-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="78b26-112">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="78b26-112">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="78b26-113">Stream</span><span class="sxs-lookup"><span data-stu-id="78b26-113">Stream</span></span>      | <span data-ttu-id="78b26-114">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="78b26-114">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="78b26-115">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="78b26-115">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="78b26-116">Stream</span><span class="sxs-lookup"><span data-stu-id="78b26-116">Stream</span></span>      | <span data-ttu-id="78b26-117">Получение тренда в отношении количества активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="78b26-117">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="78b26-118">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="78b26-118">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="78b26-119">Stream</span><span class="sxs-lookup"><span data-stu-id="78b26-119">Stream</span></span>      | <span data-ttu-id="78b26-120">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="78b26-120">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |

