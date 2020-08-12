---
title: Настройка прокси приложения с помощью API Microsoft Graph
description: Автоматическая настройка прокси приложения с помощью API Microsoft Graph для предоставления удаленного доступа и единого входа в локальные приложения.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d7b60e19cb0d3b1c6b015c47ddac604f4ebb2d55
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/12/2020
ms.locfileid: "46644004"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="cab6b-103">Автоматизация настройки прокси-сервера приложений с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cab6b-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="cab6b-104">В этой статье вы узнаете, как создать и настроить [прокси приложения](https://aka.ms/whyappproxy) Azure Active Directory (Azure AD) для приложения.</span><span class="sxs-lookup"><span data-stu-id="cab6b-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](https://aka.ms/whyappproxy) for an application.</span></span> <span data-ttu-id="cab6b-105">Прокси приложения обеспечивает безопасный удаленный доступ и единый вход в локальные веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="cab6b-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="cab6b-106">После настройки прокси приложения для приложения пользователи могут получать доступ к локальным приложениям с помощью внешнего URL-адреса, портала "Мои приложения" или других внутренних порталов приложений.</span><span class="sxs-lookup"><span data-stu-id="cab6b-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="cab6b-107">В этой статье предполагается, что вы уже установили соединитель и выполнили [необходимые условия](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) для прокси приложения, чтобы соединители могли общаться со СЛУЖБАМИ Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cab6b-107">This article assumes you have already installed a connector and completed the [prerequisites](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="cab6b-108">Убедитесь, что у вас есть соответствующие разрешения для вызова следующих API.</span><span class="sxs-lookup"><span data-stu-id="cab6b-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="cab6b-109">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="cab6b-109">Resource type</span></span> |<span data-ttu-id="cab6b-110">Метод</span><span class="sxs-lookup"><span data-stu-id="cab6b-110">Method</span></span> |
|---------|---------|
| [<span data-ttu-id="cab6b-111">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cab6b-111">applicationTemplate</span></span>](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta)| [<span data-ttu-id="cab6b-112">Создание экземпляра applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cab6b-112">Instantiate applicationTemplate</span></span>](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) |
|[<span data-ttu-id="cab6b-113">applications</span><span class="sxs-lookup"><span data-stu-id="cab6b-113">applications</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="cab6b-114">онпремисеспублишинг</span><span class="sxs-lookup"><span data-stu-id="cab6b-114">onPremisesPublishing</span></span>](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)|[<span data-ttu-id="cab6b-115">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="cab6b-115">Update application</span></span>](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="cab6b-116">Добавление приложения в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="cab6b-116">Add application to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="cab6b-117">PDIF</span><span class="sxs-lookup"><span data-stu-id="cab6b-117">connector</span></span>](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="cab6b-118">Получение соединителей</span><span class="sxs-lookup"><span data-stu-id="cab6b-118">Get connectors</span></span>](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="cab6b-119">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="cab6b-119">connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="cab6b-120">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="cab6b-120">Create connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="cab6b-121">Добавление соединителя для connectorGroup</span><span class="sxs-lookup"><span data-stu-id="cab6b-121">Add connector to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="cab6b-122">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="cab6b-122">servicePrincipals</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="cab6b-123">Обновление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="cab6b-123">Update servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [<span data-ttu-id="cab6b-124">Создание appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="cab6b-124">Create appRoleAssignments</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

>[!NOTE]
> <span data-ttu-id="cab6b-125">В запросах, показанных в этой статье, используются примеры значений.</span><span class="sxs-lookup"><span data-stu-id="cab6b-125">The requests shown in this article uses sample values.</span></span> <span data-ttu-id="cab6b-126">Их необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="cab6b-126">You will need update these.</span></span> <span data-ttu-id="cab6b-127">Отображаемые объекты ответа также могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cab6b-127">The response objects shown may also be shortened for readability.</span></span> <span data-ttu-id="cab6b-128">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cab6b-128">All the properties will be returned from an actual call.</span></span>

## <a name="step-1-create-a-custom-application"></a><span data-ttu-id="cab6b-129">Шаг 1: Создание настраиваемого приложения</span><span class="sxs-lookup"><span data-stu-id="cab6b-129">Step 1: Create a custom application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="cab6b-130">Вход в песочницу Microsoft Graph (рекомендуется), Postman или любой другой используемый клиент API</span><span class="sxs-lookup"><span data-stu-id="cab6b-130">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="cab6b-131">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="cab6b-131">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="cab6b-132">Выберите вариант **Вход с помощью учетной записи Майкрософт** и войдите, используя учетные данные глобального администратора Azure AD или администратора приложения.</span><span class="sxs-lookup"><span data-stu-id="cab6b-132">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="cab6b-133">После успешного входа вы увидите сведения об учетной записи пользователя в области слева.</span><span class="sxs-lookup"><span data-stu-id="cab6b-133">Upon successful sign-in, you'll see the user account details in the left pane.</span></span>

### <a name="create-a-custom-application"></a><span data-ttu-id="cab6b-134">Создание пользовательского приложения</span><span class="sxs-lookup"><span data-stu-id="cab6b-134">Create a custom application</span></span>

<span data-ttu-id="cab6b-135">Чтобы настроить прокси приложения для приложения с помощью API, необходимо сначала создать пользовательское приложение, а затем обновить свойство **онпремисеспублишинг** приложения, чтобы настроить параметры прокси-сервера приложения.</span><span class="sxs-lookup"><span data-stu-id="cab6b-135">To configure Application Proxy for an app using the API, you must first create a custom application, then update the application's **onPremisesPublishing** property for the app to configure the App Proxy settings.</span></span>
<span data-ttu-id="cab6b-136">Используйте [экземпляр аппликатионтемплате](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) , чтобы создать экземпляр настраиваемого приложения и участника службы в клиенте для управления.</span><span class="sxs-lookup"><span data-stu-id="cab6b-136">Use [instantiate applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) to create an instance of a custom application and service principal in your tenant for management.</span></span> <span data-ttu-id="cab6b-137">ИДЕНТИФИКАТОРом шаблона для настраиваемого приложения является: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .</span><span class="sxs-lookup"><span data-stu-id="cab6b-137">The template ID for a custom application is: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

#### <a name="request"></a><span data-ttu-id="cab6b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="cab6b-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cab6b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="cab6b-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_applicationTemplate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/8adf8e6e-67b2-4cf2-a259-e3dc5476c621/instantiate
Content-type: application/json

{
  "displayName": "Contoso IWA App"
}
```
# <a name="c"></a>[<span data-ttu-id="cab6b-140">C#</span><span class="sxs-lookup"><span data-stu-id="cab6b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cab6b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cab6b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cab6b-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cab6b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="cab6b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cab6b-143">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.applicationServicePrincipal",
    "application": {
        "objectId": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
        "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
        "applicationTemplateId": "8adf8e6e-67b2-4cf2-a259-e3dc5476c621",
        "displayName": "Contoso IWA App",
        "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=customappsso|ISV9.1|primary|z",
        "identifierUris": [],
        "publicClient": null,
        "replyUrls": [],
        "logoutUrl": null,
        "samlMetadataUrl": null,
        "errorUrl": null,
        "groupMembershipClaims": null,
        "availableToOtherTenants": false
    },
    "servicePrincipal": {
        "objectId": "b00c693f-9658-4c06-bd1b-c402c4653dea",
        "deletionTimestamp": null,
        "accountEnabled": true,
        "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
        "appDisplayName": "Contoso API",
        "applicationTemplateId": "8adf8e6e-67b2-4cf2-a259-e3dc5476c621",
        "appRoleAssignmentRequired": true,
        "displayName": "Contoso API",
        "errorUrl": null,
        "logoutUrl": null,
        "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=customappsso|ISV9.1|primary|z",
        "samlMetadataUrl": null,
        "microsoftFirstParty": null,
        "publisherName": "f/128 Photography",
        "preferredTokenSigningKeyThumbprint": null,
        "replyUrls": [],
        "servicePrincipalNames": [
            "d7fbfe28-c60e-46d2-8335-841923950d3b"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp",
            "WindowsAzureActiveDirectoryCustomSingleSignOnApplication"
        ],
        "notificationEmailAddresses": [],
        "keyCredentials": [],
        "passwordCredentials": []
    }
}
```


### <a name="retrieve-app-object-id-and-service-principal-object-id"></a><span data-ttu-id="cab6b-144">Получение идентификаторов объектов для приложения и субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="cab6b-144">Retrieve app object ID and service principal object ID</span></span>
<span data-ttu-id="cab6b-145">Из отклика на предыдущий вызов извлеките и сохраните идентификаторы объекта для приложения и субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="cab6b-145">Use the response from the previous call to retrieve and save the application object ID and service principal object ID.</span></span>
```
"application": {
    "objectId": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83"
    }
"servicePrincipal": {
    "objectId": "b00c693f-9658-4c06-bd1b-c402c4653dea"
    }
```

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="cab6b-146">Шаг 2: Настройка свойств прокси приложения</span><span class="sxs-lookup"><span data-stu-id="cab6b-146">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="cab6b-147">Настройка конфигурации Онпремисеспублишинг</span><span class="sxs-lookup"><span data-stu-id="cab6b-147">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="cab6b-148">Используйте свойство applicationId из предыдущего шага, чтобы настроить прокси приложения для приложения и обновить свойство **онпремисеспублишинг** до нужной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="cab6b-148">Use the applicationId from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="cab6b-149">В этом примере используется приложение с внутренним URL-адресом: `https://contosoiwaapp.com` и с использованием домена по умолчанию для внешнего URL-адреса: `https://contosoiwaapp-contoso.msappproxy.net` .</span><span class="sxs-lookup"><span data-stu-id="cab6b-149">In this example, you're using an app with the internal url: `https://contosoiwaapp.com` and using the default domain for the external url: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="cab6b-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="cab6b-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cab6b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="cab6b-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cab6b-152">C#</span><span class="sxs-lookup"><span data-stu-id="cab6b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cab6b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cab6b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cab6b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cab6b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cab6b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="cab6b-155">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="set-the-redirecturi-identifieruri-and-homepageurl-properties"></a><span data-ttu-id="cab6b-156">Установка свойств redirectUri, Идентифиерури и Хомепажеурл</span><span class="sxs-lookup"><span data-stu-id="cab6b-156">Set the redirectUri, identifierUri, and homepageUrl properties</span></span>
<span data-ttu-id="cab6b-157">Обновите **redirectUri**, **идентифиерури**и **хомепажеурл** приложения до внешнего URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="cab6b-157">Update the application's **redirectUri**, **identifierUri**, and **homepageUrl** propertes to the external URL.</span></span>

#### <a name="request"></a><span data-ttu-id="cab6b-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="cab6b-158">Request</span></span>

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
      "homePageUrl": "https://contosoiwaapp-contoso.msappproxy.net"
   }
}
```
#### <a name="response"></a><span data-ttu-id="cab6b-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="cab6b-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="cab6b-160">Шаг 3: назначение группы соединителей приложению</span><span class="sxs-lookup"><span data-stu-id="cab6b-160">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="cab6b-161">Получение соединителей</span><span class="sxs-lookup"><span data-stu-id="cab6b-161">Get connectors</span></span>

<span data-ttu-id="cab6b-162">Перечислите соединители и используйте ответ для получения и сохранения идентификатора объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="cab6b-162">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="cab6b-163">Идентификатор объекта Connector будет использоваться для назначения соединителя группе соединителей.</span><span class="sxs-lookup"><span data-stu-id="cab6b-163">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="cab6b-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="cab6b-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cab6b-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="cab6b-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```
# <a name="c"></a>[<span data-ttu-id="cab6b-166">C#</span><span class="sxs-lookup"><span data-stu-id="cab6b-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cab6b-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cab6b-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cab6b-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cab6b-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cab6b-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="cab6b-169">Response</span></span>

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

### <a name="create-a-connectorgroup"></a><span data-ttu-id="cab6b-170">Создание Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="cab6b-170">Create a connectorGroup</span></span>
<span data-ttu-id="cab6b-171">В этом примере создается новый Коннекторграуп с именем "Ива Demo Connector Group Connector", который используется для приложения.</span><span class="sxs-lookup"><span data-stu-id="cab6b-171">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="cab6b-172">Кроме того, вы можете пропустить этот шаг, если соединитель уже назначен соответствующему Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="cab6b-172">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="cab6b-173">Извлеките и сохраните идентификатор объекта Коннекторграуп, который будет использоваться на следующем шаге.</span><span class="sxs-lookup"><span data-stu-id="cab6b-173">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="cab6b-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="cab6b-174">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cab6b-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="cab6b-175">Response</span></span>

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

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="cab6b-176">Назначение соединителя для Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="cab6b-176">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="cab6b-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="cab6b-177">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cab6b-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="cab6b-178">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="cab6b-179">Назначение приложения для Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="cab6b-179">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="cab6b-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="cab6b-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cab6b-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="cab6b-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cab6b-182">C#</span><span class="sxs-lookup"><span data-stu-id="cab6b-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cab6b-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cab6b-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cab6b-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cab6b-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cab6b-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="cab6b-185">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="cab6b-186">Шаг 4: Настройка единого входа</span><span class="sxs-lookup"><span data-stu-id="cab6b-186">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="cab6b-187">Это приложение использует встроенную проверку подлинности Windows (ИВА).</span><span class="sxs-lookup"><span data-stu-id="cab6b-187">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="cab6b-188">Чтобы настроить Ива, установите свойства единого входа в тип ресурса [синглесигнонсеттингс](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="cab6b-188">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>


#### <a name="request"></a><span data-ttu-id="cab6b-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="cab6b-189">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cab6b-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="cab6b-190">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="cab6b-191">Шаг 5. Назначение пользователей</span><span class="sxs-lookup"><span data-stu-id="cab6b-191">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="cab6b-192">Получение Аппроле для приложения</span><span class="sxs-lookup"><span data-stu-id="cab6b-192">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="cab6b-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="cab6b-193">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cab6b-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="cab6b-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoles
```
# <a name="c"></a>[<span data-ttu-id="cab6b-195">C#</span><span class="sxs-lookup"><span data-stu-id="cab6b-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cab6b-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cab6b-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cab6b-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cab6b-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cab6b-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="cab6b-198">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('b00c693f-9658-4c06-bd1b-c402c4653dea')/appRoles",
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

<span data-ttu-id="cab6b-199">Используйте ответ из предыдущего вызова для получения и сохранения идентификатора Аппроле, который будет использоваться для следующего этапа.</span><span class="sxs-lookup"><span data-stu-id="cab6b-199">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="cab6b-200">Назначение пользователей и групп для приложения</span><span class="sxs-lookup"><span data-stu-id="cab6b-200">Assign users and groups to the application</span></span>

<span data-ttu-id="cab6b-201">Используйте следующие свойства, чтобы назначить пользователя приложению.</span><span class="sxs-lookup"><span data-stu-id="cab6b-201">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="cab6b-202">Свойство</span><span class="sxs-lookup"><span data-stu-id="cab6b-202">Property</span></span>  | <span data-ttu-id="cab6b-203">Описание</span><span class="sxs-lookup"><span data-stu-id="cab6b-203">Description</span></span> |<span data-ttu-id="cab6b-204">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="cab6b-204">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="cab6b-205">principalId</span><span class="sxs-lookup"><span data-stu-id="cab6b-205">principalId</span></span> | <span data-ttu-id="cab6b-206">Идентификатор пользователя, который будет назначен приложению</span><span class="sxs-lookup"><span data-stu-id="cab6b-206">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="cab6b-207">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="cab6b-207">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="cab6b-208">principalType</span><span class="sxs-lookup"><span data-stu-id="cab6b-208">principalType</span></span> | <span data-ttu-id="cab6b-209">Тип пользователя</span><span class="sxs-lookup"><span data-stu-id="cab6b-209">Type of user</span></span> | <span data-ttu-id="cab6b-210">Пользователь</span><span class="sxs-lookup"><span data-stu-id="cab6b-210">User</span></span> |
| <span data-ttu-id="cab6b-211">аппролеид</span><span class="sxs-lookup"><span data-stu-id="cab6b-211">appRoleId</span></span> |  <span data-ttu-id="cab6b-212">Идентификатор роли приложения по умолчанию для приложения</span><span class="sxs-lookup"><span data-stu-id="cab6b-212">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="cab6b-213">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="cab6b-213">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="cab6b-214">resourceId</span><span class="sxs-lookup"><span data-stu-id="cab6b-214">resourceId</span></span> | <span data-ttu-id="cab6b-215">Идентификатор servicePrincipal приложения</span><span class="sxs-lookup"><span data-stu-id="cab6b-215">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="cab6b-216">b00c693f-9658-4c06-bd1b-c402c4653dea</span><span class="sxs-lookup"><span data-stu-id="cab6b-216">b00c693f-9658-4c06-bd1b-c402c4653dea</span></span> |

#### <a name="request"></a><span data-ttu-id="cab6b-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="cab6b-217">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cab6b-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="cab6b-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"b00c693f-9658-4c06-bd1b-c402c4653dea"
}
```
# <a name="javascript"></a>[<span data-ttu-id="cab6b-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cab6b-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cab6b-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="cab6b-220">Response</span></span>

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
    "resourceId": "b00c693f-9658-4c06-bd1b-c402c4653dea"
}
```

<span data-ttu-id="cab6b-221">Дополнительные сведения см. в документации по типу ресурса [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="cab6b-221">For more information, see [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>



## <a name="additional-steps"></a><span data-ttu-id="cab6b-222">Дополнительные действия</span><span class="sxs-lookup"><span data-stu-id="cab6b-222">Additional steps</span></span>
- [<span data-ttu-id="cab6b-223">Автоматизация конфигурации с помощью примеров PowerShell для прокси-сервера приложений</span><span class="sxs-lookup"><span data-stu-id="cab6b-223">Automate configuration using PowerShell samples for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="cab6b-224">Автоматизация настройки единого входа на основе SAML для приложений с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cab6b-224">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
