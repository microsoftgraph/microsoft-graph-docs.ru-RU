---
title: Поставщик Microsoft Teams
description: Используйте поставщика Teams на вкладке Microsoft Teams, чтобы упростить проверку подлинности и доступ Microsoft Graph ко всем компонентам.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 463fa4afdfd4e0dd3e3cb09ad155f0cae08fb347
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664039"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="3b334-103">Поставщик Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3b334-103">Microsoft Teams provider</span></span>

<span data-ttu-id="3b334-104">Используйте поставщика Teams на вкладке Microsoft Teams, чтобы упростить проверку подлинности и доступ Microsoft Graph ко всем компонентам.</span><span class="sxs-lookup"><span data-stu-id="3b334-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="3b334-105">Дополнительные информацию о поставщиках проверки подлинности см. [в этой теме.](./providers.md)</span><span class="sxs-lookup"><span data-stu-id="3b334-105">To learn more about authentication providers, see [providers](./providers.md).</span></span>

><span data-ttu-id="3b334-106">**Совет:** Дополнительные сведения о том, как начать работу с созданием приложения Microsoft Teams с помощью поставщика Teams, см. в руководстве по началу работы с вкладками ["Создание вКладки Microsoft Teams".](../get-started/build-a-microsoft-teams-tab.md)</span><span class="sxs-lookup"><span data-stu-id="3b334-106">**Tip:** For details about how to get started with creating a Microsoft Teams application with the Teams Provider, see the [Build a Microsoft Teams tab](../get-started/build-a-microsoft-teams-tab.md) getting started guide.</span></span>

## <a name="get-started"></a><span data-ttu-id="3b334-107">Начало работы</span><span class="sxs-lookup"><span data-stu-id="3b334-107">Get started</span></span>

<span data-ttu-id="3b334-108">Перед использованием поставщика Teams необходимо убедиться, что вы ссылались на [microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) на своей странице.</span><span class="sxs-lookup"><span data-stu-id="3b334-108">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) in your page.</span></span>

# <a name="npm"></a>[<span data-ttu-id="3b334-109">npm</span><span class="sxs-lookup"><span data-stu-id="3b334-109">npm</span></span>](#tab/ts)

<span data-ttu-id="3b334-110">Обязательно установите набор средств и microsoft Teams SDK.</span><span class="sxs-lookup"><span data-stu-id="3b334-110">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```cmd
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="3b334-111">Затем импортировать и использовать поставщика.</span><span class="sxs-lookup"><span data-stu-id="3b334-111">Next, import and use the provider.</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="3b334-112">где `config` находится</span><span class="sxs-lookup"><span data-stu-id="3b334-112">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
}
```

# <a name="unpkg"></a>[<span data-ttu-id="3b334-113">unpkg</span><span class="sxs-lookup"><span data-stu-id="3b334-113">unpkg</span></span>](#tab/html)

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

### <a name="mgt-teams-provider-attributes"></a><span data-ttu-id="3b334-114">атрибуты mgt-teams-provider</span><span class="sxs-lookup"><span data-stu-id="3b334-114">mgt-teams-provider attributes</span></span>
| <span data-ttu-id="3b334-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="3b334-115">Attribute</span></span> | <span data-ttu-id="3b334-116">Описание</span><span class="sxs-lookup"><span data-stu-id="3b334-116">Description</span></span> |
| --- | --- |
| <span data-ttu-id="3b334-117">client-id</span><span class="sxs-lookup"><span data-stu-id="3b334-117">client-id</span></span>   | <span data-ttu-id="3b334-118">Строка ИД клиента (см. ["Настройка приложения Teams").](#configure-your-teams-app)</span><span class="sxs-lookup"><span data-stu-id="3b334-118">String client ID (see [Configure your Teams app](#configure-your-teams-app).</span></span> <span data-ttu-id="3b334-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b334-119">Required.</span></span> |
| <span data-ttu-id="3b334-120">auth-popup-url</span><span class="sxs-lookup"><span data-stu-id="3b334-120">auth-popup-url</span></span>  | <span data-ttu-id="3b334-121">Абсолютный или относительный путь к странице, которая будет обрабатывать auth во всплывающее окна (см. страницу создания [всплывающее).](#create-the-popup-page)</span><span class="sxs-lookup"><span data-stu-id="3b334-121">Absolute or relative path to the page that will handle auth in the popup (see [Create the popup page](#create-the-popup-page)).</span></span> <span data-ttu-id="3b334-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b334-122">Required.</span></span> |
| <span data-ttu-id="3b334-123">scopes</span><span class="sxs-lookup"><span data-stu-id="3b334-123">scopes</span></span>  | <span data-ttu-id="3b334-124">Разделенные запятой строки для областей, на которые пользователь должен согласиться при входе.</span><span class="sxs-lookup"><span data-stu-id="3b334-124">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="3b334-125">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="3b334-125">Optional.</span></span> |
| <span data-ttu-id="3b334-126">зависит от</span><span class="sxs-lookup"><span data-stu-id="3b334-126">depends-on</span></span> | <span data-ttu-id="3b334-127">Строка селектора элементов другого компонента поставщика с более высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="3b334-127">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="3b334-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="3b334-128">Optional.</span></span> |
| <span data-ttu-id="3b334-129">authority</span><span class="sxs-lookup"><span data-stu-id="3b334-129">authority</span></span>    | <span data-ttu-id="3b334-130">Строка authority.</span><span class="sxs-lookup"><span data-stu-id="3b334-130">Authority string.</span></span> <span data-ttu-id="3b334-131">По умолчанию используется общий орган.</span><span class="sxs-lookup"><span data-stu-id="3b334-131">The default is the common authority.</span></span> <span data-ttu-id="3b334-132">Для приложений с одним клиентом используйте свой ИД клиента или имя клиента.</span><span class="sxs-lookup"><span data-stu-id="3b334-132">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="3b334-133">Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="3b334-133">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="3b334-134">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="3b334-134">Optional.</span></span> |

---

### <a name="create-the-popup-page"></a><span data-ttu-id="3b334-135">Создание всплываемой страницы</span><span class="sxs-lookup"><span data-stu-id="3b334-135">Create the popup page</span></span>

<span data-ttu-id="3b334-136">Чтобы войти с помощью своих учетных данных Teams, необходимо указать URL-адрес, который приложение Teams откроет во всплывающее приложение, которое будет следовать потоку проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="3b334-136">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="3b334-137">Этот URL-адрес должен быть в вашем домене и вызывать `TeamsProvider.handleAuth();` метод.</span><span class="sxs-lookup"><span data-stu-id="3b334-137">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="3b334-138">Это единственное, что необходимо сделать на этой странице.</span><span class="sxs-lookup"><span data-stu-id="3b334-138">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="3b334-139">Примеры:</span><span class="sxs-lookup"><span data-stu-id="3b334-139">For example:</span></span>

# <a name="npm"></a>[<span data-ttu-id="3b334-140">npm</span><span class="sxs-lookup"><span data-stu-id="3b334-140">npm</span></span>](#tab/ts)

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

# <a name="unpkg"></a>[<span data-ttu-id="3b334-141">unpkg</span><span class="sxs-lookup"><span data-stu-id="3b334-141">unpkg</span></span>](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```
---

### <a name="configure-redirect-uris"></a><span data-ttu-id="3b334-142">Настройка URIS перенаправления</span><span class="sxs-lookup"><span data-stu-id="3b334-142">Configure redirect URIs</span></span>

<span data-ttu-id="3b334-143">После публикации всплываемой страницы на веб-сайте необходимо использовать URL-адрес в `auth-popup-url/authPopupUrl` свойстве.</span><span class="sxs-lookup"><span data-stu-id="3b334-143">After you publish the popup page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="3b334-144">Этот URL-адрес также необходимо настроить в качестве допустимого URI перенаправления в конфигурации приложения на портале Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b334-144">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="3b334-145">Настройка приложения Teams</span><span class="sxs-lookup"><span data-stu-id="3b334-145">Configure your Teams app</span></span>

<span data-ttu-id="3b334-146">Если вы только начинаете работу с приложениями Teams, см. вкладки "Добавление [вкладок в приложения Microsoft Teams".](/microsoftteams/platform/concepts/tabs/tabs-overview)</span><span class="sxs-lookup"><span data-stu-id="3b334-146">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="3b334-147">Вы также можете использовать [App Studio для](/microsoftteams/platform/get-started/get-started-app-studio) быстрой разработки манифеста приложения.</span><span class="sxs-lookup"><span data-stu-id="3b334-147">You can also use [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>
### <a name="creating-an-appclient-id"></a><span data-ttu-id="3b334-148">Создание приложения или ИД клиента</span><span class="sxs-lookup"><span data-stu-id="3b334-148">Creating an app/client ID</span></span>
<span data-ttu-id="3b334-149">Чтобы получить ИД клиента, необходимо зарегистрировать приложение [в](../get-started/add-aad-app-registration.md) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b334-149">In order to get a client ID, you need to [register your application](../get-started/add-aad-app-registration.md) in Azure AD.</span></span> 
><span data-ttu-id="3b334-150">**Примечание.** MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="3b334-150">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="3b334-151">Обязательно включите неявный поток в приложении на портале Azure (по умолчанию он не включен).</span><span class="sxs-lookup"><span data-stu-id="3b334-151">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="3b334-152">В **разделе "Проверка подлинности"** найдите раздел неявного предоставления и выберите для маркеров **доступа** и **маркеров ID** свои почтовые ящики. </span><span class="sxs-lookup"><span data-stu-id="3b334-152">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="see-also"></a><span data-ttu-id="3b334-153">См. также</span><span class="sxs-lookup"><span data-stu-id="3b334-153">See also</span></span>
* [<span data-ttu-id="3b334-154">Пример вкладки Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3b334-154">Microsoft Teams tab sample</span></span>](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [<span data-ttu-id="3b334-155">Создание вкладки Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3b334-155">Build a Microsoft Teams tab</span></span>](../get-started/build-a-microsoft-teams-tab.md)