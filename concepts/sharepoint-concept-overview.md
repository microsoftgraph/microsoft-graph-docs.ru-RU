---
title: Обзор API сайтов и контента SharePoint
description: SharePoint — это ваша мобильная интеллектуальная интрасеть. В SharePoint пользователи могут делиться и управлять контентом, знаниями и приложениями при работе в группах, искать необходимую информацию и вести совместную работу в рамках организации. С помощью REST API для SharePoint в Microsoft Graph вы можете интегрировать свои решения с сайтами и контентом SharePoint.
localization_priority: Priority
ms.prod: sharepoint
scenarios: getting-started
ms.openlocfilehash: 38d9b0973c1d3f1ee9c7fb0e58129d675d674955
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792879"
---
# <a name="sharepoint-sites-and-content-api-overview"></a><span data-ttu-id="34801-105">Обзор API сайтов и контента SharePoint</span><span class="sxs-lookup"><span data-stu-id="34801-105">SharePoint sites and content API overview</span></span>

<span data-ttu-id="34801-106">SharePoint — это ваша мобильная интеллектуальная интрасеть.</span><span class="sxs-lookup"><span data-stu-id="34801-106">SharePoint is your mobile, intelligent intranet.</span></span> <span data-ttu-id="34801-107">В SharePoint пользователи могут делиться и управлять контентом, знаниями и приложениями при работе в группах, искать необходимую информацию и вести совместную работу в рамках организации.</span><span class="sxs-lookup"><span data-stu-id="34801-107">With SharePoint, users can share and manage content, knowledge, and applications to empower teamwork, find information, and collaborate across an organization.</span></span> <span data-ttu-id="34801-108">С помощью REST API для SharePoint в Microsoft Graph вы можете интегрировать свои решения с сайтами и контентом SharePoint.</span><span class="sxs-lookup"><span data-stu-id="34801-108">You can use the SharePoint REST API in Microsoft Graph to integrate your solutions with SharePoint sites and content.</span></span>

## <a name="why-integrate-with-sharepoint-sites-and-content"></a><span data-ttu-id="34801-109">Зачем выполнять интеграцию с сайтами и контентом SharePoint?</span><span class="sxs-lookup"><span data-stu-id="34801-109">Why integrate with SharePoint sites and content?</span></span>

<span data-ttu-id="34801-110">Сайты SharePoint используются для связи и совместной работы в группах.</span><span class="sxs-lookup"><span data-stu-id="34801-110">SharePoint sites power team collaboration and communication.</span></span> <span data-ttu-id="34801-111">В основе групп Office 365, Microsoft Teams и порталов лежит SharePoint, поэтому с помощью Microsoft Graph вы можете получать доступ к данным независимо от того, где они хранятся.</span><span class="sxs-lookup"><span data-stu-id="34801-111">Office 365 groups, Microsoft Teams, and portals are all based on SharePoint, so you can use Microsoft Graph to access data no matter where it's kept.</span></span> <span data-ttu-id="34801-112">С помощью API SharePoint в Microsoft Graph вы можете получать доступ к указанным ниже ресурсам.</span><span class="sxs-lookup"><span data-stu-id="34801-112">Use the SharePoint API in Microsoft Graph to access:</span></span>

- <span data-ttu-id="34801-113">Сайты групп. На них хранится контент, над которым совместно работают пользователи со своими коллегами.</span><span class="sxs-lookup"><span data-stu-id="34801-113">Team sites that store the content that users collaborate on with their coworkers.</span></span>
- <span data-ttu-id="34801-114">Информационные сайты и порталы, на которых пользователи публикуют страницы с разнообразным контентом, чтобы поделиться им с другими пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="34801-114">Communication sites and portals where users publish rich content pages to share across the organization.</span></span>

### <a name="unleash-your-data-with-sharepoint-lists"></a><span data-ttu-id="34801-115">Раскройте все возможности своих данных с помощью списков SharePoint</span><span class="sxs-lookup"><span data-stu-id="34801-115">Unleash your data with SharePoint lists</span></span>

<span data-ttu-id="34801-116">[Списки][список] — это основные элементы для хранения данных в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="34801-116">[Lists][list] are the foundation for data storage in SharePoint.</span></span>
<span data-ttu-id="34801-117">[Вы можете создавать списки][создавать], чтобы хранить самые разные бизнес-данные: от простого списка контактных данных клиентов до пользовательского бизнес-приложения с интерфейсом PowerApps.</span><span class="sxs-lookup"><span data-stu-id="34801-117">[Create lists][create] to store a variety of business data, from a simple customer contact list to a custom business application, fronted with PowerApps.</span></span>
<span data-ttu-id="34801-118">Когда вы используете [столбцы][], чтобы определить свою схему, SharePoint может защитить целостность ваших данных, а также предоставить мощные функции индексирования, создания запросов и поиска.</span><span class="sxs-lookup"><span data-stu-id="34801-118">When you use [columns][] to define your schema, SharePoint can protect the integrity of your data as well as enable  rich indexing, querying, and search capabilities.</span></span>

### <a name="bring-the-power-of-lists-to-your-teams-files"></a><span data-ttu-id="34801-119">Применение функций списков к файлам группы</span><span class="sxs-lookup"><span data-stu-id="34801-119">Bring the power of lists to your team's files</span></span>

<span data-ttu-id="34801-120">SharePoint хранит файлы в [списках особого типа][], называемых библиотеками документов.</span><span class="sxs-lookup"><span data-stu-id="34801-120">SharePoint stores files in a special [list type][] called a document library.</span></span>
<span data-ttu-id="34801-121">С помощью [API OneDrive][] вы можете работать с библиотекой как с [диском][], а с помощью API SharePoint — как со [списком][].</span><span class="sxs-lookup"><span data-stu-id="34801-121">You can use the [OneDrive API][] to work with a library as a [drive][], or the SharePoint API to work with it as a [list][].</span></span>
<span data-ttu-id="34801-122">Как и при работе с обычным списком, с помощью настраиваемых столбцов вы можете расширить схему библиотеки документов для удовлетворения своих бизнес-потребностей.</span><span class="sxs-lookup"><span data-stu-id="34801-122">Just like a regular list, you can extend the schema of a Document Library to support your business needs with custom columns.</span></span>

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a><span data-ttu-id="34801-123">Наполнение приложения данными пользователей из интрасети SharePoint</span><span class="sxs-lookup"><span data-stu-id="34801-123">Light up your app with your users' SharePoint intranet data</span></span>

<span data-ttu-id="34801-124">С помощью Microsoft Graph вы можете обеспечить доступ к самым важным данным пользователей в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="34801-124">With Microsoft Graph, you can surface your users' most important data within your app.</span></span>
<span data-ttu-id="34801-125">Обновляйте данные, [отправляя запросы][] к списку, в котором хранятся данные ваших пользователей.</span><span class="sxs-lookup"><span data-stu-id="34801-125">Keep things fresh by [querying][] the list that stores your users' data.</span></span>
<span data-ttu-id="34801-126">[Создавайте][] собственные списки для приложения и предоставляйте пользователям доступ к данным в других интерфейсах SharePoint либо скрывайте данные.</span><span class="sxs-lookup"><span data-stu-id="34801-126">[Create][] your own lists for your app and let users access your data in other SharePoint experiences, or keep things hidden.</span></span>

### <a name="use-microsoft-graph-to-extend-sharepoint"></a><span data-ttu-id="34801-127">Расширение возможностей SharePoint c помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="34801-127">Use Microsoft Graph to extend SharePoint</span></span>

<span data-ttu-id="34801-128">В качестве платформы SharePoint обеспечивает несколько указанных ниже моделей расширения и интеграции.</span><span class="sxs-lookup"><span data-stu-id="34801-128">As a platform, SharePoint provides several models for extension and integration:</span></span>

- <span data-ttu-id="34801-129">[SharePoint Framework][] позволяет создавать веб-части с помощью клиентских технологий и средств с открытым кодом, которые можно разместить на страницах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="34801-129">The [SharePoint Framework][] provides a way to build web parts using client-side technologies and open source tooling that can be hosted on SharePoint pages.</span></span>
- <span data-ttu-id="34801-130">[Надстройки SharePoint][] — это автономные расширения, которые можно добавить на сайт SharePoint без необходимости выполнения пользовательского кода на сервере.</span><span class="sxs-lookup"><span data-stu-id="34801-130">[SharePoint Add-ins][] are self-contained extensions that can be added to a SharePoint site without the need for custom code to run on the server.</span></span>

<span data-ttu-id="34801-131">Если ваше приложение работает на странице SharePoint, вы можете без труда получать доступ к данным в Office 365 c помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="34801-131">When your app runs within a SharePoint page, you can easily use Microsoft Graph to access data across Office 365.</span></span>

<span data-ttu-id="34801-132">Подробные сведения об этих моделях см. на веб-страницах [центра разработки SharePoint][] и [документов по разработке в SharePoint][].</span><span class="sxs-lookup"><span data-stu-id="34801-132">To learn about these models in more detail, visit the [SharePoint Dev Center][] or the [SharePoint Developer Docs][].</span></span>

## <a name="api-reference"></a><span data-ttu-id="34801-133">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="34801-133">API reference</span></span>
<span data-ttu-id="34801-134">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="34801-134">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="34801-135">API SharePoint в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="34801-135">SharePoint API in Microsoft Graph v1.0</span></span>](/graph/api/resources/sharepoint?view=graph-rest-1.0)
- [<span data-ttu-id="34801-136">API SharePoint в бета-версии Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="34801-136">SharePoint API in Microsoft Graph beta</span></span>](/graph/api/resources/sharepoint?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="34801-137">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="34801-137">Next steps</span></span>

<span data-ttu-id="34801-138">Чтобы приступить к работе с SharePoint в Microsoft Graph, изучите дополнительные сведения о [работе с сайтами](/graph/api/resources/sharepoint?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="34801-138">Get started with SharePoint in Microsoft Graph by learning more about [working with sites](/graph/api/resources/sharepoint?view=graph-rest-1.0).</span></span>

[list]: /graph/api/resources/list?view=graph-rest-1.0
[столбцы]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[columns]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[тип списка]: /graph/api/resources/listinfo?view=graph-rest-1.0
[list type]: /graph/api/resources/listinfo?view=graph-rest-1.0
[создать]: /graph/api/list-create?view=graph-rest-1.0
[create]: /graph/api/list-create?view=graph-rest-1.0
[создание запросов]: /graph/api/listitem-get?view=graph-rest-1.0
[querying]: /graph/api/listitem-get?view=graph-rest-1.0
[диск]: /graph/api/resources/drive?view=graph-rest-1.0
[drive]: /graph/api/resources/drive?view=graph-rest-1.0
[API OneDrive]: /graph/api/resources/onedrive?view=graph-rest-1.0
[OneDrive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[SharePoint Framework]: https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview
[Надстройки SharePoint]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint Add-ins]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[Центр разработки SharePoint]: https://developer.microsoft.com/sharepoint
[SharePoint Dev Center]: https://developer.microsoft.com/sharepoint
[Документы по разработке в SharePoint]: https://aka.ms/spdev-docs
[SharePoint Developer Docs]: https://aka.ms/spdev-docs
[SharePoint]: /graph/api/resources/sharepoint?view=graph-rest-1.0
