---
title: Поставщик электронных данных
description: Поставщик MSAL для Electron использует msal-node для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: a9e391f96988f8beaf8395e872a6efa08efca8f5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471436"
---
# <a name="electron-provider"></a><span data-ttu-id="854aa-103">Поставщик электронных данных</span><span class="sxs-lookup"><span data-stu-id="854aa-103">Electron provider</span></span>

<span data-ttu-id="854aa-104">Поставщик Электронный использует [msal-node](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-node) для регистрации пользователей и приобретения маркеров для использования с Microsoft Graph в приложении Electron.</span><span class="sxs-lookup"><span data-stu-id="854aa-104">The Electron provider uses [msal-node](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-node) to sign in users and acquire tokens to use with Microsoft Graph in an Electron application.</span></span>

<span data-ttu-id="854aa-105">Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="854aa-105">To learn more about authentication providers, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="854aa-106">Начало работы</span><span class="sxs-lookup"><span data-stu-id="854aa-106">Get started</span></span>
### <a name="install-the-packages"></a><span data-ttu-id="854aa-107">Установка пакетов</span><span class="sxs-lookup"><span data-stu-id="854aa-107">Install the packages</span></span>

```bash
npm install @microsoft/mgt-element @microsoft/mgt-electron-provider
```
<span data-ttu-id="854aa-108">Необходимо инициализировать ElectronProvider в процессе рендера (передняя часть) и ElectronAuthenticator в основном процессе (задней части).</span><span class="sxs-lookup"><span data-stu-id="854aa-108">You need to initialize ElectronProvider in the renderer process (front end), and ElectronAuthenticator in the main process (back end).</span></span>


### <a name="initializing-electronprovider-in-the-renderer-process-rendererts"></a><span data-ttu-id="854aa-109">Инициализация ElectronProvider в процессе рендера (renderer.ts)</span><span class="sxs-lookup"><span data-stu-id="854aa-109">Initializing ElectronProvider in the renderer process (renderer.ts)</span></span>

<span data-ttu-id="854aa-110">ElectronProvider отвечает за связь с ElectronAuthenticator (в основном процессе) для запроса маркеров доступа и получения сведений о в журнале в состоянии, необходимом для работы компонентов.</span><span class="sxs-lookup"><span data-stu-id="854aa-110">The ElectronProvider is responsible for communicating with ElectronAuthenticator (in the main process) to request access tokens and receive information regarding logged in state that are required for the components to work.</span></span> 

```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-the-main-process-maints"></a><span data-ttu-id="854aa-111">Инициализация ElectronAuthenticator в основном процессе (main.ts)</span><span class="sxs-lookup"><span data-stu-id="854aa-111">Initializing ElectronAuthenticator in the main process (main.ts)</span></span>

<span data-ttu-id="854aa-112">ElectronAuthenticator отвечает за настройку переменных конфигурации для проверки подлинности MSAL, получения маркеров доступа и связи с ElectronProvider.</span><span class="sxs-lookup"><span data-stu-id="854aa-112">The ElectronAuthenticator is responsible for setting up the configuration variables for MSAL authentication, acquiring access tokens, and communicating with ElectronProvider.</span></span>
<span data-ttu-id="854aa-113">Инициализировать электронныйAuthenticator в основном процессе и настроить параметры конфигурации, такие как client-id.</span><span class="sxs-lookup"><span data-stu-id="854aa-113">Initialize the ElectronAuthenticator in the main process and set up the configuration variables such as client-id.</span></span>

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 

let config: MsalElectronConfig = {
  clientId: '<your_client_id>',
  authority: '<your_authority_url>', //optional
  mainWindow: mainWindow, 
  scopes: ['user.read'] //We recommend pre-consenting all the required scopes on the Azure portal
};

ElectronAuthenticator.initialize(config);
```
 
| <span data-ttu-id="854aa-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="854aa-114">Attribute</span></span>    | <span data-ttu-id="854aa-115">Описание</span><span class="sxs-lookup"><span data-stu-id="854aa-115">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="854aa-116">clientId</span><span class="sxs-lookup"><span data-stu-id="854aa-116">clientId</span></span>    | <span data-ttu-id="854aa-117">Строковая ID клиента (см. статью Создание ID приложения/клиента).</span><span class="sxs-lookup"><span data-stu-id="854aa-117">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="854aa-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="854aa-118">Required.</span></span>                                                                                                                                                                                                           |                                                                                                                                                                               |
| <span data-ttu-id="854aa-119">scopes</span><span class="sxs-lookup"><span data-stu-id="854aa-119">scopes</span></span>       | <span data-ttu-id="854aa-120">Разделенные запятой строки для областей, на которые пользователь должен дать согласие при входе.</span><span class="sxs-lookup"><span data-stu-id="854aa-120">Comma-separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="854aa-121">Рекомендуется.</span><span class="sxs-lookup"><span data-stu-id="854aa-121">Recommended.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="854aa-122">authority</span><span class="sxs-lookup"><span data-stu-id="854aa-122">authority</span></span>    | <span data-ttu-id="854aa-123">Строка Authority — по умолчанию является общим органом.</span><span class="sxs-lookup"><span data-stu-id="854aa-123">Authority string - default is the common authority.</span></span> <span data-ttu-id="854aa-124">Для однотенантного приложения используйте идентификатор клиента или имя клиента.</span><span class="sxs-lookup"><span data-stu-id="854aa-124">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="854aa-125">Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`.</span><span class="sxs-lookup"><span data-stu-id="854aa-125">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="854aa-126">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="854aa-126">Optional.</span></span> |                                                                                                                                                                                          |
| <span data-ttu-id="854aa-127">mainWindow</span><span class="sxs-lookup"><span data-stu-id="854aa-127">mainWindow</span></span>  | <span data-ttu-id="854aa-128">Экземпляр основного BrowserWindow, требуемого проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="854aa-128">Instance of the main BrowserWindow that requires authentication.</span></span>|
| <span data-ttu-id="854aa-129">cachePlugin</span><span class="sxs-lookup"><span data-stu-id="854aa-129">cachePlugin</span></span> | <span data-ttu-id="854aa-130">Плагин кэша, который вы хотите использовать для сохраняемого хранения маркеров.</span><span class="sxs-lookup"><span data-stu-id="854aa-130">Cache plugin you would like to use for persistent storage of tokens.</span></span> <span data-ttu-id="854aa-131">См. [расширения проверки подлинности Майкрософт для узла.](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions)</span><span class="sxs-lookup"><span data-stu-id="854aa-131">See [Microsoft Authentication Extensions for Node](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions).</span></span> <span data-ttu-id="854aa-132">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="854aa-132">Optional.</span></span> | 

><span data-ttu-id="854aa-133">**Примечание:** В настоящее время поставщик не поддерживает инкрементную поддержку.</span><span class="sxs-lookup"><span data-stu-id="854aa-133">**Note:** Currently, the provider does not support incremental support.</span></span> <span data-ttu-id="854aa-134">В качестве наилучшей практики обязательно соглашайтесь на все области, которые требуются компонентам.</span><span class="sxs-lookup"><span data-stu-id="854aa-134">As a best practice, be sure to consent to all the scopes that the components require.</span></span>
    
## <a name="create-an-appclient-id"></a><span data-ttu-id="854aa-135">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="854aa-135">Create an app/client ID</span></span>

### <a name="add-new-application-registration-in-azure-active-directory-to-get-a-client-id"></a><span data-ttu-id="854aa-136">Добавьте новую регистрацию приложений в Azure Active Directory, чтобы получить ID клиента</span><span class="sxs-lookup"><span data-stu-id="854aa-136">Add new application registration in Azure Active Directory to get a client ID</span></span>

<span data-ttu-id="854aa-137">Чтобы создать приложение в Azure Active Directory, добавьте новую регистрацию приложений, а затем настройте имя приложения и перенаправляйте URI.</span><span class="sxs-lookup"><span data-stu-id="854aa-137">To create an application in Azure Active Directory, add a new application registration, and then configure an app name and redirect URI.</span></span>

<span data-ttu-id="854aa-138">Создание приложения в Azure Active Directory:</span><span class="sxs-lookup"><span data-stu-id="854aa-138">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="854aa-139">Перейдите на [портал Azure.](https://portal.azure.com)</span><span class="sxs-lookup"><span data-stu-id="854aa-139">Go to the [Azure portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="854aa-140">В меню выберите **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="854aa-140">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="854aa-141">В меню Azure Active Directory выберите **Регистрация приложений**.</span><span class="sxs-lookup"><span data-stu-id="854aa-141">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="854aa-142">В верхнем меню нажмите кнопку **Новая регистрация**.</span><span class="sxs-lookup"><span data-stu-id="854aa-142">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="854aa-143">Введите имя приложения; например, `My Electron-App` .</span><span class="sxs-lookup"><span data-stu-id="854aa-143">Enter the name for your app; for example, `My Electron-App`.</span></span>
1. <span data-ttu-id="854aa-144">Для параметра [Поддерживаемые типы учетных записей](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app) выберите **Учетные записи в любом каталоге организации (любой каталог Azure AD — мультитенантный) и персональные учетные записи Майкрософт (например, Skype, Xbox)**.</span><span class="sxs-lookup"><span data-stu-id="854aa-144">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="854aa-145">В поле **Перенаправление URI** в отсеве выберите общедоступный **клиент/родной (мобильный &** рабочий стол), а в поле URL-адрес введите `msal://redirect` .</span><span class="sxs-lookup"><span data-stu-id="854aa-145">In the **Redirect URI** field, in the dropdown, select **Public client/native (mobile & desktop)**, and in the URL field, enter `msal://redirect`.</span></span>
1. <span data-ttu-id="854aa-146">Подтвердите изменения, нажав кнопку **Зарегистрировать**.</span><span class="sxs-lookup"><span data-stu-id="854aa-146">Confirm changes by selecting the **Register** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="854aa-147">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="854aa-147">Next steps</span></span>

* <span data-ttu-id="854aa-148">Ознакомьтесь с пошаговой инструкцией по [построению электронного приложения.](../get-started/build-an-electron-app.md)</span><span class="sxs-lookup"><span data-stu-id="854aa-148">Check out the step-by-step tutorial for [building an electron app](../get-started/build-an-electron-app.md).</span></span>
* <span data-ttu-id="854aa-149">Взгляните на пример [приложения Electron,](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/electron-app) которое показывает, как использовать поставщика Электронный.</span><span class="sxs-lookup"><span data-stu-id="854aa-149">Take a look at a [sample Electron application](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/electron-app) that shows how to use the Electron provider.</span></span>
