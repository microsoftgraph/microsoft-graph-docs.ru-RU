---
title: Отчеты о действиях в OneDrive
description: Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию, для использования OneDrive, изучив их взаимодействие с файлами в OneDrive. Кроме того, вы можете ознакомиться с уровнем совместной работы, в котором показано количество файлов, к которым предоставлен общий доступ.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 710b2ed88deeec26846bb5afe7503808d8c470c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009442"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="511a8-104">Отчеты о действиях в OneDrive</span><span class="sxs-lookup"><span data-stu-id="511a8-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="511a8-105">Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию, для использования OneDrive, изучив их взаимодействие с файлами в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="511a8-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="511a8-106">Кроме того, вы можете ознакомиться с уровнем совместной работы, в котором показано количество файлов, к которым предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="511a8-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="511a8-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="511a8-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="511a8-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="511a8-108">Reports</span></span>

| <span data-ttu-id="511a8-109">Функция</span><span class="sxs-lookup"><span data-stu-id="511a8-109">Function</span></span>                                 | <span data-ttu-id="511a8-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="511a8-110">CSV return type</span></span> | <span data-ttu-id="511a8-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="511a8-111">JSON return type</span></span>                         | <span data-ttu-id="511a8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="511a8-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="511a8-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="511a8-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="511a8-114">Поток</span><span class="sxs-lookup"><span data-stu-id="511a8-114">Stream</span></span>          | [<span data-ttu-id="511a8-115">Онедривеактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="511a8-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="511a8-116">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="511a8-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="511a8-117">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="511a8-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="511a8-118">Поток</span><span class="sxs-lookup"><span data-stu-id="511a8-118">Stream</span></span>          | [<span data-ttu-id="511a8-119">Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="511a8-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="511a8-120">Получение тренда в отношении количества активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="511a8-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="511a8-121">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="511a8-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="511a8-122">Stream</span><span class="sxs-lookup"><span data-stu-id="511a8-122">Stream</span></span>          | [<span data-ttu-id="511a8-123">Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="511a8-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="511a8-124">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="511a8-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
