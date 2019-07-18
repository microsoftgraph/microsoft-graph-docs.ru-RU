---
title: Управление регистрацией приложения и разрешениями API для уведомлений Microsoft Graph
description: Чтобы получать уведомления, отправляемые через Microsoft Graph, необходимо сначала зарегистрировать свое приложение на портале Microsoft Azure.
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: dc102f451b3f206bbfefe1d3c38c3995041f04fa
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778637"
---
# <a name="manage-app-registration-and-api-permission-for-microsoft-graph-notifications"></a><span data-ttu-id="d19b3-103">Управление регистрацией приложения и разрешениями API для уведомлений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d19b3-103">Manage app registration and API permission for Microsoft Graph notifications</span></span>

<span data-ttu-id="d19b3-104">Чтобы интегрировать в службу приложений уведомления Microsoft Graph, необходимо зарегистрировать свое приложение с помощью платформы удостоверений Майкрософт для поддержки учетных записей Майкрософт, рабочих или учебных учетных записей и объявить обязательные разрешение API.</span><span class="sxs-lookup"><span data-stu-id="d19b3-104">In order for your application service to integrate with Microsoft Graph notifications, you need to register your app with the Microsoft identity platform to support Microsoft accounts or work or school accounts, and declare the API permissions that are required.</span></span>

## <a name="register-your-app-to-support-microsoft-accounts-or-work-or-school-accounts"></a><span data-ttu-id="d19b3-105">Регистрация приложения для поддержки учетных записей Майкрософт, рабочих или учебных учетных записей</span><span class="sxs-lookup"><span data-stu-id="d19b3-105">Register your app to support Microsoft accounts or work or school accounts</span></span>

<span data-ttu-id="d19b3-106">Зарегистрируйте свое приложение на [портале Microsoft Azure](https://portal.azure.com/#home) для поддержки учетных записей Майкрософт, рабочих или учебных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="d19b3-106">Register your application on the [Microsoft Azure portal](https://portal.azure.com/#home) to support Microsoft accounts or work or school accounts.</span></span> <span data-ttu-id="d19b3-107">Если вы уже зарегистрировали свое приложение на [портале приложений Майкрософт](https://apps.dev.microsoft.com/), ваши существующие приложения отобразятся в новом улучшенном интерфейсе портала Azure.</span><span class="sxs-lookup"><span data-stu-id="d19b3-107">If you’ve previously registered your application on the [Microsoft Application Portal](https://apps.dev.microsoft.com/), your existing apps will show up in the new and improved Azure portal experience.</span></span>

<span data-ttu-id="d19b3-108">Сведения о регистрации приложений см. в статье [Регистрация приложения с помощью платформы удостоверений Майкрософт](auth-register-app-v2.md).</span><span class="sxs-lookup"><span data-stu-id="d19b3-108">For information about how to register your apps, see [Register an application with the Microsoft identity platform](auth-register-app-v2.md).</span></span> 


> [!NOTE]
> <span data-ttu-id="d19b3-109">Если у вас еще нет учетной записи Майкрософт и вы хотите ее получить, перейдите на страницу  [учетной записи Майкрософт](https://account.microsoft.com/account).</span><span class="sxs-lookup"><span data-stu-id="d19b3-109">If you don't already have a Microsoft account and would like to use one, go to the [Microsoft account](https://account.microsoft.com/account) page.</span></span> <span data-ttu-id="d19b3-110">Если вы создаете приложение, требующее использования Azure AD версии 1.0 в качестве платформы проверки подлинности и удостоверений для рабочей или учебной учетной записи, см. статью  [Библиотеки проверки подлинности Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span><span class="sxs-lookup"><span data-stu-id="d19b3-110">If you're writing an app that needs to use Azure AD v1.0 as an authentication and identity framework for work or school accounts, see [Azure Active Directory Authentication Libraries](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span></span> <span data-ttu-id="d19b3-111">Если вы хотите ознакомиться с новой единой платформой удостоверений Майкрософт (версия 2.0) или использовать ее, см. [сравнение конечной точки платформы удостоверений Майкрософт и конечной точки Azure AD версии 1.0](https://docs.microsoft.com/ru-RU/azure/active-directory/develop/azure-ad-endpoint-comparison).</span><span class="sxs-lookup"><span data-stu-id="d19b3-111">If you’re interested in learning about or using the new converged Microsoft identity platform (v2.0), see [Comparing the Microsoft identity platform endpoint and Azure AD v1.0 endpoint](https://docs.microsoft.com/en-us/azure/active-directory/develop/azure-ad-endpoint-comparison).</span></span>

<span data-ttu-id="d19b3-112">При регистрации приложения сохраните идентификатор приложения или идентификатор клиента под рукой.</span><span class="sxs-lookup"><span data-stu-id="d19b3-112">When you register your app, keep the application ID/client ID somewhere handy.</span></span> <span data-ttu-id="d19b3-113">Вам потребуется этот идентификатор позднее при регистрации приложения для использования на разных устройствах в [Центре партнеров Майкрософт](https://partner.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="d19b3-113">You'll need this ID later when you register your application for cross-device experiences in the [Microsoft Partner Center](https://partner.microsoft.com/).</span></span>

## <a name="app-certificates-and-secrets"></a><span data-ttu-id="d19b3-114">Сертификаты и секреты приложения</span><span class="sxs-lookup"><span data-stu-id="d19b3-114">App certificates and secrets</span></span>

<span data-ttu-id="d19b3-115">Чтобы разрешить своему приложения самостоятельную идентификацию и проверку подлинности при получении маркеров проверки подлинности, можно отправить собственный сертификат или создать новый секрет клиента, выбрав пункт **Сертификаты и секреты** на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d19b3-115">To enable your application to identify and authenticate itself when obtaining auth tokens, you can either upload your own certificate or create a new client secret by going to **Certificates & secrets** in the Azure portal.</span></span>
    
![Снимок экрана: сертификаты и секреты приложения на портале Azure](images/notifications-app-secrets.png)
    
> [!NOTE]
> <span data-ttu-id="d19b3-117">Если вы выбрали создание нового секрета клиента, обязательно скопируйте и сохраните его в надежном месте.</span><span class="sxs-lookup"><span data-stu-id="d19b3-117">If you opt to generate a new client secret, be sure to copy and keep it in a safe place.</span></span> <span data-ttu-id="d19b3-118">Вы не сможете снова получить к нему доступ после закрытия портала.</span><span class="sxs-lookup"><span data-stu-id="d19b3-118">You won’t be able to access it again after you leave the portal.</span></span>

## <a name="api-permissions"></a><span data-ttu-id="d19b3-119">Разрешения API</span><span class="sxs-lookup"><span data-stu-id="d19b3-119">Web API permissions overview</span></span>

<span data-ttu-id="d19b3-120">Вам потребуется добавить дополнительные разрешения, чтобы использовать уведомления Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d19b3-120">You'll need to add additional permissions in order to use Microsoft Graph notifications.</span></span> <span data-ttu-id="d19b3-121">Нажмите кнопку **Добавить разрешение** и в разделе интерфейсов API Майкрософт выберите **Microsoft Graph**, а затем щелкните вариант **Делегированные разрешения**.</span><span class="sxs-lookup"><span data-stu-id="d19b3-121">Choose **Add a permission**, and under Microsoft APIs, select **Microsoft Graph**, and then select **Delegated permissions**.</span></span>
    
![Снимок экрана: страница "Запрос разрешений API" на портале Azure](images/notifications-api-permissions.png)
    
<span data-ttu-id="d19b3-123">Добавьте указанные ниже разрешения.</span><span class="sxs-lookup"><span data-stu-id="d19b3-123">Add the following permissions:</span></span>

- <span data-ttu-id="d19b3-124">User.Read — разрешает вашему приложению выполнять вход пользователя</span><span class="sxs-lookup"><span data-stu-id="d19b3-124">User.Read - allows your application to sign-in your user</span></span>

- <span data-ttu-id="d19b3-125">Device.Read — разрешает идентификацию списка устройств пользователя</span><span class="sxs-lookup"><span data-stu-id="d19b3-125">Device.Read - allows identification of a user’s list of devices</span></span>

- <span data-ttu-id="d19b3-126">Device.Command — разрешает взаимодействие с устройством пользователя</span><span class="sxs-lookup"><span data-stu-id="d19b3-126">Device.Command - allows communication to a user’s device</span></span>

- <span data-ttu-id="d19b3-127">UserActivity.ReadWrite.CreatedByApp — разрешает подписку приложения на получение уведомлений</span><span class="sxs-lookup"><span data-stu-id="d19b3-127">UserActivity.ReadWrite.CreatedByApp - allows app subscription for notification retrieval</span></span>

- <span data-ttu-id="d19b3-128">Notifications.ReadWrite.CreatedByApp — разрешает доступ к уведомлениям и их доставку</span><span class="sxs-lookup"><span data-stu-id="d19b3-128">Notifications.ReadWrite.CreatedByApp - allows notification access and delivery</span></span>

- <span data-ttu-id="d19b3-129">wns.connect — разрешает подключение к службе уведомлений Windows</span><span class="sxs-lookup"><span data-stu-id="d19b3-129">wns.connect - allows connecting to windows notification service</span></span>

![Снимок экрана: делегированные разрешения для уведомлений на портале Azure](images/notifications-api-permissions-list.png)

## <a name="next-steps"></a><span data-ttu-id="d19b3-131">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="d19b3-131">Next steps</span></span>

<span data-ttu-id="d19b3-132">Узнайте больше о [разрешениях и согласии](https://docs.microsoft.com/ru-RU/azure/active-directory/develop/v2-permissions-and-consent) или просмотрите [справочник по разрешениям](https://docs.microsoft.com/ru-RU/graph/permissions-reference) Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d19b3-132">Learn more about [permissions and consent](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-permissions-and-consent) or view the Microsoft Graph [permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

<span data-ttu-id="d19b3-133">Теперь, после регистрации своего приложения, перейдите в [Центр партнеров](https://partner.microsoft.com/), чтобы настроить приложение для использования на разных устройствах и выбрать соответствующие целевые платформы приложения для получения уведомлений, отправляемых через Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d19b3-133">Now that you’ve registered your app, go to the [Partner Center](https://partner.microsoft.com/) to set up your application for cross-device experiences and to target your corresponding app platforms for notifications sent via Microsoft Graph.</span></span> <span data-ttu-id="d19b3-134">Дополнительные сведения см. в статье [Внедрение использования разных устройств](notifications-integration-cross-device-experiences-onboarding.md).</span><span class="sxs-lookup"><span data-stu-id="d19b3-134">For details, see [Onboarding to cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md).</span></span> 
