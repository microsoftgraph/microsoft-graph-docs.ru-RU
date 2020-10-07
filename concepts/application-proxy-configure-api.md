---
title: Настройка прокси приложения с помощью API Microsoft Graph
description: Автоматическая настройка прокси приложения с помощью API Microsoft Graph для предоставления удаленного доступа и единого входа в локальные приложения.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d9ff3e3c6c351768fddd0b4339840a711c864ae
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373345"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="bf6ae-103">Автоматизация настройки прокси приложения с помощью API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="bf6ae-104">В этой статье вы узнаете, как создать и настроить [прокси приложения](https://aka.ms/whyappproxy) Azure Active Directory (Azure AD) для приложения.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](https://aka.ms/whyappproxy) for an application.</span></span> <span data-ttu-id="bf6ae-105">Прокси приложения обеспечивает безопасный удаленный доступ и единый вход в локальные веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="bf6ae-106">После настройки прокси приложения для приложения пользователи могут получать доступ к локальным приложениям с помощью внешнего URL-адреса, портала "Мои приложения" или других внутренних порталов приложений.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="bf6ae-107">В этой статье предполагается, что вы уже установили соединитель и выполнили [необходимые условия](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) для прокси приложения, чтобы соединители могли общаться со СЛУЖБАМИ Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-107">This article assumes you have already installed a connector and completed the [prerequisites](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="bf6ae-108">Убедитесь, что у вас есть соответствующие разрешения для вызова следующих API.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="bf6ae-109">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="bf6ae-109">Resource type</span></span> |<span data-ttu-id="bf6ae-110">Метод</span><span class="sxs-lookup"><span data-stu-id="bf6ae-110">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="bf6ae-111">applications</span><span class="sxs-lookup"><span data-stu-id="bf6ae-111">applications</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="bf6ae-112">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="bf6ae-112">onPremisesPublishing</span></span>](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [<span data-ttu-id="bf6ae-113">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="bf6ae-113">Create application</span></span>](https://docs.microsoft.com/graph/api/application-post-applications?view=graph-rest-beta&tabs=http) <br> [<span data-ttu-id="bf6ae-114">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="bf6ae-114">Update application</span></span>](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="bf6ae-115">Добавление приложения в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="bf6ae-115">Add application to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="bf6ae-116">connector</span><span class="sxs-lookup"><span data-stu-id="bf6ae-116">connector</span></span>](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="bf6ae-117">Получение соединителей</span><span class="sxs-lookup"><span data-stu-id="bf6ae-117">Get connectors</span></span>](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="bf6ae-118">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bf6ae-118">connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="bf6ae-119">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bf6ae-119">Create connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="bf6ae-120">Добавление соединителя для connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bf6ae-120">Add connector to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="bf6ae-121">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="bf6ae-121">servicePrincipals</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="bf6ae-122">Создать servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="bf6ae-122">Create servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals?view=graph-rest-beta&tabs=http) <br> [<span data-ttu-id="bf6ae-123">Обновление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="bf6ae-123">Update servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [<span data-ttu-id="bf6ae-124">Создание appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="bf6ae-124">Create appRoleAssignments</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> <span data-ttu-id="bf6ae-125">В запросах, показанных в этой статье, используются примеры значений.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-125">The requests shown in this article use sample values.</span></span> <span data-ttu-id="bf6ae-126">Их необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-126">You will need update these.</span></span> <span data-ttu-id="bf6ae-127">Отображаемые объекты ответа также могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-127">The response objects shown might also be shortened for readability.</span></span> 

## <a name="step-1-create-an-application"></a><span data-ttu-id="bf6ae-128">Шаг 1: создание приложения</span><span class="sxs-lookup"><span data-stu-id="bf6ae-128">Step 1: Create an application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="bf6ae-129">Вход в песочницу Microsoft Graph (рекомендуется), Postman или любой другой используемый клиент API</span><span class="sxs-lookup"><span data-stu-id="bf6ae-129">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="bf6ae-130">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="bf6ae-130">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="bf6ae-131">Выберите **Вход в систему с помощью Microsoft** и войдите с помощью глобального администратора Azure AD или учетных данных администратора приложения.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-131">Select **Sign-in with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="bf6ae-132">После успешного входа вы увидите сведения об учетной записи пользователя в области слева.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-132">Upon successful sign in, you'll see the user account details in the left pane.</span></span>

### <a name="create-an-application"></a><span data-ttu-id="bf6ae-133">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="bf6ae-133">Create an application</span></span>

<span data-ttu-id="bf6ae-134">Чтобы настроить прокси приложения для приложения с помощью API, создайте приложение, добавьте субъект-службу в приложение, а затем обновите свойство **онпремисеспублишинг** приложения, чтобы настроить параметры прокси-сервера приложения.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-134">To configure Application Proxy for an app using the API, you create an application, add a service principal to the app, and then update the application's **onPremisesPublishing** property to configure the App Proxy settings.</span></span> <span data-ttu-id="bf6ae-135">При создании приложения задайте для параметра **сигнинаудиенце** приложения значение "азуреадмйорг".</span><span class="sxs-lookup"><span data-stu-id="bf6ae-135">When creating the application, set the application's **signInAudience** to "AzureADMyOrg".</span></span>

#### <a name="request"></a><span data-ttu-id="bf6ae-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bf6ae-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf6ae-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applications
Content-type: application/json

{
  "displayName": "Contoso IWA App",
  "signInAudience":"AzureADMyOrg"
}
```
# <a name="c"></a>[<span data-ttu-id="bf6ae-138">C#</span><span class="sxs-lookup"><span data-stu-id="bf6ae-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf6ae-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf6ae-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf6ae-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf6ae-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bf6ae-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "deletedDateTime": null,
  "addIns": [],
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "identifierUris": [],
  "createdDateTime": "2020-08-11T21:07:47.5919755Z",
  "description": null,
  "displayName": "Contoso IWA App",
  "isAuthorizationServiceEnabled": false,
  "isDeviceOnlyAuthSupported": null,
  "isFallbackPublicClient": null,
  "groupMembershipClaims": null,
  "notes": null,
  "optionalClaims": null,
  "orgRestrictions": [],
  "publisherDomain": "f128.info",
  "signInAudience": "AzureADandPersonalMicrosoftAccount",
  "tags": [],
  "tokenEncryptionKeyId": null,
  "uniqueName": null,
  "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
  },
}
```

### <a name="retrieve-the-application-object-id-and-appid"></a><span data-ttu-id="bf6ae-142">Получение идентификатора и appId объекта Application</span><span class="sxs-lookup"><span data-stu-id="bf6ae-142">Retrieve the application object ID and appId</span></span>
<span data-ttu-id="bf6ae-143">Используйте ответ из предыдущего вызова, чтобы получить и сохранить идентификатор объекта приложения и идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-143">Use the response from the previous call to retrieve and save the application object ID and app ID.</span></span>
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a><span data-ttu-id="bf6ae-144">Создание servicePrincipal для приложения и добавление обязательных тегов</span><span class="sxs-lookup"><span data-stu-id="bf6ae-144">Create a servicePrincipal for the application and add required tags</span></span>
<span data-ttu-id="bf6ae-145">Используйте **AppID** , чтобы создать субъекта службы для приложения.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-145">Use the **appId** to create a service principal for the application.</span></span> <span data-ttu-id="bf6ae-146">Затем добавьте теги, необходимые для настройки прокси приложения для приложения.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-146">Then add the tags required for configuring Application Proxy for an app.</span></span>

#### <a name="request"></a><span data-ttu-id="bf6ae-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bf6ae-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf6ae-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_servicePrincipal"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/serviceprincipals
Content-type: appplication/json

{
  "appId":"d7fbfe28-c60e-46d2-8335-841923950d3b",
  "tags": [
    "WindowsAzureActiveDirectoryIntegratedApp",
    "WindowsAzureActiveDirectoryOnPremApp"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="bf6ae-149">C#</span><span class="sxs-lookup"><span data-stu-id="bf6ae-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf6ae-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf6ae-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf6ae-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf6ae-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bf6ae-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals/$entity",
  "id": "a8cac399-cde5-4516-a674-819503c61313",
  "deletedDateTime": null,
  "accountEnabled": true,
  "alternativeNames": [],
  "createdDateTime": null,
  "deviceManagementAppType": null,
  "appDescription": null,
  "appDisplayName": "Contoso IWA App",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "appOwnerOrganizationId": "7918d4b5-0442-4a97-be2d-36f9f9962ece",
  "appRoleAssignmentRequired": false,
  "description": null,
  "displayName": "vtestapi2",
  "errorUrl": null,
  "homepage": null,
  "isAuthorizationServiceEnabled": false,
  "loginUrl": null,
  "logoutUrl": null,
  "notes": null,
  "notificationEmailAddresses": [],
  "preferredSingleSignOnMode": null,
  "preferredTokenSigningKeyEndDateTime": null,
  "preferredTokenSigningKeyThumbprint": null,
  "publisherName": "f/128 Photography",
  "replyUrls": [],
  "samlMetadataUrl": null,
  "samlSingleSignOnSettings": null,
  "servicePrincipalNames": [
      "b92b92d4-3874-46a5-b715-a00ea01cff93"
  ],
  "servicePrincipalType": "Application",
}
```

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="bf6ae-153">Шаг 2: Настройка свойств прокси приложения</span><span class="sxs-lookup"><span data-stu-id="bf6ae-153">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="bf6ae-154">Настройка конфигурации Онпремисеспублишинг</span><span class="sxs-lookup"><span data-stu-id="bf6ae-154">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="bf6ae-155">С помощью идентификатора объекта Application из предыдущего шага Настройте прокси приложения для приложения и обновите свойство **онпремисеспублишинг** до нужной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-155">Use the application object ID from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="bf6ae-156">В этом примере используется приложение с внутренним URL-адресом: `https://contosoiwaapp.com` и с использованием домена по умолчанию для внешнего URL-адреса: `https://contosoiwaapp-contoso.msappproxy.net` .</span><span class="sxs-lookup"><span data-stu-id="bf6ae-156">In this example, you're using an app with the internal URL: `https://contosoiwaapp.com` and using the default domain for the external URL: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="bf6ae-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bf6ae-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf6ae-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
    "onPremisesPublishing": {
        "externalAuthenticationType": "aadPreAuthentication",
        "internalUrl": "https://contosoiwaapp.com",
        "externalUrl": "https://contosoiwaapp-contoso.msappproxy.net"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="bf6ae-159">C#</span><span class="sxs-lookup"><span data-stu-id="bf6ae-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf6ae-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf6ae-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf6ae-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf6ae-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bf6ae-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a><span data-ttu-id="bf6ae-163">Завершение настройки приложения</span><span class="sxs-lookup"><span data-stu-id="bf6ae-163">Complete the configuration of the application</span></span>
<span data-ttu-id="bf6ae-164">Обновите свойства **redirectUri**, **идентифиерури**и **хомепажеурл** приложения для внешнего ур, настроенного в свойстве **онпремисеспублишинг** .</span><span class="sxs-lookup"><span data-stu-id="bf6ae-164">Update the application's **redirectUri**, **identifierUri**, and **homepageUrl** properties to the external UR configured in the **onPremisesPublishing** property.</span></span> <span data-ttu-id="bf6ae-165">Затем обновите [имплиЦитгрантсеттингс](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) до `true` **енабледтокениссуанце** и `false` для **енабледакцесстокениссуанце**.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-165">Then update [implicitGrantSettings](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) to `true` for **enabledTokenIssuance** and `false` for **enabledAccessTokenIssuance**.</span></span>

#### <a name="request"></a><span data-ttu-id="bf6ae-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-166">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
  "identifierUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
  "web": {
    "redirectUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
    "homePageUrl": "https://contosoiwaapp-contoso.msappproxy.net",
    "implicitGrantSettings": {
      "enableIdTokenIssuance": true,
      "enableAccessTokenIssuance": false
    }
  }
}
```

#### <a name="response"></a><span data-ttu-id="bf6ae-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-167">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="bf6ae-168">Шаг 3: назначение группы соединителей приложению</span><span class="sxs-lookup"><span data-stu-id="bf6ae-168">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="bf6ae-169">Получение соединителей</span><span class="sxs-lookup"><span data-stu-id="bf6ae-169">Get connectors</span></span>

<span data-ttu-id="bf6ae-170">Перечислите соединители и используйте ответ для получения и сохранения идентификатора объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-170">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="bf6ae-171">Идентификатор объекта Connector будет использоваться для назначения соединителя группе соединителей.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-171">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="bf6ae-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-172">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bf6ae-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf6ae-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```
# <a name="c"></a>[<span data-ttu-id="bf6ae-174">C#</span><span class="sxs-lookup"><span data-stu-id="bf6ae-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf6ae-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf6ae-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf6ae-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf6ae-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bf6ae-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-177">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectors",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectors",
    "value": [
        {
            "id": "d2b1e8e8-8511-49d6-a4ba-323cb083fbb0",
            "machineName": "connectorA.redmond.contoso.com"",
            "externalIp": "131.137.147.164",
            "status": "active"
        },
        {
            "id": "f2cab422-a1c8-4d70-a47e-2cb297a2e051",
            "machineName": "connectorB.contoso.com"",
            "externalIp": "68.0.191.210",
            "status": "active"
        },
        {
            "id": "8555cc3c-5c8b-48a8-a8b2-5e97c32ef907",
            "machineName": "connectorC.contoso.com",
            "externalIp": "40.78.66.161",
            "status": "active"
        }
    ]
}
```

### <a name="create-a-connectorgroup"></a><span data-ttu-id="bf6ae-178">Создание Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="bf6ae-178">Create a connectorGroup</span></span>
<span data-ttu-id="bf6ae-179">В этом примере создается новый Коннекторграуп с именем "Ива Demo Connector Group Connector", который используется для приложения.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-179">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="bf6ae-180">Кроме того, вы можете пропустить этот шаг, если соединитель уже назначен соответствующему Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-180">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="bf6ae-181">Извлеките и сохраните идентификатор объекта Коннекторграуп, который будет использоваться на следующем шаге.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-181">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="bf6ae-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-182">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups

Content-type: application/json
{
   "name": "IWA Demo Connector Group"
}
```

#### <a name="response"></a><span data-ttu-id="bf6ae-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-183">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 201
Content-type: connectorGroup/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectorGroups/$entity",
    "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
    "name": "IWA Demo Connector Group",
    "connectorGroupType": "applicationProxy",
    "isDefault": false
}
```

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="bf6ae-184">Назначение соединителя для Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="bf6ae-184">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="bf6ae-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-185">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/8555cc3c-5c8b-48a8-a8b2-5e97c32ef907/memberOf/$ref

Content-type: application/json
{
  "@odata.id":"https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a><span data-ttu-id="bf6ae-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-186">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="bf6ae-187">Назначение приложения для Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="bf6ae-187">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="bf6ae-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-188">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bf6ae-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf6ae-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
PUT https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83/connectorGroup/$ref
Content-type: application/json

{
"@odata.id":"https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```
# <a name="c"></a>[<span data-ttu-id="bf6ae-190">C#</span><span class="sxs-lookup"><span data-stu-id="bf6ae-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf6ae-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf6ae-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf6ae-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf6ae-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bf6ae-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-193">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="bf6ae-194">Шаг 4: Настройка единого входа</span><span class="sxs-lookup"><span data-stu-id="bf6ae-194">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="bf6ae-195">Это приложение использует встроенную проверку подлинности Windows (ИВА).</span><span class="sxs-lookup"><span data-stu-id="bf6ae-195">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="bf6ae-196">Чтобы настроить Ива, установите свойства единого входа в тип ресурса [синглесигнонсеттингс](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="bf6ae-196">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>

#### <a name="request"></a><span data-ttu-id="bf6ae-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-197">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
   "onPremisesPublishing": {
      "singleSignOnSettings": {
         "kerberosSignOnSettings": {
            "kerberosServicePrincipalName": "HTTP/iwademo.contoso.com",
        "kerberosSignOnMappingAttributeType": "userPrincipalName"
         },
         "singleSignOnMode": "onPremisesKerberos"
      }
   }
}
```

#### <a name="response"></a><span data-ttu-id="bf6ae-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-198">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="bf6ae-199">Шаг 5. Назначение пользователей</span><span class="sxs-lookup"><span data-stu-id="bf6ae-199">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="bf6ae-200">Получение Аппроле для приложения</span><span class="sxs-lookup"><span data-stu-id="bf6ae-200">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="bf6ae-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-201">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="bf6ae-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf6ae-202">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```
# <a name="c"></a>[<span data-ttu-id="bf6ae-203">C#</span><span class="sxs-lookup"><span data-stu-id="bf6ae-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf6ae-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf6ae-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf6ae-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf6ae-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bf6ae-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-206">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('a8cac399-cde5-4516-a674-819503c61313')/appRoles",
    "value": [
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "msiam_access",
            "displayName": "msiam_access",
            "id": "b9632174-c057-4f7e-951b-be3adc52bfe6",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        }
    ]
}
```

<span data-ttu-id="bf6ae-207">Используйте ответ из предыдущего вызова для получения и сохранения идентификатора Аппроле, который будет использоваться для следующего этапа.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-207">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="bf6ae-208">Назначение пользователей и групп для приложения</span><span class="sxs-lookup"><span data-stu-id="bf6ae-208">Assign users and groups to the application</span></span>

<span data-ttu-id="bf6ae-209">Используйте следующие свойства, чтобы назначить пользователя приложению.</span><span class="sxs-lookup"><span data-stu-id="bf6ae-209">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="bf6ae-210">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf6ae-210">Property</span></span>  | <span data-ttu-id="bf6ae-211">Описание</span><span class="sxs-lookup"><span data-stu-id="bf6ae-211">Description</span></span> |<span data-ttu-id="bf6ae-212">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="bf6ae-212">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="bf6ae-213">principalId</span><span class="sxs-lookup"><span data-stu-id="bf6ae-213">principalId</span></span> | <span data-ttu-id="bf6ae-214">Идентификатор пользователя, который будет назначен приложению</span><span class="sxs-lookup"><span data-stu-id="bf6ae-214">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="bf6ae-215">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="bf6ae-215">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="bf6ae-216">principalType</span><span class="sxs-lookup"><span data-stu-id="bf6ae-216">principalType</span></span> | <span data-ttu-id="bf6ae-217">Тип пользователя</span><span class="sxs-lookup"><span data-stu-id="bf6ae-217">Type of user</span></span> | <span data-ttu-id="bf6ae-218">Пользователь</span><span class="sxs-lookup"><span data-stu-id="bf6ae-218">User</span></span> |
| <span data-ttu-id="bf6ae-219">appRoleId</span><span class="sxs-lookup"><span data-stu-id="bf6ae-219">appRoleId</span></span> |  <span data-ttu-id="bf6ae-220">Идентификатор роли приложения по умолчанию для приложения</span><span class="sxs-lookup"><span data-stu-id="bf6ae-220">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="bf6ae-221">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="bf6ae-221">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="bf6ae-222">resourceId</span><span class="sxs-lookup"><span data-stu-id="bf6ae-222">resourceId</span></span> | <span data-ttu-id="bf6ae-223">Идентификатор servicePrincipal приложения</span><span class="sxs-lookup"><span data-stu-id="bf6ae-223">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="bf6ae-224">a8cac399-cde5-4516-a674-819503c61313</span><span class="sxs-lookup"><span data-stu-id="bf6ae-224">a8cac399-cde5-4516-a674-819503c61313</span></span> |

#### <a name="request"></a><span data-ttu-id="bf6ae-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf6ae-225">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"a8cac399-cde5-4516-a674-819503c61313"
}
```

#### <a name="response"></a><span data-ttu-id="bf6ae-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf6ae-226">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments/$entity",
    "id": "I23pL8ZdNU-CIgQmqMEVyLJ0E6fx0ixEo92az8MnhtU",
    "creationTimestamp": "2020-06-09T00:06:07.5129268Z",
    "appRoleId": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
    "principalDisplayName": "Jean Green",
    "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
    "principalType": "User",
    "resourceDisplayName": "Contoso IWA App",
    "resourceId": "a8cac399-cde5-4516-a674-819503c61313"
}
```

<span data-ttu-id="bf6ae-227">Дополнительные сведения см. в документации по типу ресурса [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="bf6ae-227">For more information, see [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>


## <a name="additional-steps"></a><span data-ttu-id="bf6ae-228">Дополнительные действия</span><span class="sxs-lookup"><span data-stu-id="bf6ae-228">Additional steps</span></span>
- [<span data-ttu-id="bf6ae-229">Автоматизация конфигурации с помощью примеров PowerShell для прокси-сервера приложений</span><span class="sxs-lookup"><span data-stu-id="bf6ae-229">Automate configuration using PowerShell samples for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="bf6ae-230">Автоматизация настройки единого входа на основе SAML для приложений с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bf6ae-230">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
