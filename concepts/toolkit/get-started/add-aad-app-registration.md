---
title: Создание приложения Azure Active Directory
description: Создание регистрации приложения Azure Active Directory для связи с Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 13b3a876e80e5c2437eba3d264053cdbbcbb5909
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982327"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="abcf3-103">Создание приложения Azure Active Directory для использования с набором инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="abcf3-103">Create an Azure Active Directory app to use with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="abcf3-104">API Microsoft Graph, который используется для подключения к Microsoft 365, защищен с помощью OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="abcf3-104">Microsoft Graph, the API that you use to connect to Microsoft 365, is secured with OAuth 2.0.</span></span> <span data-ttu-id="abcf3-105">Чтобы подключить приложение к Microsoft 365, вам потребуется создать приложение в Azure Active Directory (Azure AD) и предоставить этому приложению разрешения на доступ к определенным ресурсам от имени пользователя, использующего ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="abcf3-105">In order to connect your app to Microsoft 365, you will need to create an app in Azure Active Directory (Azure AD) and grant this app permissions to access specific resources on behalf of the person using your app.</span></span> <span data-ttu-id="abcf3-106">В этом разделе описывается регистрация и Настройка веб-приложения для использования с набором средств Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="abcf3-106">This topic describes how to register and configure a web application to use with Microsoft Graph Toolkit.</span></span>

## <a name="add-new-application-registration-in-azure-active-directory"></a><span data-ttu-id="abcf3-107">Добавление регистрации нового приложения в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="abcf3-107">Add new application registration in Azure Active Directory</span></span>

<span data-ttu-id="abcf3-108">Чтобы создать приложение в Azure Active Directory, необходимо добавить новую регистрацию приложения, а затем настроить имя приложения и расположение URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="abcf3-108">To create an application in Azure Active Directory, you need to add a new application registration, and then configure an app name and URL location.</span></span>

<span data-ttu-id="abcf3-109">Чтобы создать приложение в Azure Active Directory, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="abcf3-109">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="abcf3-110">Перейдите на портал Azure по адресу https://portal.azure.com .</span><span class="sxs-lookup"><span data-stu-id="abcf3-110">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="abcf3-111">В меню выберите **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="abcf3-111">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="abcf3-112">В меню Azure Active Directory выберите пункт **Регистрация приложений**.</span><span class="sxs-lookup"><span data-stu-id="abcf3-112">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="abcf3-113">В верхнем меню выберите **Новая кнопка регистрации** .</span><span class="sxs-lookup"><span data-stu-id="abcf3-113">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="abcf3-114">Введите имя приложения; для ексампе, `My M365 app` .</span><span class="sxs-lookup"><span data-stu-id="abcf3-114">Enter the name for your app; for exampe, `My M365 app`.</span></span>
1. <span data-ttu-id="abcf3-115">В разделе [Поддерживаемые типы учетных записей](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)выберите **учетные записи в любом организационном каталоге (любой Azure AD Active Directory) и личных учетных записях Майкрософт (например, Skype, Xbox)**.</span><span class="sxs-lookup"><span data-stu-id="abcf3-115">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="abcf3-116">В поле **URI перенаправления** в раскрывающемся списке выберите **веб-сайт** , а в поле URL-адрес введите `https://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="abcf3-116">In the **Redirect URI** field, in the dropdown, select **Web** , and in the URL field, enter `https://localhost:3000`.</span></span>
1. <span data-ttu-id="abcf3-117">Подтвердите изменения, нажав кнопку **Регистрация** .</span><span class="sxs-lookup"><span data-stu-id="abcf3-117">Confirm changes by selecting the **Register** button.</span></span>

## <a name="enable-oauth-implicit-flow"></a><span data-ttu-id="abcf3-118">Включение неявного поток OAuth</span><span class="sxs-lookup"><span data-stu-id="abcf3-118">Enable OAuth implicit flow</span></span>

<span data-ttu-id="abcf3-119">В большинстве случаев набор средств набора инструментов Microsoft Graph будет использоваться в клиентских приложениях, состоящих только из клиентского кода.</span><span class="sxs-lookup"><span data-stu-id="abcf3-119">In most cases, you will use Microsoft Graph Toolkit in client-side applications that consist only of client-side code.</span></span> <span data-ttu-id="abcf3-120">Так как клиентские приложения не могут хранить конфиденциальные данные безопасно, необходимо использовать [неявный поток OAuth](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), который предполагает удостоверение приложения на основе его идентификатора и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="abcf3-120">Because client-side apps can't store secrets securely, you need to use [OAuth implicit flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), which assumes an app's identity based on its ID and URL.</span></span>

1. <span data-ttu-id="abcf3-121">На портале Azure откройте новую регистрацию приложения.</span><span class="sxs-lookup"><span data-stu-id="abcf3-121">In the Azure Portal, open your newly created app registration.</span></span>
1. <span data-ttu-id="abcf3-122">В меню выберите пункт **Проверка подлинности**.</span><span class="sxs-lookup"><span data-stu-id="abcf3-122">From the menu, choose **Authentication**.</span></span>
1. <span data-ttu-id="abcf3-123">В разделе **неявные гранты** включите параметры **маркеров доступа** и **маркеров идентификаторов** .</span><span class="sxs-lookup"><span data-stu-id="abcf3-123">In the **Implicit grant** section, enable both **Access tokens** and **ID tokens** options.</span></span>
1. <span data-ttu-id="abcf3-124">Подтвердите изменения, нажав кнопку **сохранить** .</span><span class="sxs-lookup"><span data-stu-id="abcf3-124">Confirm your changes by choosing the **Save** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="abcf3-125">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="abcf3-125">Next steps</span></span>

- <span data-ttu-id="abcf3-126">[Создание веб-приложения](./build-a-web-app.md) (Ванилла JavaScript)</span><span class="sxs-lookup"><span data-stu-id="abcf3-126">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="abcf3-127">Создание вкладки Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="abcf3-127">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="abcf3-128">Использование набора инструментов с откликом</span><span class="sxs-lookup"><span data-stu-id="abcf3-128">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="abcf3-129">Использование набора инструментов с угловой</span><span class="sxs-lookup"><span data-stu-id="abcf3-129">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
