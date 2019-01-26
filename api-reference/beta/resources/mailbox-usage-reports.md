---
title: Отчеты об использовании почтовых ящиков
description: Вы можете получать сведения о пользователях с почтового ящика и их уровень активности в основном основанное на сообщения электронной почты, отправленных и полученных. Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: ae0b3294750271f32d91dca79f75e7cf44641045
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576327"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="ddb85-104">Отчеты об использовании почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="ddb85-104">Mailbox usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddb85-105">Вы можете получать сведения о пользователях с почтового ящика и их уровень активности в основном основанное на сообщения электронной почты, отправленных и полученных.</span><span class="sxs-lookup"><span data-stu-id="ddb85-105">You can get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="ddb85-106">Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.</span><span class="sxs-lookup"><span data-stu-id="ddb85-106">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="ddb85-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="ddb85-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="ddb85-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="ddb85-108">Reports</span></span>

| <span data-ttu-id="ddb85-109">Функция</span><span class="sxs-lookup"><span data-stu-id="ddb85-109">Function</span></span>                                 | <span data-ttu-id="ddb85-110">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="ddb85-110">CSV return type</span></span> | <span data-ttu-id="ddb85-111">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="ddb85-111">JSON return type</span></span>                         | <span data-ttu-id="ddb85-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb85-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ddb85-113">Получение сведений о почтовых ящиках</span><span class="sxs-lookup"><span data-stu-id="ddb85-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="ddb85-114">Поток</span><span class="sxs-lookup"><span data-stu-id="ddb85-114">Stream</span></span>          | [<span data-ttu-id="ddb85-115">mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="ddb85-115">mailboxUsageDetail</span></span>](../resources/mailboxusagedetail.md) | <span data-ttu-id="ddb85-116">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="ddb85-116">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="ddb85-117">Получение количества почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="ddb85-117">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="ddb85-118">Поток</span><span class="sxs-lookup"><span data-stu-id="ddb85-118">Stream</span></span>          | [<span data-ttu-id="ddb85-119">mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="ddb85-119">mailboxUsageMailboxCounts</span></span>](../resources/mailboxusagemailboxcounts.md) | <span data-ttu-id="ddb85-120">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ddb85-120">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="ddb85-121">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="ddb85-121">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="ddb85-122">Получение количества почтовых ящиков по состоянию квоты</span><span class="sxs-lookup"><span data-stu-id="ddb85-122">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="ddb85-123">Поток</span><span class="sxs-lookup"><span data-stu-id="ddb85-123">Stream</span></span>          | [<span data-ttu-id="ddb85-124">mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="ddb85-124">mailboxUsageQuotaStatusMailboxCounts</span></span>](../resources/mailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="ddb85-125">Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.</span><span class="sxs-lookup"><span data-stu-id="ddb85-125">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="ddb85-126">Получение занятого объема хранилища</span><span class="sxs-lookup"><span data-stu-id="ddb85-126">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="ddb85-127">Stream</span><span class="sxs-lookup"><span data-stu-id="ddb85-127">Stream</span></span>          | [<span data-ttu-id="ddb85-128">mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="ddb85-128">mailboxUsageStorage</span></span>](../resources/mailboxusagestorage.md) | <span data-ttu-id="ddb85-129">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="ddb85-129">Get the amount of storage used in your organization.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailbox-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
