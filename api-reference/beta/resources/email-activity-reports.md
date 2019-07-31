---
title: Отчеты о работе с электронной почтой
description: С помощью страницы отчеты вы можете получить высокоуровневое представление трафика электронной почты в вашей организации. Вы также можете перейти на мини-приложение "действия электронной почты", чтобы ознакомиться с тенденциями и сведениями о действиях с электронной почтой в вашей организации.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 2540934b93a1047df5b19c4fe1b477ba30fd798c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972273"
---
# <a name="email-activity-reports"></a><span data-ttu-id="65957-104">Отчеты о работе с электронной почтой</span><span class="sxs-lookup"><span data-stu-id="65957-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65957-105">С помощью страницы отчеты вы можете получить высокоуровневое представление трафика электронной почты в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="65957-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="65957-106">Вы также можете перейти на мини-приложение "действия электронной почты", чтобы ознакомиться с тенденциями и сведениями о действиях с электронной почтой в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="65957-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="65957-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="65957-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="65957-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="65957-108">Reports</span></span>

| <span data-ttu-id="65957-109">Функция</span><span class="sxs-lookup"><span data-stu-id="65957-109">Function</span></span>                                 | <span data-ttu-id="65957-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="65957-110">CSV return type</span></span> | <span data-ttu-id="65957-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="65957-111">JSON return type</span></span>                         | <span data-ttu-id="65957-112">Описание</span><span class="sxs-lookup"><span data-stu-id="65957-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="65957-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="65957-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="65957-114">Поток</span><span class="sxs-lookup"><span data-stu-id="65957-114">Stream</span></span>          | [<span data-ttu-id="65957-115">Емаилактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="65957-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="65957-116">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="65957-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="65957-117">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="65957-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="65957-118">Stream</span><span class="sxs-lookup"><span data-stu-id="65957-118">Stream</span></span>          | [<span data-ttu-id="65957-119">Емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="65957-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="65957-120">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="65957-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="65957-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="65957-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="65957-122">Поток</span><span class="sxs-lookup"><span data-stu-id="65957-122">Stream</span></span>          | [<span data-ttu-id="65957-123">Емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="65957-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="65957-124">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="65957-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
