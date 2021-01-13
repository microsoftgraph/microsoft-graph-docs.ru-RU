---
title: Поставщик Microsoft Teams
description: Используйте поставщика Teams в своей вкладке Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 463fa4afdfd4e0dd3e3cb09ad155f0cae08fb347
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664039"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="eb10c-103">Поставщик Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="eb10c-103">Microsoft Teams provider</span></span>

<span data-ttu-id="eb10c-104">Используйте поставщика Teams в своей вкладке Microsoft Teams для упрощения проверки подлинности и доступа Microsoft Graph ко всем компонентам.</span><span class="sxs-lookup"><span data-stu-id="eb10c-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="eb10c-105">Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="eb10c-105">To learn more about authentication providers, see [providers](./providers.md).</span></span>

><span data-ttu-id="eb10c-106">**Совет**. Сведения о том, как приступить к созданию приложения Microsoft Teams с помощью поставщика Teams, см. в руководстве по началу работы [Создание вкладки Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md).</span><span class="sxs-lookup"><span data-stu-id="eb10c-106">**Tip:** For details about how to get started with creating a Microsoft Teams application with the Teams Provider, see the [Build a Microsoft Teams tab](../get-started/build-a-microsoft-teams-tab.md) getting started guide.</span></span>

## <a name="get-started"></a><span data-ttu-id="eb10c-107">Начало работы</span><span class="sxs-lookup"><span data-stu-id="eb10c-107">Get started</span></span>

<span data-ttu-id="eb10c-108">Перед использованием поставщика Teams вам потребуется указать [SDK Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) на своей странице.</span><span class="sxs-lookup"><span data-stu-id="eb10c-108">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) in your page.</span></span>

# <a name="npm"></a>[<span data-ttu-id="eb10c-109">npm</span><span class="sxs-lookup"><span data-stu-id="eb10c-109">npm</span></span>](#tab/ts)

<span data-ttu-id="eb10c-110">Установите набор средств и пакет SDK Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="eb10c-110">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```cmd
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="eb10c-111">Затем импортируйте и используйте поставщика.</span><span class="sxs-lookup"><span data-stu-id="eb10c-111">Next, import and use the provider.</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="eb10c-112">где `config`:</span><span class="sxs-lookup"><span data-stu-id="eb10c-112">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
}
```

# <a name="unpkg"></a>[<span data-ttu-id="eb10c-113">unpkg</span><span class="sxs-lookup"><span data-stu-id="eb10c-113">unpkg</span></span>](#tab/html)

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/AUTH-PATH"
  scopes="User.Read,People.Read..."
  authority=""
></mgt-teams-provider>
```

### <a name="mgt-teams-provider-attributes"></a><span data-ttu-id="eb10c-114">Атрибуты mgt-teams-provider</span><span class="sxs-lookup"><span data-stu-id="eb10c-114">mgt-teams-provider attributes</span></span>
| <span data-ttu-id="eb10c-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="eb10c-115">Attribute</span></span> | <span data-ttu-id="eb10c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="eb10c-116">Description</span></span> |
| --- | --- |
| <span data-ttu-id="eb10c-117">client-id</span><span class="sxs-lookup"><span data-stu-id="eb10c-117">client-id</span></span>   | <span data-ttu-id="eb10c-118">Строковый идентификатор клиента (см. раздел [Настройка приложения Teams](#configure-your-teams-app)).</span><span class="sxs-lookup"><span data-stu-id="eb10c-118">String client ID (see [Configure your Teams app](#configure-your-teams-app).</span></span> <span data-ttu-id="eb10c-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb10c-119">Required.</span></span> |
| <span data-ttu-id="eb10c-120">auth-popup-url</span><span class="sxs-lookup"><span data-stu-id="eb10c-120">auth-popup-url</span></span>  | <span data-ttu-id="eb10c-121">Абсолютный или относительный путь к странице, обрабатывающей проверку подлинности во всплывающем окне (см. раздел [Создание всплывающей страницы](#create-the-popup-page)).</span><span class="sxs-lookup"><span data-stu-id="eb10c-121">Absolute or relative path to the page that will handle auth in the popup (see [Create the popup page](#create-the-popup-page)).</span></span> <span data-ttu-id="eb10c-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb10c-122">Required.</span></span> |
| <span data-ttu-id="eb10c-123">scopes</span><span class="sxs-lookup"><span data-stu-id="eb10c-123">scopes</span></span>  | <span data-ttu-id="eb10c-124">Строки с разделителями-запятыми для областей, которым пользователь должен предоставить согласие при входе.</span><span class="sxs-lookup"><span data-stu-id="eb10c-124">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="eb10c-125">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="eb10c-125">Optional.</span></span> |
| <span data-ttu-id="eb10c-126">depends-on</span><span class="sxs-lookup"><span data-stu-id="eb10c-126">depends-on</span></span> | <span data-ttu-id="eb10c-127">Строка выбора элементов другого компонента поставщика с более высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="eb10c-127">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="eb10c-128">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="eb10c-128">Optional.</span></span> |
| <span data-ttu-id="eb10c-129">authority</span><span class="sxs-lookup"><span data-stu-id="eb10c-129">authority</span></span>    | <span data-ttu-id="eb10c-130">Строка центра.</span><span class="sxs-lookup"><span data-stu-id="eb10c-130">Authority string.</span></span> <span data-ttu-id="eb10c-131">По умолчанию используется общий центр.</span><span class="sxs-lookup"><span data-stu-id="eb10c-131">The default is the common authority.</span></span> <span data-ttu-id="eb10c-132">Для однотенантного приложения используйте идентификатор клиента или имя клиента.</span><span class="sxs-lookup"><span data-stu-id="eb10c-132">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="eb10c-133">Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`.</span><span class="sxs-lookup"><span data-stu-id="eb10c-133">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="eb10c-134">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="eb10c-134">Optional.</span></span> |

---

### <a name="create-the-popup-page"></a><span data-ttu-id="eb10c-135">Создание всплывающей страницы</span><span class="sxs-lookup"><span data-stu-id="eb10c-135">Create the popup page</span></span>

<span data-ttu-id="eb10c-136">Чтобы войти с использованием своих учетных данных Teams, вам потребуется указать URL-адрес, который будет открываться приложением Teams во всплывающем окне с выполнением потока проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="eb10c-136">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="eb10c-137">Этот URL-адрес должен находиться в вашем домене и должен вызывать метод `TeamsProvider.handleAuth();`.</span><span class="sxs-lookup"><span data-stu-id="eb10c-137">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="eb10c-138">Это единственное действие, которое должно выполняться этой страницей.</span><span class="sxs-lookup"><span data-stu-id="eb10c-138">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="eb10c-139">Например:</span><span class="sxs-lookup"><span data-stu-id="eb10c-139">For example:</span></span>

# <a name="npm"></a>[<span data-ttu-id="eb10c-140">npm</span><span class="sxs-lookup"><span data-stu-id="eb10c-140">npm</span></span>](#tab/ts)

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

# <a name="unpkg"></a>[<span data-ttu-id="eb10c-141">unpkg</span><span class="sxs-lookup"><span data-stu-id="eb10c-141">unpkg</span></span>](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```
---

### <a name="configure-redirect-uris"></a><span data-ttu-id="eb10c-142">Настройка URI перенаправления</span><span class="sxs-lookup"><span data-stu-id="eb10c-142">Configure redirect URIs</span></span>

<span data-ttu-id="eb10c-143">После публикации всплывающей страницы на своем веб-сайте вам требуется использовать URL-адрес в свойстве `auth-popup-url/authPopupUrl`.</span><span class="sxs-lookup"><span data-stu-id="eb10c-143">After you publish the popup page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="eb10c-144">Этот URL-адрес также нужно настроить в качестве допустимого URI перенаправления в конфигурации приложения на портале Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eb10c-144">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="eb10c-145">Настройка приложения Teams</span><span class="sxs-lookup"><span data-stu-id="eb10c-145">Configure your Teams app</span></span>

<span data-ttu-id="eb10c-146">Если вы только приступаете к работе с приложениями Teams, см. раздел [Добавление вкладок в приложения Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview).</span><span class="sxs-lookup"><span data-stu-id="eb10c-146">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="eb10c-147">Для быстрой разработки манифеста приложения также можно использовать [App Studio](/microsoftteams/platform/get-started/get-started-app-studio).</span><span class="sxs-lookup"><span data-stu-id="eb10c-147">You can also use [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>
### <a name="creating-an-appclient-id"></a><span data-ttu-id="eb10c-148">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="eb10c-148">Creating an app/client ID</span></span>
<span data-ttu-id="eb10c-149">Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](../get-started/add-aad-app-registration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eb10c-149">In order to get a client ID, you need to [register your application](../get-started/add-aad-app-registration.md) in Azure AD.</span></span> 
><span data-ttu-id="eb10c-150">**Примечание**. MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="eb10c-150">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="eb10c-151">Включите неявный поток в своем приложении на портале Azure (он не включен по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="eb10c-151">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="eb10c-152">В области **Проверка подлинности** найдите раздел **Неявное предоставление** и установите флажки **Маркеры доступа** и **Маркеры идентификаторов**.</span><span class="sxs-lookup"><span data-stu-id="eb10c-152">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="see-also"></a><span data-ttu-id="eb10c-153">См. также</span><span class="sxs-lookup"><span data-stu-id="eb10c-153">See also</span></span>
* [<span data-ttu-id="eb10c-154">Пример вкладки Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="eb10c-154">Microsoft Teams tab sample</span></span>](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [<span data-ttu-id="eb10c-155">Создание вкладки Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="eb10c-155">Build a Microsoft Teams tab</span></span>](../get-started/build-a-microsoft-teams-tab.md)