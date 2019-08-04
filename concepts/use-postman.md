---
title: Использование Postman с API Microsoft Graph
description: Используйте коллекцию Microsoft Graph Postman, чтобы начать работу с API Microsoft Graph в считанные минуты.
author: ''
localization_priority: Priority
ms.openlocfilehash: 2140dec07328b75f7b1729cd3e7cf7c86e65f738
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038187"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a><span data-ttu-id="71da7-103">Использование Postman с API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="71da7-103">Use the Microsoft Graph API</span></span>

<span data-ttu-id="71da7-104">Вы можете использовать коллекцию Microsoft Graph Postman, чтобы начать работу с API Microsoft Graph в считанные минуты.</span><span class="sxs-lookup"><span data-stu-id="71da7-104">You can use the Microsoft Graph Postman collection to get started with Microsoft Graph APIs in minutes.</span></span>

![Изображение Postman](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

<span data-ttu-id="71da7-106">В этой статье рассказывается о том, как быстро приступить к работе с Postman и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71da7-106">This article explains how to get up and running with Postman and Microsoft Graph.</span></span> <span data-ttu-id="71da7-107">Кроме того, вы можете просматривать API Microsoft Graph непосредственно в веб-браузере с помощью [песочницы Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="71da7-107">You can also explore Microsoft Graph APIs directly in your web browser by using [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer).</span></span>

## <a name="accessing-the-collection"></a><span data-ttu-id="71da7-108">Доступ к коллекции</span><span class="sxs-lookup"><span data-stu-id="71da7-108">Accessing the collection</span></span>
<span data-ttu-id="71da7-109">Доступ к коллекции в Postman можно получить двумя способами: путем ее использования или путем добавления в нее.</span><span class="sxs-lookup"><span data-stu-id="71da7-109">You can access the collection in Postman in two ways: by consuming it or by contributing to it.</span></span> <span data-ttu-id="71da7-110">Вначале вам потребуется запустить [Postman](https://www.getpostman.com/) на компьютере.</span><span class="sxs-lookup"><span data-stu-id="71da7-110">You will need to have [Postman](https://www.getpostman.com/) running on your computer first.</span></span>

### <a name="consume-the-collection"></a><span data-ttu-id="71da7-111">Использование коллекции</span><span class="sxs-lookup"><span data-stu-id="71da7-111">Consume the collection</span></span>
<span data-ttu-id="71da7-112">Использование коллекции ⁠— самый простой способ начать работу с API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71da7-112">Consuming the collection is the easiest way to get started with Microsoft Graph APIs.</span></span> <span data-ttu-id="71da7-113">[Ссылка совместного доступа Postman](https://www.getpostman.com/collections/d89a737b5f0c0825898a) запустит Postman.</span><span class="sxs-lookup"><span data-stu-id="71da7-113">The [Postman sharing link](https://www.getpostman.com/collections/d89a737b5f0c0825898a) will launch Postman.</span></span>

<span data-ttu-id="71da7-114">Преимущество использования коллекции с общим доступом заключается в том, что новые запросы будут автоматически отображаться без каких-либо дополнительных действий с вашей стороны.</span><span class="sxs-lookup"><span data-stu-id="71da7-114">The advantage to using the shared collection is that new requests will automatically show for you without any additional steps.</span></span>

<span data-ttu-id="71da7-115">После получения доступа к коллекции необходимо настроить переменные среды:</span><span class="sxs-lookup"><span data-stu-id="71da7-115">After you have the collection, you'll need to set up the environment variables:</span></span>

1. <span data-ttu-id="71da7-116">Выберите **Файл | Импорт...**.</span><span class="sxs-lookup"><span data-stu-id="71da7-116">Choose **File | Import ...**.</span></span>
2. <span data-ttu-id="71da7-117">Выберите **Импорт из ссылки**.</span><span class="sxs-lookup"><span data-stu-id="71da7-117">Select **Import From Link**.</span></span>
3. <span data-ttu-id="71da7-118">Скопируйте и вставьте следующий URL-адрес, затем выберите **Импорт**.</span><span class="sxs-lookup"><span data-stu-id="71da7-118">Copy and paste the following URL and choose **Import**.</span></span>
 
    ```
    https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json
    ```

<span data-ttu-id="71da7-119">В правой верхней части окна должна отобразиться **среда Microsoft Graph** в виде значка с изображением глаза.</span><span class="sxs-lookup"><span data-stu-id="71da7-119">You should now see the **Microsoft Graph environment** in the top right environment drop down by the eye icon.</span></span> <span data-ttu-id="71da7-120">Теперь необходимо [настроить среду](#using-the-collection).</span><span class="sxs-lookup"><span data-stu-id="71da7-120">Now you need to  [set up your environment](#using-the-collection).</span></span>

### <a name="contribute-to-the-collection"></a><span data-ttu-id="71da7-121">Добавление в коллекцию</span><span class="sxs-lookup"><span data-stu-id="71da7-121">Contribute to the collection</span></span>
<span data-ttu-id="71da7-122">Если вы хотите добавить собственные запросы, вам потребуется создать вилку репозитория GitHub [коллекций Postman Microsoft Graph](https://github.com/microsoftgraph/microsoftgraph-postman-collections).</span><span class="sxs-lookup"><span data-stu-id="71da7-122">If you want to contribute your own requests, you will need to fork the [Microsoft Graph Postman collections](https://github.com/microsoftgraph/microsoftgraph-postman-collections) github repo.</span></span> 

<span data-ttu-id="71da7-123">Дополнительные сведения о том, как это сделать, см. в следующем видео.</span><span class="sxs-lookup"><span data-stu-id="71da7-123">For details about how to do this, watch the following video.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]

<span data-ttu-id="71da7-124">Чтобы импортировать коллекции Postman:</span><span class="sxs-lookup"><span data-stu-id="71da7-124">To import the Postman collections:</span></span>

1. <span data-ttu-id="71da7-125">Скачайте [Postman](https://www.getpostman.com/) и зарегистрируйтесь для его использования.</span><span class="sxs-lookup"><span data-stu-id="71da7-125">Download and register for [Postman](https://www.getpostman.com/).</span></span>
2. <span data-ttu-id="71da7-126">Выберите **Файл | Импорт...**.</span><span class="sxs-lookup"><span data-stu-id="71da7-126">Choose **File | Import ...**.</span></span>
3. <span data-ttu-id="71da7-127">Выберите **Импорт из ссылки**.</span><span class="sxs-lookup"><span data-stu-id="71da7-127">Select **Import From Link**.</span></span>
4. <span data-ttu-id="71da7-128">Вставьте два указанных ниже URL-адреса и выберите **Импорт** после каждого из них.</span><span class="sxs-lookup"><span data-stu-id="71da7-128">Paste the following two URLs and choose **Import** after each.</span></span>

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json

    ```

<span data-ttu-id="71da7-129">Теперь в области **Коллекции** должна отобразиться коллекция **Microsoft Graph v1.0**.</span><span class="sxs-lookup"><span data-stu-id="71da7-129">You should now see the **Microsoft Graph v1.0** collection on the **Collections** pane.</span></span>

## <a name="using-the-collection"></a><span data-ttu-id="71da7-130">Использование коллекции</span><span class="sxs-lookup"><span data-stu-id="71da7-130">Using the collection</span></span>
<span data-ttu-id="71da7-131">После создания коллекции **Microsoft Graph v1.0** и **среды Microsoftr Graph** в Postman выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="71da7-131">After you have the **Microsoft Graph v1.0** collection and the **Microsoftr Graph environment** in Postman, follow these steps.</span></span>

### <a name="set-up-application-api-calls"></a><span data-ttu-id="71da7-132">Настройка вызовов API приложений</span><span class="sxs-lookup"><span data-stu-id="71da7-132">Set up application API calls</span></span>

1. <span data-ttu-id="71da7-133">В правом верхнем углу выберите **Без среды** из раскрывающегося списка.</span><span class="sxs-lookup"><span data-stu-id="71da7-133">Choose the **No environment** drop down in top right corner.</span></span>
2. <span data-ttu-id="71da7-134">Выберите **Среда Microsoft Graph**.</span><span class="sxs-lookup"><span data-stu-id="71da7-134">Select **Microsoft Graph environment**.</span></span>
3. <span data-ttu-id="71da7-135">Щелкните значок с изображением **глаза** справа и затем выберите **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="71da7-135">Choose the **eye** icon to the right and then choose **Edit**.</span></span>
4. <span data-ttu-id="71da7-136">Введите свое приложение Microsoft Identity в **текущих** (не **начальных**) переменных: **ClientID**, **ClientSecret** и \*\* TenantID\*\*.</span><span class="sxs-lookup"><span data-stu-id="71da7-136">Enter your Microsoft Identity Application in the **current** (not **initial**) variables: **ClientID**, **ClientSecret** and **TenantID**.</span></span> 
 <span data-ttu-id="71da7-137">Дополнительные сведения о том, как создать приложение и получить согласие администратора только для приложений, см. в записи блога [Использование Postman для осуществления вызовов Microsoft Graph](https://developer.microsoft.com/en-us/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/).</span><span class="sxs-lookup"><span data-stu-id="71da7-137">For more information about how to create an application and to admin consent the app-only flow, see the [Use Postman to make Microsoft Graph calls](https://developer.microsoft.com/en-us/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/) blog post.</span></span>

5. <span data-ttu-id="71da7-138">Нажмите кнопку **Обновить**.</span><span class="sxs-lookup"><span data-stu-id="71da7-138">Select **Update**.</span></span> <span data-ttu-id="71da7-139">Закройте диалоговое окно \*\*Управление средами \*\*.</span><span class="sxs-lookup"><span data-stu-id="71da7-139">Close the **Manage Environments** dialog box.</span></span> <span data-ttu-id="71da7-140">В коллекции **MicrosoftGraph v1.0 | Приложение** с левой стороны выберите **Получить маркер доступа только для приложений**.</span><span class="sxs-lookup"><span data-stu-id="71da7-140">In the **MicrosoftGraph v1.0 | Application** collection on left side, choose **Get App-only Access Token**.</span></span> <span data-ttu-id="71da7-141">Затем в правой части нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="71da7-141">Then choose **Send** on the right.</span></span>
6. <span data-ttu-id="71da7-142">Разверните папку **Приложение | Пользователи** и выберите **Получить пользователей**.</span><span class="sxs-lookup"><span data-stu-id="71da7-142">Expand the **Application | Users** folder and choose **Get Users**.</span></span> <span data-ttu-id="71da7-143">Затем нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="71da7-143">Then choose **Send**.</span></span>

<span data-ttu-id="71da7-144">Теперь вы можете работать с коллекциями Microsoft Graph v 1.0.</span><span class="sxs-lookup"><span data-stu-id="71da7-144">You are now up and running with the Microsoft Graph v1.0 collections.</span></span>

><span data-ttu-id="71da7-145">**Примечание.** Если вы хотите использовать другие API в коллекции, вам будет необходимо подтвердить разрешения, необходимые для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="71da7-145">**Note:** If you want to run other APIs in the collection, you will need to consent the required permissions for your application.</span></span>

### <a name="set-up-on-behalf-of-api-calls"></a><span data-ttu-id="71da7-146">Настройка вызовов API по сценарию "от имени"</span><span class="sxs-lookup"><span data-stu-id="71da7-146">Set up on-behalf-of API calls</span></span>
<span data-ttu-id="71da7-147">Самый простой способ настроить вызовы API по сценарию "от имени" ⁠— это указать **UserName** (Имя пользователя) и **UserPassword** (Пароль пользователя) в параметрах среды и использовать **От имени пользователя | Получить маркер доступа пользователя**.</span><span class="sxs-lookup"><span data-stu-id="71da7-147">The simplest way to set up on-behalf-of API calls is to provide a **UserName** and **UserPassword** in the environment settings and use the **On Behalf of a User | Get User Access Token**.</span></span> 

><span data-ttu-id="71da7-148">**Важно!** Мы не рекомендуем использовать учетные записи пользователей рабочей среды, так как эта информация хранится непосредственно в Postman.</span><span class="sxs-lookup"><span data-stu-id="71da7-148">**Important:** We don't recommend using production user accounts because this information is stored directly in Postman.</span></span> <span data-ttu-id="71da7-149">Также не рекомендуем использовать этот способ для получения маркеров доступа в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="71da7-149">We also don't  recommend using this approach to obtain access tokens in production.</span></span> <span data-ttu-id="71da7-150">Используйте его только в целях тестирования.</span><span class="sxs-lookup"><span data-stu-id="71da7-150">Use it only for testing purposes.</span></span>

<span data-ttu-id="71da7-151">Если вы не хотите хранить имена пользователей и пароли в переменных среды, которые синхронизируются с вашей облачной учетной записью Postman, можно использовать возможность **Получить новый маркер доступа**, чтобы получить маркер, не выходя из Postman.</span><span class="sxs-lookup"><span data-stu-id="71da7-151">If you don't want to store user names and passwords in environment variables that sync to your Postman cloud account, you can use the  **Get New Access Token** capability to get a token without leaving Postman.</span></span>

1. <span data-ttu-id="71da7-152">Выберите **От имени пользователя | Получить маркер доступа с помощью Postman**.</span><span class="sxs-lookup"><span data-stu-id="71da7-152">Select **On behalf of a User | Get Access Token using Postman**.</span></span>
2. <span data-ttu-id="71da7-153">Откройте вкладку **Авторизация**.</span><span class="sxs-lookup"><span data-stu-id="71da7-153">Choose the Authorization tab in the Request Editor.</span></span>
3. <span data-ttu-id="71da7-154">Нажмите кнопку **Получить новый маркер доступа**.</span><span class="sxs-lookup"><span data-stu-id="71da7-154">Choose the **get access token** button.</span></span>
4. <span data-ttu-id="71da7-155">Заполните приведенные ниже поля реальными значениями для клиента и приложения.</span><span class="sxs-lookup"><span data-stu-id="71da7-155">Fill out the following boxes with your real tenant and application values.</span></span> <span data-ttu-id="71da7-156">Обратите внимание на то, что здесь вы не можете использовать переменные среды: необходимо использовать фактические значения.</span><span class="sxs-lookup"><span data-stu-id="71da7-156">Note that you cannot use the environment variables here; you have to use the actual values.</span></span> <span data-ttu-id="71da7-157">Их можно найти, выбрав **EndPoints** (Конечные точки) в колонке приложения на portal.azure.com.</span><span class="sxs-lookup"><span data-stu-id="71da7-157">You can find them by selecting **EndPoints** in the application blade in portal.azure.com.</span></span>

    - <span data-ttu-id="71da7-158">URL-адрес обратного вызова: https://app.getpostman.com/oauth2/callback</span><span class="sxs-lookup"><span data-stu-id="71da7-158">Callback URL: https://app.getpostman.com/oauth2/callback</span></span>
    - <span data-ttu-id="71da7-159">URL-адрес проверки подлинности: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize</span><span class="sxs-lookup"><span data-stu-id="71da7-159">Auth URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize</span></span>
    - <span data-ttu-id="71da7-160">URL-адрес маркера доступа: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token</span><span class="sxs-lookup"><span data-stu-id="71da7-160">Access Token URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token</span></span>
    - <span data-ttu-id="71da7-161">Идентификатор клиента: **CLIENTID**</span><span class="sxs-lookup"><span data-stu-id="71da7-161">Client ID: **CLIENTID**</span></span>
    - <span data-ttu-id="71da7-162">Секрет клиента: **CLIENTSECRET**</span><span class="sxs-lookup"><span data-stu-id="71da7-162">Client Secret: **CLIENTSECRET**</span></span>
    - <span data-ttu-id="71da7-163">Область: https://graph.microsoft.com/.default</span><span class="sxs-lookup"><span data-stu-id="71da7-163">https://graph.microsoft.com/.default</span></span>
    - <span data-ttu-id="71da7-164">Состояние: **RANDOMSTRING**</span><span class="sxs-lookup"><span data-stu-id="71da7-164">State: **RANDOMSTRING**</span></span>
 
5. <span data-ttu-id="71da7-165">Нажмите **Запросить маркер**.</span><span class="sxs-lookup"><span data-stu-id="71da7-165">Choose **Request Token**.</span></span> <span data-ttu-id="71da7-166">Вы увидите запрос пользовательского интерфейса на вход в систему и одобрение разрешений.</span><span class="sxs-lookup"><span data-stu-id="71da7-166">You should see a UI prompt to sign in and consent permissions.</span></span>
6. <span data-ttu-id="71da7-167">Скопируйте маркер доступа, откройте ваши переменные среды и вставьте его в поле **UserAccessToken** (Маркер доступа пользователя).</span><span class="sxs-lookup"><span data-stu-id="71da7-167">Copy the access token, open your environment variables, and paste it into the **UserAccessToken** field.</span></span>

<span data-ttu-id="71da7-168">Теперь все ваши запросы будут рабочими.</span><span class="sxs-lookup"><span data-stu-id="71da7-168">Now all your requests will work.</span></span>
