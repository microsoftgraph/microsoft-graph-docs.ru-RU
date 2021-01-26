---
title: Отчеты о работе с электронной почтой
description: Вы можете получить высокоуровневый вид трафика электронной почты в организации на странице "Отчеты". Кроме того, вы можете подробно и подробно разобраться в мини-приложениях "Действия с электронной почтой" в вашей организации.
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: db9ea032b418a6beca7afb7c15eb16b762e6ed11
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983800"
---
# <a name="email-activity-reports"></a><span data-ttu-id="1f5a6-104">Отчеты о работе с электронной почтой</span><span class="sxs-lookup"><span data-stu-id="1f5a6-104">Email activity reports</span></span>

<span data-ttu-id="1f5a6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f5a6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f5a6-106">Вы можете получить высокоуровневый вид трафика электронной почты в организации на странице "Отчеты".</span><span class="sxs-lookup"><span data-stu-id="1f5a6-106">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="1f5a6-107">Вы также можете и подробно разобраться в мини-приложениях "Действия с электронной почтой" в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="1f5a6-107">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="1f5a6-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Действия с почтой](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="1f5a6-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="1f5a6-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="1f5a6-109">Reports</span></span>

| <span data-ttu-id="1f5a6-110">Функция</span><span class="sxs-lookup"><span data-stu-id="1f5a6-110">Function</span></span>                                 | <span data-ttu-id="1f5a6-111">Тип возврата CSV</span><span class="sxs-lookup"><span data-stu-id="1f5a6-111">CSV return type</span></span> | <span data-ttu-id="1f5a6-112">Тип возврата JSON</span><span class="sxs-lookup"><span data-stu-id="1f5a6-112">JSON return type</span></span>                         | <span data-ttu-id="1f5a6-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1f5a6-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="1f5a6-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="1f5a6-114">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="1f5a6-115">Stream</span><span class="sxs-lookup"><span data-stu-id="1f5a6-115">Stream</span></span>          | [<span data-ttu-id="1f5a6-116">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="1f5a6-116">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="1f5a6-117">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="1f5a6-117">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="1f5a6-118">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="1f5a6-118">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="1f5a6-119">Stream</span><span class="sxs-lookup"><span data-stu-id="1f5a6-119">Stream</span></span>          | [<span data-ttu-id="1f5a6-120">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="1f5a6-120">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="1f5a6-121">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="1f5a6-121">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="1f5a6-122">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="1f5a6-122">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="1f5a6-123">Stream</span><span class="sxs-lookup"><span data-stu-id="1f5a6-123">Stream</span></span>          | [<span data-ttu-id="1f5a6-124">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="1f5a6-124">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="1f5a6-125">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="1f5a6-125">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |


