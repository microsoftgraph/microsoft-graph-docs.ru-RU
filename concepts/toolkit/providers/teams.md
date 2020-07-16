---
title: Поставщик Microsoft Teams
description: Используйте поставщика Teams в рамках вкладки Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 62dba210d4fbf7d3540df7fd58d33e275f0065c3
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990257"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="e23ee-103">Поставщик Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e23ee-103">Microsoft Teams provider</span></span>

<span data-ttu-id="e23ee-104">Используйте поставщика Teams в рамках вкладки Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.</span><span class="sxs-lookup"><span data-stu-id="e23ee-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="e23ee-105">Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="e23ee-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="e23ee-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="e23ee-106">Get started</span></span>

<span data-ttu-id="e23ee-107">Перед использованием поставщика Teams необходимо убедиться, что на странице есть ссылка на [пакет SDK Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) .</span><span class="sxs-lookup"><span data-stu-id="e23ee-107">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) in your page.</span></span>

### <a name="via-script-tag"></a><span data-ttu-id="e23ee-108">тег сценария Via</span><span class="sxs-lookup"><span data-stu-id="e23ee-108">via script tag</span></span>
<span data-ttu-id="e23ee-109">В следующем примере используется поставщик в HTML (через CDN).</span><span class="sxs-lookup"><span data-stu-id="e23ee-109">The following example uses the provider in HTML (via CDN).</span></span>

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
  authority=""
></mgt-teams-provider>
```

| <span data-ttu-id="e23ee-110">Атрибут</span><span class="sxs-lookup"><span data-stu-id="e23ee-110">Attribute</span></span> | <span data-ttu-id="e23ee-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e23ee-111">Description</span></span> |
| --- | --- |
| <span data-ttu-id="e23ee-112">Client — ID</span><span class="sxs-lookup"><span data-stu-id="e23ee-112">client-id</span></span>   | <span data-ttu-id="e23ee-113">Строковый идентификатор клиента (см. раздел [Настройка приложения Teams](#configure-your-teams-app)).</span><span class="sxs-lookup"><span data-stu-id="e23ee-113">String client ID (see [Configure your Teams app](#configure-your-teams-app).</span></span> <span data-ttu-id="e23ee-114">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e23ee-114">Required.</span></span> |
| <span data-ttu-id="e23ee-115">auth-контекстное-URL</span><span class="sxs-lookup"><span data-stu-id="e23ee-115">auth-popup-url</span></span>  | <span data-ttu-id="e23ee-116">Абсолютный или относительный путь к странице, которая будет обрабатывать проверку подлинности в всплывающем окне (см. раздел [Создание всплывающей страницы](#create-the-popup-page)).</span><span class="sxs-lookup"><span data-stu-id="e23ee-116">Absolute or relative path to the page that will handle auth in the popup (see [Create the popup page](#create-the-popup-page)).</span></span> <span data-ttu-id="e23ee-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e23ee-117">Required.</span></span> |
| <span data-ttu-id="e23ee-118">scopes</span><span class="sxs-lookup"><span data-stu-id="e23ee-118">scopes</span></span>  | <span data-ttu-id="e23ee-119">Строки, разделенные запятыми, для областей, которые пользователь должен согласиться на вход в систему.</span><span class="sxs-lookup"><span data-stu-id="e23ee-119">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="e23ee-120">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e23ee-120">Optional.</span></span> |
| <span data-ttu-id="e23ee-121">зависит от</span><span class="sxs-lookup"><span data-stu-id="e23ee-121">depends-on</span></span> | <span data-ttu-id="e23ee-122">Строка выбора элемента другого компонента поставщика с более высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="e23ee-122">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="e23ee-123">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e23ee-123">Optional.</span></span> |
| <span data-ttu-id="e23ee-124">авторитет</span><span class="sxs-lookup"><span data-stu-id="e23ee-124">authority</span></span>    | <span data-ttu-id="e23ee-125">Строка Authority.</span><span class="sxs-lookup"><span data-stu-id="e23ee-125">Authority string.</span></span> <span data-ttu-id="e23ee-126">По умолчанию используется общий центр.</span><span class="sxs-lookup"><span data-stu-id="e23ee-126">The default is the common authority.</span></span> <span data-ttu-id="e23ee-127">Для приложений с одним клиентом используйте идентификатор клиента или имя клиента.</span><span class="sxs-lookup"><span data-stu-id="e23ee-127">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="e23ee-128">Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="e23ee-128">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="e23ee-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e23ee-129">Optional.</span></span> |


### <a name="via-npm"></a><span data-ttu-id="e23ee-130">с помощью NPM</span><span class="sxs-lookup"><span data-stu-id="e23ee-130">via NPM</span></span>
<span data-ttu-id="e23ee-131">В следующем примере используется поставщик в JS-модулях (через NPM).</span><span class="sxs-lookup"><span data-stu-id="e23ee-131">The following example uses the provider in JS modules (via NPM).</span></span>

<span data-ttu-id="e23ee-132">Обязательно установите набор средств и пакет SDK Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e23ee-132">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="e23ee-133">После этого импортируйте и используйте поставщика.</span><span class="sxs-lookup"><span data-stu-id="e23ee-133">Next, import and use the provider.</span></span>

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt';
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="e23ee-134">где `config` находится</span><span class="sxs-lookup"><span data-stu-id="e23ee-134">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

<span data-ttu-id="e23ee-135">Кроме того, может потребоваться задать ссылку на библиотеку Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e23ee-135">Alternatively, you might need to set the reference to the Microsoft Teams Library.</span></span> <span data-ttu-id="e23ee-136">Вот пример:</span><span class="sxs-lookup"><span data-stu-id="e23ee-136">Here is an example:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="e23ee-137">Полный пример приведен в [статье пример вкладки Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span><span class="sxs-lookup"><span data-stu-id="e23ee-137">For a complete example, see [Microsoft Teams tab sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="e23ee-138">Настройка приложения Teams</span><span class="sxs-lookup"><span data-stu-id="e23ee-138">Configure your Teams app</span></span>

<span data-ttu-id="e23ee-139">Если вы только начинаете работать с приложениями Teams, ознакомьтесь с разделом [Добавление вкладок в приложения Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview).</span><span class="sxs-lookup"><span data-stu-id="e23ee-139">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="e23ee-140">Кроме того, с помощью [app Studio](/microsoftteams/platform/get-started/get-started-app-studio) можно быстро разработать манифест приложения.</span><span class="sxs-lookup"><span data-stu-id="e23ee-140">You can also use [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>

<span data-ttu-id="e23ee-141">После установки приложения на вкладке и готовности к использованию компонентов необходимо убедиться, что у вашего приложения есть необходимые разрешения для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e23ee-141">After you install your app with a tab, and you're ready to use the components, you need to make sure that your app has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="e23ee-142">Чтобы настроить приложение с необходимыми разрешениями:</span><span class="sxs-lookup"><span data-stu-id="e23ee-142">To configure your app with the necessary permissions:</span></span>

1. [<span data-ttu-id="e23ee-143">Получение имени домена</span><span class="sxs-lookup"><span data-stu-id="e23ee-143">Retrieve your domain name</span></span>](/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [<span data-ttu-id="e23ee-144">Создание регистрации нового приложения</span><span class="sxs-lookup"><span data-stu-id="e23ee-144">Create a new app registration</span></span>](/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [<span data-ttu-id="e23ee-145">Предоставление разрешения на доступ к приложению</span><span class="sxs-lookup"><span data-stu-id="e23ee-145">Grant your application permission</span></span>](/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

<span data-ttu-id="e23ee-146">Важно добавить правое разрешение на **странице Добавление доступа к API**.</span><span class="sxs-lookup"><span data-stu-id="e23ee-146">It's important to add the right permission on the **Add API access page**.</span></span> <span data-ttu-id="e23ee-147">Для добавления и утверждения разрешений необходимо быть администратором в зависимости от того, какой компонент вам необходим.</span><span class="sxs-lookup"><span data-stu-id="e23ee-147">You will need an administrator to add and approve the permissions, depending on which component you need.</span></span>

><span data-ttu-id="e23ee-148">**Совет:** Если вы не знаете, какие разрешения следует добавить, ознакомьтесь с документацией по каждому компоненту.</span><span class="sxs-lookup"><span data-stu-id="e23ee-148">**Tip:** If you're not sure what permissions to add, see the documentation for each component.</span></span>

### <a name="enable-implicit-grant-flow"></a><span data-ttu-id="e23ee-149">Разрешить неявный поток предоставления</span><span class="sxs-lookup"><span data-stu-id="e23ee-149">Enable implicit grant Flow</span></span>

<span data-ttu-id="e23ee-150">Не забудьте включить неявный поток предоставления; Это требование для веб-приложений, запрашивающих маркеры от клиентской стороны.</span><span class="sxs-lookup"><span data-stu-id="e23ee-150">Make sure to enable implicit grant flow; this is a requirement for web apps that request tokens from the client side.</span></span> <span data-ttu-id="e23ee-151">На портале Azure при управлении регистрацией приложений измените манифест и измените `oauth2AllowImplicitFlow` его на `true` .</span><span class="sxs-lookup"><span data-stu-id="e23ee-151">In the Azure Portal, when managing your app registration, edit the manifest and change `oauth2AllowImplicitFlow` to `true`.</span></span>

### <a name="create-the-popup-page"></a><span data-ttu-id="e23ee-152">Создание всплывающей страницы</span><span class="sxs-lookup"><span data-stu-id="e23ee-152">Create the popup page</span></span>

<span data-ttu-id="e23ee-153">Чтобы войти в систему с помощью учетных данных Teams, необходимо предоставить URL-адрес, который приложение Teams будет открывать во всплывающем окне, которое будет проходить процесс проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e23ee-153">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="e23ee-154">Этот URL-адрес должен находиться в вашем домене и должен вызывать `TeamsProvider.handleAuth();` метод.</span><span class="sxs-lookup"><span data-stu-id="e23ee-154">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="e23ee-155">Это единственный элемент, который требуется для выполнения этой страницы.</span><span class="sxs-lookup"><span data-stu-id="e23ee-155">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="e23ee-156">Например:</span><span class="sxs-lookup"><span data-stu-id="e23ee-156">For example:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

<span data-ttu-id="e23ee-157">или через модуль, указанный в всплывающем окне проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="e23ee-157">or via a module referenced in your auth popup page:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

### <a name="configure-redirect-uris"></a><span data-ttu-id="e23ee-158">Настройка URI перенаправления</span><span class="sxs-lookup"><span data-stu-id="e23ee-158">Configure redirect URIs</span></span>

<span data-ttu-id="e23ee-159">После публикации этой страницы на веб-сайте необходимо использовать URL-адрес в `auth-popup-url/authPopupUrl` свойстве.</span><span class="sxs-lookup"><span data-stu-id="e23ee-159">After you publish this page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="e23ee-160">Этот URL-адрес также необходимо настроить в качестве действительного URI перенаправления в конфигурации приложения на портале Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e23ee-160">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>
