---
title: Создание приложения Azure Active Directory
description: Создание регистрации приложения Azure Active Directory для связи с Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 7534d0d15b9ff1b2e1d94fe8d5e8e9e8f771ca91
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659171"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="4ceab-103">Создание приложения Azure Active Directory для использования с Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="4ceab-103">Create an Azure Active Directory app to use with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="4ceab-104">Microsoft Graph — это API, используемый для подключения к Microsoft 365. Он защищен с помощью OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="4ceab-104">Microsoft Graph, the API that you use to connect to Microsoft 365, is secured with OAuth 2.0.</span></span> <span data-ttu-id="4ceab-105">Чтобы подключить приложение к Microsoft 365, вам потребуется создать приложение в Azure Active Directory (Azure AD) и предоставить этому приложению разрешения на доступ к определенным ресурсам от имени пользователя, применяющего ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="4ceab-105">In order to connect your app to Microsoft 365, you will need to create an app in Azure Active Directory (Azure AD) and grant this app permissions to access specific resources on behalf of the person using your app.</span></span> <span data-ttu-id="4ceab-106">В этой статье описано, как зарегистрировать и настроить веб-приложение для использования с Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="4ceab-106">This topic describes how to register and configure a web application to use with Microsoft Graph Toolkit.</span></span>

## <a name="add-new-application-registration-in-azure-active-directory"></a><span data-ttu-id="4ceab-107">Добавление новой регистрации приложения в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4ceab-107">Add new application registration in Azure Active Directory</span></span>

<span data-ttu-id="4ceab-108">Чтобы создать приложение в Azure Active Directory, вам требуется добавить новую регистрацию приложения, а затем настроить имя приложения и URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="4ceab-108">To create an application in Azure Active Directory, you need to add a new application registration, and then configure an app name and URL location.</span></span>

<span data-ttu-id="4ceab-109">Создание приложения в Azure Active Directory:</span><span class="sxs-lookup"><span data-stu-id="4ceab-109">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="4ceab-110">Перейдите на портал Azure по адресу https://portal.azure.com.</span><span class="sxs-lookup"><span data-stu-id="4ceab-110">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="4ceab-111">В меню выберите **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="4ceab-111">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="4ceab-112">В меню Azure Active Directory выберите **Регистрация приложений**.</span><span class="sxs-lookup"><span data-stu-id="4ceab-112">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="4ceab-113">В верхнем меню нажмите кнопку **Новая регистрация**.</span><span class="sxs-lookup"><span data-stu-id="4ceab-113">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="4ceab-114">Введите имя приложения, например `My M365 app`.</span><span class="sxs-lookup"><span data-stu-id="4ceab-114">Enter the name for your app; for exampe, `My M365 app`.</span></span>
1. <span data-ttu-id="4ceab-115">Для параметра [Поддерживаемые типы учетных записей](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app) выберите **Учетные записи в любом каталоге организации (любой каталог Azure AD — мультитенантный) и персональные учетные записи Майкрософт (например, Skype, Xbox)**.</span><span class="sxs-lookup"><span data-stu-id="4ceab-115">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="4ceab-116">В разделе **URI перенаправления** в раскрывающемся списке выберите **Веб**, а в поле URL-адреса введите `http://localhost:3000`.</span><span class="sxs-lookup"><span data-stu-id="4ceab-116">In the **Redirect URI** field, in the dropdown, select **Web**, and in the URL field, enter `http://localhost:3000`.</span></span>
1. <span data-ttu-id="4ceab-117">Подтвердите изменения, нажав кнопку **Зарегистрировать**.</span><span class="sxs-lookup"><span data-stu-id="4ceab-117">Confirm changes by selecting the **Register** button.</span></span>

## <a name="enable-oauth-implicit-flow"></a><span data-ttu-id="4ceab-118">Включение неявного потока OAuth</span><span class="sxs-lookup"><span data-stu-id="4ceab-118">Enable OAuth implicit flow</span></span>

<span data-ttu-id="4ceab-119">В большинстве случаев вы будете использовать Microsoft Graph Toolkit в клиентских приложениях, содержащих только клиентский код.</span><span class="sxs-lookup"><span data-stu-id="4ceab-119">In most cases, you will use Microsoft Graph Toolkit in client-side applications that consist only of client-side code.</span></span> <span data-ttu-id="4ceab-120">Так как клиентские приложения не могут безопасно сохранять секреты, вам потребуется использовать [неявный поток OAuth](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), в котором предполагается удостоверение приложения на основе его идентификатора и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="4ceab-120">Because client-side apps can't store secrets securely, you need to use [OAuth implicit flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), which assumes an app's identity based on its ID and URL.</span></span>

1. <span data-ttu-id="4ceab-121">На портале Azure откройте созданную регистрацию приложения.</span><span class="sxs-lookup"><span data-stu-id="4ceab-121">In the Azure Portal, open your newly created app registration.</span></span>
1. <span data-ttu-id="4ceab-122">В меню выберите **Проверка подлинности**.</span><span class="sxs-lookup"><span data-stu-id="4ceab-122">From the menu, choose **Authentication**.</span></span>
1. <span data-ttu-id="4ceab-123">В разделе **Неявное предоставление разрешения** включите оба параметра: **Токены доступа** и **Токены ИД**</span><span class="sxs-lookup"><span data-stu-id="4ceab-123">In the **Implicit grant** section, enable both **Access tokens** and **ID tokens** options.</span></span>
1. <span data-ttu-id="4ceab-124">Подтвердите изменения, нажав кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="4ceab-124">Confirm your changes by choosing the **Save** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4ceab-125">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="4ceab-125">Next steps</span></span>

- <span data-ttu-id="4ceab-126">[Создание веб-приложения](./build-a-web-app.md) (обычный JavaScript)</span><span class="sxs-lookup"><span data-stu-id="4ceab-126">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="4ceab-127">Создание вкладки Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4ceab-127">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="4ceab-128">Использование набора средств Toolkit с React</span><span class="sxs-lookup"><span data-stu-id="4ceab-128">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="4ceab-129">Использование набора средств Toolkit с Angular</span><span class="sxs-lookup"><span data-stu-id="4ceab-129">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
