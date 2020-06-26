---
title: Отчеты о действиях в OneDrive
description: Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию, для использования OneDrive, изучив их взаимодействие с файлами в OneDrive. Кроме того, вы можете ознакомиться с уровнем совместной работы, в котором показано количество файлов, к которым предоставлен общий доступ.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 199b2f58b591e011bdb530bd109619cdc125a637
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897101"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="0971a-104">Отчеты о действиях в OneDrive</span><span class="sxs-lookup"><span data-stu-id="0971a-104">OneDrive activity reports</span></span>

<span data-ttu-id="0971a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0971a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0971a-106">Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию, для использования OneDrive, изучив их взаимодействие с файлами в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0971a-106">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="0971a-107">Кроме того, вы можете ознакомиться с уровнем совместной работы, в котором показано количество файлов, к которым предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="0971a-107">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="0971a-108">**Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-Activity for OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="0971a-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="0971a-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="0971a-109">Reports</span></span>

| <span data-ttu-id="0971a-110">Функция</span><span class="sxs-lookup"><span data-stu-id="0971a-110">Function</span></span>                                 | <span data-ttu-id="0971a-111">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="0971a-111">CSV return type</span></span> | <span data-ttu-id="0971a-112">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="0971a-112">JSON return type</span></span>                         | <span data-ttu-id="0971a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="0971a-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="0971a-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="0971a-114">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="0971a-115">Stream</span><span class="sxs-lookup"><span data-stu-id="0971a-115">Stream</span></span>          | [<span data-ttu-id="0971a-116">онедривеактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="0971a-116">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="0971a-117">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="0971a-117">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="0971a-118">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="0971a-118">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="0971a-119">Stream</span><span class="sxs-lookup"><span data-stu-id="0971a-119">Stream</span></span>          | [<span data-ttu-id="0971a-120">ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="0971a-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="0971a-121">Получение тренда в отношении количества активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0971a-121">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="0971a-122">Получение количества файлов</span><span class="sxs-lookup"><span data-stu-id="0971a-122">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="0971a-123">Stream</span><span class="sxs-lookup"><span data-stu-id="0971a-123">Stream</span></span>          | [<span data-ttu-id="0971a-124">ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="0971a-124">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="0971a-125">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0971a-125">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
