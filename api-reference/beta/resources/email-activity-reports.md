---
title: Отчеты о работе с электронной почтой
description: С помощью страницы отчеты вы можете получить высокоуровневое представление трафика электронной почты в вашей организации. Вы также можете перейти на мини-приложение "действия электронной почты", чтобы ознакомиться с тенденциями и сведениями о действиях с электронной почтой в вашей организации.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 7dcfaf2d5cc2d1dbd38cdc4a8a7c5eac71e9539b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499808"
---
# <a name="email-activity-reports"></a><span data-ttu-id="b240f-104">Отчеты о работе с электронной почтой</span><span class="sxs-lookup"><span data-stu-id="b240f-104">Email activity reports</span></span>

<span data-ttu-id="b240f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b240f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b240f-106">С помощью страницы отчеты вы можете получить высокоуровневое представление трафика электронной почты в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="b240f-106">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="b240f-107">Вы также можете перейти на мини-приложение "действия электронной почты", чтобы ознакомиться с тенденциями и сведениями о действиях с электронной почтой в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="b240f-107">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="b240f-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="b240f-108">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="b240f-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="b240f-109">Reports</span></span>

| <span data-ttu-id="b240f-110">Функция</span><span class="sxs-lookup"><span data-stu-id="b240f-110">Function</span></span>                                 | <span data-ttu-id="b240f-111">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="b240f-111">CSV return type</span></span> | <span data-ttu-id="b240f-112">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="b240f-112">JSON return type</span></span>                         | <span data-ttu-id="b240f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b240f-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="b240f-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="b240f-114">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="b240f-115">Stream</span><span class="sxs-lookup"><span data-stu-id="b240f-115">Stream</span></span>          | [<span data-ttu-id="b240f-116">емаилактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="b240f-116">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="b240f-117">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="b240f-117">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="b240f-118">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="b240f-118">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="b240f-119">Stream</span><span class="sxs-lookup"><span data-stu-id="b240f-119">Stream</span></span>          | [<span data-ttu-id="b240f-120">емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="b240f-120">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="b240f-121">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="b240f-121">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="b240f-122">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="b240f-122">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="b240f-123">Stream</span><span class="sxs-lookup"><span data-stu-id="b240f-123">Stream</span></span>          | [<span data-ttu-id="b240f-124">емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="b240f-124">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="b240f-125">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="b240f-125">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
