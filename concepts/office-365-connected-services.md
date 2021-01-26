---
title: Вызов служб Microsoft 365 в Visual Studio 2017 с помощью API Microsoft Graph
description: Вы можете сделать так, чтобы приложение вызывало API Microsoft Graph, с помощью Подключенных служб Visual Studio. В этой статье описано, как получить фотографию профиля вошедшего пользователя, передать ее в OneDrive и отправить письмо со ссылкой для общего доступа к фотографии.
localization_priority: Priority
ms.prod: reports
author: sarahwxy
ms.openlocfilehash: ce2d4bc8ccaa2ebae79c4d65ca243aeb9d489b54
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982287"
---
# <a name="call-microsoft-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a><span data-ttu-id="0c1f3-104">Вызов служб Microsoft 365 в Visual Studio 2017 с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0c1f3-104">Call Microsoft 365 services in Visual Studio 2017 with the Microsoft Graph API</span></span>

<span data-ttu-id="0c1f3-p102">Вы можете сделать так, чтобы приложение вызывало API Microsoft Graph, с помощью Подключенных служб Visual Studio. В этой статье описано, как получить фотографию профиля вошедшего пользователя, передать ее в OneDrive и отправить письмо со ссылкой для общего доступа к фотографии.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-p102">You can use the Connected Services in Visual Studio to configure your app to call the Microsoft Graph API. This article describes how to get a signed in user's profile photo, upload it to OneDrive, and send an email with a sharing link to the photo.</span></span>

## <a name="get-set-up"></a><span data-ttu-id="0c1f3-107">Настройка</span><span class="sxs-lookup"><span data-stu-id="0c1f3-107">Get set up</span></span>

<span data-ttu-id="0c1f3-108">Чтобы использовать Подключенные службы Office 365 с помощью Microsoft Graph, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="0c1f3-108">To use the Office 365 Connected Services with Microsoft Graph, you'll need to do the following:</span></span>

- <span data-ttu-id="0c1f3-p103">Скачайте [предварительную версию Visual Studio 2017](https://www.visualstudio.com/vs/preview/). Предварительную версию Visual Studio 2017 можно использовать параллельно с более ранней версией Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-p103">Download the [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/), if you haven't already. If you're using an earlier version of Visual Studio, you can use Visual Studio 2017 Preview side by side with your current version.</span></span>

- <span data-ttu-id="0c1f3-p104">Оформите подписку на Microsoft 365. Чтобы получить бесплатную пробную версию, зарегистрируйтесь в [Программе для разработчиков Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="0c1f3-p104">Get a Microsoft 365 subscription. To get a free trial, join the [Microsoft 365 Developer program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span>

## <a name="get-the-starter-project"></a><span data-ttu-id="0c1f3-113">Получение исходного проекта</span><span class="sxs-lookup"><span data-stu-id="0c1f3-113">Get the starter project</span></span>

<span data-ttu-id="0c1f3-p105">Скачайте [пример Подключенных служб ASP.NET Microsoft Graph](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip). Этот пример включает ссылки, которые необходимо проверить на подлинность в Microsoft Graph. Скачав исходный проект, распакуйте и откройте пример в предварительной версии Visual Studio 2017.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-p105">Download the [Microsoft Graph ASP.NET Connected Services Sample](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip). This sample includes the references that you need to authenticate against Microsoft Graph. After you download the starter project, unzip, and open the sample in Visual Studio 2017 Preview.</span></span>

## <a name="add-the-connected-service"></a><span data-ttu-id="0c1f3-117">Добавление подключенной службы</span><span class="sxs-lookup"><span data-stu-id="0c1f3-117">Add the Connected Service</span></span>

<span data-ttu-id="0c1f3-118">Теперь можно добавить службу Microsoft Graph в проект Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-118">You're now ready to add the Microsoft Graph service to your Visual Studio project.</span></span> 

1. <span data-ttu-id="0c1f3-119">Выберите в обозревателе решений **Подключенные службы**, чтобы открыть одноименную вкладку.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-119">In Solution Explorer, choose **Connected Services** to open the Connected Services tab.</span></span> 

2. <span data-ttu-id="0c1f3-120">Выберите поставщика **Доступ к службам Microsoft 365 с помощью Microsoft Graph**.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-120">Choose the **Access Microsoft 365 services with Microsoft Graph** provider.</span></span> <span data-ttu-id="0c1f3-121">Следуйте указаниям мастера.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-121">Follow the wizard.</span></span> <span data-ttu-id="0c1f3-122">Выберите следующие разрешения (позже их можно будет изменить):</span><span class="sxs-lookup"><span data-stu-id="0c1f3-122">Select the following permissions (you can change the permissions later):</span></span>

    - <span data-ttu-id="0c1f3-123">Для API **File** установите разрешения **Полный доступ к вашим файлам**.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-123">For the **File** APIs, set permissions to **Have full access to your files**.</span></span>
    - <span data-ttu-id="0c1f3-124">Для API **Mail** установите разрешения **Отправка почты от вашего имени**.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-124">For the **Mail** APIs, set permissions to **Send mail as you**.</span></span>
    - <span data-ttu-id="0c1f3-125">Для API **User** установите разрешения **Вход и чтение своего профиля**.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-125">For the **User** APIs, set permissions to **Sign you in and read your profile**.</span></span>

## <a name="call-the-microsoft-graph-api"></a><span data-ttu-id="0c1f3-126">Вызов API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0c1f3-126">Call the Microsoft Graph API</span></span>

<span data-ttu-id="0c1f3-p107">Настройки исходного приложения позволяют отправить простое письмо. Используя Microsoft Graph, вы можете сделать так, чтобы приложение отправляло письмо со ссылкой на фотографию из профиля вошедшего пользователя в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-p107">The starter sample is configured to send a simple email. You can use Microsoft Graph to update the sample to send an email with a link to the signed-in user's profile photo in OneDrive.</span></span>

1. <span data-ttu-id="0c1f3-129">Откройте файл Models\GraphService.cs, который содержит код для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-129">Go to 'Models\GraphService.cs', which hosts the code to call Microsoft Graph.</span></span>

2. <span data-ttu-id="0c1f3-p108">Найдите и **раскомментируйте** вызовы пакетов SDK в указанных ниже методах. Здесь показано, как вызвать Microsoft Graph, чтобы получить фотографию профиля, передать файл в OneDrive и получить ссылку для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-p108">Find and **Uncomment** calls to the SDK in the following methods. This shows how to call Microsoft Graph to get a profile photo, upload a file to OneDrive, and get a sharing link.</span></span>

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> <span data-ttu-id="0c1f3-132">**Совет.** Каждый комментарий начинается с "//Uncomment:"</span><span class="sxs-lookup"><span data-stu-id="0c1f3-132">**Tip:** Each comment starts with '//Uncomment:'</span></span>
 

## <a name="run-the-sample"></a><span data-ttu-id="0c1f3-133">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="0c1f3-133">Run the sample</span></span>
<span data-ttu-id="0c1f3-p109">Выполните сборку и запуск приложения. Выберите ссылку **Sign-in** (Войти) справа вверху, а затем **Get email address** (Получить адрес электронной почты) и **Send email** (Отправить письмо).</span><span class="sxs-lookup"><span data-stu-id="0c1f3-p109">Build and run the sample. Next, choose the **Sign-in** link on the top right, and then choose **Get email address** followed by **Send email**.</span></span>

<span data-ttu-id="0c1f3-136">В результате будет отправлено письмо со ссылкой на вашу фотографию профиля.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-136">This will send an email that includes a link to your profile photo.</span></span>

><span data-ttu-id="0c1f3-137">**Примечания.**</span><span class="sxs-lookup"><span data-stu-id="0c1f3-137">**Notes:**</span></span>

>- <span data-ttu-id="0c1f3-138">Если вы остановите и перезапустите приложение в Visual Studio, для его работы может потребоваться выйти из учетной записи.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-138">If you stop and rerun the sample from Visual Studio, you might need to explicitly sign out for the sample to work.</span></span>
>- <span data-ttu-id="0c1f3-139">Если вы получите сообщение о том, что не выполнена проверка пользователя, повторите шаг [Добавление подключенной службы](#add-the-connected-service).</span><span class="sxs-lookup"><span data-stu-id="0c1f3-139">If you get an exception that indicates that the User is not authenticated, you might need to repeat the [Add the Connected Service](#add-the-connected-service) step.</span></span>
    

## <a name="explore-the-code"></a><span data-ttu-id="0c1f3-140">Обзор кода</span><span class="sxs-lookup"><span data-stu-id="0c1f3-140">Explore the code</span></span>

<span data-ttu-id="0c1f3-p110">Теперь можно использовать Visual Studio 2017 для подключения к службам и их настройки. Исходное приложение само создает шаблоны и ссылки.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-p110">You can now use Visual Studio 2017 to connect to and configure your services. The starter sample creates the scaffolding and references for you.</span></span>  

<span data-ttu-id="0c1f3-143">Исходное приложение включает следующие файлы:</span><span class="sxs-lookup"><span data-stu-id="0c1f3-143">The starter sample includes the following files:</span></span>

- <span data-ttu-id="0c1f3-144">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) выполняет аутентификацию текущего пользователя и инициализирует кэш маркеров приложения.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-144">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) - Authenticates the current user and initializes the sample's token cache.</span></span>

- <span data-ttu-id="0c1f3-p111">Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) содержит сведения о маркере пользователя. Вы можете заменить его на собственный кэш маркеров. Дополнительные сведения см. в статье [Кэширование маркеров доступа в мультитенантном приложении](/azure/architecture/multitenant-identity/token-cache).</span><span class="sxs-lookup"><span data-stu-id="0c1f3-p111">Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - Stores the user's token information. You can replace this with your own custom token cache. For more information, see [Caching access tokens in a multitenant application](/azure/architecture/multitenant-identity/token-cache).</span></span>

- <span data-ttu-id="0c1f3-148">Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) реализует локальный интерфейс IAuthProvider и получает маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-148">Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) - Implements the local IAuthProvider interface, and gets an access token.</span></span> 

- <span data-ttu-id="0c1f3-149">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) инициализирует **GraphServiceClient** из [клиентской библиотеки Microsoft Graph .NET](https://github.com/microsoftgraph/msgraph-sdk-dotnet), которая используется для взаимодействия с Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-149">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) - Initializes the **GraphServiceClient** from the [Microsoft Graph .NET Client Library](https://github.com/microsoftgraph/msgraph-sdk-dotnet) that is used to interact with the Microsoft Graph.</span></span>

- <span data-ttu-id="0c1f3-150">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) содержит методы, использующие **GraphServiceClient** для создания и отправки вызовов в службу Microsoft Graph и обработки ответа.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-150">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) - Contains methods that use the **GraphServiceClient** to build and send calls to the Microsoft Graph service and to process the response.</span></span>

- <span data-ttu-id="0c1f3-151">Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) содержит пользовательский интерфейс приложения.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-151">Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) - Contains the UI for the sample.</span></span> 


## <a name="need-help"></a><span data-ttu-id="0c1f3-152">Нужна помощь?</span><span class="sxs-lookup"><span data-stu-id="0c1f3-152">Need help?</span></span>

<span data-ttu-id="0c1f3-p112">Если вам нужна помощь, задавайте вопросы на сайте [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Отметьте вашу запись тегом {microsoftgraph}.</span><span class="sxs-lookup"><span data-stu-id="0c1f3-p112">If you need help, post your questions on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Tag your post with {microsoftgraph}.</span></span>