---
title: Поставщик Microsoft Teams
description: Используйте поставщика Teams в рамках вкладки Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b102d216b9a9b4181fa070c6c95f543098fa0ba0
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086608"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="e7c3e-103">Поставщик Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e7c3e-103">Microsoft Teams provider</span></span>

<span data-ttu-id="e7c3e-104">Используйте поставщика Teams в рамках вкладки Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="e7c3e-105">Чтобы узнать больше о поставщиках проверки подлинности, ознакомьтесь со статьей [поставщики](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="e7c3e-105">To learn more about authentication providers, see [providers](../providers.md).</span></span>

><span data-ttu-id="e7c3e-106">**Совет:** Сведения о том, как приступить к созданию приложения микросот Teams с помощью поставщика Teams, можно найти в разделе Создание руководства по началу работы с помощью [вкладки Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md) .</span><span class="sxs-lookup"><span data-stu-id="e7c3e-106">**Tip:** For details about how to get started with creating a Microsot Teams application with the Teams Provider, see the [Build a Microsoft Teams tab](../get-started/build-a-microsoft-teams-tab.md) getting started guide.</span></span>

## <a name="get-started"></a><span data-ttu-id="e7c3e-107">Начало работы</span><span class="sxs-lookup"><span data-stu-id="e7c3e-107">Get started</span></span>

<span data-ttu-id="e7c3e-108">Перед использованием поставщика Teams необходимо убедиться, что на странице есть ссылка на [пакет SDK Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) .</span><span class="sxs-lookup"><span data-stu-id="e7c3e-108">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) in your page.</span></span>

### <a name="via-script-tag"></a><span data-ttu-id="e7c3e-109">тег сценария Via</span><span class="sxs-lookup"><span data-stu-id="e7c3e-109">via script tag</span></span>
<span data-ttu-id="e7c3e-110">В следующем примере используется поставщик в HTML (через CDN).</span><span class="sxs-lookup"><span data-stu-id="e7c3e-110">The following example uses the provider in HTML (via CDN).</span></span>

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

| <span data-ttu-id="e7c3e-111">Атрибут</span><span class="sxs-lookup"><span data-stu-id="e7c3e-111">Attribute</span></span> | <span data-ttu-id="e7c3e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e7c3e-112">Description</span></span> |
| --- | --- |
| <span data-ttu-id="e7c3e-113">Client — ID</span><span class="sxs-lookup"><span data-stu-id="e7c3e-113">client-id</span></span>   | <span data-ttu-id="e7c3e-114">Строковый идентификатор клиента (см. раздел [Настройка приложения Teams](#configure-your-teams-app)).</span><span class="sxs-lookup"><span data-stu-id="e7c3e-114">String client ID (see [Configure your Teams app](#configure-your-teams-app).</span></span> <span data-ttu-id="e7c3e-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-115">Required.</span></span> |
| <span data-ttu-id="e7c3e-116">auth-контекстное-URL</span><span class="sxs-lookup"><span data-stu-id="e7c3e-116">auth-popup-url</span></span>  | <span data-ttu-id="e7c3e-117">Абсолютный или относительный путь к странице, которая будет обрабатывать проверку подлинности в всплывающем окне (см. раздел [Создание всплывающей страницы](#create-the-popup-page)).</span><span class="sxs-lookup"><span data-stu-id="e7c3e-117">Absolute or relative path to the page that will handle auth in the popup (see [Create the popup page](#create-the-popup-page)).</span></span> <span data-ttu-id="e7c3e-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-118">Required.</span></span> |
| <span data-ttu-id="e7c3e-119">scopes</span><span class="sxs-lookup"><span data-stu-id="e7c3e-119">scopes</span></span>  | <span data-ttu-id="e7c3e-120">Строки, разделенные запятыми, для областей, которые пользователь должен согласиться на вход в систему.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-120">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="e7c3e-121">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-121">Optional.</span></span> |
| <span data-ttu-id="e7c3e-122">зависит от</span><span class="sxs-lookup"><span data-stu-id="e7c3e-122">depends-on</span></span> | <span data-ttu-id="e7c3e-123">Строка выбора элемента другого компонента поставщика с более высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-123">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="e7c3e-124">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-124">Optional.</span></span> |
| <span data-ttu-id="e7c3e-125">авторитет</span><span class="sxs-lookup"><span data-stu-id="e7c3e-125">authority</span></span>    | <span data-ttu-id="e7c3e-126">Строка Authority.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-126">Authority string.</span></span> <span data-ttu-id="e7c3e-127">По умолчанию используется общий центр.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-127">The default is the common authority.</span></span> <span data-ttu-id="e7c3e-128">Для приложений с одним клиентом используйте идентификатор клиента или имя клиента.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-128">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="e7c3e-129">Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="e7c3e-129">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="e7c3e-130">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-130">Optional.</span></span> |


### <a name="via-npm"></a><span data-ttu-id="e7c3e-131">с помощью NPM</span><span class="sxs-lookup"><span data-stu-id="e7c3e-131">via NPM</span></span>
<span data-ttu-id="e7c3e-132">В следующем примере используется поставщик в JS-модулях (через NPM).</span><span class="sxs-lookup"><span data-stu-id="e7c3e-132">The following example uses the provider in JS modules (via NPM).</span></span>

<span data-ttu-id="e7c3e-133">Обязательно установите набор средств и пакет SDK Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-133">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="e7c3e-134">После этого импортируйте и используйте поставщика.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-134">Next, import and use the provider.</span></span>

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt';
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="e7c3e-135">где `config` находится</span><span class="sxs-lookup"><span data-stu-id="e7c3e-135">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

<span data-ttu-id="e7c3e-136">Кроме того, может потребоваться задать ссылку на библиотеку Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-136">Alternatively, you might need to set the reference to the Microsoft Teams Library.</span></span> <span data-ttu-id="e7c3e-137">Вот пример:</span><span class="sxs-lookup"><span data-stu-id="e7c3e-137">Here is an example:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="e7c3e-138">Полный пример приведен в [статье пример вкладки Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span><span class="sxs-lookup"><span data-stu-id="e7c3e-138">For a complete example, see [Microsoft Teams tab sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="e7c3e-139">Настройка приложения Teams</span><span class="sxs-lookup"><span data-stu-id="e7c3e-139">Configure your Teams app</span></span>

<span data-ttu-id="e7c3e-140">Если вы только начинаете работать с приложениями Teams, ознакомьтесь с разделом [Добавление вкладок в приложения Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview).</span><span class="sxs-lookup"><span data-stu-id="e7c3e-140">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="e7c3e-141">Кроме того, с помощью [app Studio](/microsoftteams/platform/get-started/get-started-app-studio) можно быстро разработать манифест приложения.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-141">You can also use [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>

<span data-ttu-id="e7c3e-142">После установки приложения на вкладке и готовности к использованию компонентов необходимо убедиться, что у вашего приложения есть необходимые разрешения для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-142">After you install your app with a tab, and you're ready to use the components, you need to make sure that your app has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="e7c3e-143">Чтобы настроить приложение с необходимыми разрешениями:</span><span class="sxs-lookup"><span data-stu-id="e7c3e-143">To configure your app with the necessary permissions:</span></span>

1. [<span data-ttu-id="e7c3e-144">Получение имени домена</span><span class="sxs-lookup"><span data-stu-id="e7c3e-144">Retrieve your domain name</span></span>](/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [<span data-ttu-id="e7c3e-145">Создание регистрации нового приложения</span><span class="sxs-lookup"><span data-stu-id="e7c3e-145">Create a new app registration</span></span>](../get-started/add-aad-app-registration.md)
3. [<span data-ttu-id="e7c3e-146">Предоставление разрешения на доступ к приложению</span><span class="sxs-lookup"><span data-stu-id="e7c3e-146">Grant your application permission</span></span>](/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

<span data-ttu-id="e7c3e-147">Важно добавить правое разрешение на **странице Добавление доступа к API**.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-147">It's important to add the right permission on the **Add API access page**.</span></span> <span data-ttu-id="e7c3e-148">Для добавления и утверждения разрешений необходимо быть администратором в зависимости от того, какой компонент вам необходим.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-148">You will need an administrator to add and approve the permissions, depending on which component you need.</span></span>

><span data-ttu-id="e7c3e-149">**Совет:** Если вы не знаете, какие разрешения следует добавить, ознакомьтесь с документацией по каждому компоненту.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-149">**Tip:** If you're not sure what permissions to add, see the documentation for each component.</span></span>

### <a name="enable-implicit-grant-flow"></a><span data-ttu-id="e7c3e-150">Разрешить неявный поток предоставления</span><span class="sxs-lookup"><span data-stu-id="e7c3e-150">Enable implicit grant Flow</span></span>

<span data-ttu-id="e7c3e-151">Не забудьте включить неявный поток предоставления; Это требование для веб-приложений, запрашивающих маркеры от клиентской стороны.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-151">Make sure to enable implicit grant flow; this is a requirement for web apps that request tokens from the client side.</span></span> <span data-ttu-id="e7c3e-152">На портале Azure при управлении регистрацией приложений измените манифест и измените `oauth2AllowImplicitFlow` его на `true` .</span><span class="sxs-lookup"><span data-stu-id="e7c3e-152">In the Azure Portal, when managing your app registration, edit the manifest and change `oauth2AllowImplicitFlow` to `true`.</span></span>

### <a name="create-the-popup-page"></a><span data-ttu-id="e7c3e-153">Создание всплывающей страницы</span><span class="sxs-lookup"><span data-stu-id="e7c3e-153">Create the popup page</span></span>

<span data-ttu-id="e7c3e-154">Чтобы войти в систему с помощью учетных данных Teams, необходимо предоставить URL-адрес, который приложение Teams будет открывать во всплывающем окне, которое будет проходить процесс проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-154">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="e7c3e-155">Этот URL-адрес должен находиться в вашем домене и должен вызывать `TeamsProvider.handleAuth();` метод.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-155">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="e7c3e-156">Это единственный элемент, который требуется для выполнения этой страницы.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-156">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="e7c3e-157">Пример:</span><span class="sxs-lookup"><span data-stu-id="e7c3e-157">For example:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

<span data-ttu-id="e7c3e-158">или через модуль, указанный в всплывающем окне проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="e7c3e-158">or via a module referenced in your auth popup page:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

### <a name="configure-redirect-uris"></a><span data-ttu-id="e7c3e-159">Настройка URI перенаправления</span><span class="sxs-lookup"><span data-stu-id="e7c3e-159">Configure redirect URIs</span></span>

<span data-ttu-id="e7c3e-160">После публикации этой страницы на веб-сайте необходимо использовать URL-адрес в `auth-popup-url/authPopupUrl` свойстве.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-160">After you publish this page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="e7c3e-161">Этот URL-адрес также необходимо настроить в качестве действительного URI перенаправления в конфигурации приложения на портале Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e7c3e-161">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>
