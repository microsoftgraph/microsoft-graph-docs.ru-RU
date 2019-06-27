---
title: Поставщик Microsoft Teams
description: Используйте поставщика Teams в рамках вкладки Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 348980225f04adfac4ded6f79a72654fbeec81e7
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243073"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="052af-103">Поставщик Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="052af-103">Microsoft Teams provider</span></span>

<span data-ttu-id="052af-104">Используйте поставщика Teams в рамках вкладки Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.</span><span class="sxs-lookup"><span data-stu-id="052af-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="052af-105">Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="052af-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="052af-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="052af-106">Get started</span></span>

<span data-ttu-id="052af-107">Перед использованием поставщика Teams необходимо убедиться, что на странице есть ссылка на [пакет SDK Microsoft Teams](https://docs.microsoft.com/en-us/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) .</span><span class="sxs-lookup"><span data-stu-id="052af-107">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](https://docs.microsoft.com/en-us/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) in your page.</span></span>

<span data-ttu-id="052af-108">В следующем примере используется поставщик в HTML (через CDN).</span><span class="sxs-lookup"><span data-stu-id="052af-108">The following example uses the provider in HTML (via CDN).</span></span>

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
></mgt-teams-provider>
```

<span data-ttu-id="052af-109">В следующем примере используется поставщик в JS-модулях (через NPM).</span><span class="sxs-lookup"><span data-stu-id="052af-109">The following example uses the provider in JS modules (via NPM).</span></span>

<span data-ttu-id="052af-110">Обязательно установите набор средств и пакет SDK Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="052af-110">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="052af-111">После этого импортируйте и используйте поставщика.</span><span class="sxs-lookup"><span data-stu-id="052af-111">Next, import and use the provider.</span></span>

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt'; 
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="052af-112">где `config` находится</span><span class="sxs-lookup"><span data-stu-id="052af-112">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

<span data-ttu-id="052af-113">Полный пример приведен в [статье пример вкладки Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span><span class="sxs-lookup"><span data-stu-id="052af-113">For a complete example, see [Microsoft Teams tab sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="052af-114">Настройка приложения Teams</span><span class="sxs-lookup"><span data-stu-id="052af-114">Configure your Teams app</span></span>

<span data-ttu-id="052af-115">Если вы только начинаете работать с приложениями Teams, ознакомьтесь с разделом [Добавление вкладок в приложения Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview).</span><span class="sxs-lookup"><span data-stu-id="052af-115">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="052af-116">Кроме того, с помощью [app Studio](https://docs.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-app-studio) можно быстро разработать манифест приложения.</span><span class="sxs-lookup"><span data-stu-id="052af-116">You can also use [App Studio](https://docs.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>

<span data-ttu-id="052af-117">После установки приложения на вкладке и готовности к использованию компонентов необходимо убедиться, что у вашего приложения есть необходимые разрешения для доступа к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="052af-117">After you install your app with a tab, and you're ready to use the components, you need to make sure that your app has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="052af-118">Чтобы настроить приложение с необходимыми разрешениями:</span><span class="sxs-lookup"><span data-stu-id="052af-118">To configure your app with the necessary permissions:</span></span>

1. [<span data-ttu-id="052af-119">Получение имени домена</span><span class="sxs-lookup"><span data-stu-id="052af-119">Retrieve your domain name</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [<span data-ttu-id="052af-120">Создание регистрации нового приложения</span><span class="sxs-lookup"><span data-stu-id="052af-120">Create a new app registration</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [<span data-ttu-id="052af-121">Предоставление разрешения на доступ к приложению</span><span class="sxs-lookup"><span data-stu-id="052af-121">Grant your application permission</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

<span data-ttu-id="052af-122">Важно добавить правое разрешение на **странице Добавление доступа к API**.</span><span class="sxs-lookup"><span data-stu-id="052af-122">It's important to add the right permission on the **Add API access page**.</span></span> <span data-ttu-id="052af-123">Для добавления и утверждения разрешений необходимо быть администратором в зависимости от того, какой компонент вам необходим.</span><span class="sxs-lookup"><span data-stu-id="052af-123">You will need an administrator to add and approve the permissions, depending on which component you need.</span></span>

><span data-ttu-id="052af-124">**Совет:** Если вы не знаете, какие разрешения следует добавить, ознакомьтесь с документацией по каждому компоненту.</span><span class="sxs-lookup"><span data-stu-id="052af-124">**Tip:** If you're not sure what permissions to add, see the documentation for each component.</span></span>

### <a name="enable-implicit-grant-flow"></a><span data-ttu-id="052af-125">Разрешить неявный поток предоставления</span><span class="sxs-lookup"><span data-stu-id="052af-125">Enable implicit grant Flow</span></span>

<span data-ttu-id="052af-126">Не забудьте включить неявный поток предоставления; Это требование для веб-приложений, запрашивающих маркеры от клиентской стороны.</span><span class="sxs-lookup"><span data-stu-id="052af-126">Make sure to enable implicit grant flow; this is a requirement for web apps that request tokens from the client side.</span></span> <span data-ttu-id="052af-127">На портале Azure при управлении регистрацией приложений измените манифест и измените `oauth2AllowImplicitFlow` его на. `true`</span><span class="sxs-lookup"><span data-stu-id="052af-127">In the Azure Portal, when managing your app registration, edit the manifest and change `oauth2AllowImplicitFlow` to `true`.</span></span>

### <a name="create-the-popup-page"></a><span data-ttu-id="052af-128">Создание всплывающей страницы</span><span class="sxs-lookup"><span data-stu-id="052af-128">Create the popup page</span></span>

<span data-ttu-id="052af-129">Чтобы войти в систему с помощью учетных данных Teams, необходимо предоставить URL-адрес, который приложение Teams будет открывать во всплывающем окне, которое будет проходить процесс проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="052af-129">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="052af-130">Этот URL-адрес должен находиться в вашем домене и должен вызывать `TeamsProvider.handleAuth();` метод.</span><span class="sxs-lookup"><span data-stu-id="052af-130">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="052af-131">Это единственный элемент, который требуется для выполнения этой страницы.</span><span class="sxs-lookup"><span data-stu-id="052af-131">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="052af-132">Пример:</span><span class="sxs-lookup"><span data-stu-id="052af-132">For example:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

<script>        
  mgt.TeamsProvider.handleAuth();
</script>
```

### <a name="configure-redirect-uris"></a><span data-ttu-id="052af-133">Настройка URI перенаправления</span><span class="sxs-lookup"><span data-stu-id="052af-133">Configure redirect URIs</span></span>

<span data-ttu-id="052af-134">После публикации этой страницы на веб-сайте необходимо использовать URL-адрес в `auth-popup-url/authPopupUrl` свойстве.</span><span class="sxs-lookup"><span data-stu-id="052af-134">After you publish this page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="052af-135">Этот URL-адрес также необходимо настроить в качестве действительного URI перенаправления в конфигурации приложения на портале Azure AD.</span><span class="sxs-lookup"><span data-stu-id="052af-135">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>
