---
title: Настройка прокси приложения с помощью API Microsoft Graph
description: Автоматически настраивать прокси приложения с помощью API Microsoft Graph, чтобы обеспечить удаленный доступ и единый вход в локальном приложении.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 28bb376b094a648d246bba5401764952d5aec863
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943684"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="71c84-103">Автоматизация настройки прокси приложения с помощью API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71c84-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="71c84-104">В этой статье вы узнаете, как создать и настроить прокси [](/azure/active-directory/manage-apps/what-is-application-proxy) приложения Azure Active Directory (Azure AD) для приложения.</span><span class="sxs-lookup"><span data-stu-id="71c84-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](/azure/active-directory/manage-apps/what-is-application-proxy) for an application.</span></span> <span data-ttu-id="71c84-105">Прокси приложения обеспечивает безопасный удаленный доступ и единый вход в локальное веб-приложение.</span><span class="sxs-lookup"><span data-stu-id="71c84-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="71c84-106">После настройки прокси приложения пользователи могут получать доступ к своим приложениям через внешний URL-адрес, портал "Мои приложения" или другие внутренние порталы приложений.</span><span class="sxs-lookup"><span data-stu-id="71c84-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="71c84-107">В этой статье предполагается, что вы [](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) уже установили соединители и выполнили необходимые условия для прокси приложения, чтобы соединители могли взаимодействовать со службами Azure AD.</span><span class="sxs-lookup"><span data-stu-id="71c84-107">This article assumes you have already installed a connector and completed the [prerequisites](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="71c84-108">Убедитесь, что у вас есть соответствующие разрешения для вызова следующих API.</span><span class="sxs-lookup"><span data-stu-id="71c84-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="71c84-109">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="71c84-109">Resource type</span></span> |<span data-ttu-id="71c84-110">Метод</span><span class="sxs-lookup"><span data-stu-id="71c84-110">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="71c84-111">applications</span><span class="sxs-lookup"><span data-stu-id="71c84-111">applications</span></span>](/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="71c84-112">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="71c84-112">onPremisesPublishing</span></span>](/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [<span data-ttu-id="71c84-113">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="71c84-113">Create application</span></span>](/graph/api/application-post-applications?tabs=http&view=graph-rest-beta) <br> [<span data-ttu-id="71c84-114">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="71c84-114">Update application</span></span>](/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="71c84-115">Добавление приложения в connectorGroup</span><span class="sxs-lookup"><span data-stu-id="71c84-115">Add application to connectorGroup</span></span>](/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="71c84-116">connector</span><span class="sxs-lookup"><span data-stu-id="71c84-116">connector</span></span>](/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="71c84-117">Получить соединители</span><span class="sxs-lookup"><span data-stu-id="71c84-117">Get connectors</span></span>](/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="71c84-118">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="71c84-118">connectorGroup</span></span>](/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="71c84-119">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="71c84-119">Create connectorGroup</span></span>](/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="71c84-120">Добавление соединителя для connectorGroup</span><span class="sxs-lookup"><span data-stu-id="71c84-120">Add connector to connectorGroup</span></span>](/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="71c84-121">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="71c84-121">servicePrincipals</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="71c84-122">Создать servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="71c84-122">Create servicePrincipal</span></span>](/graph/api/serviceprincipal-post-serviceprincipals?tabs=http&view=graph-rest-beta) <br> [<span data-ttu-id="71c84-123">Обновление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="71c84-123">Update servicePrincipal</span></span>](/graph/api/serviceprincipal-update?tabs=http&view=graph-rest-1.0) <br> [<span data-ttu-id="71c84-124">Создание appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="71c84-124">Create appRoleAssignments</span></span>](/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> <span data-ttu-id="71c84-125">В запросах, показанных в этой статье, используются примеры значений.</span><span class="sxs-lookup"><span data-stu-id="71c84-125">The requests shown in this article use sample values.</span></span> <span data-ttu-id="71c84-126">Вам потребуется обновить их.</span><span class="sxs-lookup"><span data-stu-id="71c84-126">You will need update these.</span></span> <span data-ttu-id="71c84-127">Показанные объекты ответа также могут быть сокращены для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="71c84-127">The response objects shown might also be shortened for readability.</span></span> 

## <a name="step-1-create-an-application"></a><span data-ttu-id="71c84-128">Шаг 1. Создание приложения</span><span class="sxs-lookup"><span data-stu-id="71c84-128">Step 1: Create an application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="71c84-129">Вход в песочницу Microsoft Graph (рекомендуется), Postman или любой другой используемый клиент API</span><span class="sxs-lookup"><span data-stu-id="71c84-129">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="71c84-130">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="71c84-130">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="71c84-131">Выберите **вход с помощью Майкрософт** и во входе с помощью учетных данных глобального администратора Azure AD или администратора приложений.</span><span class="sxs-lookup"><span data-stu-id="71c84-131">Select **Sign-in with Microsoft** and sign in using Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="71c84-132">После успешного входе вы увидите сведения об учетной записи пользователя в левой области.</span><span class="sxs-lookup"><span data-stu-id="71c84-132">Upon successful sign in, you'll see the user account details in the left pane.</span></span>

> [!NOTE]
> <span data-ttu-id="71c84-133">Вход с помощью основного службы в настоящее время не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c84-133">Sign in using a service principal is not currently supported.</span></span> 

### <a name="create-an-application"></a><span data-ttu-id="71c84-134">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="71c84-134">Create an application</span></span>

<span data-ttu-id="71c84-135">Чтобы настроить прокси приложения для приложения с помощью API, необходимо создать приложение, добавить в него основной объект-службу, а затем обновить свойство **onPremisesPublishing** приложения, чтобы настроить параметры прокси приложения.</span><span class="sxs-lookup"><span data-stu-id="71c84-135">To configure Application Proxy for an app using the API, you create an application, add a service principal to the app, and then update the application's **onPremisesPublishing** property to configure the App Proxy settings.</span></span> <span data-ttu-id="71c84-136">При создании приложения установите для **signInAudience** приложения "AzureADMyOrg".</span><span class="sxs-lookup"><span data-stu-id="71c84-136">When creating the application, set the application's **signInAudience** to "AzureADMyOrg".</span></span>

#### <a name="request"></a><span data-ttu-id="71c84-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="71c84-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="71c84-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="71c84-139">C#</span><span class="sxs-lookup"><span data-stu-id="71c84-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71c84-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71c84-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71c84-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71c84-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71c84-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-142">Response</span></span>

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

### <a name="retrieve-the-application-object-id-and-appid"></a><span data-ttu-id="71c84-143">Получение ИД объекта приложения и appId</span><span class="sxs-lookup"><span data-stu-id="71c84-143">Retrieve the application object ID and appId</span></span>
<span data-ttu-id="71c84-144">Используйте ответ из предыдущего вызова, чтобы получить и сохранить ИД объекта приложения и ИД приложения.</span><span class="sxs-lookup"><span data-stu-id="71c84-144">Use the response from the previous call to retrieve and save the application object ID and app ID.</span></span>
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a><span data-ttu-id="71c84-145">Создание servicePrincipal для приложения и добавление необходимых тегов</span><span class="sxs-lookup"><span data-stu-id="71c84-145">Create a servicePrincipal for the application and add required tags</span></span>
<span data-ttu-id="71c84-146">Используйте **appId для** создания основного приложения-службы.</span><span class="sxs-lookup"><span data-stu-id="71c84-146">Use the **appId** to create a service principal for the application.</span></span> <span data-ttu-id="71c84-147">Затем добавьте теги, необходимые для настройки прокси приложения для приложения.</span><span class="sxs-lookup"><span data-stu-id="71c84-147">Then add the tags required for configuring Application Proxy for an app.</span></span>

#### <a name="request"></a><span data-ttu-id="71c84-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="71c84-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="71c84-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="71c84-150">C#</span><span class="sxs-lookup"><span data-stu-id="71c84-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71c84-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71c84-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71c84-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71c84-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71c84-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-153">Response</span></span>
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

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="71c84-154">Шаг 2. Настройка свойств прокси приложения</span><span class="sxs-lookup"><span data-stu-id="71c84-154">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="71c84-155">Настройка конфигурации onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="71c84-155">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="71c84-156">Используйте ИД объекта приложения из предыдущего шага, чтобы настроить прокси приложения и обновить свойство **onPremisesPublishing** до нужной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="71c84-156">Use the application object ID from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="71c84-157">В этом примере вы используете приложение с внутренним URL-адресом и доменом по умолчанию `https://contosoiwaapp.com` для внешнего URL-адреса: `https://contosoiwaapp-contoso.msappproxy.net` .</span><span class="sxs-lookup"><span data-stu-id="71c84-157">In this example, you're using an app with the internal URL: `https://contosoiwaapp.com` and using the default domain for the external URL: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="71c84-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="71c84-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="71c84-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="71c84-160">C#</span><span class="sxs-lookup"><span data-stu-id="71c84-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71c84-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71c84-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71c84-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71c84-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71c84-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-163">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a><span data-ttu-id="71c84-164">Завершение настройки приложения</span><span class="sxs-lookup"><span data-stu-id="71c84-164">Complete the configuration of the application</span></span>
<span data-ttu-id="71c84-165">Обновите свойства **redirectUri,** **identifierUri** и **homepageUrl** приложения до внешнего URL-адреса, настроенного в свойстве **onPremisesPublishing.**</span><span class="sxs-lookup"><span data-stu-id="71c84-165">Update the application's **redirectUri**, **identifierUri**, and **homepageUrl** properties to the external UR configured in the **onPremisesPublishing** property.</span></span> <span data-ttu-id="71c84-166">Затем [обновите implicitGrantSettings](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) для `true` **enabledTokenIssuance** и `false` **enabledAccessTokenIssuance.**</span><span class="sxs-lookup"><span data-stu-id="71c84-166">Then update [implicitGrantSettings](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) to `true` for **enabledTokenIssuance** and `false` for **enabledAccessTokenIssuance**.</span></span>

#### <a name="request"></a><span data-ttu-id="71c84-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-167">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="71c84-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-168">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="71c84-169">Шаг 3. Назначение группы соединители приложению</span><span class="sxs-lookup"><span data-stu-id="71c84-169">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="71c84-170">Получить соединители</span><span class="sxs-lookup"><span data-stu-id="71c84-170">Get connectors</span></span>

<span data-ttu-id="71c84-171">Перечислите соединители и используйте ответ для извлечения и сохранения ИД объекта соединители.</span><span class="sxs-lookup"><span data-stu-id="71c84-171">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="71c84-172">Для назначения соединители группе соединители будет использоваться ИД объекта соединитела.</span><span class="sxs-lookup"><span data-stu-id="71c84-172">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="71c84-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-173">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="71c84-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="71c84-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```
# <a name="c"></a>[<span data-ttu-id="71c84-175">C#</span><span class="sxs-lookup"><span data-stu-id="71c84-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71c84-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71c84-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71c84-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71c84-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71c84-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-178">Response</span></span>

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

### <a name="create-a-connectorgroup"></a><span data-ttu-id="71c84-179">Создание соединителиГруппы</span><span class="sxs-lookup"><span data-stu-id="71c84-179">Create a connectorGroup</span></span>
<span data-ttu-id="71c84-180">В этом примере создается новая группа connectorGroup с именем "Группа демонстрационных соединитеев IWA", которая используется для приложения.</span><span class="sxs-lookup"><span data-stu-id="71c84-180">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="71c84-181">Этот шаг также можно пропустить, если соединители уже назначены соответствующей группе соединитеев.</span><span class="sxs-lookup"><span data-stu-id="71c84-181">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="71c84-182">Извлеките и сохраните ИД объекта connectorGroup, который будет применяться на следующем этапе.</span><span class="sxs-lookup"><span data-stu-id="71c84-182">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="71c84-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-183">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="71c84-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-184">Response</span></span>

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

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="71c84-185">Назначение соединители соединители группе</span><span class="sxs-lookup"><span data-stu-id="71c84-185">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="71c84-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-186">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="71c84-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-187">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="71c84-188">Назначение приложения соединителигруппе</span><span class="sxs-lookup"><span data-stu-id="71c84-188">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="71c84-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-189">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="71c84-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="71c84-190">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="71c84-191">C#</span><span class="sxs-lookup"><span data-stu-id="71c84-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71c84-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71c84-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71c84-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71c84-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71c84-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-194">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="71c84-195">Шаг 4. Настройка единого входов</span><span class="sxs-lookup"><span data-stu-id="71c84-195">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="71c84-196">Это приложение использует встроенную проверку подлинности Windows (IWA).</span><span class="sxs-lookup"><span data-stu-id="71c84-196">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="71c84-197">Чтобы настроить IWA, установите свойства единого вход в типе ресурса [singleSignOnSettings.](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="71c84-197">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>

#### <a name="request"></a><span data-ttu-id="71c84-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-198">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="71c84-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-199">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="71c84-200">Шаг 5. Назначение пользователей</span><span class="sxs-lookup"><span data-stu-id="71c84-200">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="71c84-201">Получение appRole для приложения</span><span class="sxs-lookup"><span data-stu-id="71c84-201">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="71c84-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-202">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="71c84-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="71c84-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```
# <a name="c"></a>[<span data-ttu-id="71c84-204">C#</span><span class="sxs-lookup"><span data-stu-id="71c84-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71c84-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71c84-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71c84-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71c84-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71c84-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-207">Response</span></span>

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

<span data-ttu-id="71c84-208">Используйте ответ из предыдущего вызова, чтобы получить и сохранить ИД appRole для использования на следующем шаге.</span><span class="sxs-lookup"><span data-stu-id="71c84-208">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="71c84-209">Назначение пользователей и групп для приложения</span><span class="sxs-lookup"><span data-stu-id="71c84-209">Assign users and groups to the application</span></span>

<span data-ttu-id="71c84-210">Используйте следующие свойства, чтобы назначить пользователя приложению.</span><span class="sxs-lookup"><span data-stu-id="71c84-210">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="71c84-211">Свойство</span><span class="sxs-lookup"><span data-stu-id="71c84-211">Property</span></span>  | <span data-ttu-id="71c84-212">Описание</span><span class="sxs-lookup"><span data-stu-id="71c84-212">Description</span></span> |<span data-ttu-id="71c84-213">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="71c84-213">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="71c84-214">principalId</span><span class="sxs-lookup"><span data-stu-id="71c84-214">principalId</span></span> | <span data-ttu-id="71c84-215">ИД пользователя, который будет назначен приложению</span><span class="sxs-lookup"><span data-stu-id="71c84-215">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="71c84-216">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="71c84-216">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="71c84-217">principalType</span><span class="sxs-lookup"><span data-stu-id="71c84-217">principalType</span></span> | <span data-ttu-id="71c84-218">Тип пользователя</span><span class="sxs-lookup"><span data-stu-id="71c84-218">Type of user</span></span> | <span data-ttu-id="71c84-219">Пользователь</span><span class="sxs-lookup"><span data-stu-id="71c84-219">User</span></span> |
| <span data-ttu-id="71c84-220">appRoleId</span><span class="sxs-lookup"><span data-stu-id="71c84-220">appRoleId</span></span> |  <span data-ttu-id="71c84-221">ИД роли приложения для роли приложения по умолчанию в приложении</span><span class="sxs-lookup"><span data-stu-id="71c84-221">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="71c84-222">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="71c84-222">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="71c84-223">resourceId</span><span class="sxs-lookup"><span data-stu-id="71c84-223">resourceId</span></span> | <span data-ttu-id="71c84-224">ServicePrincipal ID приложения</span><span class="sxs-lookup"><span data-stu-id="71c84-224">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="71c84-225">a8cac399-cde5-4516-a674-819503c61313</span><span class="sxs-lookup"><span data-stu-id="71c84-225">a8cac399-cde5-4516-a674-819503c61313</span></span> |

#### <a name="request"></a><span data-ttu-id="71c84-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c84-226">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="71c84-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c84-227">Response</span></span>

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

<span data-ttu-id="71c84-228">Дополнительные сведения см. в документации по типу ресурса [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="71c84-228">For more information, see [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>


## <a name="additional-steps"></a><span data-ttu-id="71c84-229">Дополнительные действия</span><span class="sxs-lookup"><span data-stu-id="71c84-229">Additional steps</span></span>
- [<span data-ttu-id="71c84-230">Автоматизация настройки с помощью примеров PowerShell для прокси приложения</span><span class="sxs-lookup"><span data-stu-id="71c84-230">Automate configuration using PowerShell samples for Application Proxy</span></span>](/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="71c84-231">Автоматизация настройки единого входа на основе SAML для приложений с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="71c84-231">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
