---
title: Настройка прокси приложения с помощью API Microsoft Graph
description: Автоматическая настройка прокси приложения с помощью API Microsoft Graph для предоставления удаленного доступа и единого входа в локальные приложения.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cc99857905a0a308f49ddc41bf22da993ca8f1b4
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873106"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="b08f5-103">Автоматизация настройки прокси-сервера приложений с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b08f5-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="b08f5-104">В этой статье вы узнаете, как создать и настроить [прокси приложения](https://aka.ms/whyappproxy) Azure Active Directory (Azure AD) для приложения.</span><span class="sxs-lookup"><span data-stu-id="b08f5-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](https://aka.ms/whyappproxy) for an application.</span></span> <span data-ttu-id="b08f5-105">Прокси приложения обеспечивает безопасный удаленный доступ и единый вход в локальные веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="b08f5-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="b08f5-106">После настройки прокси приложения для приложения пользователи могут получать доступ к локальным приложениям с помощью внешнего URL-адреса, портала "Мои приложения" или других внутренних порталов приложений.</span><span class="sxs-lookup"><span data-stu-id="b08f5-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="b08f5-107">В этой статье предполагается, что вы уже установили соединитель и выполнили [необходимые условия](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) для прокси приложения, чтобы соединители могли общаться со СЛУЖБАМИ Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b08f5-107">This article assumes you have already installed a connector and completed the [prerequisites](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="b08f5-108">Убедитесь, что у вас есть соответствующие разрешения для вызова следующих API.</span><span class="sxs-lookup"><span data-stu-id="b08f5-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="b08f5-109">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="b08f5-109">Resource type</span></span> |<span data-ttu-id="b08f5-110">Метод</span><span class="sxs-lookup"><span data-stu-id="b08f5-110">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="b08f5-111">applications</span><span class="sxs-lookup"><span data-stu-id="b08f5-111">applications</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="b08f5-112">онпремисеспублишинг</span><span class="sxs-lookup"><span data-stu-id="b08f5-112">onPremisesPublishing</span></span>](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [<span data-ttu-id="b08f5-113">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="b08f5-113">Create application</span></span>](https://docs.microsoft.com/graph/api/application-post-applications?view=graph-rest-beta&tabs=http) <br> [<span data-ttu-id="b08f5-114">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="b08f5-114">Update application</span></span>](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="b08f5-115">Добавление приложения в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="b08f5-115">Add application to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="b08f5-116">PDIF</span><span class="sxs-lookup"><span data-stu-id="b08f5-116">connector</span></span>](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="b08f5-117">Получение соединителей</span><span class="sxs-lookup"><span data-stu-id="b08f5-117">Get connectors</span></span>](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="b08f5-118">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="b08f5-118">connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="b08f5-119">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="b08f5-119">Create connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="b08f5-120">Добавление соединителя для connectorGroup</span><span class="sxs-lookup"><span data-stu-id="b08f5-120">Add connector to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="b08f5-121">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="b08f5-121">servicePrincipals</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="b08f5-122">Создать servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b08f5-122">Create servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals?view=graph-rest-beta&tabs=http) <br> [<span data-ttu-id="b08f5-123">Обновление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b08f5-123">Update servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [<span data-ttu-id="b08f5-124">Создание appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="b08f5-124">Create appRoleAssignments</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> <span data-ttu-id="b08f5-125">В запросах, показанных в этой статье, используются примеры значений.</span><span class="sxs-lookup"><span data-stu-id="b08f5-125">The requests shown in this article use sample values.</span></span> <span data-ttu-id="b08f5-126">Их необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b08f5-126">You will need update these.</span></span> <span data-ttu-id="b08f5-127">Отображаемые объекты ответа также могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b08f5-127">The response objects shown might also be shortened for readability.</span></span> 

## <a name="step-1-create-an-application"></a><span data-ttu-id="b08f5-128">Шаг 1: создание приложения</span><span class="sxs-lookup"><span data-stu-id="b08f5-128">Step 1: Create an application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="b08f5-129">Вход в песочницу Microsoft Graph (рекомендуется), Postman или любой другой используемый клиент API</span><span class="sxs-lookup"><span data-stu-id="b08f5-129">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="b08f5-130">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="b08f5-130">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="b08f5-131">Выберите **Вход в систему с помощью Microsoft** и войдите с помощью глобального администратора Azure AD или учетных данных администратора приложения.</span><span class="sxs-lookup"><span data-stu-id="b08f5-131">Select **Sign-in with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="b08f5-132">После успешного входа вы увидите сведения об учетной записи пользователя в области слева.</span><span class="sxs-lookup"><span data-stu-id="b08f5-132">Upon successful sign in, you'll see the user account details in the left pane.</span></span>

### <a name="create-an-application"></a><span data-ttu-id="b08f5-133">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="b08f5-133">Create an application</span></span>

<span data-ttu-id="b08f5-134">Чтобы настроить прокси приложения для приложения с помощью API, создайте приложение, добавьте субъект-службу в приложение, а затем обновите свойство **онпремисеспублишинг** приложения, чтобы настроить параметры прокси-сервера приложения.</span><span class="sxs-lookup"><span data-stu-id="b08f5-134">To configure Application Proxy for an app using the API, you create an application, add a service principal to the app, and then update the application's **onPremisesPublishing** property to configure the App Proxy settings.</span></span> <span data-ttu-id="b08f5-135">При создании приложения задайте для параметра **сигнинаудиенце** приложения значение "азуреадмйорг".</span><span class="sxs-lookup"><span data-stu-id="b08f5-135">When creating the application, set the application's **signInAudience** to "AzureADMyOrg".</span></span>

#### <a name="request"></a><span data-ttu-id="b08f5-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-136">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b08f5-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="b08f5-137">Response</span></span>

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

### <a name="retrieve-the-application-object-id-and-appid"></a><span data-ttu-id="b08f5-138">Получение идентификатора и appId объекта Application</span><span class="sxs-lookup"><span data-stu-id="b08f5-138">Retrieve the application object ID and appId</span></span>
<span data-ttu-id="b08f5-139">Используйте ответ из предыдущего вызова, чтобы получить и сохранить идентификатор объекта приложения и идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="b08f5-139">Use the response from the previous call to retrieve and save the application object ID and app ID.</span></span>
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a><span data-ttu-id="b08f5-140">Создание servicePrincipal для приложения и добавление обязательных тегов</span><span class="sxs-lookup"><span data-stu-id="b08f5-140">Create a servicePrincipal for the application and add required tags</span></span>
<span data-ttu-id="b08f5-141">Используйте **AppID** , чтобы создать субъекта службы для приложения.</span><span class="sxs-lookup"><span data-stu-id="b08f5-141">Use the **appId** to create a service principal for the application.</span></span> <span data-ttu-id="b08f5-142">Затем добавьте теги, необходимые для настройки прокси приложения для приложения.</span><span class="sxs-lookup"><span data-stu-id="b08f5-142">Then add the tags required for configuring Application Proxy for an app.</span></span>

#### <a name="request"></a><span data-ttu-id="b08f5-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-143">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b08f5-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="b08f5-144">Response</span></span>
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

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="b08f5-145">Шаг 2: Настройка свойств прокси приложения</span><span class="sxs-lookup"><span data-stu-id="b08f5-145">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="b08f5-146">Настройка конфигурации Онпремисеспублишинг</span><span class="sxs-lookup"><span data-stu-id="b08f5-146">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="b08f5-147">С помощью идентификатора объекта Application из предыдущего шага Настройте прокси приложения для приложения и обновите свойство **онпремисеспублишинг** до нужной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="b08f5-147">Use the application object ID from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="b08f5-148">В этом примере используется приложение с внутренним URL-адресом: `https://contosoiwaapp.com` и с использованием домена по умолчанию для внешнего URL-адреса: `https://contosoiwaapp-contoso.msappproxy.net` .</span><span class="sxs-lookup"><span data-stu-id="b08f5-148">In this example, you're using an app with the internal URL: `https://contosoiwaapp.com` and using the default domain for the external URL: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="b08f5-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-149">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b08f5-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="b08f5-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a><span data-ttu-id="b08f5-151">Завершение настройки приложения</span><span class="sxs-lookup"><span data-stu-id="b08f5-151">Complete the configuration of the application</span></span>
<span data-ttu-id="b08f5-152">Обновите свойства **redirectUri**, **идентифиерури**и **хомепажеурл** приложения для внешнего ур, настроенного в свойстве **онпремисеспублишинг** .</span><span class="sxs-lookup"><span data-stu-id="b08f5-152">Update the application's **redirectUri**, **identifierUri**, and **homepageUrl** properties to the external UR configured in the **onPremisesPublishing** property.</span></span> <span data-ttu-id="b08f5-153">Затем обновите [имплиЦитгрантсеттингс](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) до `true` **енабледтокениссуанце** и `false` для **енабледакцесстокениссуанце**.</span><span class="sxs-lookup"><span data-stu-id="b08f5-153">Then update [implicitGrantSettings](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) to `true` for **enabledTokenIssuance** and `false` for **enabledAccessTokenIssuance**.</span></span>

#### <a name="request"></a><span data-ttu-id="b08f5-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-154">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="b08f5-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="b08f5-155">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="b08f5-156">Шаг 3: назначение группы соединителей приложению</span><span class="sxs-lookup"><span data-stu-id="b08f5-156">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="b08f5-157">Получение соединителей</span><span class="sxs-lookup"><span data-stu-id="b08f5-157">Get connectors</span></span>

<span data-ttu-id="b08f5-158">Перечислите соединители и используйте ответ для получения и сохранения идентификатора объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="b08f5-158">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="b08f5-159">Идентификатор объекта Connector будет использоваться для назначения соединителя группе соединителей.</span><span class="sxs-lookup"><span data-stu-id="b08f5-159">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="b08f5-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```

#### <a name="response"></a><span data-ttu-id="b08f5-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="b08f5-161">Response</span></span>

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

### <a name="create-a-connectorgroup"></a><span data-ttu-id="b08f5-162">Создание Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="b08f5-162">Create a connectorGroup</span></span>
<span data-ttu-id="b08f5-163">В этом примере создается новый Коннекторграуп с именем "Ива Demo Connector Group Connector", который используется для приложения.</span><span class="sxs-lookup"><span data-stu-id="b08f5-163">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="b08f5-164">Кроме того, вы можете пропустить этот шаг, если соединитель уже назначен соответствующему Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="b08f5-164">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="b08f5-165">Извлеките и сохраните идентификатор объекта Коннекторграуп, который будет использоваться на следующем шаге.</span><span class="sxs-lookup"><span data-stu-id="b08f5-165">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="b08f5-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-166">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b08f5-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="b08f5-167">Response</span></span>

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

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="b08f5-168">Назначение соединителя для Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="b08f5-168">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="b08f5-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-169">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b08f5-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="b08f5-170">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="b08f5-171">Назначение приложения для Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="b08f5-171">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="b08f5-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-172">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b08f5-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="b08f5-173">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="b08f5-174">Шаг 4: Настройка единого входа</span><span class="sxs-lookup"><span data-stu-id="b08f5-174">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="b08f5-175">Это приложение использует встроенную проверку подлинности Windows (ИВА).</span><span class="sxs-lookup"><span data-stu-id="b08f5-175">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="b08f5-176">Чтобы настроить Ива, установите свойства единого входа в тип ресурса [синглесигнонсеттингс](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="b08f5-176">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>

#### <a name="request"></a><span data-ttu-id="b08f5-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-177">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b08f5-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="b08f5-178">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="b08f5-179">Шаг 5. Назначение пользователей</span><span class="sxs-lookup"><span data-stu-id="b08f5-179">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="b08f5-180">Получение Аппроле для приложения</span><span class="sxs-lookup"><span data-stu-id="b08f5-180">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="b08f5-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-181">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```

#### <a name="response"></a><span data-ttu-id="b08f5-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="b08f5-182">Response</span></span>

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

<span data-ttu-id="b08f5-183">Используйте ответ из предыдущего вызова для получения и сохранения идентификатора Аппроле, который будет использоваться для следующего этапа.</span><span class="sxs-lookup"><span data-stu-id="b08f5-183">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="b08f5-184">Назначение пользователей и групп для приложения</span><span class="sxs-lookup"><span data-stu-id="b08f5-184">Assign users and groups to the application</span></span>

<span data-ttu-id="b08f5-185">Используйте следующие свойства, чтобы назначить пользователя приложению.</span><span class="sxs-lookup"><span data-stu-id="b08f5-185">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="b08f5-186">Свойство</span><span class="sxs-lookup"><span data-stu-id="b08f5-186">Property</span></span>  | <span data-ttu-id="b08f5-187">Описание</span><span class="sxs-lookup"><span data-stu-id="b08f5-187">Description</span></span> |<span data-ttu-id="b08f5-188">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="b08f5-188">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="b08f5-189">principalId</span><span class="sxs-lookup"><span data-stu-id="b08f5-189">principalId</span></span> | <span data-ttu-id="b08f5-190">Идентификатор пользователя, который будет назначен приложению</span><span class="sxs-lookup"><span data-stu-id="b08f5-190">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="b08f5-191">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="b08f5-191">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="b08f5-192">principalType</span><span class="sxs-lookup"><span data-stu-id="b08f5-192">principalType</span></span> | <span data-ttu-id="b08f5-193">Тип пользователя</span><span class="sxs-lookup"><span data-stu-id="b08f5-193">Type of user</span></span> | <span data-ttu-id="b08f5-194">Пользователь</span><span class="sxs-lookup"><span data-stu-id="b08f5-194">User</span></span> |
| <span data-ttu-id="b08f5-195">аппролеид</span><span class="sxs-lookup"><span data-stu-id="b08f5-195">appRoleId</span></span> |  <span data-ttu-id="b08f5-196">Идентификатор роли приложения по умолчанию для приложения</span><span class="sxs-lookup"><span data-stu-id="b08f5-196">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="b08f5-197">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="b08f5-197">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="b08f5-198">resourceId</span><span class="sxs-lookup"><span data-stu-id="b08f5-198">resourceId</span></span> | <span data-ttu-id="b08f5-199">Идентификатор servicePrincipal приложения</span><span class="sxs-lookup"><span data-stu-id="b08f5-199">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="b08f5-200">a8cac399-cde5-4516-a674-819503c61313</span><span class="sxs-lookup"><span data-stu-id="b08f5-200">a8cac399-cde5-4516-a674-819503c61313</span></span> |

#### <a name="request"></a><span data-ttu-id="b08f5-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="b08f5-201">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b08f5-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="b08f5-202">Response</span></span>

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

<span data-ttu-id="b08f5-203">Дополнительные сведения см. в документации по типу ресурса [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="b08f5-203">For more information, see [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>


## <a name="additional-steps"></a><span data-ttu-id="b08f5-204">Дополнительные действия</span><span class="sxs-lookup"><span data-stu-id="b08f5-204">Additional steps</span></span>
- [<span data-ttu-id="b08f5-205">Автоматизация конфигурации с помощью примеров PowerShell для прокси-сервера приложений</span><span class="sxs-lookup"><span data-stu-id="b08f5-205">Automate configuration using PowerShell samples for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="b08f5-206">Автоматизация настройки единого входа на основе SAML для приложений с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b08f5-206">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
