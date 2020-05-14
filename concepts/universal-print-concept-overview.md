---
title: Обзор API облачной среды универсальной печати
description: Универсальная печать — это современное решение печати, которое можно использовать в организациях для управления инфраструктурой печати через облачные службы от Майкрософт.
author: braedenp-msft
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: d3df3a36ac9994b3ce4560b995a52288dd197e34
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44215656"
---
# <a name="universal-print-cloud-printing-api-overview"></a><span data-ttu-id="1c06d-103">Обзор API облачной среды универсальной печати</span><span class="sxs-lookup"><span data-stu-id="1c06d-103">Universal Print cloud printing API overview</span></span>

<span data-ttu-id="1c06d-104">Универсальная печать — это современное решение печати, которое можно использовать в организациях для управления инфраструктурой печати через облачные службы от Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1c06d-104">Universal Print is a modern print solution that organizations can use to manage their print infrastructure through cloud services from Microsoft.</span></span>

![Снимок экрана с изображением главной страницы универсальной печати на портале Azure](images/universal-print-portal-homepage.png)

## <a name="why-use-universal-print"></a><span data-ttu-id="1c06d-106">Зачем нужна универсальная печать?</span><span class="sxs-lookup"><span data-stu-id="1c06d-106">Why use Universal Print?</span></span>

<span data-ttu-id="1c06d-107">Универсальная печать — это функции печати Windows Server, перенесенные в облако Microsoft 365, благодаря которым организации теперь могут обойтись без локальных серверов печати и не устанавливать драйверы печати на устройствах.</span><span class="sxs-lookup"><span data-stu-id="1c06d-107">Universal Print moves key Windows Server print functionality to the Microsoft 365 cloud, so organizations no longer need on-premises print servers and do not need to install printer drivers on devices.</span></span> <span data-ttu-id="1c06d-108">Кроме того, в рамках универсальной печати предусмотрены дополнительные функции, например, группы безопасности для доступа к принтеру, обнаружение принтеров на основе расположения и расширенными возможностями для администраторов.</span><span class="sxs-lookup"><span data-stu-id="1c06d-108">In addition, Universal Print adds key functionality like security groups for printer access, location-based printer discovery, and a rich administrator experience.</span></span>

<span data-ttu-id="1c06d-109">По мере внедрения универсальной печати в организациях организации и независимые поставщики программного обеспечения могут использовать API универсальной печати в Microsoft Graph, чтобы создавать и расширять приложения для поддержки новых сценариев.</span><span class="sxs-lookup"><span data-stu-id="1c06d-109">As organizations adopt Universal Print, organizations and independent software vendors (ISVs) can use the Universal Print API in Microsoft Graph to build and extend applications to support new scenarios.</span></span>

### <a name="print-documents-from-web-and-mobile-applications"></a><span data-ttu-id="1c06d-110">Печать документов из веб-приложений и мобильных приложений</span><span class="sxs-lookup"><span data-stu-id="1c06d-110">Print documents from web and mobile applications</span></span>

<span data-ttu-id="1c06d-111">Благодаря перемещению инфраструктуры печати в облако печатать документы можно непосредственно из веб-приложений и мобильных приложений.</span><span class="sxs-lookup"><span data-stu-id="1c06d-111">Moving print infrastructure to the cloud enables printing documents directly from web and mobile applications.</span></span>

<span data-ttu-id="1c06d-112">Чтобы приступить к работе с API универсальной печати, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="1c06d-112">To get started with the Universal Print API:</span></span>

1. <span data-ttu-id="1c06d-113">[Создайте задание печати](/graph/api/printer-post-jobs?view=graph-rest-beta) и сохраните идентификатор полученного документа.</span><span class="sxs-lookup"><span data-stu-id="1c06d-113">[Create a print job](/graph/api/printer-post-jobs?view=graph-rest-beta) and store the resulting document ID.</span></span>
2. <span data-ttu-id="1c06d-114">[Отправьте данные документа](/graph/api/printdocument-uploaddata?view=graph-rest-beta) в документ.</span><span class="sxs-lookup"><span data-stu-id="1c06d-114">[Upload document data](/graph/api/printdocument-uploaddata?view=graph-rest-beta) to the document.</span></span>
3. <span data-ttu-id="1c06d-115">[Запустите задание печати](/graph/api/printjob-startprintjob?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="1c06d-115">[Start the print job](/graph/api/printjob-startprintjob?view=graph-rest-beta).</span></span>

### <a name="manage-printers"></a><span data-ttu-id="1c06d-116">Управление принтерами</span><span class="sxs-lookup"><span data-stu-id="1c06d-116">Manage printers</span></span>

<span data-ttu-id="1c06d-117">Отследить принтеры организации, настройки принтеров и их использование — непростая задача.</span><span class="sxs-lookup"><span data-stu-id="1c06d-117">Keeping track of an organization's printers, printer configurations, and printer usage is a complex task.</span></span> <span data-ttu-id="1c06d-118">Благодаря API универсальной печати можно интегрировать эти три направления.</span><span class="sxs-lookup"><span data-stu-id="1c06d-118">The Universal Print API enables integration in all three areas.</span></span>

* <span data-ttu-id="1c06d-119">**Отслеживать состояние принтеров, их настройки и доступность**можно через [Список принтеров](/graph/api/print-list-printers?view=graph-rest-beta) и [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="1c06d-119">**Keep an eye on printer status, configurations, and availability** by using [List printers](/graph/api/print-list-printers?view=graph-rest-beta) and [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta).</span></span>

* <span data-ttu-id="1c06d-120">**Узнать, кто из пользователей использует принтеры и сколько страниц они печатают** можно через отчетные API:</span><span class="sxs-lookup"><span data-stu-id="1c06d-120">**See who's using your printers and how much they're printing** by using the reporting APIs:</span></span>
  * [<span data-ttu-id="1c06d-121">Список dailyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="1c06d-121">List dailyPrintUsageSummariesByUser</span></span>](/graph/api/reportroot-list-dailyprintusagesummariesbyuser?view=graph-rest-beta)
  * [<span data-ttu-id="1c06d-122">Список monthlyPrintUsageSummariesByUser</span><span class="sxs-lookup"><span data-stu-id="1c06d-122">List monthlyPrintUsageSummariesByUser</span></span>](/graph/api/reportroot-list-monthlyprintusagesummariesbyuser?view=graph-rest-beta)
  * [<span data-ttu-id="1c06d-123">Список dailyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="1c06d-123">List dailyPrintUsageSummariesByPrinter</span></span>](/graph/api/reportroot-list-dailyprintusagesummariesbyprinter?view=graph-rest-beta)
  * [<span data-ttu-id="1c06d-124">Список monthlyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="1c06d-124">List monthlyPrintUsageSummariesByPrinter</span></span>](/graph/api/reportroot-list-monthlyprintusagesummariesbyprinter?view=graph-rest-beta)

* <span data-ttu-id="1c06d-125">**Настройка разрешений для пользователей** через изменения в членстве пользователей и групп касательно принтеров:</span><span class="sxs-lookup"><span data-stu-id="1c06d-125">**Configure user permissions** by modifying user and group membership on printers:</span></span>
  * [<span data-ttu-id="1c06d-126">Список allowedUsers</span><span class="sxs-lookup"><span data-stu-id="1c06d-126">List allowedUsers</span></span>](/graph/api/printer-list-allowedusers?view=graph-rest-beta)
  * [<span data-ttu-id="1c06d-127">Добавление allowedUser</span><span class="sxs-lookup"><span data-stu-id="1c06d-127">Add allowedUser</span></span>](/graph/api/printer-post-allowedusers?view=graph-rest-beta)
  * [<span data-ttu-id="1c06d-128">Удаление allowedUser</span><span class="sxs-lookup"><span data-stu-id="1c06d-128">Remove allowedUser</span></span>](/graph/api/printer-delete-alloweduser?view=graph-rest-beta)
  * [<span data-ttu-id="1c06d-129">Список allowedGroups</span><span class="sxs-lookup"><span data-stu-id="1c06d-129">List allowedGroups</span></span>](/graph/api/printer-list-allowedgroups?view=graph-rest-beta)
  * [<span data-ttu-id="1c06d-130">Добавление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="1c06d-130">Add allowedGroup</span></span>](/graph/api/printer-post-allowedgroups?view=graph-rest-beta)
  * [<span data-ttu-id="1c06d-131">Удаление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="1c06d-131">Remove allowedGroup</span></span>](/graph/api/printer-delete-allowedgroup?view=graph-rest-beta)

### <a name="seamlessly-replace-or-update-printer-hardware"></a><span data-ttu-id="1c06d-132">Комфорт при замене и обновлении оборудования для печати</span><span class="sxs-lookup"><span data-stu-id="1c06d-132">Seamlessly replace or update printer hardware</span></span>

<span data-ttu-id="1c06d-133">Принтеры не видны пользователям до момента, когда они получают к ним [доступ](/graph/api/print-post-shares?view=graph-rest-beta). Это позволяет администраторам детально контролировать доступность определенного оборудования для печати в определенный момент времени.</span><span class="sxs-lookup"><span data-stu-id="1c06d-133">Printers are not visible to users until they are [shared](/graph/api/print-post-shares?view=graph-rest-beta), providing administrators fine-grained control over which printer hardware is available at a given time.</span></span>

<span data-ttu-id="1c06d-134">При общем доступе к принтеру создается ресурс [printerShare](/graph/api/resources/printershare?view=graph-rest-beta), который в любой момент можно обновить для перевода на другой принтер, что упрощает замену неисправного оборудования для печати и отправку принтеров в текущий ремонт.</span><span class="sxs-lookup"><span data-stu-id="1c06d-134">Sharing a printer creates a [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) resource that can be updated at any time to point to a different printer, making it easy to replace broken printer hardware or take printers offline for maintenance.</span></span>

<span data-ttu-id="1c06d-135">Чтобы применить эту возможность в своем приложении, перейдите в [Обновление printerShare](/graph/api/printershare-update?view=graph-rest-beta) и обновите ссылку `printer` на printerShare.</span><span class="sxs-lookup"><span data-stu-id="1c06d-135">To use this in your application, use [Update printerShare](/graph/api/printershare-update?view=graph-rest-beta) to update the printerShare's `printer` reference.</span></span>

## <a name="api-reference"></a><span data-ttu-id="1c06d-136">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="1c06d-136">API reference</span></span>
<span data-ttu-id="1c06d-137">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="1c06d-137">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="1c06d-138">API универсальной печати в бета-версии Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1c06d-138">Universal Print API in Microsoft Graph beta</span></span>](/graph/api/resources/print?view=graph-rest-beta)

## <a name="see-also"></a><span data-ttu-id="1c06d-139">См. также</span><span class="sxs-lookup"><span data-stu-id="1c06d-139">See also</span></span>

- [<span data-ttu-id="1c06d-140">Что такое универсальная печать</span><span class="sxs-lookup"><span data-stu-id="1c06d-140">What is Universal Print</span></span>](https://docs.microsoft.com/universal-print/fundamentals/universal-print-whatis)
- <span data-ttu-id="1c06d-141">Мы будем рады узнать ваше мнение об API универсальной печати через [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)!</span><span class="sxs-lookup"><span data-stu-id="1c06d-141">We'd love to hear your feedback about the Universal Print APIs over at [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)!</span></span>
