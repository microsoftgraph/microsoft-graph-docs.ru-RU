---
title: Отчеты о работе с электронной почтой
description: Высокоуровневое представление трафика электронной почты можно получить в рамках организации на странице отчеты. Вы также можете перейти в мини-приложения электронной почты активности понять тенденции и сведения на одного пользователя действия электронной почты в вашей организации.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: e11de43f197e520d653961af9b9090d06b085369
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528307"
---
# <a name="email-activity-reports"></a><span data-ttu-id="7d01c-104">Отчеты о работе с электронной почтой</span><span class="sxs-lookup"><span data-stu-id="7d01c-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d01c-105">Высокоуровневое представление трафика электронной почты можно получить в рамках организации на странице отчеты.</span><span class="sxs-lookup"><span data-stu-id="7d01c-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="7d01c-106">Вы также можете перейти в мини-приложения электронной почты активности понять тенденции и сведения на одного пользователя действия электронной почты в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="7d01c-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="7d01c-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="7d01c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="7d01c-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="7d01c-108">Reports</span></span>

| <span data-ttu-id="7d01c-109">Функция</span><span class="sxs-lookup"><span data-stu-id="7d01c-109">Function</span></span>                                 | <span data-ttu-id="7d01c-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="7d01c-110">CSV return type</span></span> | <span data-ttu-id="7d01c-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="7d01c-111">JSON return type</span></span>                         | <span data-ttu-id="7d01c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7d01c-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="7d01c-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="7d01c-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="7d01c-114">Stream</span><span class="sxs-lookup"><span data-stu-id="7d01c-114">Stream</span></span>          | [<span data-ttu-id="7d01c-115">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7d01c-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="7d01c-116">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="7d01c-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="7d01c-117">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="7d01c-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="7d01c-118">Stream</span><span class="sxs-lookup"><span data-stu-id="7d01c-118">Stream</span></span>          | [<span data-ttu-id="7d01c-119">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="7d01c-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="7d01c-120">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="7d01c-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="7d01c-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="7d01c-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="7d01c-122">Поток</span><span class="sxs-lookup"><span data-stu-id="7d01c-122">Stream</span></span>          | [<span data-ttu-id="7d01c-123">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="7d01c-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="7d01c-124">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="7d01c-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
