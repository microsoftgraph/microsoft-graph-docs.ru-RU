---
title: Отчеты об использовании почтовых ящиков
description: Вы можете получить сведения о пользователях с почтовым ящиком и их уровнем активности, которые в основном основаны на отправленных и полученных сообщениях электронной почты. Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: ae0b3294750271f32d91dca79f75e7cf44641045
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463532"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="5e80f-104">Отчеты об использовании почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="5e80f-104">Mailbox usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e80f-105">Вы можете получить сведения о пользователях с почтовым ящиком и их уровнем активности, которые в основном основаны на отправленных и полученных сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5e80f-105">You can get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="5e80f-106">Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.</span><span class="sxs-lookup"><span data-stu-id="5e80f-106">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="5e80f-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="5e80f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="5e80f-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="5e80f-108">Reports</span></span>

| <span data-ttu-id="5e80f-109">Функция</span><span class="sxs-lookup"><span data-stu-id="5e80f-109">Function</span></span>                                 | <span data-ttu-id="5e80f-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="5e80f-110">CSV return type</span></span> | <span data-ttu-id="5e80f-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="5e80f-111">JSON return type</span></span>                         | <span data-ttu-id="5e80f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5e80f-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="5e80f-113">Получение сведений о почтовых ящиках</span><span class="sxs-lookup"><span data-stu-id="5e80f-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="5e80f-114">Stream</span><span class="sxs-lookup"><span data-stu-id="5e80f-114">Stream</span></span>          | [<span data-ttu-id="5e80f-115">Маилбоксусажедетаил</span><span class="sxs-lookup"><span data-stu-id="5e80f-115">mailboxUsageDetail</span></span>](../resources/mailboxusagedetail.md) | <span data-ttu-id="5e80f-116">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="5e80f-116">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="5e80f-117">Получение количества почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="5e80f-117">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="5e80f-118">Stream</span><span class="sxs-lookup"><span data-stu-id="5e80f-118">Stream</span></span>          | [<span data-ttu-id="5e80f-119">Маилбоксусажемаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="5e80f-119">mailboxUsageMailboxCounts</span></span>](../resources/mailboxusagemailboxcounts.md) | <span data-ttu-id="5e80f-120">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5e80f-120">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="5e80f-121">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="5e80f-121">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="5e80f-122">Получение количества почтовых ящиков по состоянию квоты</span><span class="sxs-lookup"><span data-stu-id="5e80f-122">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="5e80f-123">Stream</span><span class="sxs-lookup"><span data-stu-id="5e80f-123">Stream</span></span>          | [<span data-ttu-id="5e80f-124">Маилбоксусажекуотастатусмаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="5e80f-124">mailboxUsageQuotaStatusMailboxCounts</span></span>](../resources/mailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="5e80f-125">Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.</span><span class="sxs-lookup"><span data-stu-id="5e80f-125">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="5e80f-126">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="5e80f-126">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="5e80f-127">Stream</span><span class="sxs-lookup"><span data-stu-id="5e80f-127">Stream</span></span>          | [<span data-ttu-id="5e80f-128">Маилбоксусажестораже</span><span class="sxs-lookup"><span data-stu-id="5e80f-128">mailboxUsageStorage</span></span>](../resources/mailboxusagestorage.md) | <span data-ttu-id="5e80f-129">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="5e80f-129">Get the amount of storage used in your organization.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailbox-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
