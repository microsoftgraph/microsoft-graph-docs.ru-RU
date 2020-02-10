---
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.topic: include
ms.openlocfilehash: dc5323fff895802f4af0bfa44059d35f8adfa243
ms.sourcegitcommit: 3d22631d6a8c235f7b9ec0575f60c3fb557a1368
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/07/2020
ms.locfileid: "41839976"
---
<!-- markdownlint-disable MD041-->

<span data-ttu-id="69a49-101">API Microsoft Graph поддерживает доступ к данным в _основных_ и [общих почтовых ящиках](https://support.office.com/article/open-and-use-a-shared-mailbox-in-outlook-d94a8e9e-21f1-4240-808b-de9c9c088afd) пользователей.</span><span class="sxs-lookup"><span data-stu-id="69a49-101">The Microsoft Graph API supports accessing data in users' _primary_ mailboxes and in [shared mailboxes](https://support.office.com/article/open-and-use-a-shared-mailbox-in-outlook-d94a8e9e-21f1-4240-808b-de9c9c088afd).</span></span> <span data-ttu-id="69a49-102">Это могут быть календарь, почта или личные контакты в почтовом ящике, хранящиеся в облаке на сервере Exchange Online (составной части Office 365) или на локальном сервере Exchange в [гибридном развертывании](/graph/hybrid-rest-support).</span><span class="sxs-lookup"><span data-stu-id="69a49-102">The data can be calendar, mail, or personal contacts stored in a mailbox in the cloud on Exchange Online as part of Office 365, or on Exchange on-premises in a [hybrid deployment](/graph/hybrid-rest-support).</span></span>

<span data-ttu-id="69a49-103">API _не_ поддерживает доступ к почтовым ящикам архива на месте ни на сервере [Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-archiving-service-description/archive-features#archive-mailbox), ни [на сервере Exchange Server](https://docs.microsoft.com/Exchange/policy-and-compliance/in-place-archiving/in-place-archiving?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="69a49-103">The API does _not_ support accessing in-place archive mailboxes, not [on Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-archiving-service-description/archive-features#archive-mailbox) nor [on Exchange Server](https://docs.microsoft.com/Exchange/policy-and-compliance/in-place-archiving/in-place-archiving?view=exchserver-2019).</span></span>