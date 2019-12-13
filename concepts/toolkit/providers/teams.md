---
title: Поставщик Microsoft Teams
description: Используйте поставщика Teams в рамках вкладки Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 335673ba2faa04916c2f8548999077a68202bbf0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955759"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="69f58-103">Поставщик Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="69f58-103">Microsoft Teams provider</span></span>

<span data-ttu-id="69f58-104">Используйте поставщика Teams в рамках вкладки Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.</span><span class="sxs-lookup"><span data-stu-id="69f58-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="69f58-105">Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="69f58-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="69f58-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="69f58-106">Get started</span></span>

<span data-ttu-id="69f58-107">Перед использованием поставщика Teams необходимо убедиться, что на странице есть ссылка на [пакет SDK Microsoft Teams](https://docs.microsoft.com/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) .</span><span class="sxs-lookup"><span data-stu-id="69f58-107">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](https://docs.microsoft.com/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) in your page.</span></span>

### <a name="via-script-tag"></a><span data-ttu-id="69f58-108">тег сценария Via</span><span class="sxs-lookup"><span data-stu-id="69f58-108">via script tag</span></span>
<span data-ttu-id="69f58-109">В следующем примере используется поставщик в HTML (через CDN).</span><span class="sxs-lookup"><span data-stu-id="69f58-109">The following example uses the provider in HTML (via CDN).</span></span>

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
></mgt-teams-provider>
```

| <span data-ttu-id="69f58-110">Атрибут</span><span class="sxs-lookup"><span data-stu-id="69f58-110">Attribute</span></span> | <span data-ttu-id="69f58-111">Описание</span><span class="sxs-lookup"><span data-stu-id="69f58-111">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="69f58-112">Client — ID</span><span class="sxs-lookup"><span data-stu-id="69f58-112">client-id</span></span>   | <span data-ttu-id="69f58-113">Идентификатор строкового клиента (см. Настройка приложения Teams).</span><span class="sxs-lookup"><span data-stu-id="69f58-113">String client ID (see Configure your Teams app).</span></span> <span data-ttu-id="69f58-114">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="69f58-114">Required.</span></span> |
| <span data-ttu-id="69f58-115">auth-контекстное-URL</span><span class="sxs-lookup"><span data-stu-id="69f58-115">auth-popup-url</span></span>  | <span data-ttu-id="69f58-116">Абсолютный или относительный путь к странице, которая будет обрабатывать проверку подлинности в всплывающем окне (см. раздел Создание всплывающей страницы).</span><span class="sxs-lookup"><span data-stu-id="69f58-116">Absolute or relative path to the page that will handle auth in the popup (see Create the popup page).</span></span> <span data-ttu-id="69f58-117">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="69f58-117">Required.</span></span> |
| <span data-ttu-id="69f58-118">scopes</span><span class="sxs-lookup"><span data-stu-id="69f58-118">scopes</span></span>  | <span data-ttu-id="69f58-119">Строки, разделенные запятыми, для областей, которые пользователь должен согласиться на вход в систему.</span><span class="sxs-lookup"><span data-stu-id="69f58-119">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="69f58-120">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="69f58-120">Optional.</span></span> |
| <span data-ttu-id="69f58-121">зависит от</span><span class="sxs-lookup"><span data-stu-id="69f58-121">depends-on</span></span> | <span data-ttu-id="69f58-122">Строка выбора элемента другого компонента поставщика с более высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="69f58-122">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="69f58-123">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="69f58-123">Optional.</span></span> |

### <a name="via-npm"></a><span data-ttu-id="69f58-124">с помощью NPM</span><span class="sxs-lookup"><span data-stu-id="69f58-124">via NPM</span></span> 
<span data-ttu-id="69f58-125">В следующем примере используется поставщик в JS-модулях (через NPM).</span><span class="sxs-lookup"><span data-stu-id="69f58-125">The following example uses the provider in JS modules (via NPM).</span></span>

<span data-ttu-id="69f58-126">Обязательно установите набор средств и пакет SDK Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="69f58-126">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="69f58-127">После этого импортируйте и используйте поставщика.</span><span class="sxs-lookup"><span data-stu-id="69f58-127">Next, import and use the provider.</span></span>

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt'; 
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="69f58-128">где `config` находится</span><span class="sxs-lookup"><span data-stu-id="69f58-128">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

<span data-ttu-id="69f58-129">Кроме того, может потребоваться задать ссылку на библиотеку Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="69f58-129">Alternatively, you might need to set the reference to the Microsoft Teams Library.</span></span> <span data-ttu-id="69f58-130">Вот пример:</span><span class="sxs-lookup"><span data-stu-id="69f58-130">Here is an example:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt'; 

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="69f58-131">Полный пример приведен в [статье пример вкладки Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span><span class="sxs-lookup"><span data-stu-id="69f58-131">For a complete example, see [Microsoft Teams tab sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="69f58-132">Настройка приложения Teams</span><span class="sxs-lookup"><span data-stu-id="69f58-132">Configure your Teams app</span></span>

<span data-ttu-id="69f58-133">Если вы только начинаете работать с приложениями Teams, ознакомьтесь с разделом [Добавление вкладок в приложения Microsoft Teams](https://docs.microsoft.com/microsoftteams/platform/concepts/tabs/tabs-overview).</span><span class="sxs-lookup"><span data-stu-id="69f58-133">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](https://docs.microsoft.com/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="69f58-134">Кроме того, с помощью [app Studio](https://docs.microsoft.com/microsoftteams/platform/get-started/get-started-app-studio) можно быстро разработать манифест приложения.</span><span class="sxs-lookup"><span data-stu-id="69f58-134">You can also use [App Studio](https://docs.microsoft.com/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>

<span data-ttu-id="69f58-135">После установки приложения на вкладке и готовности к использованию компонентов необходимо убедиться, что у вашего приложения есть необходимые разрешения для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="69f58-135">After you install your app with a tab, and you're ready to use the components, you need to make sure that your app has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="69f58-136">Чтобы настроить приложение с необходимыми разрешениями:</span><span class="sxs-lookup"><span data-stu-id="69f58-136">To configure your app with the necessary permissions:</span></span>

1. [<span data-ttu-id="69f58-137">Получение имени домена</span><span class="sxs-lookup"><span data-stu-id="69f58-137">Retrieve your domain name</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [<span data-ttu-id="69f58-138">Создание регистрации нового приложения</span><span class="sxs-lookup"><span data-stu-id="69f58-138">Create a new app registration</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [<span data-ttu-id="69f58-139">Предоставление разрешения на доступ к приложению</span><span class="sxs-lookup"><span data-stu-id="69f58-139">Grant your application permission</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

<span data-ttu-id="69f58-140">Важно добавить правое разрешение на **странице Добавление доступа к API**.</span><span class="sxs-lookup"><span data-stu-id="69f58-140">It's important to add the right permission on the **Add API access page**.</span></span> <span data-ttu-id="69f58-141">Для добавления и утверждения разрешений необходимо быть администратором в зависимости от того, какой компонент вам необходим.</span><span class="sxs-lookup"><span data-stu-id="69f58-141">You will need an administrator to add and approve the permissions, depending on which component you need.</span></span>

><span data-ttu-id="69f58-142">**Совет:** Если вы не знаете, какие разрешения следует добавить, ознакомьтесь с документацией по каждому компоненту.</span><span class="sxs-lookup"><span data-stu-id="69f58-142">**Tip:** If you're not sure what permissions to add, see the documentation for each component.</span></span>

### <a name="enable-implicit-grant-flow"></a><span data-ttu-id="69f58-143">Разрешить неявный поток предоставления</span><span class="sxs-lookup"><span data-stu-id="69f58-143">Enable implicit grant Flow</span></span>

<span data-ttu-id="69f58-144">Не забудьте включить неявный поток предоставления; Это требование для веб-приложений, запрашивающих маркеры от клиентской стороны.</span><span class="sxs-lookup"><span data-stu-id="69f58-144">Make sure to enable implicit grant flow; this is a requirement for web apps that request tokens from the client side.</span></span> <span data-ttu-id="69f58-145">На портале Azure при управлении регистрацией приложений измените манифест и измените `oauth2AllowImplicitFlow` его на. `true`</span><span class="sxs-lookup"><span data-stu-id="69f58-145">In the Azure Portal, when managing your app registration, edit the manifest and change `oauth2AllowImplicitFlow` to `true`.</span></span>

### <a name="create-the-popup-page"></a><span data-ttu-id="69f58-146">Создание всплывающей страницы</span><span class="sxs-lookup"><span data-stu-id="69f58-146">Create the popup page</span></span>

<span data-ttu-id="69f58-147">Чтобы войти в систему с помощью учетных данных Teams, необходимо предоставить URL-адрес, который приложение Teams будет открывать во всплывающем окне, которое будет проходить процесс проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="69f58-147">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="69f58-148">Этот URL-адрес должен находиться в вашем домене и должен вызывать `TeamsProvider.handleAuth();` метод.</span><span class="sxs-lookup"><span data-stu-id="69f58-148">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="69f58-149">Это единственный элемент, который требуется для выполнения этой страницы.</span><span class="sxs-lookup"><span data-stu-id="69f58-149">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="69f58-150">Пример:</span><span class="sxs-lookup"><span data-stu-id="69f58-150">For example:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

<script>        
  mgt.TeamsProvider.handleAuth();
</script>
```

<span data-ttu-id="69f58-151">или через модуль, указанный в всплывающем окне проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="69f58-151">or via a module referenced in your auth popup page:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt'; 

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

### <a name="configure-redirect-uris"></a><span data-ttu-id="69f58-152">Настройка URI перенаправления</span><span class="sxs-lookup"><span data-stu-id="69f58-152">Configure redirect URIs</span></span>

<span data-ttu-id="69f58-153">После публикации этой страницы на веб-сайте необходимо использовать URL-адрес в `auth-popup-url/authPopupUrl` свойстве.</span><span class="sxs-lookup"><span data-stu-id="69f58-153">After you publish this page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="69f58-154">Этот URL-адрес также необходимо настроить в качестве действительного URI перенаправления в конфигурации приложения на портале Azure AD.</span><span class="sxs-lookup"><span data-stu-id="69f58-154">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>
