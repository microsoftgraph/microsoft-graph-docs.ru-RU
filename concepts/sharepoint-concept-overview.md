# <a name="sharepoint-sites-and-content-api-overview"></a><span data-ttu-id="6164c-101">Обзор API сайтов и контента SharePoint</span><span class="sxs-lookup"><span data-stu-id="6164c-101">SharePoint sites and content API overview</span></span>

<span data-ttu-id="6164c-102">SharePoint — это ваша мобильная интеллектуальная интрасеть.</span><span class="sxs-lookup"><span data-stu-id="6164c-102">SharePoint is your mobile, intelligent intranet.</span></span> <span data-ttu-id="6164c-103">В SharePoint пользователи могут делиться и управлять контентом, знаниями и приложениями при работе в группах, искать необходимую информацию и вести совместную работу в рамках организации.</span><span class="sxs-lookup"><span data-stu-id="6164c-103">With SharePoint, users can share and manage content, knowledge, and applications to empower teamwork, find information, and collaborate across an organization.</span></span> <span data-ttu-id="6164c-104">С помощью REST API для SharePoint в Microsoft Graph вы можете интегрировать свои решения с сайтами и контентом SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6164c-104">You can use the SharePoint REST API in Microsoft Graph to integrate your solutions with SharePoint sites and content.</span></span>

## <a name="why-integrate-with-sharepoint-sites-and-content"></a><span data-ttu-id="6164c-105">Зачем выполнять интеграцию с сайтами и контентом SharePoint?</span><span class="sxs-lookup"><span data-stu-id="6164c-105">Why integrate with SharePoint sites and content?</span></span>

<span data-ttu-id="6164c-106">Сайты SharePoint используются для связи и совместной работы в группах.</span><span class="sxs-lookup"><span data-stu-id="6164c-106">SharePoint sites power team collaboration and communication.</span></span> <span data-ttu-id="6164c-107">В основе групп Office 365, Microsoft Teams и порталов лежит SharePoint, поэтому с помощью Microsoft Graph вы можете получать доступ к данным независимо от того, где они хранятся.</span><span class="sxs-lookup"><span data-stu-id="6164c-107">Office 365 groups, Microsoft Teams, and portals are all based on SharePoint, so you can use Microsoft Graph to access data no matter where it's kept.</span></span> <span data-ttu-id="6164c-108">С помощью API SharePoint в Microsoft Graph вы можете получать доступ к указанным ниже ресурсам.</span><span class="sxs-lookup"><span data-stu-id="6164c-108">Use the SharePoint API in Microsoft Graph to access:</span></span>

- <span data-ttu-id="6164c-109">Сайты групп. На них хранится контент, над которым совместно работают пользователи со своими коллегами.</span><span class="sxs-lookup"><span data-stu-id="6164c-109">Team sites that store the content that users collaborate on with their coworkers.</span></span>
- <span data-ttu-id="6164c-110">Информационные сайты и порталы, на которых пользователи публикуют страницы с разнообразным контентом, чтобы поделиться им с другими пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="6164c-110">Communication sites and portals where users publish rich content pages to share across the organization.</span></span>

### <a name="unleash-your-data-with-sharepoint-lists"></a><span data-ttu-id="6164c-111">Раскройте все возможности своих данных с помощью списков SharePoint</span><span class="sxs-lookup"><span data-stu-id="6164c-111">Unleash your data with SharePoint lists</span></span>

<span data-ttu-id="6164c-112">[Списки][список] — это основные элементы для хранения данных в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6164c-112">[Lists][list] are the foundation for data storage in SharePoint.</span></span>
<span data-ttu-id="6164c-113">[Вы можете создавать списки][создавать], чтобы хранить самые разные бизнес-данные: от простого списка контактных данных клиентов до пользовательского бизнес-приложения с интерфейсом PowerApps.</span><span class="sxs-lookup"><span data-stu-id="6164c-113">[Create lists][create] to store a variety of business data, from a simple customer contact list to a custom business application, fronted with PowerApps.</span></span>
<span data-ttu-id="6164c-114">Когда вы используете [столбцы][], чтобы определить свою схему, SharePoint может защитить целостность ваших данных, а также предоставить мощные функции индексирования, создания запросов и поиска.</span><span class="sxs-lookup"><span data-stu-id="6164c-114">When you use [columns][] to define your schema, SharePoint can protect the integrity of your data as well as enable  rich indexing, querying, and search capabilities.</span></span>

### <a name="bring-the-power-of-lists-to-your-teams-files"></a><span data-ttu-id="6164c-115">Применение функций списков к файлам группы</span><span class="sxs-lookup"><span data-stu-id="6164c-115">Bring the power of lists to your team's files</span></span>

<span data-ttu-id="6164c-116">SharePoint хранит файлы в [списках особого типа][], называемых библиотеками документов.</span><span class="sxs-lookup"><span data-stu-id="6164c-116">SharePoint stores files in a special [list type][] called a document library.</span></span>
<span data-ttu-id="6164c-117">С помощью [API OneDrive][] вы можете работать с библиотекой как с [диском][], а с помощью API SharePoint — как со [списком][].</span><span class="sxs-lookup"><span data-stu-id="6164c-117">You can use the [OneDrive API][] to work with a library as a [drive][], or the SharePoint API to work with it as a [list][].</span></span>
<span data-ttu-id="6164c-118">Как и при работе с обычным списком, с помощью настраиваемых столбцов вы можете расширить схему библиотеки документов для удовлетворения своих бизнес-потребностей.</span><span class="sxs-lookup"><span data-stu-id="6164c-118">Just like a regular list, you can extend the schema of a Document Library to support your business needs with custom columns.</span></span>

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a><span data-ttu-id="6164c-119">Наполнение приложения данными пользователей из интрасети SharePoint</span><span class="sxs-lookup"><span data-stu-id="6164c-119">Light up your app with your users' SharePoint intranet data</span></span>

<span data-ttu-id="6164c-120">С помощью Microsoft Graph вы можете обеспечить доступ к самым важным данным пользователей в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="6164c-120">With Microsoft Graph, you can surface your users' most important data within your app.</span></span>
<span data-ttu-id="6164c-121">Обновляйте данные, [отправляя запросы][] к списку, в котором хранятся данные ваших пользователей.</span><span class="sxs-lookup"><span data-stu-id="6164c-121">Keep things fresh by [querying][] the list that stores your users' data.</span></span>
<span data-ttu-id="6164c-122">[Создавайте][] собственные списки для приложения и предоставляйте пользователям доступ к данным в других интерфейсах SharePoint либо скрывайте данные.</span><span class="sxs-lookup"><span data-stu-id="6164c-122">[Create][] your own lists for your app and let users access your data in other SharePoint experiences, or keep things hidden.</span></span>

### <a name="use-microsoft-graph-to-extend-sharepoint"></a><span data-ttu-id="6164c-123">Расширение возможностей SharePoint c помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6164c-123">Use Microsoft Graph to extend SharePoint</span></span>

<span data-ttu-id="6164c-124">В качестве платформы SharePoint обеспечивает несколько указанных ниже моделей расширения и интеграции.</span><span class="sxs-lookup"><span data-stu-id="6164c-124">As a platform, SharePoint provides several models for extension and integration:</span></span>

- <span data-ttu-id="6164c-125">[SharePoint Framework][] позволяет создавать веб-части с помощью клиентских технологий и средств с открытым кодом, которые можно разместить на страницах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6164c-125">The [SharePoint Framework][] provides a way to build web parts using client-side technologies and open source tooling that can be hosted on SharePoint pages.</span></span>
- <span data-ttu-id="6164c-126">[Надстройки SharePoint][] — это автономные расширения, которые можно добавить на сайт SharePoint без необходимости выполнения пользовательского кода на сервере.</span><span class="sxs-lookup"><span data-stu-id="6164c-126">[SharePoint Add-ins][] are self-contained extensions that can be added to a SharePoint site without the need for custom code to run on the server.</span></span>

<span data-ttu-id="6164c-127">Если ваше приложение работает на странице SharePoint, вы можете без труда получать доступ к данным в Office 365 c помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6164c-127">When your app runs within a SharePoint page, you can easily use Microsoft Graph to access data across Office 365.</span></span>

<span data-ttu-id="6164c-128">Подробные сведения об этих моделях см. на веб-страницах [центра разработки SharePoint][] и [документов по разработке в SharePoint][].</span><span class="sxs-lookup"><span data-stu-id="6164c-128">To learn about these models in more detail, visit the [SharePoint Dev Center][] or the [SharePoint Developer Docs][].</span></span>

## <a name="next-steps"></a><span data-ttu-id="6164c-129">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="6164c-129">Next steps</span></span>

<span data-ttu-id="6164c-130">Чтобы приступить к работе с SharePoint в Microsoft Graph, изучите дополнительные сведения о [работе с сайтами][SharePoint].</span><span class="sxs-lookup"><span data-stu-id="6164c-130">Get started with SharePoint in Microsoft Graph by learning more about [working with sites][SharePoint].</span></span>

[списки]: ../api-reference/v1.0/resources/list.md
[list]: ../api-reference/v1.0/resources/list.md
[столбцы]: ../api-reference/v1.0/resources/columndefinition.md
[columns]: ../api-reference/v1.0/resources/columndefinition.md
[тип списка]: ../api-reference/v1.0/resources/listinfo.md
[List Type]: ../api-reference/v1.0/resources/listinfo.md
[создать]: ../api-reference/v1.0/api/list_create.md
[Create]: ../api-reference/v1.0/api/list_create.md.
[создание запросов]: ../api-reference/v1.0/api/listitem_get.md
[querying]: ../api-reference/v1.0/api/listitem_get.md
[диск]: ../api-reference/v1.0/resources/drive.md
[drive]: ../api-reference/v1.0/resources/drive.md
<span data-ttu-id="6164c-137">
  [API OneDrive]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive</span><span class="sxs-lookup"><span data-stu-id="6164c-137">[onedrive api]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive</span></span>
[SharePoint Framework]: https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview
[Надстройки SharePoint]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint Add-ins]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[Центр разработки SharePoint]: https://developer.microsoft.com/sharepoint
[SharePoint Dev Center]: https://developer.microsoft.com/sharepoint
[Документы по разработке в SharePoint]: http://aka.ms/spdev-docs
[SharePoint Developer Docs]: http://aka.ms/spdev-docs
[SharePoint]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/sharepoint
