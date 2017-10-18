# <a name="getting-started-building-microsoft-graph-apps"></a><span data-ttu-id="bd6d4-101">Начало создания приложений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bd6d4-101">Getting started building Microsoft Graph apps</span></span>

<span data-ttu-id="bd6d4-p101">Статьи, перечисленные в этом разделе, содержат подробные указания по созданию приложений для подключения к Microsoft Graph на различных языках и платформах разработки. Каждая статья начинается с простого начального проекта для соответствующей платформы и содержит указания по добавлению функций проверки подлинности пользователя и отправки в службу Microsoft Graph простого запроса на отправку электронного сообщения со своей учетной записи. Готовый проект идентичен [примеру Connect в репозитории Microsoft Graph](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) для соответствующей платформы.</span><span class="sxs-lookup"><span data-stu-id="bd6d4-p101">The articles in this section provide detailed guidance on how to build apps that connect to Microsoft Graph across a variety of languages and development platforms. Each article starts with a sample starter project for the appropriate platform, and walks you through adding functionality that authenticates the user and makes a sample request to have Microsoft Graph send an email from their account. The completed project is identical to the [Connect sample in the Microsoft Graph repo](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) for that platform.</span></span>

<span data-ttu-id="bd6d4-105">Выберите статью, посвященную выбранным вами поставщику проверки подлинности и платформе разработки, и приступайте к подключению к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bd6d4-105">Choose the article that covers the authentication provider and development platform of your choice, and get started connecting to Microsoft Graph.</span></span> <span data-ttu-id="bd6d4-106">Дополнительные сведения см. в статье [Чем отличается конечная точка версии 2.0?](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-compare)</span><span class="sxs-lookup"><span data-stu-id="bd6d4-106">For more information, see [What's different about the v2.0 endpoint?](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-compare)</span></span>

<span data-ttu-id="bd6d4-107">Вы можете выполнить действия, указанные в статье, посвященной вашей платформе разработки, либо воспользоваться [кратким руководством](https://developer.microsoft.com/graph/quick-start), чтобы быстро подготовить решение к работе.</span><span class="sxs-lookup"><span data-stu-id="bd6d4-107">You can follow the steps in the article that covers the development platform that you choose, or, to quickly get a working solution up and running, try out the [quick start](https://developer.microsoft.com/graph/quick-start) experience.</span></span>

<span data-ttu-id="bd6d4-p103">Готовые примеры Connect вы найдете в репозитории [Microsoft Graph ](https://github.com/microsoftgraph) на сайте GitHub. Ниже представлены примеры для разных поставщиков проверки подлинности и платформ, а также указано, что они используют для подключения к Microsoft Graph: REST или клиентскую библиотеку Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bd6d4-p103">To explore the finished Connect samples, see [Microsoft Graph](https://github.com/microsoftgraph) in GitHub. The following table lists the samples by authentication provider and platform, and notes whether they connect to Microsoft Graph using REST or a Microsoft Graph client library.</span></span>

<table>
  <tr>
    <th><span data-ttu-id="bd6d4-110">Платформа</span><span class="sxs-lookup"><span data-stu-id="bd6d4-110">Platform</span></span></th>
    <th><span data-ttu-id="bd6d4-111">Конечная точка Azure AD</span><span class="sxs-lookup"><span data-stu-id="bd6d4-111">Azure AD endpoint</span></span></th> 
    <th><span data-ttu-id="bd6d4-112">Конечная точка Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="bd6d4-112">Azure AD v2.0 endpoint</span></span></th>
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-113">Android</span><span class="sxs-lookup"><span data-stu-id="bd6d4-113">Android</span></span></td>
    <td><span data-ttu-id="bd6d4-114">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">Пример с использованием пакета SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-114">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK sample</a>
    </span></span></td> 
        <td><span data-ttu-id="bd6d4-115">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">Пример с использованием пакета SDK</a> ¶или <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-115">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-116">AngularJS</span><span class="sxs-lookup"><span data-stu-id="bd6d4-116">AngularJS</span></span></td>
    <td><span data-ttu-id="bd6d4-117">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-117">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td> 
        <td><span data-ttu-id="bd6d4-118">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">Пример с использованием пакета SDK</a> ¶или <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-118">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-119">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="bd6d4-119">ASP.NET</span></span></td>
    <td><span data-ttu-id="bd6d4-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="bd6d4-121">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">Пример с использованием пакета SDK</a> ¶или <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-121">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-122">iOS (Obj-C)</span><span class="sxs-lookup"><span data-stu-id="bd6d4-122">iOS (Obj-C)</span></span></td>
    <td><span data-ttu-id="bd6d4-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">Пример с использованием REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="bd6d4-124">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">Пример с использованием пакета SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-124">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-125">iOS (Swift)</span><span class="sxs-lookup"><span data-stu-id="bd6d4-125">iOS (Swift)</span></span></td>
    <td><span data-ttu-id="bd6d4-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">Пример с использованием REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="bd6d4-127">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">Пример с использованием пакета SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-127">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-128">NodeJS</span><span class="sxs-lookup"><span data-stu-id="bd6d4-128">NodeJS</span></span></td>
    <td><span data-ttu-id="bd6d4-129">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-129">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td>    
        <span data-ttu-id="bd6d4-130"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">Пример с использованием пакета SDK</a> или <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-130"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-131">PHP</span><span class="sxs-lookup"><span data-stu-id="bd6d4-131">PHP</span></span></td>
    <td><span data-ttu-id="bd6d4-132">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-132">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="bd6d4-133">
            <a href="https://github.com/microsoftgraph/php-connect-sample">Пример с использованием пакета SDK</a> ¶или <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-133">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-134">Python</span><span class="sxs-lookup"><span data-stu-id="bd6d4-134">Python</span></span></td>
    <td><span data-ttu-id="bd6d4-135">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">Пример с использованием REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-135">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td>
    </td> 
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-136">Ruby</span><span class="sxs-lookup"><span data-stu-id="bd6d4-136">Ruby</span></span></td>
    <td><span data-ttu-id="bd6d4-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="bd6d4-138">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">Пример с использованием REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-138">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-139">UWP</span><span class="sxs-lookup"><span data-stu-id="bd6d4-139">UWP</span></span></td>
    <td><span data-ttu-id="bd6d4-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="bd6d4-141">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">Пример с использованием пакета SDK</a> ¶или <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-141">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="bd6d4-142">Xamarin</span><span class="sxs-lookup"><span data-stu-id="bd6d4-142">Xamarin</span></span></td>
    <td>
    </td>     
    <td><span data-ttu-id="bd6d4-143">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">Пример с использованием пакета SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="bd6d4-143">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
</table>

## <a name="see-also"></a><span data-ttu-id="bd6d4-144">См. также</span><span class="sxs-lookup"><span data-stu-id="bd6d4-144">See also</span></span>

- <span data-ttu-id="bd6d4-145">Опробуйте примеры вызовов REST в [песочнице Graph](https://developer.microsoft.com/en-us/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="bd6d4-145">Try out sample REST calls in our [API Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer).</span></span>
- [<span data-ttu-id="bd6d4-146">Документация по конечной точке Azure AD</span><span class="sxs-lookup"><span data-stu-id="bd6d4-146">Azure AD endpoint documentation</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-developers-guide)
- [<span data-ttu-id="bd6d4-147">Документация по конечной точке Azure AD версии 2.0</span><span class="sxs-lookup"><span data-stu-id="bd6d4-147">Azure AD v2.0 endpoint documentation</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-appmodel-v2-overview)
