---
title: Отчеты о работе с электронной почтой
description: Высокоуровневое представление трафика электронной почты можно получить в рамках организации на странице отчеты. Вы также можете перейти в мини-приложения электронной почты активности понять тенденции и сведения на одного пользователя действия электронной почты в вашей организации.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 748199a2e846cc71a3f04c3ea1bda97dcf2c7301
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573902"
---
# <a name="email-activity-reports"></a><span data-ttu-id="f7b49-104">Отчеты о работе с электронной почтой</span><span class="sxs-lookup"><span data-stu-id="f7b49-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b49-105">Высокоуровневое представление трафика электронной почты можно получить в рамках организации на странице отчеты.</span><span class="sxs-lookup"><span data-stu-id="f7b49-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="f7b49-106">Вы также можете перейти в мини-приложения электронной почты активности понять тенденции и сведения на одного пользователя действия электронной почты в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="f7b49-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="f7b49-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="f7b49-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="f7b49-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="f7b49-108">Reports</span></span>

| <span data-ttu-id="f7b49-109">Функция</span><span class="sxs-lookup"><span data-stu-id="f7b49-109">Function</span></span>                                 | <span data-ttu-id="f7b49-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="f7b49-110">CSV return type</span></span> | <span data-ttu-id="f7b49-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="f7b49-111">JSON return type</span></span>                         | <span data-ttu-id="f7b49-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f7b49-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="f7b49-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="f7b49-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="f7b49-114">Stream</span><span class="sxs-lookup"><span data-stu-id="f7b49-114">Stream</span></span>          | [<span data-ttu-id="f7b49-115">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f7b49-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="f7b49-116">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="f7b49-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="f7b49-117">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="f7b49-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="f7b49-118">Stream</span><span class="sxs-lookup"><span data-stu-id="f7b49-118">Stream</span></span>          | [<span data-ttu-id="f7b49-119">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="f7b49-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="f7b49-120">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="f7b49-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="f7b49-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="f7b49-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="f7b49-122">Stream</span><span class="sxs-lookup"><span data-stu-id="f7b49-122">Stream</span></span>          | [<span data-ttu-id="f7b49-123">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="f7b49-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="f7b49-124">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="f7b49-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
