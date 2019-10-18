---
title: Отчеты об использовании почтовых ящиков
description: Эти отчеты позволяют получить сведения о пользователях почтовых ящиков и уровне их активности, основанном на количестве отправленных и полученных писем. Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.
localization_priority: Priority
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: f88f940541bee75a6898ac638fe80e44fc368320
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036297"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="084d5-104">Отчеты об использовании почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="084d5-104">Mailbox usage reports</span></span>

<span data-ttu-id="084d5-105">Эти отчеты позволяют получить сведения о пользователях почтовых ящиков и уровне их активности, основанном на количестве отправленных и полученных писем.</span><span class="sxs-lookup"><span data-stu-id="084d5-105">Use the mailbox usage reports to get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="084d5-106">Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.</span><span class="sxs-lookup"><span data-stu-id="084d5-106">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="084d5-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="084d5-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="084d5-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="084d5-108">Reports</span></span>

| <span data-ttu-id="084d5-109">Функция</span><span class="sxs-lookup"><span data-stu-id="084d5-109">Function</span></span>                                 | <span data-ttu-id="084d5-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="084d5-110">Return Type</span></span> | <span data-ttu-id="084d5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="084d5-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="084d5-112">Получение сведений о почтовых ящиках</span><span class="sxs-lookup"><span data-stu-id="084d5-112">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="084d5-113">Поток</span><span class="sxs-lookup"><span data-stu-id="084d5-113">Stream</span></span>      | <span data-ttu-id="084d5-114">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="084d5-114">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="084d5-115">Получение количества почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="084d5-115">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="084d5-116">Поток</span><span class="sxs-lookup"><span data-stu-id="084d5-116">Stream</span></span>      | <span data-ttu-id="084d5-117">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="084d5-117">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="084d5-118">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="084d5-118">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="084d5-119">Получение количества почтовых ящиков по состоянию квоты</span><span class="sxs-lookup"><span data-stu-id="084d5-119">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="084d5-120">Поток</span><span class="sxs-lookup"><span data-stu-id="084d5-120">Stream</span></span>      | <span data-ttu-id="084d5-121">Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.</span><span class="sxs-lookup"><span data-stu-id="084d5-121">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="084d5-122">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="084d5-122">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="084d5-123">Поток</span><span class="sxs-lookup"><span data-stu-id="084d5-123">Stream</span></span>      | <span data-ttu-id="084d5-124">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="084d5-124">Get the amount of storage used in your organization.</span></span> |
