---
title: Использование Postman с API Microsoft Graph
description: Используйте коллекцию Microsoft Graph Postman, чтобы начать работу с API Microsoft Graph в считанные минуты.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: c7029a68314c0a093e0943bcdad46be27155ca25
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556217"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a><span data-ttu-id="64e6d-103">Использование Postman с API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="64e6d-103">Use Postman with the Microsoft Graph API</span></span>

<span data-ttu-id="64e6d-104">Вы можете использовать коллекцию Microsoft Graph Postman, чтобы начать работу с API Microsoft Graph в считанные минуты.</span><span class="sxs-lookup"><span data-stu-id="64e6d-104">You can use the Microsoft Graph Postman collection to get started with Microsoft Graph APIs in minutes.</span></span>

![Изображение Postman](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

<span data-ttu-id="64e6d-106">В этой статье рассказывается о том, как быстро приступить к работе с Postman и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="64e6d-106">This article explains how to get up and running with Postman and Microsoft Graph.</span></span> <span data-ttu-id="64e6d-107">Кроме того, вы можете просматривать API Microsoft Graph непосредственно в веб-браузере с помощью [песочницы Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="64e6d-107">You can also explore Microsoft Graph APIs directly in your web browser by using [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

## <a name="accessing-the-collection"></a><span data-ttu-id="64e6d-108">Доступ к коллекции</span><span class="sxs-lookup"><span data-stu-id="64e6d-108">Accessing the collection</span></span>
<span data-ttu-id="64e6d-109">Доступ к коллекции в Postman можно получить двумя способами: путем ее использования или путем добавления в нее.</span><span class="sxs-lookup"><span data-stu-id="64e6d-109">You can access the collection in Postman in two ways: by consuming it or by contributing to it.</span></span> <span data-ttu-id="64e6d-110">Вначале вам потребуется запустить [Postman](https://www.getpostman.com/) на компьютере.</span><span class="sxs-lookup"><span data-stu-id="64e6d-110">You will need to have [Postman](https://www.getpostman.com/) running on your computer first.</span></span>

### <a name="consume-the-collection"></a><span data-ttu-id="64e6d-111">Использование коллекции</span><span class="sxs-lookup"><span data-stu-id="64e6d-111">Consume the collection</span></span>
<span data-ttu-id="64e6d-112">Использование коллекции ⁠— самый простой способ начать работу с API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="64e6d-112">Consuming the collection is the easiest way to get started with Microsoft Graph APIs.</span></span> <span data-ttu-id="64e6d-113">Чтобы импортировать коллекции Postman:</span><span class="sxs-lookup"><span data-stu-id="64e6d-113">To import the Postman collections:</span></span>

1. <span data-ttu-id="64e6d-114">Скачайте [Postman](https://www.getpostman.com/) и зарегистрируйтесь для его использования.</span><span class="sxs-lookup"><span data-stu-id="64e6d-114">Download and register for [Postman](https://www.getpostman.com/).</span></span>
2. <span data-ttu-id="64e6d-115">Выберите **Файл | Импорт...**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-115">Choose **File | Import ...**.</span></span>
3. <span data-ttu-id="64e6d-116">Выберите **Импорт из ссылки**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-116">Select **Import From Link**.</span></span>
4. <span data-ttu-id="64e6d-117">Вставьте два указанных ниже URL-адреса и выберите **Импорт** после каждого из них.</span><span class="sxs-lookup"><span data-stu-id="64e6d-117">Paste the following two URLs and choose **Import** after each.</span></span>

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_environment.json

    ```

<span data-ttu-id="64e6d-118">В правой верхней части окна должна отобразиться **среда Microsoft Graph** в виде значка с изображением глаза.</span><span class="sxs-lookup"><span data-stu-id="64e6d-118">You should now see the **Microsoft Graph environment** in the top right environment drop down by the eye icon.</span></span> <span data-ttu-id="64e6d-119">Теперь необходимо [настроить среду](#using-the-collection).</span><span class="sxs-lookup"><span data-stu-id="64e6d-119">Now you need to  [set up your environment](#using-the-collection).</span></span>

## <a name="using-the-collection"></a><span data-ttu-id="64e6d-120">Использование коллекции</span><span class="sxs-lookup"><span data-stu-id="64e6d-120">Using the collection</span></span>
<span data-ttu-id="64e6d-121">После создания коллекции **Microsoft Graph** и **среды Microsoft Graph** в Postman выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="64e6d-121">After you have the **Microsoft Graph** collection and the **Microsoft Graph environment** in Postman, follow these steps.</span></span>

### <a name="set-up-application-api-calls"></a><span data-ttu-id="64e6d-122">Настройка вызовов API приложений</span><span class="sxs-lookup"><span data-stu-id="64e6d-122">Set up application API calls</span></span>

1. <span data-ttu-id="64e6d-123">В правом верхнем углу выберите **Без среды** из раскрывающегося списка.</span><span class="sxs-lookup"><span data-stu-id="64e6d-123">Choose the **No environment** drop down in top right corner.</span></span>
2. <span data-ttu-id="64e6d-124">Выберите **Среда Microsoft Graph**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-124">Select **Microsoft Graph environment**.</span></span>
3. <span data-ttu-id="64e6d-125">Щелкните значок с изображением **глаза** справа и затем выберите **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-125">Choose the **eye** icon to the right and then choose **Edit**.</span></span>
4. <span data-ttu-id="64e6d-126">Введите свое приложение Microsoft Identity в **текущих** (не **начальных** ) переменных: **ClientID** , **ClientSecret** и **TenantID**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-126">Enter your Microsoft Identity Application in the **current** (not **initial** ) variables: **ClientID** , **ClientSecret** and **TenantID**.</span></span> 
 <span data-ttu-id="64e6d-127">Дополнительные сведения о том, как создать приложение и получить согласие администратора только для приложений, см. в записи блога [Использование Postman для осуществления вызовов Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/).</span><span class="sxs-lookup"><span data-stu-id="64e6d-127">For more information about how to create an application and to admin consent the app-only flow, see the [Use Postman to make Microsoft Graph calls](https://developer.microsoft.com/ru-RU/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/) blog post.</span></span>

5. <span data-ttu-id="64e6d-128">Нажмите кнопку **Обновить**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-128">Select **Update**.</span></span> <span data-ttu-id="64e6d-129">Закройте диалоговое окно **Управление средами**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-129">Close the **Manage Environments** dialog box.</span></span> <span data-ttu-id="64e6d-130">В коллекции **MicrosoftGraph | Приложение** с левой стороны выберите **Получить маркер доступа только для приложений**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-130">In the **MicrosoftGraph | Application** collection on left side, choose **Get App-only Access Token**.</span></span> <span data-ttu-id="64e6d-131">Затем в правой части нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-131">Then choose **Send** on the right.</span></span>
6. <span data-ttu-id="64e6d-132">Разверните папку **Приложение | Пользователи** и выберите **Получить пользователей**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-132">Expand the **Application | Users** folder and choose **Get Users**.</span></span> <span data-ttu-id="64e6d-133">Затем нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-133">Then choose **Send**.</span></span>

<span data-ttu-id="64e6d-134">Теперь вы можете работать с коллекциями Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="64e6d-134">You are now up and running with the Microsoft Graph collections.</span></span>

><span data-ttu-id="64e6d-135">**Примечание.** Если вы хотите использовать другие API в коллекции, вам будет необходимо подтвердить разрешения, необходимые для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="64e6d-135">**Note:** If you want to run other APIs in the collection, you will need to consent the required permissions for your application.</span></span>

### <a name="set-up-on-behalf-of-api-calls"></a><span data-ttu-id="64e6d-136">Настройка вызовов API по сценарию "от имени"</span><span class="sxs-lookup"><span data-stu-id="64e6d-136">Set up on-behalf-of API calls</span></span>
<span data-ttu-id="64e6d-137">Самый простой способ настроить вызовы API по сценарию "от имени" ⁠— это указать **UserName** (Имя пользователя) и **UserPassword** (Пароль пользователя) в параметрах среды и использовать **От имени пользователя | Получить маркер доступа пользователя**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-137">The simplest way to set up on-behalf-of API calls is to provide a **UserName** and **UserPassword** in the environment settings and use the **On Behalf of a User | Get User Access Token**.</span></span> 

><span data-ttu-id="64e6d-138">**Важно!** Мы не рекомендуем использовать учетные записи пользователей рабочей среды, так как эта информация хранится непосредственно в Postman.</span><span class="sxs-lookup"><span data-stu-id="64e6d-138">**Important:** We don't recommend using production user accounts because this information is stored directly in Postman.</span></span> <span data-ttu-id="64e6d-139">Также не рекомендуем использовать этот способ для получения маркеров доступа в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="64e6d-139">We also don't  recommend using this approach to obtain access tokens in production.</span></span> <span data-ttu-id="64e6d-140">Используйте его только в целях тестирования.</span><span class="sxs-lookup"><span data-stu-id="64e6d-140">Use it only for testing purposes.</span></span>

<span data-ttu-id="64e6d-141">Если вы не хотите хранить имена пользователей и пароли в переменных среды, которые синхронизируются с вашей облачной учетной записью Postman, можно использовать возможность **Получить новый маркер доступа** , чтобы получить маркер, не выходя из Postman.</span><span class="sxs-lookup"><span data-stu-id="64e6d-141">If you don't want to store user names and passwords in environment variables that sync to your Postman cloud account, you can use the  **Get New Access Token** capability to get a token without leaving Postman.</span></span>

1. <span data-ttu-id="64e6d-142">Выберите **От имени пользователя | Получить маркер доступа с помощью Postman**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-142">Select **On behalf of a User | Get Access Token using Postman**.</span></span>
2. <span data-ttu-id="64e6d-143">Откройте вкладку **Авторизация**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-143">Choose the **Authorization** tab.</span></span>
3. <span data-ttu-id="64e6d-144">Нажмите кнопку **Получить новый маркер доступа**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-144">Choose the **get access token** button.</span></span>
4. <span data-ttu-id="64e6d-145">Заполните приведенные ниже поля реальными значениями для клиента и приложения.</span><span class="sxs-lookup"><span data-stu-id="64e6d-145">Fill out the following boxes with your real tenant and application values.</span></span> <span data-ttu-id="64e6d-146">Обратите внимание на то, что здесь вы не можете использовать переменные среды: необходимо использовать фактические значения.</span><span class="sxs-lookup"><span data-stu-id="64e6d-146">Note that you cannot use the environment variables here; you have to use the actual values.</span></span> <span data-ttu-id="64e6d-147">Их можно найти, выбрав **EndPoints** (Конечные точки) в колонке приложения на portal.azure.com.</span><span class="sxs-lookup"><span data-stu-id="64e6d-147">You can find them by selecting **EndPoints** in the application blade in portal.azure.com.</span></span>

    - <span data-ttu-id="64e6d-148">URL-адрес обратного вызова: https://app.getpostman.com/oauth2/callback</span><span class="sxs-lookup"><span data-stu-id="64e6d-148">Callback URL: https://app.getpostman.com/oauth2/callback</span></span>
    - <span data-ttu-id="64e6d-149">URL-адрес проверки подлинности: https://login.microsoftonline.com/**TENANTID** /oauth2/v2.0/authorize</span><span class="sxs-lookup"><span data-stu-id="64e6d-149">Auth URL: https://login.microsoftonline.com/**TENANTID** /oauth2/v2.0/authorize</span></span>
    - <span data-ttu-id="64e6d-150">URL-адрес маркера доступа: https://login.microsoftonline.com/**TENANTID** /oauth2/v2.0/token</span><span class="sxs-lookup"><span data-stu-id="64e6d-150">Access Token URL: https://login.microsoftonline.com/**TENANTID** /oauth2/v2.0/token</span></span>
    - <span data-ttu-id="64e6d-151">Идентификатор клиента: **CLIENTID**</span><span class="sxs-lookup"><span data-stu-id="64e6d-151">Client ID: **CLIENTID**</span></span>
    - <span data-ttu-id="64e6d-152">Секрет клиента: **CLIENTSECRET**</span><span class="sxs-lookup"><span data-stu-id="64e6d-152">Client Secret: **CLIENTSECRET**</span></span>
    - <span data-ttu-id="64e6d-153">Область: https://graph.microsoft.com/.default</span><span class="sxs-lookup"><span data-stu-id="64e6d-153">Scope: https://graph.microsoft.com/.default</span></span>
    - <span data-ttu-id="64e6d-154">Состояние: **RANDOMSTRING**</span><span class="sxs-lookup"><span data-stu-id="64e6d-154">State: **RANDOMSTRING**</span></span>
 
5. <span data-ttu-id="64e6d-155">Нажмите **Запросить маркер**.</span><span class="sxs-lookup"><span data-stu-id="64e6d-155">Choose **Request Token**.</span></span> <span data-ttu-id="64e6d-156">Вы увидите запрос пользовательского интерфейса на вход в систему и одобрение разрешений.</span><span class="sxs-lookup"><span data-stu-id="64e6d-156">You should see a UI prompt to sign in and consent permissions.</span></span>
6. <span data-ttu-id="64e6d-157">Скопируйте маркер доступа, откройте ваши переменные среды и вставьте его в поле **UserAccessToken** (Маркер доступа пользователя).</span><span class="sxs-lookup"><span data-stu-id="64e6d-157">Copy the access token, open your environment variables, and paste it into the **UserAccessToken** field.</span></span>

<span data-ttu-id="64e6d-158">Теперь все ваши запросы будут рабочими.</span><span class="sxs-lookup"><span data-stu-id="64e6d-158">Now all your requests will work.</span></span>


### <a name="contribute-to-the-collection"></a><span data-ttu-id="64e6d-159">Добавление в коллекцию</span><span class="sxs-lookup"><span data-stu-id="64e6d-159">Contribute to the collection</span></span>
<span data-ttu-id="64e6d-160">Если вы хотите добавить собственные запросы, вам потребуется создать вилку репозитория GitHub [коллекций Postman Microsoft Graph](https://github.com/microsoftgraph/microsoftgraph-postman-collections).</span><span class="sxs-lookup"><span data-stu-id="64e6d-160">If you want to contribute your own requests, you will need to fork the [Microsoft Graph Postman collections](https://github.com/microsoftgraph/microsoftgraph-postman-collections) github repo.</span></span> 

<span data-ttu-id="64e6d-161">Дополнительные сведения о том, как это сделать, см. в следующем видео.</span><span class="sxs-lookup"><span data-stu-id="64e6d-161">For details about how to do this, watch the following video.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]
