---
title: Настройка единого входа на основе SAML с помощью API Microsoft Graph
description: Узнайте, как экономить время с помощью API Microsoft Graph, чтобы автоматизировать настройку единого входа на основе SAML.
author: kenwith
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: 2596edb4e88638e18b67a0a95137743ea38b290c
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563942"
---
# <a name="automate-saml-based-sso-app-configuration-with-microsoft-graph-api"></a><span data-ttu-id="39493-103">Автоматизация настройки единого входа на основе SAML для приложений с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="39493-103">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>

<span data-ttu-id="39493-104">Из этой статьи вы узнаете, как создать и настроить приложение из коллекции Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="39493-104">In this article, you'll learn how to create and configure an application from the Azure Active Directory (Azure AD) Gallery.</span></span> <span data-ttu-id="39493-105">В этой статье в качестве примера используется AWS, но описанные здесь шаги можно применить для любого другого приложения на основе SAML, включенного в коллекцию Azure AD.</span><span class="sxs-lookup"><span data-stu-id="39493-105">This article uses AWS as an example, but you can use the steps in this article for any SAML-based app in the Azure AD Gallery.</span></span>

<span data-ttu-id="39493-106">**Шаги по автоматизации настройки единого входа на основе SAML с помощью API Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="39493-106">**Steps to use Microsoft Graph APIs to automate configuration of SAML-based single sign-on**</span></span>

| <span data-ttu-id="39493-107">Шаг</span><span class="sxs-lookup"><span data-stu-id="39493-107">Step</span></span>  | <span data-ttu-id="39493-108">Сведения</span><span class="sxs-lookup"><span data-stu-id="39493-108">Details</span></span>  |
|---------|---------|
| [<span data-ttu-id="39493-109">1. Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="39493-109">1. Create the gallery application</span></span>](#step-1-create-the-gallery-application) | <span data-ttu-id="39493-110">Вход в клиент API</span><span class="sxs-lookup"><span data-stu-id="39493-110">Sign in to the API client</span></span> <br> <span data-ttu-id="39493-111">Получение приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="39493-111">Retrieve the gallery application</span></span> <br> <span data-ttu-id="39493-112">Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="39493-112">Create the gallery application</span></span>|
| [<span data-ttu-id="39493-113">2. Настройка единого входа</span><span class="sxs-lookup"><span data-stu-id="39493-113">2. Configure single sign-on</span></span>](#step-2-configure-single-sign-on) | <span data-ttu-id="39493-114">Получение идентификаторов объектов для приложения и субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="39493-114">Retrieve app object ID and service principal object ID</span></span> <br> <span data-ttu-id="39493-115">Настройка режима единого входа</span><span class="sxs-lookup"><span data-stu-id="39493-115">Set single sign-on mode</span></span> <br> <span data-ttu-id="39493-116">Настройка основных URL-адресов SAML, таких как идентификатор, URL-адрес ответа и URL-адрес входа</span><span class="sxs-lookup"><span data-stu-id="39493-116">Set basic SAML URLs such as identifier, reply URL, sign-on URL</span></span> <br> <span data-ttu-id="39493-117">Добавление ролей приложения (необязательно)</span><span class="sxs-lookup"><span data-stu-id="39493-117">Add app roles (Optional)</span></span>|
| [<span data-ttu-id="39493-118">3. Настройка сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="39493-118">3. Configure claims mapping</span></span>](#step-3-configure-claims-mapping) | <span data-ttu-id="39493-119">Создание политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="39493-119">Create claims mapping policy</span></span> <br> <span data-ttu-id="39493-120">Назначение политики сопоставления утверждений субъекту-службе</span><span class="sxs-lookup"><span data-stu-id="39493-120">Assign claims mapping policy to service principal</span></span>|
| [<span data-ttu-id="39493-121">4. Настройка сертификата для подписи</span><span class="sxs-lookup"><span data-stu-id="39493-121">4. Configure signing certificate</span></span>](#step-4-configure-signing-certificate) | <span data-ttu-id="39493-122">Создание сертификата</span><span class="sxs-lookup"><span data-stu-id="39493-122">Create a certificate</span></span> <BR> <span data-ttu-id="39493-123">Добавление пользовательского ключа подписывания</span><span class="sxs-lookup"><span data-stu-id="39493-123">Add a custom signing key</span></span> <br> <span data-ttu-id="39493-124">Активация пользовательского ключа подписывания</span><span class="sxs-lookup"><span data-stu-id="39493-124">Activate the custom signing key</span></span>|
| [<span data-ttu-id="39493-125">5. Назначение пользователей</span><span class="sxs-lookup"><span data-stu-id="39493-125">5. Assign users</span></span>](#step-5-assign-users) | <span data-ttu-id="39493-126">Назначение пользователей и групп для приложения</span><span class="sxs-lookup"><span data-stu-id="39493-126">Assign users and groups to the application</span></span>
| [<span data-ttu-id="39493-127">6. Настройка на стороне приложения</span><span class="sxs-lookup"><span data-stu-id="39493-127">6. Configure the application side</span></span>](#step-6-configure-the-application-side)| <span data-ttu-id="39493-128">Получение метаданных SAML из Azure AD</span><span class="sxs-lookup"><span data-stu-id="39493-128">Get Azure AD SAML metadata</span></span>

<span data-ttu-id="39493-129">**Список всех API, используемых в этой статье**</span><span class="sxs-lookup"><span data-stu-id="39493-129">**List of all APIs used in the article**</span></span>

<span data-ttu-id="39493-130">Убедитесь, что у вас есть соответствующие разрешения для вызова следующих API.</span><span class="sxs-lookup"><span data-stu-id="39493-130">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="39493-131">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="39493-131">Resource type</span></span> |<span data-ttu-id="39493-132">Метод</span><span class="sxs-lookup"><span data-stu-id="39493-132">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="39493-133">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="39493-133">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-beta)|[<span data-ttu-id="39493-134">Перечисление applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="39493-134">List applicationTemplate</span></span>](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta) <br>[<span data-ttu-id="39493-135">Создание экземпляра applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="39493-135">Instantiate applicationTemplate</span></span>](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta)|
|[<span data-ttu-id="39493-136">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="39493-136">servicePrincipals</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="39493-137">Обновление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="39493-137">Update servicePrincipal</span></span>](/graph/api/serviceprincipal-update?tabs=http&view=graph-rest-1.0) <br> [<span data-ttu-id="39493-138">Создание appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="39493-138">Create appRoleAssignments</span></span>](/graph/api/serviceprincipal-post-approleassignments?tabs=http&view=graph-rest-1.0) <br> [<span data-ttu-id="39493-139">Назначение claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="39493-139">Assign claimsMappingPolicies</span></span>](/graph/api/serviceprincipal-post-claimsmappingpolicies?tabs=http&view=graph-rest-beta)|
|[<span data-ttu-id="39493-140">applications</span><span class="sxs-lookup"><span data-stu-id="39493-140">applications</span></span>](/graph/api/resources/application?view=graph-rest-1.0)|[<span data-ttu-id="39493-141">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="39493-141">Update application</span></span>](/graph/api/application-update?tabs=http&view=graph-rest-1.0)|
|[<span data-ttu-id="39493-142">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="39493-142">claimsMappingPolicy</span></span>](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)| [<span data-ttu-id="39493-143">Создание claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="39493-143">Create claimsMappingPolicy</span></span>](/graph/api/claimsmappingpolicy-post-claimsmappingpolicies?tabs=http&view=graph-rest-beta)

>[!NOTE]
><span data-ttu-id="39493-144">Объекты отклика, приведенные в этой статье, могут быть сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="39493-144">The response objects shown in this article might be shortened for readability.</span></span> <span data-ttu-id="39493-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39493-145">All the properties will be returned from an actual call.</span></span>

## <a name="step-1-create-the-gallery-application"></a><span data-ttu-id="39493-146">Шаг 1. Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="39493-146">Step 1: Create the gallery application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="39493-147">Вход в песочницу Microsoft Graph (рекомендуется), Postman или любой другой используемый клиент API</span><span class="sxs-lookup"><span data-stu-id="39493-147">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="39493-148">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="39493-148">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="39493-149">Выберите вариант **Вход с помощью учетной записи Майкрософт** и войдите, используя учетные данные глобального администратора Azure AD или администратора приложения.</span><span class="sxs-lookup"><span data-stu-id="39493-149">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="39493-150">После успешного входа вы увидите данные учетной записи пользователя на панели слева.</span><span class="sxs-lookup"><span data-stu-id="39493-150">Upon successful sign-in, you'll see the user account details in the left-hand pane.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="39493-151">Получение идентификатора шаблона для приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="39493-151">Retrieve the gallery application template identifier</span></span>

<span data-ttu-id="39493-152">У каждого приложения в коллекции приложений Azure AD есть [шаблон](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta), описывающий метаданные для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="39493-152">Applications in the Azure AD application gallery each have an [application template](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta) that describes the metadata for that application.</span></span> <span data-ttu-id="39493-153">По этому шаблону вы можете создать экземпляр приложения и субъект-службу в клиенте для управления им.</span><span class="sxs-lookup"><span data-stu-id="39493-153">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span>

#### <a name="request"></a><span data-ttu-id="39493-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="39493-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="39493-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="39493-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="39493-156">C#</span><span class="sxs-lookup"><span data-stu-id="39493-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39493-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39493-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39493-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39493-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39493-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="39493-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
  {
    "id": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "Amazon Web Services (AWS)",
        "homePageUrl": "http://aws.amazon.com/",
        "supportedSingleSignOnModes": [
             "password",
             "saml",
             "external"
         ],
         "supportedProvisioningTypes": [
             "sync"
         ],
         "logoUrl": "https://az495088.vo.msecnd.net/app-logo/aws_215.png",
         "categories": [
             "developerServices"
         ],
         "publisher": "Amazon",
         "description": null    
  
}
```

### <a name="create-the-gallery-application"></a><span data-ttu-id="39493-160">Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="39493-160">Create the gallery application</span></span>

<span data-ttu-id="39493-161">Используя идентификатор шаблона, полученный для приложения на предыдущем шаге, [создайте экземпляр](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta) приложения и субъект-службу в клиенте.</span><span class="sxs-lookup"><span data-stu-id="39493-161">Using the template ID that you retrieved for your application in the last step, [create an instance](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta) of the application and service principal in your tenant.</span></span>

> [!NOTE] 
> <span data-ttu-id="39493-162">Вы можете использовать API applicationTemplate для создания экземпляров [приложений не из коллекции](/azure/active-directory/manage-apps/view-applications-portal).</span><span class="sxs-lookup"><span data-stu-id="39493-162">You can use applicationTemplate API to instantiate [Non-Gallery apps](/azure/active-directory/manage-apps/view-applications-portal).</span></span> <span data-ttu-id="39493-163">Используйте applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span><span class="sxs-lookup"><span data-stu-id="39493-163">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

> [!NOTE]
> <span data-ttu-id="39493-164">Подождите некоторое время, пока приложение будет подготовлено в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="39493-164">Allow some time for the app to be provisioned into your Azure AD tenant.</span></span> <span data-ttu-id="39493-165">Это не происходит сразу.</span><span class="sxs-lookup"><span data-stu-id="39493-165">It is not instant.</span></span> <span data-ttu-id="39493-166">Одной из стратегий является выполнение запроса GET для объекта приложения или субъекта-службы каждые 5–10 секунд до тех пор, пока запрос не будет успешным.</span><span class="sxs-lookup"><span data-stu-id="39493-166">One strategy is to do a GET query on the application / service principal object every 5-10 seconds until the query is successful.</span></span>


#### <a name="request"></a><span data-ttu-id="39493-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="39493-167">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="39493-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="39493-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```
# <a name="c"></a>[<span data-ttu-id="39493-169">C#</span><span class="sxs-lookup"><span data-stu-id="39493-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39493-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39493-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39493-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39493-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39493-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="39493-172">Response</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json


{
    "application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63",
        "appId": "92653dd4-aa3a-3323-80cf-e8cfefcc8d5d",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "AWS Contoso",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "logoutUrl": null,
        "samlMetadataUrl": null,
    },
    "servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e",
        "appDisplayName": "AWS Contoso",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "appRoleAssignmentRequired": true,
        "displayName": "My custom name",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "servicePrincipalNames": [
            "93653dd4-aa3a-4323-80cf-e8cfefcc8d7d"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp"
        ],
    }
}
```

## <a name="step-2-configure-single-sign-on"></a><span data-ttu-id="39493-173">Шаг 2. Настройка единого входа</span><span class="sxs-lookup"><span data-stu-id="39493-173">Step 2: Configure single sign-on</span></span>

### <a name="retrieve-app-object-id-and-service-principal-object-id"></a><span data-ttu-id="39493-174">Получение идентификаторов объектов для приложения и субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="39493-174">Retrieve app object ID and service principal object ID</span></span>

<span data-ttu-id="39493-175">Из отклика на предыдущий вызов извлеките и сохраните идентификаторы объекта для приложения и субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="39493-175">Use the response from the previous call to retrieve and save the application object ID and service principal object ID.</span></span>

```json
"application":{
  "objectId":"cbc071a6-0fa5-4859-8g55-e983ef63df63"
},
"servicePrincipal":{
  "objectId":"f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```
### <a name="set-single-sign-on-mode"></a><span data-ttu-id="39493-176">Настройка режима единого входа</span><span class="sxs-lookup"><span data-stu-id="39493-176">Set single sign-on mode</span></span>

<span data-ttu-id="39493-177">В этом примере вы настроите режим единого входа `saml` для [типа ресурса servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="39493-177">In this example, you'll set `saml` as the single sign-on mode in the [servicePrincipal resource type](/graph/api/resources/serviceprincipal?view=graph-rest-1.0).</span></span> <span data-ttu-id="39493-178">Также вы можете настроить другие свойства единого входа SAML: `notificationEmailAddresses`, `loginUrl` и `samlSingleSignOnSettings.relayState`.</span><span class="sxs-lookup"><span data-stu-id="39493-178">Other SAML SSO properties that you can configure are: `notificationEmailAddresses`, `loginUrl`, and `samlSingleSignOnSettings.relayState`.</span></span>

<span data-ttu-id="39493-179">Прежде чем этот запрос заработает, необходимо предоставить согласие на вкладке **Изменить разрешения** в песочнице Graph.</span><span class="sxs-lookup"><span data-stu-id="39493-179">Before this query will work you need to provide consent on the **Modify permissions** tab in Graph Explorer.</span></span> <span data-ttu-id="39493-180">Кроме того, используйте идентификатор **servicePrincipal**, полученный ранее.</span><span class="sxs-lookup"><span data-stu-id="39493-180">Also, make sure you are using the **servicePrincipal** ID that you obtained earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="39493-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="39493-181">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="39493-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="39493-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: application/json

{
    "preferredSingleSignOnMode": "saml"
}
```
# <a name="c"></a>[<span data-ttu-id="39493-183">C#</span><span class="sxs-lookup"><span data-stu-id="39493-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39493-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39493-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39493-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39493-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39493-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="39493-186">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls-such-as-identifier-reply-url-sign-on-url"></a><span data-ttu-id="39493-187">Настройка основных URL-адресов SAML, таких как идентификатор, URL-адрес ответа и URL-адрес входа</span><span class="sxs-lookup"><span data-stu-id="39493-187">Set basic SAML URLs such as identifier, reply URL, sign-on URL</span></span>

<span data-ttu-id="39493-188">Настройте идентификатор и URL-адреса ответа для AWS в объекте приложения.</span><span class="sxs-lookup"><span data-stu-id="39493-188">Set the identifier and reply URLs for AWS in the application object.</span></span>

<span data-ttu-id="39493-189">Используйте идентификатор **application**, полученный ранее.</span><span class="sxs-lookup"><span data-stu-id="39493-189">Make sure you are using the **application** id obtained earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="39493-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="39493-190">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="39493-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="39493-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/applications/cbc071a6-0fa5-4859-8g55-e983ef63df63
Content-type: applications/json

{
    "web": {
        "redirectUris": [
            "https://signin.aws.amazon.com/saml"
        ] 
    },
    "identifierUris": [
        "https://signin.aws.amazon.com/saml"
    ]    
}
```
# <a name="c"></a>[<span data-ttu-id="39493-192">C#</span><span class="sxs-lookup"><span data-stu-id="39493-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39493-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39493-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39493-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39493-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39493-195">Java</span><span class="sxs-lookup"><span data-stu-id="39493-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="39493-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="39493-196">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204
```
### <a name="add-app-roles-optional"></a><span data-ttu-id="39493-197">Добавление ролей приложения (необязательно)</span><span class="sxs-lookup"><span data-stu-id="39493-197">Add app roles (Optional)</span></span>

<span data-ttu-id="39493-198">Если приложение ожидает получить сведения о роли в маркере, добавьте определение ролей в объект приложения.</span><span class="sxs-lookup"><span data-stu-id="39493-198">If the application requires the role information in the token, add the definition of the roles in the application object.</span></span> <span data-ttu-id="39493-199">Для AWS вы можете [включить подготовку пользователя](/azure/active-directory/app-provisioning/application-provisioning-configure-api), чтобы автоматически получать все роли из учетной записи AWS.</span><span class="sxs-lookup"><span data-stu-id="39493-199">For AWS, you can [enable user provisioning](/azure/active-directory/app-provisioning/application-provisioning-configure-api) to fetch all the roles from that AWS account.</span></span> 

<span data-ttu-id="39493-200">Дополнительные сведения см. в статье [Настройка утверждения роли, выдаваемого в маркере SAML](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span><span class="sxs-lookup"><span data-stu-id="39493-200">For more information, see [Configure the role claim issued in the SAML token](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span></span>

> [!NOTE] 
> <span data-ttu-id="39493-201">При добавлении ролей приложения не изменяйте стандартные роли приложения msiam_access.</span><span class="sxs-lookup"><span data-stu-id="39493-201">When adding app roles, don't modify the default app roles msiam_access.</span></span> 

#### <a name="request"></a><span data-ttu-id="39493-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="39493-202">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="39493-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="39493-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/serviceprincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: application/json

{
"appRoles": [
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "msiam_access",
            "displayName": "msiam_access",
            "id": "7dfd756e-8c27-4472-b2b7-38c17fc5de5e",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "Admin,WAAD",
            "displayName": "Admin,WAAD",
            "id": "454dc4c2-8176-498e-99df-8c4efcde41ef",
            "isEnabled": true,
            "value": "arn:aws:iam::212743507312:role/accountname-aws-admin,arn:aws:iam::212743507312:saml-provider/WAAD"
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "Finance,WAAD",
            "displayName": "Finance,WAAD",
            "id": "8642d5fa-18a3-4245-ab8c-a96000c1a217",
            "isEnabled": true,
            "value": "arn:aws:iam::212743507312:role/accountname-aws-finance,arn:aws:iam::212743507312:saml-provider/WAAD"
        }
    ]

}
```
# <a name="c"></a>[<span data-ttu-id="39493-204">C#</span><span class="sxs-lookup"><span data-stu-id="39493-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39493-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39493-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39493-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39493-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39493-207">Java</span><span class="sxs-lookup"><span data-stu-id="39493-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39493-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="39493-208">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a><span data-ttu-id="39493-209">Шаг 3. Настройка сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="39493-209">Step 3: Configure claims mapping</span></span>

### <a name="create-claims-mapping-policy"></a><span data-ttu-id="39493-210">Создание политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="39493-210">Create claims mapping policy</span></span>

<span data-ttu-id="39493-211">В дополнение к основным утверждениям настройте следующие, чтобы служба Azure AD включала их в маркер SAML.</span><span class="sxs-lookup"><span data-stu-id="39493-211">In addition to the basic claims, configure the following claims for Azure AD to emit in the SAML token:</span></span>

| <span data-ttu-id="39493-212">Имя утверждения</span><span class="sxs-lookup"><span data-stu-id="39493-212">Claim name</span></span> | <span data-ttu-id="39493-213">Источник</span><span class="sxs-lookup"><span data-stu-id="39493-213">Source</span></span>  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | <span data-ttu-id="39493-214">assignedroles</span><span class="sxs-lookup"><span data-stu-id="39493-214">assignedroles</span></span>| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | <span data-ttu-id="39493-215">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="39493-215">userprincipalname</span></span> |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | <span data-ttu-id="39493-216">"900"</span><span class="sxs-lookup"><span data-stu-id="39493-216">"900"</span></span> |
| <span data-ttu-id="39493-217">roles</span><span class="sxs-lookup"><span data-stu-id="39493-217">roles</span></span> | <span data-ttu-id="39493-218">assignedroles</span><span class="sxs-lookup"><span data-stu-id="39493-218">assignedroles</span></span> |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | <span data-ttu-id="39493-219">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="39493-219">userprincipalname</span></span> |

<span data-ttu-id="39493-220">Дополнительные сведения см. в статье [Настройка утверждений, добавляемых в маркеры](/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="39493-220">For more information, see [Customize claims emitted in token](/azure/active-directory/develop/active-directory-claims-mapping).</span></span>

> [!NOTE]
> <span data-ttu-id="39493-221">Некоторые ключи в политике сопоставления утверждений чувствительны к регистру (например, "Version").</span><span class="sxs-lookup"><span data-stu-id="39493-221">Some keys in the claims mapping policy are case sensitive (for example, "Version").</span></span> <span data-ttu-id="39493-222">Если появляется сообщение об ошибке "Свойство имеет недопустимое значение", это может быть проблема, связанная с регистром.</span><span class="sxs-lookup"><span data-stu-id="39493-222">If you receive an error message such as "Property has an invalid value", it might be a case sensitive issue.</span></span>

#### <a name="request"></a><span data-ttu-id="39493-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="39493-223">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="39493-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="39493-224">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: application/json

{
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Value\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims Policy",
    "isOrganizationDefault": false
}
```
# <a name="c"></a>[<span data-ttu-id="39493-225">C#</span><span class="sxs-lookup"><span data-stu-id="39493-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39493-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39493-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39493-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39493-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39493-228">Java</span><span class="sxs-lookup"><span data-stu-id="39493-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39493-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="39493-229">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicies",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/claimsMappingPolicies/$entity",
    "id": "a7b19e62-9adb-4edb-8521-cd35305f095d",
    "deletedDateTime": null,
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Value\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims Policy",
    "isOrganizationDefault": false
}
```

### <a name="assign-claims-mapping-policy-to-service-principal"></a><span data-ttu-id="39493-230">Назначение политики сопоставления утверждений субъекту-службе</span><span class="sxs-lookup"><span data-stu-id="39493-230">Assign claims mapping policy to service principal</span></span>

#### <a name="request"></a><span data-ttu-id="39493-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="39493-231">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/claimsMappingPolicies/$ref

Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/6b33aa8e-51f3-41a6-a0fd-d660d276197a"
}
```


#### <a name="response"></a><span data-ttu-id="39493-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="39493-232">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-4-configure-signing-certificate"></a><span data-ttu-id="39493-233">Шаг 4. Настройка сертификата для подписи</span><span class="sxs-lookup"><span data-stu-id="39493-233">Step 4: Configure signing certificate</span></span>

<span data-ttu-id="39493-234">При использовании API [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-beta)сертификат для подписи не создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="39493-234">Using the [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-beta) API doesn't create a signing certificate by default.</span></span> <span data-ttu-id="39493-235">Создайте пользовательский сертификат для подписи и назначьте его приложению.</span><span class="sxs-lookup"><span data-stu-id="39493-235">Create your custom signing cert and assign it to the application.</span></span> 

### <a name="create-a-custom-signing-certificate"></a><span data-ttu-id="39493-236">Создание пользовательского сертификата для подписи</span><span class="sxs-lookup"><span data-stu-id="39493-236">Create a custom signing certificate</span></span>

<span data-ttu-id="39493-237">Для целей тестирования можно создать самозаверяющий сертификат с помощью следующих команд PowerShell.</span><span class="sxs-lookup"><span data-stu-id="39493-237">To test, you can use the following PowerShell command to get a self-signed certificate.</span></span> <span data-ttu-id="39493-238">Затем потребуется вручную обработать и извлечь нужные значения с помощью других средств.</span><span class="sxs-lookup"><span data-stu-id="39493-238">You will then need to manipulate and pull the values you need manually using other tools.</span></span> <span data-ttu-id="39493-239">При создании сертификата для подписи в рабочей среде применяйте все самые передовые рекомендации по безопасности, используемые в вашей компании.</span><span class="sxs-lookup"><span data-stu-id="39493-239">Use the best security practice from your company to create a signing certificate for production.</span></span>

```powershell
Param(
    [Parameter(Mandatory=$true)]
    [string]$fqdn,
    [Parameter(Mandatory=$true)]
    [string]$pwd,
    [Parameter(Mandatory=$true)]
    [string]$location
) 

if (!$PSBoundParameters.ContainsKey('location'))
{
    $location = "."
} 

$cert = New-SelfSignedCertificate -certstorelocation cert:\currentuser\my -DnsName $fqdn
$pwdSecure = ConvertTo-SecureString -String $pwd -Force -AsPlainText
$path = 'cert:\currentuser\my\' + $cert.Thumbprint
$cerFile = $location + "\\" + $fqdn + ".cer"
$pfxFile = $location + "\\" + $fqdn + ".pfx" 

Export-PfxCertificate -cert $path -FilePath $pfxFile -Password $pwdSecure
Export-Certificate -cert $path -FilePath $cerFile
```

<span data-ttu-id="39493-240">Кроме того, в качестве подтверждения концепции можно использовать следующее консольное приложение C#, чтобы понять, как можно получить необходимые значения.</span><span class="sxs-lookup"><span data-stu-id="39493-240">Alternatively, the following C# console app can be used as a Proof of Concept to understand how the required values can be obtained.</span></span> <span data-ttu-id="39493-241">Обратите внимание, что этот код предназначен **ТОЛЬКО для обучения и справочных материалов** и не должен использоваться "как есть" в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="39493-241">Note that this code is for **learning and reference ONLY** and should not be used as-is in production.</span></span>

```csharp
using System;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;
using System.Text;


/* CONSOLE APP - PROOF OF CONCEPT CODE ONLY!!
 * This code uses a self signed certificate and should not be used 
 * in production. This code is for reference and learning ONLY.
 */
namespace Self_signed_cert
{
    class Program
    {
        static void Main(string[] args)
        {
            // Generate a guid to use as a password and then create the cert.
            string password = Guid.NewGuid().ToString();
            var selfsignedCert = buildSelfSignedServerCertificate(password);

            // Print values so we can copy paste into the JSON fields.
            // Print out the private key in base64 format.
            Console.WriteLine("Private Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Pfx, password)), Environment.NewLine);

            // Print out the start date in ISO 8601 format.
            DateTime startDate = DateTime.Parse(selfsignedCert.GetEffectiveDateString()).ToUniversalTime();
            Console.WriteLine("For All startDateTime: " + startDate.ToString("o"));

            // Print out the end date in ISO 8601 format.
            DateTime endDate = DateTime.Parse(selfsignedCert.GetExpirationDateString()).ToUniversalTime();
            Console.WriteLine("For All endDateTime: " + endDate.ToString("o"));

            // Print the GUID used for keyId
            string signAndPasswordGuid = Guid.NewGuid().ToString();
            string verifyGuid = Guid.NewGuid().ToString();
            Console.WriteLine("GUID to use for keyId for keyCredentials->Usage == Sign and passwordCredentials: " + signAndPasswordGuid);
            Console.WriteLine("GUID to use for keyId for keyCredentials->Usage == Verify: " + verifyGuid);

            // Print out the password.
            Console.WriteLine("Password is: {0}", password);

            // Print out a displayName to use as an example.
            Console.WriteLine("displayName to use: CN=Example");
            Console.WriteLine();

            // Print out the public key.
            Console.WriteLine("Public Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Cert)), Environment.NewLine);
            Console.WriteLine();

            // Generate the customKeyIdentifier using hash of thumbprint.
            Console.WriteLine("You can generate the customKeyIdentifier by getting the SHA256 hash of the certs thumprint.\nThe certs thumbprint is: {0}{1}", selfsignedCert.Thumbprint, Environment.NewLine);
            Console.WriteLine("The hash of the thumbprint that we will use for customeKeyIdentifier is:");
            string keyIdentifier = GetSha256FromThumbprint(selfsignedCert.Thumbprint);
            Console.WriteLine(keyIdentifier);
        }

        // Generate a self-signed certificate.
        private static X509Certificate2 buildSelfSignedServerCertificate(string password)
        {
            const string CertificateName = @"Microsoft Azure Federated SSO Certificate TEST";
            DateTime certificateStartDate = DateTime.UtcNow;
            DateTime certificateEndDate = certificateStartDate.AddYears(2).ToUniversalTime();

            X500DistinguishedName distinguishedName = new X500DistinguishedName($"CN={CertificateName}");

            using (RSA rsa = RSA.Create(2048))
            {
                var request = new CertificateRequest(distinguishedName, rsa, HashAlgorithmName.SHA256, RSASignaturePadding.Pkcs1);

                request.CertificateExtensions.Add(
                    new X509KeyUsageExtension(X509KeyUsageFlags.DataEncipherment | X509KeyUsageFlags.KeyEncipherment | X509KeyUsageFlags.DigitalSignature, false));

                var certificate = request.CreateSelfSigned(new DateTimeOffset(certificateStartDate), new DateTimeOffset(certificateEndDate));
                certificate.FriendlyName = CertificateName;

                return new X509Certificate2(certificate.Export(X509ContentType.Pfx, password), password, X509KeyStorageFlags.Exportable);
            }
        }

        // Generate hash from thumbprint.
        public static string GetSha256FromThumbprint(string thumbprint)
        {
            var message = Encoding.ASCII.GetBytes(thumbprint);
            SHA256Managed hashString = new SHA256Managed();
            return Convert.ToBase64String(hashString.ComputeHash(message));
        }
    }
}
```

### <a name="add-a-custom-signing-key"></a><span data-ttu-id="39493-242">Добавление пользовательского ключа подписывания</span><span class="sxs-lookup"><span data-stu-id="39493-242">Add a custom signing key</span></span>

<span data-ttu-id="39493-243">Добавьте следующие сведения в субъект-службу.</span><span class="sxs-lookup"><span data-stu-id="39493-243">Add the following information to the service principal:</span></span>

* <span data-ttu-id="39493-244">Закрытый ключ</span><span class="sxs-lookup"><span data-stu-id="39493-244">Private key</span></span>
* <span data-ttu-id="39493-245">Пароль</span><span class="sxs-lookup"><span data-stu-id="39493-245">Password</span></span>
* <span data-ttu-id="39493-246">Открытый ключ</span><span class="sxs-lookup"><span data-stu-id="39493-246">Public key</span></span> 

<span data-ttu-id="39493-247">Извлеките закрытый и открытый ключи в кодировке Base64 из PFX-файла.</span><span class="sxs-lookup"><span data-stu-id="39493-247">Extract the private and public key Base64 encoded from the PFX file.</span></span> <span data-ttu-id="39493-248">Дополнительные сведения об их свойствах см. в описании [типа ресурса keyCredential](/graph/api/resources/keycredential?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="39493-248">To learn more about the properties, see [keyCredential resource type](/graph/api/resources/keycredential?view=graph-rest-1.0).</span></span>

<span data-ttu-id="39493-249">Убедитесь, что значение keyId для keyCredential, примененное для параметра Sign, соответствует значению keyId для passwordCredential.</span><span class="sxs-lookup"><span data-stu-id="39493-249">Make sure that the keyId for the keyCredential used for "Sign" matches the keyId of the passwordCredential.</span></span> <span data-ttu-id="39493-250">Вы можете создать `customkeyIdentifier`, получив хэш отпечатка сертификата.</span><span class="sxs-lookup"><span data-stu-id="39493-250">You can generate the `customkeyIdentifier` by getting the hash of the cert's thumbprint.</span></span> <span data-ttu-id="39493-251">См. предыдущий код ссылки C#.</span><span class="sxs-lookup"><span data-stu-id="39493-251">See the previous C# reference code.</span></span>

#### <a name="request"></a><span data-ttu-id="39493-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="39493-252">Request</span></span>

> [!NOTE]
> <span data-ttu-id="39493-253">Значение key в свойстве keyCredentials сокращено для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="39493-253">The "key" value in the keyCredentials property is shortened for readability.</span></span> <span data-ttu-id="39493-254">Значение представлено в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="39493-254">The value is base 64 encoded.</span></span> <span data-ttu-id="39493-255">Для закрытого ключа свойство `usage` имеет значение "Sign".</span><span class="sxs-lookup"><span data-stu-id="39493-255">For the private key the property `usage` is "Sign".</span></span> <span data-ttu-id="39493-256">Для открытого ключа свойство `usage` имеет значение "Verify".</span><span class="sxs-lookup"><span data-stu-id="39493-256">For the public key the property `usage` is "Verify".</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: application/json

{
    "keyCredentials":[
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "endDateTime": "2021-04-22T22:10:13Z",
            "keyId": "4c266507-3e74-4b91-aeba-18a25b450f6e",
            "startDateTime": "2020-04-22T21:50:13Z",
            "type": "X509CertAndPassword",
            "usage": "Sign",
            "key":"MIIKIAIBAz.....HBgUrDgMCERE20nuTptI9MEFCh2Ih2jaaLZBZGeZBRFVNXeZmAAgIH0A==",
            "displayName": "CN=awsAPI"
        },
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "endDateTime": "2021-04-22T22:10:13Z",
            "keyId": "e35a7d11-fef0-49ad-9f3e-aacbe0a42c42",
            "startDateTime": "2020-04-22T21:50:13Z",
            "type": "AsymmetricX509Cert",
            "usage": "Verify",
            "key": "MIIDJzCCAg+gAw......CTxQvJ/zN3bafeesMSueR83hlCSyg==",
            "displayName": "CN=awsAPI"
        }

    ],
    "passwordCredentials": [
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "keyId": "4c266507-3e74-4b91-aeba-18a25b450f6e",
            "endDateTime": "2022-01-27T19:40:33Z",
            "startDateTime": "2020-04-20T19:40:33Z",
            "secretText": "61891f4ee44d"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="39493-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="39493-257">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a><span data-ttu-id="39493-258">Активация пользовательского ключа подписывания</span><span class="sxs-lookup"><span data-stu-id="39493-258">Activate the custom signing key</span></span>

<span data-ttu-id="39493-259">Вам нужно задать для свойства `preferredTokenSigningKeyThumbprint` значение отпечатка сертификата, с помощью которого Azure AD будет подписывать ответ SAML.</span><span class="sxs-lookup"><span data-stu-id="39493-259">You need to set the `preferredTokenSigningKeyThumbprint` property to the thumbprint of the certificate you want Azure AD to use to sign the SAML response.</span></span> 

#### <a name="request"></a><span data-ttu-id="39493-260">Запрос</span><span class="sxs-lookup"><span data-stu-id="39493-260">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: application/json

{
    "preferredTokenSigningKeyThumbprint": "AC09FEF18DDE6983EE2A164FBA3C4DD7518BD787"
}
```

#### <a name="response"></a><span data-ttu-id="39493-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="39493-261">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```
## <a name="step-5-assign-users"></a><span data-ttu-id="39493-262">Шаг 5. Назначение пользователей</span><span class="sxs-lookup"><span data-stu-id="39493-262">Step 5: Assign users</span></span>

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="39493-263">Назначение пользователей и групп для приложения</span><span class="sxs-lookup"><span data-stu-id="39493-263">Assign users and groups to the application</span></span>

<span data-ttu-id="39493-264">Назначьте субъекту-службе следующего пользователя и роль AWS_Role1.</span><span class="sxs-lookup"><span data-stu-id="39493-264">Assign the following user to the service principal and assign the AWS_Role1.</span></span> 

| <span data-ttu-id="39493-265">Имя</span><span class="sxs-lookup"><span data-stu-id="39493-265">Name</span></span>  | <span data-ttu-id="39493-266">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="39493-266">ID</span></span>  |
|---------|---------|
| <span data-ttu-id="39493-267">Идентификатор пользователя (principalId)</span><span class="sxs-lookup"><span data-stu-id="39493-267">User ID (principalId)</span></span> | <span data-ttu-id="39493-268">6cad4079-4e79-4a3f-9efb-ea30a14bdb26</span><span class="sxs-lookup"><span data-stu-id="39493-268">6cad4079-4e79-4a3f-9efb-ea30a14bdb26</span></span> |
| <span data-ttu-id="39493-269">Тип (principalType)</span><span class="sxs-lookup"><span data-stu-id="39493-269">Type (principalType)</span></span> | <span data-ttu-id="39493-270">Пользователь</span><span class="sxs-lookup"><span data-stu-id="39493-270">User</span></span> |
| <span data-ttu-id="39493-271">Идентификатор роли приложения (appRoleId)</span><span class="sxs-lookup"><span data-stu-id="39493-271">App role ID (appRoleId)</span></span> | <span data-ttu-id="39493-272">454dc4c2-8176-498e-99df-8c4efcde41ef</span><span class="sxs-lookup"><span data-stu-id="39493-272">454dc4c2-8176-498e-99df-8c4efcde41ef</span></span> |
| <span data-ttu-id="39493-273">Идентификатор субъекта-службы (resourceId)</span><span class="sxs-lookup"><span data-stu-id="39493-273">servicePrincipalID (resourceId)</span></span> | <span data-ttu-id="39493-274">f47a6776-bca7-4f2e-bc6c-eec59d058e3e</span><span class="sxs-lookup"><span data-stu-id="39493-274">f47a6776-bca7-4f2e-bc6c-eec59d058e3e</span></span> |

#### <a name="request"></a><span data-ttu-id="39493-275">Запрос</span><span class="sxs-lookup"><span data-stu-id="39493-275">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/appRoleAssignments

Content-type: application/json

{
  "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
  "principalType": "User",
  "appRoleId":"454dc4c2-8176-498e-99df-8c4efcde41ef",
  "resourceId":"f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```

#### <a name="response"></a><span data-ttu-id="39493-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="39493-276">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 201 
Content-type: application/json

{
    "id": "rq7hyzl4yECaNZleMrTpDV-OCe5TEl5Ao_o76XMrRFU",
    "creationTimestamp": "2020-04-23T17:38:13.2508567Z",
    "appRoleId": "454dc4c2-8176-498e-99df-8c4efcde41ef",
    "principalDisplayName": "User 1",
    "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
    "principalType": "User",
    "resourceDisplayName": "AWS API Created",
    "resourceId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```

<span data-ttu-id="39493-277">Подробнее см. в описании [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="39493-277">For more information, see [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-1.0).</span></span>

## <a name="step-6-configure-the-application-side"></a><span data-ttu-id="39493-278">Шаг 6. Настройка на стороне приложения</span><span class="sxs-lookup"><span data-stu-id="39493-278">Step 6: Configure the application side</span></span>

### <a name="get-azure-ad-saml-metadata"></a><span data-ttu-id="39493-279">Получение метаданных SAML из Azure AD</span><span class="sxs-lookup"><span data-stu-id="39493-279">Get Azure AD SAML metadata</span></span>

<span data-ttu-id="39493-280">Используйте следующий URL-адрес, чтобы получить метаданные SAML из Azure AD для конкретного настроенного приложения.</span><span class="sxs-lookup"><span data-stu-id="39493-280">Use the following URL to get the Azure AD SAML metadata for the specific configured application.</span></span> <span data-ttu-id="39493-281">Эти метаданные содержат такие сведения, как сертификат для подписи, идентификатор сущности Azure AD (entityID), служба единого входа Azure AD (SingleSignOnService) и т. д.</span><span class="sxs-lookup"><span data-stu-id="39493-281">The metadata contains information such as the signing certificate, Azure AD entityID, and Azure AD SingleSignOnService, among others.</span></span>

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

> [!NOTE]
> <span data-ttu-id="39493-282">Приложение должно быть способно анализировать метку порядка байтов из XML-данных метаданных федерации, отображаемую с помощью `https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`.</span><span class="sxs-lookup"><span data-stu-id="39493-282">The application should be capable of parsing the byte order mark present in the federation metadata XML data rendered using `https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`.</span></span> <span data-ttu-id="39493-283">Метка порядка байтов представлена в виде непечатаемого символа ASCII `»¿` и в шестнадцатеричном формате выглядит как `EF BB BF` при просмотре XML-данных.</span><span class="sxs-lookup"><span data-stu-id="39493-283">Byte order mark is represented as a nonprintable ASCII character `»¿` and in Hex it is represented as `EF BB BF` when reviewing the XML data.</span></span>

 

## <a name="next-steps"></a><span data-ttu-id="39493-284">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="39493-284">Next steps</span></span>
- [<span data-ttu-id="39493-285">Настройка подготовки пользователей с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="39493-285">Use Microsoft Graph APIs to configure user provisioning</span></span>](/azure/active-directory/app-provisioning/application-provisioning-configure-api)
- [<span data-ttu-id="39493-286">Использование отчета о действиях приложения AD FS для миграции приложений в Azure AD</span><span class="sxs-lookup"><span data-stu-id="39493-286">Use the AD FS application activity report to migrate applications to Azure AD</span></span>](/azure/active-directory/manage-apps/migrate-adfs-application-activity)
