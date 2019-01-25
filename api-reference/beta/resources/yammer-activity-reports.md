---
title: Отчеты о действиях в Yammer
description: Вы понимаете обязательства вашей организации с помощью Yammer с активности создается в организации и число уникальных пользователей, публиковать, такие как и читать сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 252748b639f256467b2a01336488e1df086c69cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509940"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="25854-103">Отчеты о действиях в Yammer</span><span class="sxs-lookup"><span data-stu-id="25854-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25854-104">Вы понимаете обязательства вашей организации с помощью Yammer с активности создается в организации и число уникальных пользователей, публиковать, такие как и читать сообщения в Yammer.</span><span class="sxs-lookup"><span data-stu-id="25854-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="25854-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="25854-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="25854-106">Отчеты</span><span class="sxs-lookup"><span data-stu-id="25854-106">Reports</span></span>

| <span data-ttu-id="25854-107">Функция</span><span class="sxs-lookup"><span data-stu-id="25854-107">Function</span></span>                                 | <span data-ttu-id="25854-108">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="25854-108">CSV return type</span></span> | <span data-ttu-id="25854-109">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="25854-109">JSON return type</span></span>                         | <span data-ttu-id="25854-110">Описание</span><span class="sxs-lookup"><span data-stu-id="25854-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="25854-111">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="25854-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="25854-112">Stream</span><span class="sxs-lookup"><span data-stu-id="25854-112">Stream</span></span>          | [<span data-ttu-id="25854-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="25854-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="25854-114">Получение сведений о действиях в Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="25854-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="25854-115">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="25854-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="25854-116">Stream</span><span class="sxs-lookup"><span data-stu-id="25854-116">Stream</span></span>          | [<span data-ttu-id="25854-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="25854-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="25854-118">Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="25854-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="25854-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="25854-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="25854-120">Поток</span><span class="sxs-lookup"><span data-stu-id="25854-120">Stream</span></span>          | [<span data-ttu-id="25854-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="25854-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="25854-122">Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.</span><span class="sxs-lookup"><span data-stu-id="25854-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
