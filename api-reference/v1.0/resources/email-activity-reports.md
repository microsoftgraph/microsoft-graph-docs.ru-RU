---
title: Отчеты о работе с электронной почтой
description: Эти отчеты позволяют получить общее представление о трафике электронной почты в организации. Вы также можете посмотреть развернутые отчеты, чтобы понять динамику и особенности работы с электронной почтой каждого пользователя в организации.
localization_priority: Priority
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 110502c61a25ae046aa17fde72a5ffc64368b1eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531488"
---
# <a name="email-activity-reports"></a><span data-ttu-id="32d0d-104">Отчеты о работе с электронной почтой</span><span class="sxs-lookup"><span data-stu-id="32d0d-104">Email activity reports</span></span>

<span data-ttu-id="32d0d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32d0d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32d0d-106">Эти отчеты позволяют получить общее представление о трафике электронной почты в организации.</span><span class="sxs-lookup"><span data-stu-id="32d0d-106">Use the email activity reports to get a high level view of email traffic within your organization.</span></span> <span data-ttu-id="32d0d-107">Вы также можете посмотреть развернутые отчеты, чтобы понять динамику и особенности работы с электронной почтой каждого пользователя в организации.</span><span class="sxs-lookup"><span data-stu-id="32d0d-107">You can also drill into the Email Activity widget to understand the trends and details of the email activity per user in your organization.</span></span>

> <span data-ttu-id="32d0d-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="32d0d-108">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="32d0d-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="32d0d-109">Reports</span></span>

| <span data-ttu-id="32d0d-110">Функция</span><span class="sxs-lookup"><span data-stu-id="32d0d-110">Function</span></span>                                 | <span data-ttu-id="32d0d-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="32d0d-111">Return Type</span></span> | <span data-ttu-id="32d0d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="32d0d-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="32d0d-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="32d0d-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="32d0d-114">Поток</span><span class="sxs-lookup"><span data-stu-id="32d0d-114">Stream</span></span>      | <span data-ttu-id="32d0d-115">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="32d0d-115">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="32d0d-116">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="32d0d-116">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="32d0d-117">Поток</span><span class="sxs-lookup"><span data-stu-id="32d0d-117">Stream</span></span>      | <span data-ttu-id="32d0d-118">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="32d0d-118">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="32d0d-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="32d0d-119">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="32d0d-120">Поток</span><span class="sxs-lookup"><span data-stu-id="32d0d-120">Stream</span></span>      | <span data-ttu-id="32d0d-121">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="32d0d-121">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
