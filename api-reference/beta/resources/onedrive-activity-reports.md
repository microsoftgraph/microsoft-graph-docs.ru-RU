---
title: Отчеты о действиях в OneDrive
description: Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию, для использования OneDrive, изучив их взаимодействие с файлами в OneDrive. Кроме того, вы можете ознакомиться с уровнем совместной работы, в котором показано количество файлов, к которым предоставлен общий доступ.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d545f1d92beee89e19eb47cfd8c6ba8c391c5349
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457100"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="219cf-104">Отчеты о действиях в OneDrive</span><span class="sxs-lookup"><span data-stu-id="219cf-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="219cf-105">Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию, для использования OneDrive, изучив их взаимодействие с файлами в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="219cf-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="219cf-106">Кроме того, вы можете ознакомиться с уровнем совместной работы, в котором показано количество файлов, к которым предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="219cf-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="219cf-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="219cf-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="219cf-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="219cf-108">Reports</span></span>

| <span data-ttu-id="219cf-109">Функция</span><span class="sxs-lookup"><span data-stu-id="219cf-109">Function</span></span>                                 | <span data-ttu-id="219cf-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="219cf-110">CSV return type</span></span> | <span data-ttu-id="219cf-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="219cf-111">JSON return type</span></span>                         | <span data-ttu-id="219cf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="219cf-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="219cf-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="219cf-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="219cf-114">Stream</span><span class="sxs-lookup"><span data-stu-id="219cf-114">Stream</span></span>          | [<span data-ttu-id="219cf-115">Онедривеактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="219cf-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="219cf-116">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="219cf-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="219cf-117">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="219cf-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="219cf-118">Stream</span><span class="sxs-lookup"><span data-stu-id="219cf-118">Stream</span></span>          | [<span data-ttu-id="219cf-119">Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="219cf-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="219cf-120">Получение тренда в отношении количества активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="219cf-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="219cf-121">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="219cf-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="219cf-122">Stream</span><span class="sxs-lookup"><span data-stu-id="219cf-122">Stream</span></span>          | [<span data-ttu-id="219cf-123">Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="219cf-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="219cf-124">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="219cf-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
