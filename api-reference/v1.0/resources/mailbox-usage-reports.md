---
title: Отчеты об использовании почтовых ящиков
description: Эти отчеты позволяют получить сведения о пользователях почтовых ящиков и уровне их активности, основанном на количестве отправленных и полученных писем. Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.
localization_priority: Priority
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: d460f2c72878065abdd1df2fa58dc0eb8f4d411b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981118"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="64d6a-104">Отчеты об использовании почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="64d6a-104">Mailbox usage reports</span></span>

<span data-ttu-id="64d6a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64d6a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64d6a-106">Эти отчеты позволяют получить сведения о пользователях почтовых ящиков и уровне их активности, основанном на количестве отправленных и полученных писем.</span><span class="sxs-lookup"><span data-stu-id="64d6a-106">Use the mailbox usage reports to get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="64d6a-107">Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.</span><span class="sxs-lookup"><span data-stu-id="64d6a-107">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="64d6a-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — использование почтовых ящиков](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="64d6a-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="64d6a-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="64d6a-109">Reports</span></span>

| <span data-ttu-id="64d6a-110">Функция</span><span class="sxs-lookup"><span data-stu-id="64d6a-110">Function</span></span>                                 | <span data-ttu-id="64d6a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="64d6a-111">Return Type</span></span> | <span data-ttu-id="64d6a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="64d6a-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="64d6a-113">Получение сведений о почтовых ящиках</span><span class="sxs-lookup"><span data-stu-id="64d6a-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="64d6a-114">Поток</span><span class="sxs-lookup"><span data-stu-id="64d6a-114">Stream</span></span>      | <span data-ttu-id="64d6a-115">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="64d6a-115">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="64d6a-116">Получение количества почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="64d6a-116">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="64d6a-117">Поток</span><span class="sxs-lookup"><span data-stu-id="64d6a-117">Stream</span></span>      | <span data-ttu-id="64d6a-118">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="64d6a-118">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="64d6a-119">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="64d6a-119">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="64d6a-120">Получение количества почтовых ящиков по состоянию квоты</span><span class="sxs-lookup"><span data-stu-id="64d6a-120">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="64d6a-121">Поток</span><span class="sxs-lookup"><span data-stu-id="64d6a-121">Stream</span></span>      | <span data-ttu-id="64d6a-122">Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.</span><span class="sxs-lookup"><span data-stu-id="64d6a-122">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="64d6a-123">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="64d6a-123">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="64d6a-124">Поток</span><span class="sxs-lookup"><span data-stu-id="64d6a-124">Stream</span></span>      | <span data-ttu-id="64d6a-125">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="64d6a-125">Get the amount of storage used in your organization.</span></span> |

