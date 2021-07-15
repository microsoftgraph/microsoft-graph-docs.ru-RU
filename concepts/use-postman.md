---
title: Использование Postman с API Microsoft Graph
description: Используйте коллекцию Microsoft Graph Postman, чтобы начать работу с API Microsoft Graph в считанные минуты.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: b5dbeb6c779bcd02cd1ae329b3b63df6c44a1da8
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430136"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a><span data-ttu-id="94b83-103">Использование Postman с API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="94b83-103">Use Postman with the Microsoft Graph API</span></span>

<span data-ttu-id="94b83-104">Вы можете использовать коллекцию Microsoft Graph Postman, чтобы начать работу с API Microsoft Graph в считанные минуты.</span><span class="sxs-lookup"><span data-stu-id="94b83-104">You can use the Microsoft Graph Postman collection to get started with Microsoft Graph APIs in minutes.</span></span>

![Изображение Postman](images/postman-screenshot.png)

<span data-ttu-id="94b83-106">В этой статье рассказывается о том, как быстро приступить к работе с Postman и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="94b83-106">This article explains how to get up and running with Postman and Microsoft Graph.</span></span> <span data-ttu-id="94b83-107">Кроме того, вы можете просматривать API Microsoft Graph непосредственно в веб-браузере с помощью [песочницы Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="94b83-107">You can also explore Microsoft Graph APIs directly in your web browser by using [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="94b83-108">Чтобы узнать, как это сделать, выполните действия, описанные в этой статье, или посмотрите видео [Начало работы с рабочей областью Microsoft Graph Postman](https://youtu.be/3RTHY3jScmA).</span><span class="sxs-lookup"><span data-stu-id="94b83-108">For details about how to do this, follow the steps in this article or watch the [Getting started with Microsoft Graph Postman workspace](https://youtu.be/3RTHY3jScmA) video.</span></span>

## <a name="step-1---forking-the-microsoft-graph-postman-collection"></a><span data-ttu-id="94b83-109">Шаг 1. Разветвление коллекции Microsoft Graph Postman</span><span class="sxs-lookup"><span data-stu-id="94b83-109">Step 1 - Forking the Microsoft Graph Postman collection</span></span>

<span data-ttu-id="94b83-110">Чтобы воспользоваться коллекцией Postman, создайте ее вилку в своей рабочей области Postman.</span><span class="sxs-lookup"><span data-stu-id="94b83-110">To use the Postman collection, fork it to your own Postman workspace.</span></span> <span data-ttu-id="94b83-111">Выполните это в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="94b83-111">Do this from the web browser.</span></span>

1. <span data-ttu-id="94b83-112">Откройте [Postman](https://www.postman.com/) и войдите.</span><span class="sxs-lookup"><span data-stu-id="94b83-112">Go to [Postman](https://www.postman.com/) and sign in.</span></span>
1. <span data-ttu-id="94b83-113">Перейдите в коллекцию Postman с меткой [Microsoft Graph](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/collection/455214-085f7047-1bec-4570-9ed0-3a7253be148c/fork).</span><span class="sxs-lookup"><span data-stu-id="94b83-113">Go to the Postman collection labeled [Microsoft Graph](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/collection/455214-085f7047-1bec-4570-9ed0-3a7253be148c/fork).</span></span>
1. <span data-ttu-id="94b83-114">Укажите метку для своей вилки.</span><span class="sxs-lookup"><span data-stu-id="94b83-114">Fill in a label for your own fork.</span></span> <span data-ttu-id="94b83-115">Это может быть любой текст.</span><span class="sxs-lookup"><span data-stu-id="94b83-115">This can be any text.</span></span>
1. <span data-ttu-id="94b83-116">В разделе рабочей области выберите **My Workspace** (Моя рабочая область) в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="94b83-116">Under Workspace, ensure that **My Workspace** is selected in the drop-down list.</span></span>
1. <span data-ttu-id="94b83-117">Нажмите **Fork Collection** (Разветвление коллекции).</span><span class="sxs-lookup"><span data-stu-id="94b83-117">Click **Fork Collection**.</span></span>

<span data-ttu-id="94b83-118">Вы будете перенаправлены в вилку главной коллекции Microsoft Graph Postman в своей рабочей области.</span><span class="sxs-lookup"><span data-stu-id="94b83-118">You will be redirected to a fork of the main Microsoft Graph Postman collection in your own workspace.</span></span>

## <a name="step-2---optional---postman-web-browser-only-download-the-postman-agent"></a><span data-ttu-id="94b83-119">Шаг 2. Скачивание агента (необязательно, только в веб-браузере Postman)</span><span class="sxs-lookup"><span data-stu-id="94b83-119">Step 2 - (Optional - Postman Web browser only) Download the Postman Agent</span></span>

<span data-ttu-id="94b83-120">Чтобы использовать эту конкретную коллекцию Postman в своем веб-браузере, скачайте [классический агент Postman](https://www.postman.com/downloads).</span><span class="sxs-lookup"><span data-stu-id="94b83-120">To use this particular Postman collection in your web browser, download the [Postman Desktop Agent](https://www.postman.com/downloads).</span></span> <span data-ttu-id="94b83-121">Без этого вы не можете использовать Postman для Интернета из-за ограничений CORS в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="94b83-121">You can't use Postman for the web without this due to CORS restrictions in the web browser.</span></span>

<span data-ttu-id="94b83-122">Вам не требуется агент, если вы используете Postman для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="94b83-122">You don't need the agent if you're using the Postman for Windows app.</span></span> <span data-ttu-id="94b83-123">Если вы открываете Postman для Windows, вы увидите эту разветвленную коллекцию в своей рабочей области.</span><span class="sxs-lookup"><span data-stu-id="94b83-123">If you open Postman for Windows, you will see this forked collection in your workspace.</span></span>

## <a name="step-3---create-an-azure-ad-application"></a><span data-ttu-id="94b83-124">Шаг 3. Создание приложения Azure AD</span><span class="sxs-lookup"><span data-stu-id="94b83-124">Step 3 - Create an Azure AD application</span></span>

<span data-ttu-id="94b83-125">Чтобы использовать эту коллекцию в своем клиенте разработчика, создайте приложение Azure AD и предоставьте ему соответствующие разрешения для запросов, которые нужно выполнять.</span><span class="sxs-lookup"><span data-stu-id="94b83-125">To use this collection in your own developer tenant, create an Azure AD application and give it the appropriate permissions for the requests you want to call.</span></span> <span data-ttu-id="94b83-126">Если у вас нет клиента разработчика, вы можете зарегистрироваться для получения одного из них в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="94b83-126">If you don't have a developer tenant, you can sign up for one through the [Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span>

1. <span data-ttu-id="94b83-127">Перейдите на сайт [portal.azure.com](https://portal.azure.com/) и войдите, используя свою учетную запись администратора клиента разработчика.</span><span class="sxs-lookup"><span data-stu-id="94b83-127">Go to [portal.azure.com](https://portal.azure.com/) and sign in with your developer tenant administrator account.</span></span>
1. <span data-ttu-id="94b83-128">В разделе **Службы Azure** нажмите **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="94b83-128">Under **Azure Services**, click **Azure Active Directory**.</span></span>
1. <span data-ttu-id="94b83-129">В меню слева выберите **Регистрация приложений**.</span><span class="sxs-lookup"><span data-stu-id="94b83-129">On the left menu, click **App registrations**.</span></span>
1. <span data-ttu-id="94b83-130">В горизонтальном меню нажмите **Новая регистрация**.</span><span class="sxs-lookup"><span data-stu-id="94b83-130">On the horizontal menu, click **New registration**.</span></span>
1. <span data-ttu-id="94b83-131">В качестве **имени приложения** укажите `Postman`.</span><span class="sxs-lookup"><span data-stu-id="94b83-131">Set the **Application name** to `Postman`.</span></span>
1. <span data-ttu-id="94b83-132">Присвойте параметру **URI перенаправления** значение `https://oauth.pstmn.io/v1/browser-callback`.</span><span class="sxs-lookup"><span data-stu-id="94b83-132">Set the **Redirect URI** to `https://oauth.pstmn.io/v1/browser-callback`.</span></span>
1. <span data-ttu-id="94b83-133">Нажмите **Зарегистрировать**.</span><span class="sxs-lookup"><span data-stu-id="94b83-133">Click **Register**.</span></span>
1. <span data-ttu-id="94b83-134">В меню слева выберите **Разрешения API**.</span><span class="sxs-lookup"><span data-stu-id="94b83-134">On the left menu, click **API Permissions**.</span></span>
1. <span data-ttu-id="94b83-135">В горизонтальном меню щелкните **Добавить разрешение**, выберите **Microsoft Graph** и нажмите **Делегированные разрешения**.</span><span class="sxs-lookup"><span data-stu-id="94b83-135">In the horizontal menu, click **Add a permission**, select **Microsoft Graph**, and then select **Delegated Permissions**.</span></span>
1. <span data-ttu-id="94b83-136">Введите `Mail.`, разверните параметры **Mail** и установите флажок **Mail.Read**.</span><span class="sxs-lookup"><span data-stu-id="94b83-136">Type `Mail.`, expand the **Mail** options, and check **Mail.Read**.</span></span>
1. <span data-ttu-id="94b83-137">Щелкните **Разрешения приложений**, введите `User.`и просмотрите **разрешения приложений**.</span><span class="sxs-lookup"><span data-stu-id="94b83-137">Click **Application permissions** and type `User.`, and check **Application Permissions**.</span></span>
1. <span data-ttu-id="94b83-138">Разверните параметры **User** и установите флажок **User.Read.All**.</span><span class="sxs-lookup"><span data-stu-id="94b83-138">Expand the **User** options and check **User.Read.All**.</span></span>
1. <span data-ttu-id="94b83-139">Щелкните **Добавить разрешения**.</span><span class="sxs-lookup"><span data-stu-id="94b83-139">Click **Add permissions**.</span></span>
1. <span data-ttu-id="94b83-140">В горизонтальном меню нажмите **Предоставить согласие администратора для** и нажмите **Да**.</span><span class="sxs-lookup"><span data-stu-id="94b83-140">In the horizontal menu, click **Grant admin consent for**, and click **Yes**.</span></span>
1. <span data-ttu-id="94b83-141">В меню слева щелкните **Обзор**.</span><span class="sxs-lookup"><span data-stu-id="94b83-141">In the left menu, click **Overview**.</span></span> <span data-ttu-id="94b83-142">Здесь можно узнать **Идентификатор приложения (клиент)** и **Идентификатор каталога (клиент)**.</span><span class="sxs-lookup"><span data-stu-id="94b83-142">From here, you can get the **Application (client) ID** and **Directory (tenant) ID**.</span></span> <span data-ttu-id="94b83-143">Они понадобятся вам на шаге 4.</span><span class="sxs-lookup"><span data-stu-id="94b83-143">You will need these in step 4.</span></span>
1. <span data-ttu-id="94b83-144">В меню слева выберите **Сертификаты и секреты**.</span><span class="sxs-lookup"><span data-stu-id="94b83-144">In the left menu, click **Certificates & secrets**.</span></span>
1. <span data-ttu-id="94b83-145">Щелкните **Новый секрет клиента**, введите описание и нажмите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="94b83-145">Click **New client secret**, enter a description, and click **Add**.</span></span> <span data-ttu-id="94b83-146">Наведите курсор на **значение** нового секрета клиента и скопируйте его.</span><span class="sxs-lookup"><span data-stu-id="94b83-146">Hover over the new client secret **Value** and copy it.</span></span> <span data-ttu-id="94b83-147">Оно понадобится вам на шаге 4.</span><span class="sxs-lookup"><span data-stu-id="94b83-147">You will need this in step 4.</span></span>

<span data-ttu-id="94b83-148">У приложения Azure AD теперь есть разрешения на выполнение запросов от имени пользователя для вызова Mail.Read и вызова User.Read.All в качестве приложения.</span><span class="sxs-lookup"><span data-stu-id="94b83-148">The Azure AD application now has permissions to make requests on behalf of a user to call Mail.Read and as an application for User.Read.All.</span></span>

## <a name="step-4---configuring-authentication-in-postman"></a><span data-ttu-id="94b83-149">Шаг 4. Настройка проверки подлинности в Postman</span><span class="sxs-lookup"><span data-stu-id="94b83-149">Step 4 - Configuring authentication in Postman</span></span>

<span data-ttu-id="94b83-150">На этом шаге вы настроите переменные среды, используемые для получения маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="94b83-150">In this step, you set up the environment variables used to retrieve an access token.</span></span>

1. <span data-ttu-id="94b83-151">Перейдите в [Развилку среды](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/environment/455214-efbc69b2-69bd-402e-9e72-850b3a49bb21/fork).</span><span class="sxs-lookup"><span data-stu-id="94b83-151">Go to [Fork environment](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/environment/455214-efbc69b2-69bd-402e-9e72-850b3a49bb21/fork).</span></span>
1. <span data-ttu-id="94b83-152">Добавьте метку для развилки.</span><span class="sxs-lookup"><span data-stu-id="94b83-152">Add a label for fork.</span></span> <span data-ttu-id="94b83-153">Это может быть любой текст.</span><span class="sxs-lookup"><span data-stu-id="94b83-153">This can be any text.</span></span>
1. <span data-ttu-id="94b83-154">В разделе рабочей области выберите **My Workspace** (Моя рабочая область) в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="94b83-154">Under Workspace, ensure that **My Workspace** is selected in the drop-down list.</span></span>
1. <span data-ttu-id="94b83-155">Нажмите **Развилка среды**.</span><span class="sxs-lookup"><span data-stu-id="94b83-155">Click **Fork Environment**.</span></span>
1. <span data-ttu-id="94b83-156">В `ClientID` задайте **Текущее значение** для значения ИД приложения (клиента) из шага 3.15.</span><span class="sxs-lookup"><span data-stu-id="94b83-156">In `ClientID`, set the **Current value** to the application (client) ID value from step 3.15.</span></span>
1. <span data-ttu-id="94b83-157">В `ClientSecret` задайте **Текущее значение** для секретного значения клиента из шага 3.17.</span><span class="sxs-lookup"><span data-stu-id="94b83-157">In `ClientSecret`, set the **Current value** to the client secret value from step 3.17.</span></span>
1. <span data-ttu-id="94b83-158">В `TenantID` задайте **Текущее значение** для значения ИД каталога (клиента) из шага 3.15.</span><span class="sxs-lookup"><span data-stu-id="94b83-158">In `TenantID`, set the **Current value** to the directory (tenant) ID value from step 3.15.</span></span>
1. <span data-ttu-id="94b83-159">В правом верхнем углу нажмите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="94b83-159">On the top right, click **Save**.</span></span>
1. <span data-ttu-id="94b83-160">Закройте диалоговое окно **Управление средами**.</span><span class="sxs-lookup"><span data-stu-id="94b83-160">Close the **Manage Environments** tab.</span></span>
1. <span data-ttu-id="94b83-161">В правом верхнем углу рядом со значком глаза убедитесь, что в раскрывающемся меню выбрано значение **Среда M365**, а не значение **Без среды**.</span><span class="sxs-lookup"><span data-stu-id="94b83-161">On the top right, next to the eye icon, verify that **M365 Environment** is selected in the drop down and not **No environment**.</span></span>

## <a name="step-5---get-a-delegated-access-token"></a><span data-ttu-id="94b83-162">Шаг 5. Получение маркера делегированного доступа</span><span class="sxs-lookup"><span data-stu-id="94b83-162">Step 5 - Get a delegated access token</span></span>

<span data-ttu-id="94b83-163">Так как вы впервые выполняете запрос в виде делегированного потока проверки подлинности, вам потребуется получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="94b83-163">Because this is the first time you are running a request as a delegated authentication flow, you need to get an access token.</span></span>

1. <span data-ttu-id="94b83-164">Наведите курсор на папку **Делегированное**, щелкните многоточие и выберите **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="94b83-164">Hover over the **Delegated** folder, click the ellipsis, and select **Edit**</span></span>
1. <span data-ttu-id="94b83-165">Щелкните вкладку **Authorization** (Авторизация).</span><span class="sxs-lookup"><span data-stu-id="94b83-165">Click the **Authorization** tab.</span></span>
1. <span data-ttu-id="94b83-166">Прокрутите страницу вправо и щелкните **Get New Access Token** (Получить новый маркер доступа).</span><span class="sxs-lookup"><span data-stu-id="94b83-166">Scroll down on the right and click **Get New Access Token**.</span></span>
1. <span data-ttu-id="94b83-167">Войдите с помощью учетной записи администратора клиента разработчика.</span><span class="sxs-lookup"><span data-stu-id="94b83-167">Sign in with your developer tenant administrator account.</span></span>
1. <span data-ttu-id="94b83-168">Щелкните **Proceed** (Продолжить) и нажмите кнопку **Use Token** (Использовать маркер).</span><span class="sxs-lookup"><span data-stu-id="94b83-168">Click **Proceed**, and then click the **Use Token** button.</span></span>
1. <span data-ttu-id="94b83-169">В правом нижнем углу диалогового окна щелкните **Update** (Обновить).</span><span class="sxs-lookup"><span data-stu-id="94b83-169">On the botton right of the dialog, click **Update**.</span></span>

<span data-ttu-id="94b83-170">Теперь у вас есть действительный маркер доступа для использования в делегированных запросах.</span><span class="sxs-lookup"><span data-stu-id="94b83-170">You now have a valid access token to use for delegated requests.</span></span>

## <a name="step-6---run-your-first-delegated-request"></a><span data-ttu-id="94b83-171">Шаг 6. Выполнение первого делегированного запроса</span><span class="sxs-lookup"><span data-stu-id="94b83-171">Step 6 - Run your first delegated request</span></span>

<span data-ttu-id="94b83-172">В папке **Делегированное** расположены запросы различных рабочих нагрузок Microsoft Graph, которые вы можете вызвать.</span><span class="sxs-lookup"><span data-stu-id="94b83-172">Inside the **Delegated** folder are requests for various Microsoft Graph workloads you can call.</span></span>

1. <span data-ttu-id="94b83-173">Разверните папку **Делегированное**, а затем — папку **Почта**.</span><span class="sxs-lookup"><span data-stu-id="94b83-173">Expand the **Delegated** folder and then expand the **Mail** folder.</span></span>
1. <span data-ttu-id="94b83-174">Дважды щелкните **Get my messages** (Получить мои сообщения), чтобы создать запрос.</span><span class="sxs-lookup"><span data-stu-id="94b83-174">Double-click **Get my messages** to open the request.</span></span>
1. <span data-ttu-id="94b83-175">В правом верхнем углу нажмите **Send** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="94b83-175">On the top right, click **Send**.</span></span>

<span data-ttu-id="94b83-176">Вы успешно выполнили вызов Microsoft Graph с помощью делегированной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="94b83-176">You have now successfully made a Microsoft Graph call using delegated authentication.</span></span>

## <a name="step-7---get-an-application-access-token"></a><span data-ttu-id="94b83-177">Действие 7. Получение маркера доступа приложения</span><span class="sxs-lookup"><span data-stu-id="94b83-177">Step 7 - Get an application access token</span></span>

<span data-ttu-id="94b83-178">Так как вы впервые выполняете запрос в виде потока проверки подлинности приложения, вам потребуется получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="94b83-178">Because this is the first time you are running a request as a application authentication flow, you need to get an access token.</span></span>

1. <span data-ttu-id="94b83-179">Наведите курсор на папку **Application** (Приложение), щелкните многоточие и выберите **Edit** (Изменить).</span><span class="sxs-lookup"><span data-stu-id="94b83-179">Hover over the **Application** folder, click the ellipsis, and select **Edit**.</span></span>
1. <span data-ttu-id="94b83-180">Щелкните вкладку **Authorization** (Авторизация).</span><span class="sxs-lookup"><span data-stu-id="94b83-180">Click the **Authorization** tab</span></span>
1. <span data-ttu-id="94b83-181">Прокрутите страницу вправо и щелкните **Get New Access Token** (Получить новый маркер доступа).</span><span class="sxs-lookup"><span data-stu-id="94b83-181">Scroll down on the right side and click **Get New Access Token**.</span></span>
1. <span data-ttu-id="94b83-182">Щелкните **Proceed** (Продолжить) и нажмите кнопку **Use Token** (Использовать маркер).</span><span class="sxs-lookup"><span data-stu-id="94b83-182">Click **Proceed**, and then click the **Use Token** button.</span></span>
1. <span data-ttu-id="94b83-183">В правом нижнем углу диалогового окна щелкните **Update** (Обновить).</span><span class="sxs-lookup"><span data-stu-id="94b83-183">On the bottom right of the dialog, click **Update**.</span></span>

<span data-ttu-id="94b83-184">Теперь у вас есть действительный маркер доступа для использования в запросах приложения.</span><span class="sxs-lookup"><span data-stu-id="94b83-184">You now have a valid access token to use for application requests.</span></span>

## <a name="step-8---run-your-first-application-request"></a><span data-ttu-id="94b83-185">Шаг 8. Выполнение первого запроса приложения</span><span class="sxs-lookup"><span data-stu-id="94b83-185">Step 8 - Run your first application request</span></span>

<span data-ttu-id="94b83-186">В папке **Application** (Приложение) расположены запросы различных рабочих нагрузок Microsoft Graph, которые вы можете вызвать.</span><span class="sxs-lookup"><span data-stu-id="94b83-186">Inside the **Application** folder are requests for various Microsoft Graph workloads you can call.</span></span>

1. <span data-ttu-id="94b83-187">Разверните папку **Application** (Приложение), а затем — папку **User** (Пользователь).</span><span class="sxs-lookup"><span data-stu-id="94b83-187">Expand the **Application** folder and then expand the **User** folder.</span></span>
1. <span data-ttu-id="94b83-188">Дважды щелкните **Get Users** (Получить пользователей), чтобы создать запрос.</span><span class="sxs-lookup"><span data-stu-id="94b83-188">Double-click **Get Users** to open the request.</span></span>
1. <span data-ttu-id="94b83-189">В правом верхнем углу нажмите **Send** (Отправить).</span><span class="sxs-lookup"><span data-stu-id="94b83-189">On the top right, click **Send**.</span></span>

<span data-ttu-id="94b83-190">Вы успешно выполнили вызов Microsoft Graph с помощью проверки подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="94b83-190">You have now successfully made a Microsoft Graph call using application authentication.</span></span>

<span data-ttu-id="94b83-p110">Чтобы осуществить другие запросы в Microsoft Graph, можно выполнить следующие действия. Помните, что для выполнения других запросов вам требуется добавить разрешение для приложения Azure AD. В противном случае в ваших откликах будут возникать ошибки с отказом в получении разрешений.</span><span class="sxs-lookup"><span data-stu-id="94b83-p110">You can follow these steps to make other requests to Microsoft Graph. Remember that you have to add permissions to your Azure AD application for other requests to work; Otherwise, you will get permission denied errors in your responses.</span></span>

### <a name="contribute-to-the-collection"></a><span data-ttu-id="94b83-193">Добавление в коллекцию</span><span class="sxs-lookup"><span data-stu-id="94b83-193">Contribute to the collection</span></span>

<span data-ttu-id="94b83-194">Если вы хотите добавить собственные запросы, вам потребуется лицензия Postman.</span><span class="sxs-lookup"><span data-stu-id="94b83-194">If you want to contribute your own requests, you will need a Postman license.</span></span> <span data-ttu-id="94b83-195">Вы можете внести изменения в разветвленную коллекцию, а затем навести курсор на верхний узел коллекции и выбрать пункт **Create pull request** (Создать запрос на вытягивание).</span><span class="sxs-lookup"><span data-stu-id="94b83-195">You can make your changes to the forked collection, and then hover over the collection top node and select **Create pull request**.</span></span>

## <a name="see-also"></a><span data-ttu-id="94b83-196">См. также</span><span class="sxs-lookup"><span data-stu-id="94b83-196">See also</span></span>

<span data-ttu-id="94b83-197">Чтобы узнать, как это сделать, посмотрите видео [Начало работы с коллекцией Microsoft Graph Postman](https://youtu.be/3RTHY3jScmA).</span><span class="sxs-lookup"><span data-stu-id="94b83-197">For details about how to do this, watch the [Getting started with Microsoft Graph Postman collection](https://youtu.be/3RTHY3jScmA) video.</span></span>
