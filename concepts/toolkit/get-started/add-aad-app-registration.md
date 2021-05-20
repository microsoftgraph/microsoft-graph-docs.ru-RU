---
title: Создание приложения Azure Active Directory
description: Создание регистрации приложения Azure Active Directory для связи с Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: b68281473d884309c23a72979ae07a8a9c752d2f
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579923"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="36a75-103">Создание приложения Azure Active Directory для использования с Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="36a75-103">Create an Azure Active Directory app to use with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="36a75-104">Microsoft Graph — это API, используемый для подключения к Microsoft 365. Он защищен с помощью OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="36a75-104">Microsoft Graph, the API that you use to connect to Microsoft 365, is secured with OAuth 2.0.</span></span> <span data-ttu-id="36a75-105">Чтобы подключить приложение к Microsoft 365, вам потребуется создать приложение в Azure Active Directory (Azure AD) и предоставить этому приложению разрешения на доступ к определенным ресурсам от имени пользователя, применяющего ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="36a75-105">In order to connect your app to Microsoft 365, you will need to create an app in Azure Active Directory (Azure AD) and grant this app permissions to access specific resources on behalf of the person using your app.</span></span> <span data-ttu-id="36a75-106">В этой статье описано, как зарегистрировать и настроить веб-приложение для использования с Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="36a75-106">This topic describes how to register and configure a web application to use with Microsoft Graph Toolkit.</span></span>

## <a name="add-new-application-registration-in-azure-active-directory"></a><span data-ttu-id="36a75-107">Добавление новой регистрации приложения в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="36a75-107">Add new application registration in Azure Active Directory</span></span>

<span data-ttu-id="36a75-108">Чтобы создать приложение в Azure Active Directory, вам требуется добавить новую регистрацию приложения, а затем настроить имя приложения и URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="36a75-108">To create an application in Azure Active Directory, you need to add a new application registration, and then configure an app name and URL location.</span></span>

<span data-ttu-id="36a75-109">Создание приложения в Azure Active Directory:</span><span class="sxs-lookup"><span data-stu-id="36a75-109">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="36a75-110">Перейдите на портал Azure по адресу https://portal.azure.com.</span><span class="sxs-lookup"><span data-stu-id="36a75-110">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="36a75-111">В меню выберите **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="36a75-111">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="36a75-112">В меню Azure Active Directory выберите **Регистрация приложений**.</span><span class="sxs-lookup"><span data-stu-id="36a75-112">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="36a75-113">В верхнем меню нажмите кнопку **Новая регистрация**.</span><span class="sxs-lookup"><span data-stu-id="36a75-113">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="36a75-114">Введите имя приложения; например, `My M365 app` .</span><span class="sxs-lookup"><span data-stu-id="36a75-114">Enter the name for your app; for example, `My M365 app`.</span></span>
1. <span data-ttu-id="36a75-115">Для параметра [Поддерживаемые типы учетных записей](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app) выберите **Учетные записи в любом каталоге организации (любой каталог Azure AD — мультитенантный) и персональные учетные записи Майкрософт (например, Skype, Xbox)**.</span><span class="sxs-lookup"><span data-stu-id="36a75-115">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="36a75-116">В поле **Перенаправление URI** в отсеве выберите приложение для одной страницы **(SPA)** и в поле URL-адрес введите `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="36a75-116">In the **Redirect URI** field, in the dropdown, select **Single Page Application (SPA)**, and in the URL field, enter `http://localhost:3000`.</span></span> <span data-ttu-id="36a75-117">Примечание. Если вы используете поставщика MSAL, а не поставщика MSAL 2.0, вам потребуется выбрать **Веб** вместо **SPA.**</span><span class="sxs-lookup"><span data-stu-id="36a75-117">Note: if you are using MSAL Provider and not MSAL 2.0 Provider, you will need to select **Web** instead of **SPA**.</span></span>
1. <span data-ttu-id="36a75-118">Подтвердите изменения, нажав кнопку **Зарегистрировать**.</span><span class="sxs-lookup"><span data-stu-id="36a75-118">Confirm changes by selecting the **Register** button.</span></span>

## <a name="enable-oauth-implicit-flow-only-for-msal-10-provider"></a><span data-ttu-id="36a75-119">Включить неявный поток OAuth (только для поставщика MSAL 1.0)</span><span class="sxs-lookup"><span data-stu-id="36a75-119">Enable OAuth implicit flow (only for MSAL 1.0 provider)</span></span>

<span data-ttu-id="36a75-120">В большинстве случаев вы будете использовать Microsoft Graph Toolkit в клиентских приложениях, содержащих только клиентский код.</span><span class="sxs-lookup"><span data-stu-id="36a75-120">In most cases, you will use Microsoft Graph Toolkit in client-side applications that consist only of client-side code.</span></span> <span data-ttu-id="36a75-121">Так как клиентские приложения не могут безопасно сохранять секреты, вам потребуется использовать [неявный поток OAuth](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), в котором предполагается удостоверение приложения на основе его идентификатора и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="36a75-121">Because client-side apps can't store secrets securely, you need to use [OAuth implicit flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), which assumes an app's identity based on its ID and URL.</span></span>

1. <span data-ttu-id="36a75-122">На портале Azure откройте созданную регистрацию приложения.</span><span class="sxs-lookup"><span data-stu-id="36a75-122">In the Azure Portal, open your newly created app registration.</span></span>
1. <span data-ttu-id="36a75-123">В меню выберите **Проверка подлинности**.</span><span class="sxs-lookup"><span data-stu-id="36a75-123">From the menu, choose **Authentication**.</span></span>
1. <span data-ttu-id="36a75-124">В разделе **Неявное предоставление разрешения** включите оба параметра: **Токены доступа** и **Токены ИД**</span><span class="sxs-lookup"><span data-stu-id="36a75-124">In the **Implicit grant** section, enable both **Access tokens** and **ID tokens** options.</span></span>
1. <span data-ttu-id="36a75-125">Подтвердите изменения, нажав кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="36a75-125">Confirm your changes by choosing the **Save** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="36a75-126">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="36a75-126">Next steps</span></span>

- <span data-ttu-id="36a75-127">[Создание веб-приложения](./build-a-web-app.md) (обычный JavaScript)</span><span class="sxs-lookup"><span data-stu-id="36a75-127">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="36a75-128">Создание вкладки Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="36a75-128">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="36a75-129">Использование набора средств Toolkit с React</span><span class="sxs-lookup"><span data-stu-id="36a75-129">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="36a75-130">Использование набора средств Toolkit с Angular</span><span class="sxs-lookup"><span data-stu-id="36a75-130">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
