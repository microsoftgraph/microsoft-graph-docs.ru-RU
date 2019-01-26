---
title: Отчеты о действиях в Yammer
description: Вы понимаете обязательства вашей организации с помощью Yammer с активности создается в организации и число уникальных пользователей, публиковать, такие как и читать сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d5953d8bd53158b2ec0532deb47c48028ba1b8c9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571802"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="8d4d0-103">Отчеты о действиях в Yammer</span><span class="sxs-lookup"><span data-stu-id="8d4d0-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d4d0-104">Вы понимаете обязательства вашей организации с помощью Yammer с активности создается в организации и число уникальных пользователей, публиковать, такие как и читать сообщения в Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d4d0-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="8d4d0-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="8d4d0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="8d4d0-106">Отчеты</span><span class="sxs-lookup"><span data-stu-id="8d4d0-106">Reports</span></span>

| <span data-ttu-id="8d4d0-107">Функция</span><span class="sxs-lookup"><span data-stu-id="8d4d0-107">Function</span></span>                                 | <span data-ttu-id="8d4d0-108">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="8d4d0-108">CSV return type</span></span> | <span data-ttu-id="8d4d0-109">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="8d4d0-109">JSON return type</span></span>                         | <span data-ttu-id="8d4d0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8d4d0-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="8d4d0-111">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="8d4d0-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="8d4d0-112">Stream</span><span class="sxs-lookup"><span data-stu-id="8d4d0-112">Stream</span></span>          | [<span data-ttu-id="8d4d0-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="8d4d0-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="8d4d0-114">Получение сведений о действиях в Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="8d4d0-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="8d4d0-115">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="8d4d0-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="8d4d0-116">Stream</span><span class="sxs-lookup"><span data-stu-id="8d4d0-116">Stream</span></span>          | [<span data-ttu-id="8d4d0-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="8d4d0-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="8d4d0-118">Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="8d4d0-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="8d4d0-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="8d4d0-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="8d4d0-120">Stream</span><span class="sxs-lookup"><span data-stu-id="8d4d0-120">Stream</span></span>          | [<span data-ttu-id="8d4d0-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="8d4d0-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="8d4d0-122">Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d4d0-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
