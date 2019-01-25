---
title: Отчеты о действиях в OneDrive
description: Можно получить активности каждый пользователь с лицензии на использование OneDrive, посмотрев их взаимодействие с файлами на OneDrive. Он также помогает понять уровень совместной работы более подробное с отображением число общих файлов.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 9075bd042a0c27debc8017a007351428191e9d43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519229"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="c01e2-104">Отчеты о действиях в OneDrive</span><span class="sxs-lookup"><span data-stu-id="c01e2-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c01e2-105">Можно получить активности каждый пользователь с лицензии на использование OneDrive, посмотрев их взаимодействие с файлами на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c01e2-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="c01e2-106">Он также помогает понять уровень совместной работы более подробное с отображением число общих файлов.</span><span class="sxs-lookup"><span data-stu-id="c01e2-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="c01e2-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="c01e2-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="c01e2-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="c01e2-108">Reports</span></span>

| <span data-ttu-id="c01e2-109">Функция</span><span class="sxs-lookup"><span data-stu-id="c01e2-109">Function</span></span>                                 | <span data-ttu-id="c01e2-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="c01e2-110">CSV return type</span></span> | <span data-ttu-id="c01e2-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="c01e2-111">JSON return type</span></span>                         | <span data-ttu-id="c01e2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c01e2-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="c01e2-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="c01e2-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="c01e2-114">Stream</span><span class="sxs-lookup"><span data-stu-id="c01e2-114">Stream</span></span>          | [<span data-ttu-id="c01e2-115">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c01e2-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="c01e2-116">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="c01e2-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="c01e2-117">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="c01e2-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="c01e2-118">Stream</span><span class="sxs-lookup"><span data-stu-id="c01e2-118">Stream</span></span>          | [<span data-ttu-id="c01e2-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="c01e2-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="c01e2-120">Получение тренда в отношении количества активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c01e2-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="c01e2-121">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="c01e2-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="c01e2-122">Stream</span><span class="sxs-lookup"><span data-stu-id="c01e2-122">Stream</span></span>          | [<span data-ttu-id="c01e2-123">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="c01e2-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="c01e2-124">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c01e2-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
