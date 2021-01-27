---
title: Использование graph Explorer для использования API Microsoft Graph
description: Используйте graph Explorer, чтобы попробовать API Microsoft Graph в образце клиента по умолчанию, чтобы изучить возможности, или войти в собственный клиент и использовать его в качестве средства создания образцов для выполнения сценариев приложений.
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: 3f957d940d4dde483324492f1778ede970a5aefc
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013802"
---
# <a name="use-graph-explorer-to-try-microsoft-graph-apis"></a><span data-ttu-id="36f18-103">Использование обозревателя Graph для использования API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="36f18-103">Use Graph Explorer to try Microsoft Graph APIs</span></span>

<span data-ttu-id="36f18-104">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) — это средство разработчика, которое позволяет удобно создавать запросы REST API Microsoft Graph и просматривать соответствующие ответы.</span><span class="sxs-lookup"><span data-stu-id="36f18-104">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) is a developer tool that lets you conveniently make Microsoft Graph REST API requests and view corresponding responses.</span></span> <span data-ttu-id="36f18-105">Используйте обозреватель Graph, чтобы попробовать API в образце клиента по умолчанию для изучения возможностей, или войти в собственный клиент и использовать его в качестве средства создания собственных примеров для выполнения сценариев приложений.</span><span class="sxs-lookup"><span data-stu-id="36f18-105">Use Graph Explorer to try APIs on the default sample tenant to explore capabilities, or sign in to your own tenant and use it as a prototyping tool to fulfill your app scenarios.</span></span> <span data-ttu-id="36f18-106">Это средство включает полезные функции, такие как фрагменты кода на C#, Java, JavaScript и Objective C; Интеграция набор средств и адаптивных картОчек Microsoft Graph; и не только.</span><span class="sxs-lookup"><span data-stu-id="36f18-106">This tool includes helpful features such as code snippets in C#, Java, JavaScript, and Objective C; Microsoft Graph Toolkit and adaptive cards integration; and more.</span></span>

<span data-ttu-id="36f18-107">Используйте graph Explorer для:</span><span class="sxs-lookup"><span data-stu-id="36f18-107">Use Graph Explorer to:</span></span>

- <span data-ttu-id="36f18-108">Сделайте запросы API Microsoft Graph (GET, POST, PUT, PATCH и DELETE) и посмотрите ответы, включая код ответа, а также любые заголовки и текст.</span><span class="sxs-lookup"><span data-stu-id="36f18-108">Make Microsoft Graph API requests (GET, POST, PUT, PATCH and DELETE) and see responses including response code and any headers and bodies.</span></span>
- <span data-ttu-id="36f18-109">Согласие на разрешения.</span><span class="sxs-lookup"><span data-stu-id="36f18-109">Consent to permissions.</span></span>
- <span data-ttu-id="36f18-110">Добавьте в запрос тело запроса и заголовщик запроса.</span><span class="sxs-lookup"><span data-stu-id="36f18-110">Add a request body and request header to your query.</span></span>
- <span data-ttu-id="36f18-111">Просмотр и копирование маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="36f18-111">View and copy the access token.</span></span>
- <span data-ttu-id="36f18-112">Просмотр примеров запросов для различных служб в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="36f18-112">View sample queries for different services in Microsoft Graph.</span></span>
- <span data-ttu-id="36f18-113">Просмотр, скачивание и удаление запросов, которые вы запустили за последние 30 дней.</span><span class="sxs-lookup"><span data-stu-id="36f18-113">View, download, or delete the queries you ran in the last 30 days.</span></span>
- <span data-ttu-id="36f18-114">Просмотр и копирование фрагментов кода каждого запроса, который вы запустите на C#, Java, JavaScript и Objective C.</span><span class="sxs-lookup"><span data-stu-id="36f18-114">View and copy code snippets of each query you run in C#, Java, JavaScript, and Objective C.</span></span>
- <span data-ttu-id="36f18-115">Доступ к компонентам набор средств Microsoft Graph и адаптивным карточкам для некоторых примеров запросов.</span><span class="sxs-lookup"><span data-stu-id="36f18-115">Access Microsoft Graph Toolkit components and adaptive cards for some sample queries.</span></span>
- <span data-ttu-id="36f18-116">Совместное выполнение запросов, включая тело запроса и заглавные разделы запросов.</span><span class="sxs-lookup"><span data-stu-id="36f18-116">Share queries, including the request body and request headers.</span></span>

<span data-ttu-id="36f18-117">Процесс проверки подлинности обрабатывается в проводнике Graph.</span><span class="sxs-lookup"><span data-stu-id="36f18-117">Graph Explorer handles the authentication process for you.</span></span> <span data-ttu-id="36f18-118">Настройте пользовательский эффект, вынившись на боковой панели и изменив тему.</span><span class="sxs-lookup"><span data-stu-id="36f18-118">Customize the experience by collapsing the sidebar and changing the theme.</span></span>

## <a name="get-started"></a><span data-ttu-id="36f18-119">Начало работы</span><span class="sxs-lookup"><span data-stu-id="36f18-119">Get started</span></span>

<span data-ttu-id="36f18-120">Graph Explorer — это веб-приложение, которое находится в [Центре разработчиков Microsoft Graph.](https://developer.microsoft.com/en-us/graph/graph-explorer)</span><span class="sxs-lookup"><span data-stu-id="36f18-120">Graph Explorer is a web application hosted on the [Microsoft Graph developer center](https://developer.microsoft.com/en-us/graph/graph-explorer).</span></span> <span data-ttu-id="36f18-121">Это проект с открытым исходным кодом, и мы будем рады вашим вкладам и отзывам в [репозитарии GitHub.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4)</span><span class="sxs-lookup"><span data-stu-id="36f18-121">It's an open source project,  and we welcome your contributions and feedback in the [GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4).</span></span>

<span data-ttu-id="36f18-122">В проводнике Graph есть следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="36f18-122">Graph Explorer includes the following elements:</span></span>

1. <span data-ttu-id="36f18-123">В выпадаемом списке http verb</span><span class="sxs-lookup"><span data-stu-id="36f18-123">HTTP verb drop-down list</span></span>
2. <span data-ttu-id="36f18-124">В выпадаемом списке версий API</span><span class="sxs-lookup"><span data-stu-id="36f18-124">API version drop-down list</span></span>
3. <span data-ttu-id="36f18-125">Адресная стойка запроса запроса</span><span class="sxs-lookup"><span data-stu-id="36f18-125">Request query address bar</span></span>
4. <span data-ttu-id="36f18-126">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="36f18-126">Sample query</span></span>
5. <span data-ttu-id="36f18-127">Ссылка на документацию для примера запроса</span><span class="sxs-lookup"><span data-stu-id="36f18-127">Documentation link for the sample query</span></span>

![Снимок экрана: пользовательский интерфейс обозревателя Graph](./images/getting-started.png)

### <a name="make-a-get-request-in-graph-explorer"></a><span data-ttu-id="36f18-129">Запрос GET в обозревателе Graph</span><span class="sxs-lookup"><span data-stu-id="36f18-129">Make a GET request in Graph Explorer</span></span>

<span data-ttu-id="36f18-130">Для запуска запроса GET в graph Explorer вам не нужно вписаться.</span><span class="sxs-lookup"><span data-stu-id="36f18-130">To run a GET request in Graph Explorer, you don’t have to be signed in.</span></span> <span data-ttu-id="36f18-131">Просто щелкните пример запроса, и образцы данных отметят в предварительном просмотре отклика.</span><span class="sxs-lookup"><span data-stu-id="36f18-131">Just click a sample query and sample data will show in the response preview.</span></span> 

![Снимок экрана: пример запроса в обозревателе Graph](./images/making-a-get-request.png)

<span data-ttu-id="36f18-133">Чтобы сделать запрос, сделайте:</span><span class="sxs-lookup"><span data-stu-id="36f18-133">To make a request:</span></span>

1. <span data-ttu-id="36f18-134">Выберите пример запроса и запустите его.</span><span class="sxs-lookup"><span data-stu-id="36f18-134">Select a sample query and run it.</span></span>
2. <span data-ttu-id="36f18-135">Получите код отклика HTTP.</span><span class="sxs-lookup"><span data-stu-id="36f18-135">Get the HTTP response code.</span></span>
3. <span data-ttu-id="36f18-136">См. ответ от API Microsoft Graph с примерами данных.</span><span class="sxs-lookup"><span data-stu-id="36f18-136">See the response from the Microsoft Graph API with sample data.</span></span>

<span data-ttu-id="36f18-137">При входе в обозреватель Graph и нажатии того же запроса возвращается ответ с реальными данными от клиента, в который вы вошел.</span><span class="sxs-lookup"><span data-stu-id="36f18-137">When you sign in to Graph Explorer and click the same query, the response will be returned with real data from the tenant you signed in to.</span></span>

### <a name="running-non-get-requests-in-graph-explorer"></a><span data-ttu-id="36f18-138">Запуск запросов, не отсланных от GET, в обозревателе Graph</span><span class="sxs-lookup"><span data-stu-id="36f18-138">Running non-GET requests in Graph Explorer</span></span>

<span data-ttu-id="36f18-139">Чтобы попробовать запросы POST, PUT, PATCH и DELETE, во sign in to Graph Explorer using a Microsoft 365 account. Это может быть учетная запись организации для тестирования или демонстрации.</span><span class="sxs-lookup"><span data-stu-id="36f18-139">To try POST, PUT, PATCH and DELETE requests, sign in to Graph Explorer using a Microsoft 365 account.This can be an organizational account for testing or demonstration purpose.</span></span> <span data-ttu-id="36f18-140">Чтобы получить бесплатный пример подписки разработчика Microsoft 365 E5, а также инструментов и других ресурсов, которые помогут вам создавать решения для платформы Microsoft 365, присоединяйтесь к программе для разработчиков [Microsoft 365.](https://developer.microsoft.com/microsoft-365/dev-program)</span><span class="sxs-lookup"><span data-stu-id="36f18-140">To get a free sample Microsoft 365 E5 developer subscription, along with tools and other resources to help you build solutions for the Microsoft 365 platform, join the [Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> 

>[!IMPORTANT]
><span data-ttu-id="36f18-141">Если вы решили войти с помощью учетной записи организации, запуск запроса, не относястого к GET, может повлиять на данные в клиенте.</span><span class="sxs-lookup"><span data-stu-id="36f18-141">If you choose to sign in using your organizational account, running a non-GET request can affect the data in the tenant.</span></span>

<span data-ttu-id="36f18-142">Например, чтобы выполнить запрос POST, выберите POST в выпадаемом списке для команды HTTP и добавьте тело запроса и заглавные столбцы запроса соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="36f18-142">For example, to run a POST request, select POST in the drop-down list for the HTTP verb, and add a request body and request headers as appropriate.</span></span>

![Снимок экрана: запрос POST в обозревателе Graph](./images/making-a-post-request.png)

1. <span data-ttu-id="36f18-144">Выберите пример запроса POST.</span><span class="sxs-lookup"><span data-stu-id="36f18-144">Select a POST sample query.</span></span>
2. <span data-ttu-id="36f18-145">Обновление **тела запроса;** например, придать приложению имя.</span><span class="sxs-lookup"><span data-stu-id="36f18-145">Update **Request body**; for example, give the application a name.</span></span>
3. <span data-ttu-id="36f18-146">Нажмите **кнопку "Выполнить запрос".**</span><span class="sxs-lookup"><span data-stu-id="36f18-146">Click **Run query**.</span></span>
4. <span data-ttu-id="36f18-147">См. ответ от API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="36f18-147">See the response from the Microsoft Graph API.</span></span>

<span data-ttu-id="36f18-148">Чтобы просмотреть ответ в формате, который не  является JSON по умолчанию, выберите вкладку "Задайте заглавные кнопки" в области запросов, определите пару "ключ-значение" и нажмите кнопку **"Добавить".**</span><span class="sxs-lookup"><span data-stu-id="36f18-148">To view the response in a format other than the default JSON, choose the **Request headers** tab in the request pane, define the key/value pair, and click **Add**.</span></span>

![Снимок экрана: вкладка "Заглавные страницы запроса" в проводнике Graph](./images/adding-key-value-pairs.png)

## <a name="next-steps"></a><span data-ttu-id="36f18-150">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="36f18-150">Next steps</span></span>

- <span data-ttu-id="36f18-151">Посетите [обозреватель Graph.](https://developer.microsoft.com/graph/graph-explorer/)</span><span class="sxs-lookup"><span data-stu-id="36f18-151">Visit [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/).</span></span>
- <span data-ttu-id="36f18-152">Узнайте больше о [функциях graph Explorer.](./graph-explorer-features.md)</span><span class="sxs-lookup"><span data-stu-id="36f18-152">Learn more about [Graph Explorer features](./graph-explorer-features.md).</span></span>
- <span data-ttu-id="36f18-153">Участие или предоставление отзывов в [репозитарии GitHub.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose)</span><span class="sxs-lookup"><span data-stu-id="36f18-153">Contribute or provide feedback in the [GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).</span></span>
