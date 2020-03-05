---
title: Отчеты о действиях в OneDrive
description: Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию, для использования OneDrive, изучив их взаимодействие с файлами в OneDrive. Кроме того, вы можете ознакомиться с уровнем совместной работы, в котором показано количество файлов, к которым предоставлен общий доступ.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0aba91a64b7dbefc894a968a427995bd6e984f79
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522409"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="eac33-104">Отчеты о действиях в OneDrive</span><span class="sxs-lookup"><span data-stu-id="eac33-104">OneDrive activity reports</span></span>

<span data-ttu-id="eac33-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eac33-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eac33-106">Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию, для использования OneDrive, изучив их взаимодействие с файлами в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="eac33-106">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="eac33-107">Кроме того, вы можете ознакомиться с уровнем совместной работы, в котором показано количество файлов, к которым предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="eac33-107">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="eac33-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="eac33-108">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="eac33-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="eac33-109">Reports</span></span>

| <span data-ttu-id="eac33-110">Функция</span><span class="sxs-lookup"><span data-stu-id="eac33-110">Function</span></span>                                 | <span data-ttu-id="eac33-111">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="eac33-111">CSV return type</span></span> | <span data-ttu-id="eac33-112">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="eac33-112">JSON return type</span></span>                         | <span data-ttu-id="eac33-113">Описание</span><span class="sxs-lookup"><span data-stu-id="eac33-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="eac33-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="eac33-114">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="eac33-115">Stream</span><span class="sxs-lookup"><span data-stu-id="eac33-115">Stream</span></span>          | [<span data-ttu-id="eac33-116">онедривеактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="eac33-116">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="eac33-117">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="eac33-117">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="eac33-118">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="eac33-118">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="eac33-119">Stream</span><span class="sxs-lookup"><span data-stu-id="eac33-119">Stream</span></span>          | [<span data-ttu-id="eac33-120">ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="eac33-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="eac33-121">Получение тренда в отношении количества активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="eac33-121">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="eac33-122">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="eac33-122">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="eac33-123">Stream</span><span class="sxs-lookup"><span data-stu-id="eac33-123">Stream</span></span>          | [<span data-ttu-id="eac33-124">ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="eac33-124">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="eac33-125">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="eac33-125">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
