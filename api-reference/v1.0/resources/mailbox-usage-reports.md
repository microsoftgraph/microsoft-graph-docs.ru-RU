---
title: Отчеты об использовании почтовых ящиков
description: Эти отчеты позволяют получить сведения о пользователях почтовых ящиков и уровне их активности, основанном на количестве отправленных и полученных писем. Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.
localization_priority: Priority
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 3c7b932bf7f0747ff6b5050f7e19accf871c1b1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447516"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="011cd-104">Отчеты об использовании почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="011cd-104">Mailbox usage reports</span></span>

<span data-ttu-id="011cd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="011cd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="011cd-106">Эти отчеты позволяют получить сведения о пользователях почтовых ящиков и уровне их активности, основанном на количестве отправленных и полученных писем.</span><span class="sxs-lookup"><span data-stu-id="011cd-106">Use the mailbox usage reports to get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="011cd-107">Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.</span><span class="sxs-lookup"><span data-stu-id="011cd-107">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="011cd-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="011cd-108">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="011cd-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="011cd-109">Reports</span></span>

| <span data-ttu-id="011cd-110">Функция</span><span class="sxs-lookup"><span data-stu-id="011cd-110">Function</span></span>                                 | <span data-ttu-id="011cd-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="011cd-111">Return Type</span></span> | <span data-ttu-id="011cd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="011cd-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="011cd-113">Получение сведений о почтовых ящиках</span><span class="sxs-lookup"><span data-stu-id="011cd-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="011cd-114">Поток</span><span class="sxs-lookup"><span data-stu-id="011cd-114">Stream</span></span>      | <span data-ttu-id="011cd-115">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="011cd-115">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="011cd-116">Получение количества почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="011cd-116">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="011cd-117">Поток</span><span class="sxs-lookup"><span data-stu-id="011cd-117">Stream</span></span>      | <span data-ttu-id="011cd-118">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="011cd-118">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="011cd-119">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="011cd-119">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="011cd-120">Получение количества почтовых ящиков по состоянию квоты</span><span class="sxs-lookup"><span data-stu-id="011cd-120">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="011cd-121">Поток</span><span class="sxs-lookup"><span data-stu-id="011cd-121">Stream</span></span>      | <span data-ttu-id="011cd-122">Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.</span><span class="sxs-lookup"><span data-stu-id="011cd-122">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="011cd-123">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="011cd-123">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="011cd-124">Поток</span><span class="sxs-lookup"><span data-stu-id="011cd-124">Stream</span></span>      | <span data-ttu-id="011cd-125">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="011cd-125">Get the amount of storage used in your organization.</span></span> |
