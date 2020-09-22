---
title: Отчеты о работе с электронной почтой
description: Эти отчеты позволяют получить общее представление о трафике электронной почты в организации. Вы также можете посмотреть развернутые отчеты, чтобы понять динамику и особенности работы с электронной почтой каждого пользователя в организации.
localization_priority: Priority
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 59a003d8dc14f913efbfe8dc42c993093b11b21d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018587"
---
# <a name="email-activity-reports"></a><span data-ttu-id="d39d3-104">Отчеты о работе с электронной почтой</span><span class="sxs-lookup"><span data-stu-id="d39d3-104">Email activity reports</span></span>

<span data-ttu-id="d39d3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d39d3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d39d3-106">Эти отчеты позволяют получить общее представление о трафике электронной почты в организации.</span><span class="sxs-lookup"><span data-stu-id="d39d3-106">Use the email activity reports to get a high level view of email traffic within your organization.</span></span> <span data-ttu-id="d39d3-107">Вы также можете посмотреть развернутые отчеты, чтобы понять динамику и особенности работы с электронной почтой каждого пользователя в организации.</span><span class="sxs-lookup"><span data-stu-id="d39d3-107">You can also drill into the Email Activity widget to understand the trends and details of the email activity per user in your organization.</span></span>

> <span data-ttu-id="d39d3-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Действия с почтой](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="d39d3-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="d39d3-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="d39d3-109">Reports</span></span>

| <span data-ttu-id="d39d3-110">Функция</span><span class="sxs-lookup"><span data-stu-id="d39d3-110">Function</span></span>                                 | <span data-ttu-id="d39d3-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d39d3-111">Return Type</span></span> | <span data-ttu-id="d39d3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d39d3-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="d39d3-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="d39d3-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="d39d3-114">Поток</span><span class="sxs-lookup"><span data-stu-id="d39d3-114">Stream</span></span>      | <span data-ttu-id="d39d3-115">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="d39d3-115">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="d39d3-116">Получение количества действий</span><span class="sxs-lookup"><span data-stu-id="d39d3-116">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="d39d3-117">Поток</span><span class="sxs-lookup"><span data-stu-id="d39d3-117">Stream</span></span>      | <span data-ttu-id="d39d3-118">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="d39d3-118">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="d39d3-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="d39d3-119">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="d39d3-120">Поток</span><span class="sxs-lookup"><span data-stu-id="d39d3-120">Stream</span></span>      | <span data-ttu-id="d39d3-121">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="d39d3-121">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |

