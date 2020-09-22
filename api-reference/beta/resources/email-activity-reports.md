---
title: Отчеты о работе с электронной почтой
description: С помощью страницы отчеты вы можете получить высокоуровневое представление трафика электронной почты в вашей организации. Вы также можете перейти на мини-приложение "действия электронной почты", чтобы ознакомиться с тенденциями и сведениями о действиях с электронной почтой в вашей организации.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: f3c1ccd2700bce7a054cfec8fed943c01a3f4a1c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055549"
---
# <a name="email-activity-reports"></a><span data-ttu-id="672aa-104">Отчеты о работе с электронной почтой</span><span class="sxs-lookup"><span data-stu-id="672aa-104">Email activity reports</span></span>

<span data-ttu-id="672aa-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="672aa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="672aa-106">С помощью страницы отчеты вы можете получить высокоуровневое представление трафика электронной почты в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="672aa-106">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="672aa-107">Вы также можете перейти на мини-приложение "действия электронной почты", чтобы ознакомиться с тенденциями и сведениями о действиях с электронной почтой в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="672aa-107">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="672aa-108">**Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-Activity email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="672aa-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="672aa-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="672aa-109">Reports</span></span>

| <span data-ttu-id="672aa-110">Функция</span><span class="sxs-lookup"><span data-stu-id="672aa-110">Function</span></span>                                 | <span data-ttu-id="672aa-111">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="672aa-111">CSV return type</span></span> | <span data-ttu-id="672aa-112">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="672aa-112">JSON return type</span></span>                         | <span data-ttu-id="672aa-113">Описание</span><span class="sxs-lookup"><span data-stu-id="672aa-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="672aa-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="672aa-114">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="672aa-115">Stream</span><span class="sxs-lookup"><span data-stu-id="672aa-115">Stream</span></span>          | [<span data-ttu-id="672aa-116">емаилактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="672aa-116">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="672aa-117">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="672aa-117">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="672aa-118">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="672aa-118">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="672aa-119">Stream</span><span class="sxs-lookup"><span data-stu-id="672aa-119">Stream</span></span>          | [<span data-ttu-id="672aa-120">емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="672aa-120">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="672aa-121">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="672aa-121">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="672aa-122">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="672aa-122">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="672aa-123">Stream</span><span class="sxs-lookup"><span data-stu-id="672aa-123">Stream</span></span>          | [<span data-ttu-id="672aa-124">емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="672aa-124">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="672aa-125">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="672aa-125">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |


