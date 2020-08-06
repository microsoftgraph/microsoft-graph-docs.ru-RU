---
title: Настройка единого входа на основе SAML с помощью API Microsoft Graph
description: Узнайте, как экономить время с помощью API Microsoft Graph, чтобы автоматизировать настройку единого входа на основе SAML.
author: kenwith
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: b4e2c02fb5583febdaee7eb2e20bca7083b32635
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567472"
---
# <a name="automate-saml-based-sso-app-configuration-with-microsoft-graph-api"></a><span data-ttu-id="02f79-103">Автоматизация настройки единого входа на основе SAML для приложений с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="02f79-103">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>

<span data-ttu-id="02f79-104">Из этой статьи вы узнаете, как создать и настроить приложение из коллекции Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="02f79-104">In this article, you'll learn how to create and configure an application from the Azure Active Directory (Azure AD) Gallery.</span></span> <span data-ttu-id="02f79-105">В этой статье в качестве примера используется AWS, но описанные в этой статье шаги можно применить для любого другого приложения на основе SAML, включенного в коллекцию Azure AD.</span><span class="sxs-lookup"><span data-stu-id="02f79-105">This article uses AWS as an example but you can use the steps in this article for any SAML-based app in the Azure AD Gallery.</span></span>

<span data-ttu-id="02f79-106">**Шаги по автоматизации настройки единого входа на основе SAML с помощью API Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="02f79-106">**Steps to use Microsoft Graph APIs to automate configuration of SAML-based single sign-on**</span></span>

| <span data-ttu-id="02f79-107">Шаг</span><span class="sxs-lookup"><span data-stu-id="02f79-107">Step</span></span>  | <span data-ttu-id="02f79-108">Сведения</span><span class="sxs-lookup"><span data-stu-id="02f79-108">Details</span></span>  |
|---------|---------|
| [<span data-ttu-id="02f79-109">1. Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="02f79-109">1. Create the gallery application</span></span>](#step-1-create-the-gallery-application) | <span data-ttu-id="02f79-110">Вход в клиент API</span><span class="sxs-lookup"><span data-stu-id="02f79-110">Sign in to the API client</span></span> <br> <span data-ttu-id="02f79-111">Получение приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="02f79-111">Retrieve the gallery application</span></span> <br> <span data-ttu-id="02f79-112">Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="02f79-112">Create the gallery application</span></span>|
| [<span data-ttu-id="02f79-113">2. Настройка единого входа</span><span class="sxs-lookup"><span data-stu-id="02f79-113">2. Configure single sign-on</span></span>](#step-2-configure-single-sign-on) | <span data-ttu-id="02f79-114">Получение идентификаторов объектов для приложения и субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="02f79-114">Retrieve app object ID and service principal object ID</span></span> <br> <span data-ttu-id="02f79-115">Настройка режима единого входа</span><span class="sxs-lookup"><span data-stu-id="02f79-115">Set single sign-on mode</span></span> <br> <span data-ttu-id="02f79-116">Настройка основных URL-адресов SAML, таких как идентификатор, URL-адрес ответа и URL-адрес входа</span><span class="sxs-lookup"><span data-stu-id="02f79-116">Set basic SAML URLs such as identifier, reply URL, sign-on URL</span></span> <br> <span data-ttu-id="02f79-117">Добавление ролей приложения (необязательно)</span><span class="sxs-lookup"><span data-stu-id="02f79-117">Add app roles (Optional)</span></span>|
| [<span data-ttu-id="02f79-118">3. Настройка сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="02f79-118">3. Configure claims mapping</span></span>](#step-3-configure-claims-mapping) | <span data-ttu-id="02f79-119">Создание политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="02f79-119">Create claims mapping policy</span></span> <br> <span data-ttu-id="02f79-120">Назначение политики сопоставления утверждений субъекту-службе</span><span class="sxs-lookup"><span data-stu-id="02f79-120">Assign claims mapping policy to service principal</span></span>|
| [<span data-ttu-id="02f79-121">4. Настройка сертификата для подписи</span><span class="sxs-lookup"><span data-stu-id="02f79-121">4. Configure signing certificate</span></span>](#step-4-configure-signing-certificate) | <span data-ttu-id="02f79-122">Создание сертификата</span><span class="sxs-lookup"><span data-stu-id="02f79-122">Create a certificate</span></span> <BR> <span data-ttu-id="02f79-123">Добавление пользовательского ключа подписывания</span><span class="sxs-lookup"><span data-stu-id="02f79-123">Add a custom signing key</span></span> <br> <span data-ttu-id="02f79-124">Активация пользовательского ключа подписывания</span><span class="sxs-lookup"><span data-stu-id="02f79-124">Activate the custom signing key</span></span>|
| [<span data-ttu-id="02f79-125">5. Назначение пользователей</span><span class="sxs-lookup"><span data-stu-id="02f79-125">5. Assign users</span></span>](#step-5-assign-users) | <span data-ttu-id="02f79-126">Назначение пользователей и групп для приложения</span><span class="sxs-lookup"><span data-stu-id="02f79-126">Assign users and groups to the application</span></span>
| [<span data-ttu-id="02f79-127">6. Настройка на стороне приложения</span><span class="sxs-lookup"><span data-stu-id="02f79-127">6. Configure the application side</span></span>](#step-6-configure-the-application-side)| <span data-ttu-id="02f79-128">Получение метаданных SAML из Azure AD</span><span class="sxs-lookup"><span data-stu-id="02f79-128">Get Azure AD SAML metadata</span></span>

<span data-ttu-id="02f79-129">**Список всех API, используемых в этой документации**</span><span class="sxs-lookup"><span data-stu-id="02f79-129">**List of all APIs used in the documentation**</span></span>

<span data-ttu-id="02f79-130">Убедитесь, что у вас есть соответствующие разрешения для вызова следующих API.</span><span class="sxs-lookup"><span data-stu-id="02f79-130">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="02f79-131">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="02f79-131">Resource type</span></span> |<span data-ttu-id="02f79-132">Метод</span><span class="sxs-lookup"><span data-stu-id="02f79-132">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="02f79-133">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="02f79-133">applicationTemplate</span></span>](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta)|[<span data-ttu-id="02f79-134">Перечисление applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="02f79-134">List applicationTemplate</span></span>](https://docs.microsoft.com/graph/api/applicationtemplate-list?view=graph-rest-beta&tabs=http) <br>[<span data-ttu-id="02f79-135">Создание экземпляра applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="02f79-135">Instantiate applicationTemplate</span></span>](https://docs.microsoft.com/graph/api/applicationtemplate-instantiate?view=graph-rest-beta&tabs=http)|
|[<span data-ttu-id="02f79-136">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="02f79-136">servicePrincipals</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="02f79-137">Обновление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="02f79-137">Update servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [<span data-ttu-id="02f79-138">Создание appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="02f79-138">Create appRoleAssignments</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-1.0&tabs=http) <br> [<span data-ttu-id="02f79-139">Назначение claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="02f79-139">Assign claimsMappingPolicies</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-claimsmappingpolicies?view=graph-rest-beta&tabs=http)|
|[<span data-ttu-id="02f79-140">applications</span><span class="sxs-lookup"><span data-stu-id="02f79-140">applications</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)|[<span data-ttu-id="02f79-141">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="02f79-141">Update application</span></span>](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-1.0&tabs=http)|
|[<span data-ttu-id="02f79-142">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="02f79-142">claimsMappingPolicy</span></span>](https://docs.microsoft.com/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)| [<span data-ttu-id="02f79-143">Создание claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="02f79-143">Create claimsMappingPolicy</span></span>](https://docs.microsoft.com/graph/api/claimsmappingpolicy-post-claimsmappingpolicies?view=graph-rest-beta&tabs=http)

>[!NOTE]
><span data-ttu-id="02f79-144">Объекты отклика, приведенные в этой статье, могут быть сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="02f79-144">The response objects shown in this article may be shortened for readability.</span></span> <span data-ttu-id="02f79-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02f79-145">All the properties will be returned from an actual call.</span></span>

## <a name="step-1-create-the-gallery-application"></a><span data-ttu-id="02f79-146">Шаг 1. Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="02f79-146">Step 1: Create the gallery application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="02f79-147">Вход в песочницу Microsoft Graph (рекомендуется), Postman или любой другой используемый клиент API</span><span class="sxs-lookup"><span data-stu-id="02f79-147">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="02f79-148">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer)</span><span class="sxs-lookup"><span data-stu-id="02f79-148">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer)</span></span>
2. <span data-ttu-id="02f79-149">Выберите вариант **Вход с помощью учетной записи Майкрософт** и войдите, используя учетные данные глобального администратора Azure AD или администратора приложения.</span><span class="sxs-lookup"><span data-stu-id="02f79-149">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="02f79-150">После успешного входа вы увидите данные учетной записи пользователя на панели слева.</span><span class="sxs-lookup"><span data-stu-id="02f79-150">Upon successful sign-in, you'll see the user account details in the left-hand pane.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="02f79-151">Получение идентификатора шаблона для приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="02f79-151">Retrieve the gallery application template identifier</span></span>

<span data-ttu-id="02f79-152">У каждого приложения в коллекции приложений Azure AD есть [шаблон](https://docs.microsoft.com/graph/api/applicationtemplate-list?view=graph-rest-beta&tabs=http), описывающий метаданные для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="02f79-152">Applications in the Azure AD application gallery each have an [application template](https://docs.microsoft.com/graph/api/applicationtemplate-list?view=graph-rest-beta&tabs=http) that describes the metadata for that application.</span></span> <span data-ttu-id="02f79-153">По этому шаблону вы можете создать экземпляр приложения и субъект-службу в клиенте для управления им.</span><span class="sxs-lookup"><span data-stu-id="02f79-153">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span>

#### <a name="request"></a><span data-ttu-id="02f79-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f79-154">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```

#### <a name="response"></a><span data-ttu-id="02f79-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f79-155">Response</span></span>

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

### <a name="create-the-gallery-application"></a><span data-ttu-id="02f79-156">Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="02f79-156">Create the gallery application</span></span>

<span data-ttu-id="02f79-157">Используя идентификатор шаблона, полученный для приложения на предыдущем шаге, [создайте экземпляр](https://docs.microsoft.com/graph/api/applicationtemplate-instantiate?view=graph-rest-beta&tabs=http) приложения и субъект-службу в клиенте.</span><span class="sxs-lookup"><span data-stu-id="02f79-157">Using the template ID that you retrieved for your application in the last step, [create an instance](https://docs.microsoft.com/graph/api/applicationtemplate-instantiate?view=graph-rest-beta&tabs=http) of the application and service principal in your tenant.</span></span>

> [!NOTE] 
> <span data-ttu-id="02f79-158">Вы можете использовать API applicationTemplate для создания экземпляров [приложений не из коллекции](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal).</span><span class="sxs-lookup"><span data-stu-id="02f79-158">You can use applicationTemplate API to instantiate [Non-Gallery apps](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal).</span></span> <span data-ttu-id="02f79-159">Используйте applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span><span class="sxs-lookup"><span data-stu-id="02f79-159">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

> [!NOTE]
> <span data-ttu-id="02f79-160">Подождите некоторое время, пока приложение будет подготовлено в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="02f79-160">Allow some time for the app to be provisioned into your Azure AD tenant.</span></span> <span data-ttu-id="02f79-161">Это не происходит сразу.</span><span class="sxs-lookup"><span data-stu-id="02f79-161">It is not instant.</span></span> <span data-ttu-id="02f79-162">Одной из стратегий является выполнение запроса GET для объекта приложения или субъекта-службы каждые 5–10 секунд до тех пор, пока запрос не будет успешным.</span><span class="sxs-lookup"><span data-stu-id="02f79-162">One strategy is to do a GET query on the application / service principal object every 5-10 seconds until the query is successful.</span></span>


#### <a name="request"></a><span data-ttu-id="02f79-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f79-163">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="02f79-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f79-164">Response</span></span>


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

## <a name="step-2-configure-single-sign-on"></a><span data-ttu-id="02f79-165">Шаг 2. Настройка единого входа</span><span class="sxs-lookup"><span data-stu-id="02f79-165">Step 2: Configure single sign-on</span></span>

### <a name="retrieve-app-object-id-and-service-principal-object-id"></a><span data-ttu-id="02f79-166">Получение идентификаторов объектов для приложения и субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="02f79-166">Retrieve app object ID and service principal object ID</span></span>

<span data-ttu-id="02f79-167">Из отклика на предыдущий вызов извлеките и сохраните идентификаторы объекта для приложения и субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="02f79-167">Use the response from the previous call to retrieve and save the application object ID and service principal object ID.</span></span>

```
"application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63"
}
"servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```
### <a name="set-single-sign-on-mode"></a><span data-ttu-id="02f79-168">Настройка режима единого входа</span><span class="sxs-lookup"><span data-stu-id="02f79-168">Set single sign-on mode</span></span>

<span data-ttu-id="02f79-169">В этом примере вы настроите режим единого входа `saml` для [типа ресурса servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="02f79-169">In this example, you'll set `saml` as the single sign-on mode in the [servicePrincipal resource type](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0).</span></span> <span data-ttu-id="02f79-170">Также вы можете настроить другие свойства единого входа SAML: `notificationEmailAddresses`, `loginUrl` и `samlSingleSignOnSettings.relayState`</span><span class="sxs-lookup"><span data-stu-id="02f79-170">Other SAML SSO properties that you can configure are: `notificationEmailAddresses`, `loginUrl`, and `samlSingleSignOnSettings.relayState`</span></span>

<span data-ttu-id="02f79-171">Прежде чем этот запрос заработает, необходимо предоставить согласие на вкладке **Изменить разрешения** в песочнице Graph.</span><span class="sxs-lookup"><span data-stu-id="02f79-171">Before this query will work you need to provide consent on the **Modify permissions** tab in Graph Explorer.</span></span> <span data-ttu-id="02f79-172">Кроме того, используйте идентификатор **servicePrincipal**, полученный ранее.</span><span class="sxs-lookup"><span data-stu-id="02f79-172">Also, make sure you are using the **servicePrincipal** id obtained earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="02f79-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f79-173">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: servicePrincipal/json

{
    "preferredSingleSignOnMode": "saml"
}
```

#### <a name="response"></a><span data-ttu-id="02f79-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f79-174">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls-such-as-identifier-reply-url-sign-on-url"></a><span data-ttu-id="02f79-175">Настройка основных URL-адресов SAML, таких как идентификатор, URL-адрес ответа и URL-адрес входа</span><span class="sxs-lookup"><span data-stu-id="02f79-175">Set basic SAML URLs such as identifier, reply URL, sign-on URL</span></span>

<span data-ttu-id="02f79-176">Настройте идентификатор и URL-адреса ответа для AWS в объекте приложения.</span><span class="sxs-lookup"><span data-stu-id="02f79-176">Set the identifier and reply URLs for AWS in the application object.</span></span>

<span data-ttu-id="02f79-177">Используйте идентификатор **application**, полученный ранее.</span><span class="sxs-lookup"><span data-stu-id="02f79-177">Make sure you are using the **application** id obtained earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="02f79-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f79-178">Request</span></span>

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
#### <a name="response"></a><span data-ttu-id="02f79-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f79-179">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204
```
### <a name="add-app-roles-optional"></a><span data-ttu-id="02f79-180">Добавление ролей приложения (необязательно)</span><span class="sxs-lookup"><span data-stu-id="02f79-180">Add app roles (Optional)</span></span>

<span data-ttu-id="02f79-181">Если приложение ожидает получить сведения о роли в маркере, добавьте определение ролей в объект приложения.</span><span class="sxs-lookup"><span data-stu-id="02f79-181">If the application requires the role information in the token, add the definition of the roles in the application object.</span></span> <span data-ttu-id="02f79-182">Для AWS вы можете [включить подготовку пользователя](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api), чтобы автоматически получать все роли из учетной записи AWS.</span><span class="sxs-lookup"><span data-stu-id="02f79-182">For AWS, you can [enable user provisioning](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api) to fetch all the roles from that AWS account.</span></span> 

<span data-ttu-id="02f79-183">Дополнительные сведения см. в статье [Настройка утверждения роли, выдаваемого в маркере SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span><span class="sxs-lookup"><span data-stu-id="02f79-183">For more information, read [Configure the role claim issued in the SAML token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)</span></span>

> [!NOTE] 
> <span data-ttu-id="02f79-184">При добавлении ролей приложения не изменяйте стандартные роли приложения msiam_access.</span><span class="sxs-lookup"><span data-stu-id="02f79-184">When adding app roles, don't modify the default app roles msiam_access.</span></span> 

#### <a name="request"></a><span data-ttu-id="02f79-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f79-185">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/serviceprincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: serviceprincipals/json

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

#### <a name="response"></a><span data-ttu-id="02f79-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f79-186">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a><span data-ttu-id="02f79-187">Шаг 3. Настройка сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="02f79-187">Step 3: Configure claims mapping</span></span>

### <a name="create-claims-mapping-policy"></a><span data-ttu-id="02f79-188">Создание политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="02f79-188">Create claims mapping policy</span></span>

<span data-ttu-id="02f79-189">В дополнение к основным утверждениям настройте следующие, чтобы служба Azure AD включала их в маркер SAML.</span><span class="sxs-lookup"><span data-stu-id="02f79-189">In addition to the basic claims, configure the following claims for Azure AD to emit in the SAML token:</span></span>

| <span data-ttu-id="02f79-190">Имя утверждения</span><span class="sxs-lookup"><span data-stu-id="02f79-190">Claim name</span></span> | <span data-ttu-id="02f79-191">Источник</span><span class="sxs-lookup"><span data-stu-id="02f79-191">Source</span></span>  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | <span data-ttu-id="02f79-192">assignedroles</span><span class="sxs-lookup"><span data-stu-id="02f79-192">assignedroles</span></span>| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | <span data-ttu-id="02f79-193">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="02f79-193">userprincipalname</span></span> |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | <span data-ttu-id="02f79-194">"900"</span><span class="sxs-lookup"><span data-stu-id="02f79-194">"900"</span></span> |
| <span data-ttu-id="02f79-195">roles</span><span class="sxs-lookup"><span data-stu-id="02f79-195">roles</span></span> | <span data-ttu-id="02f79-196">assignedroles</span><span class="sxs-lookup"><span data-stu-id="02f79-196">assignedroles</span></span> |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | <span data-ttu-id="02f79-197">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="02f79-197">userprincipalname</span></span> |

<span data-ttu-id="02f79-198">Дополнительные сведения см. в статье [Настройка утверждений, добавляемых в маркеры](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="02f79-198">For more information, see [Customize claims emitted in token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>

> [!NOTE]
> <span data-ttu-id="02f79-199">Некоторые ключи в политике сопоставления утверждений чувствительны к регистру (например, "Version").</span><span class="sxs-lookup"><span data-stu-id="02f79-199">Some keys in the claims mapping policy are case sensitive (e.g. "Version").</span></span> <span data-ttu-id="02f79-200">Если появляется сообщение об ошибке "Свойство имеет недопустимое значение", это может быть проблемой, связанной с регистром.</span><span class="sxs-lookup"><span data-stu-id="02f79-200">If you receive an error message such as "Property has an invalid value", it could be a case sensitive issue.</span></span>

#### <a name="request"></a><span data-ttu-id="02f79-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f79-201">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: claimsMappingPolicies/json

{
    "definition":[
            "{\"ClaimsMappingPolicy\": {
                \"Version\": 1,
                \"IncludeBasicClaimSet\": \"true\",
                \"ClaimsSchema\": [
                    {
                        \"Source\": \"user\",
                        \"ID\": \"assignedroles\",
                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"userprincipalname\",
                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"900\",
                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"assignedroles\",
                        \"SamlClaimType\": \"appRoles\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"userprincipalname\",
                        \"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"
                    }
                ]
            }
        }"

    ],
    "displayName": "AWS Claims policy",
    "isOrganizationDefault": false
}
```

#### <a name="response"></a><span data-ttu-id="02f79-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f79-202">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicies",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: claimsMappingPolicies/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/claimsMappingPolicies/$entity",
    "id": "6b33aa8e-51f3-41a6-a0fd-d660d276197a",
    "definition": [
        "{\"ClaimsMappingPolicy\": {\"Version\": 1,\"IncludeBasicClaimSet\": \"true\",\"ClaimsSchema\": [{\"Source\": \"user\",\"ID\": \"assignedroles\",\"SamlClaimType\":\"https://aws.amazon.com/SAML/Attributes/Role\"\r\n                    },{\"Source\": \"user\",\"ID\": \"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"},{\"Source\": \"user\",\"ID\": \"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"},{\"Source\": \"user\",\"ID\": \"assignedroles\",\"SamlClaimType\":\"appRoles\"},{\"Source\": \"user\",\"ID\": \"userprincipalname\",\"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims policy",
    "isOrganizationDefault": false
}
```

### <a name="assign-claims-mapping-policy-to-service-principal"></a><span data-ttu-id="02f79-203">Назначение политики сопоставления утверждений субъекту-службе</span><span class="sxs-lookup"><span data-stu-id="02f79-203">Assign claims mapping policy to service principal</span></span>

#### <a name="request"></a><span data-ttu-id="02f79-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f79-204">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/claimsMappingPolicies/$ref

Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/6b33aa8e-51f3-41a6-a0fd-d660d276197a"
}
```

#### <a name="response"></a><span data-ttu-id="02f79-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f79-205">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-4-configure-signing-certificate"></a><span data-ttu-id="02f79-206">Шаг 4. Настройка сертификата для подписи</span><span class="sxs-lookup"><span data-stu-id="02f79-206">Step 4: Configure signing certificate</span></span>

<span data-ttu-id="02f79-207">При использовании API [applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta)сертификат для подписи не создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="02f79-207">Using the [applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) API doesn't create a signing certificate by default.</span></span> <span data-ttu-id="02f79-208">Создайте пользовательский сертификат для подписи и назначьте его приложению.</span><span class="sxs-lookup"><span data-stu-id="02f79-208">Create your custom signing cert and assign it to the application.</span></span> 

### <a name="create-a-custom-signing-certificate"></a><span data-ttu-id="02f79-209">Создание пользовательского сертификата для подписи</span><span class="sxs-lookup"><span data-stu-id="02f79-209">Create a custom signing certificate</span></span>

<span data-ttu-id="02f79-210">Для целей тестирования можно создать самозаверяющий сертификат с помощью следующих команд PowerShell.</span><span class="sxs-lookup"><span data-stu-id="02f79-210">To test, you can use the following PowerShell command to get a self-signed certificate.</span></span> <span data-ttu-id="02f79-211">Затем потребуется вручную обработать и извлечь нужные значения с помощью других средств.</span><span class="sxs-lookup"><span data-stu-id="02f79-211">You will then need to manipulate and pull the values you need manually using other tools.</span></span> <span data-ttu-id="02f79-212">При создании сертификата для подписи в рабочей среде применяйте все самые передовые рекомендации по безопасности, используемые в вашей компании.</span><span class="sxs-lookup"><span data-stu-id="02f79-212">Use the best security practice from your company to create a signing certificate for production.</span></span>

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

<span data-ttu-id="02f79-213">Кроме того, в качестве подтверждения концепции можно использовать следующее консольное приложение C#, чтобы понять, как можно получить необходимые значения.</span><span class="sxs-lookup"><span data-stu-id="02f79-213">Alternatively, the following C# console app can be used as a Proof of Concept to understand how the required values can be obtained.</span></span> <span data-ttu-id="02f79-214">Обратите внимание, что этот код предназначен **ТОЛЬКО для обучения и справочных материалов** и не должен использоваться "как есть" в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="02f79-214">Note that this code is for **learning and reference ONLY** and should not be used as-is in production.</span></span>

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

### <a name="add-a-custom-signing-key"></a><span data-ttu-id="02f79-215">Добавление пользовательского ключа подписывания</span><span class="sxs-lookup"><span data-stu-id="02f79-215">Add a custom signing key</span></span>

<span data-ttu-id="02f79-216">Добавьте следующие сведения в субъект-службу.</span><span class="sxs-lookup"><span data-stu-id="02f79-216">Add the following information to the service principal:</span></span>

* <span data-ttu-id="02f79-217">Закрытый ключ</span><span class="sxs-lookup"><span data-stu-id="02f79-217">Private key</span></span>
* <span data-ttu-id="02f79-218">Пароль</span><span class="sxs-lookup"><span data-stu-id="02f79-218">Password</span></span>
* <span data-ttu-id="02f79-219">Открытый ключ</span><span class="sxs-lookup"><span data-stu-id="02f79-219">Public key</span></span> 

<span data-ttu-id="02f79-220">Извлеките закрытый и открытый ключи в кодировке Base64 из PFX-файла.</span><span class="sxs-lookup"><span data-stu-id="02f79-220">Extract the private and public key Base64 encoded from the PFX file.</span></span> <span data-ttu-id="02f79-221">Дополнительные сведения об их свойствах см. в описании [типа ресурса keyCredential](https://docs.microsoft.com/graph/api/resources/keycredential?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="02f79-221">To learn more about the properties, read [keyCredential resource type](https://docs.microsoft.com/graph/api/resources/keycredential?view=graph-rest-1.0).</span></span>

<span data-ttu-id="02f79-222">Убедитесь, что значение keyId для keyCredential, примененное для параметра Sign, соответствует значению keyId для passwordCredential.</span><span class="sxs-lookup"><span data-stu-id="02f79-222">Make sure that the keyId for the keyCredential used for "Sign" matches the keyId of the passwordCredential.</span></span> <span data-ttu-id="02f79-223">Вы можете создать `customkeyIdentifier`, получив хэш отпечатка сертификата.</span><span class="sxs-lookup"><span data-stu-id="02f79-223">You can generate the `customkeyIdentifier` by getting the hash of the cert's thumbprint.</span></span> <span data-ttu-id="02f79-224">См. справочный код C# выше.</span><span class="sxs-lookup"><span data-stu-id="02f79-224">See C# reference code above.</span></span>

#### <a name="request"></a><span data-ttu-id="02f79-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f79-225">Request</span></span>

> [!NOTE]
> <span data-ttu-id="02f79-226">Значение key в свойстве keyCredentials сокращено для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="02f79-226">The "key" value in the keyCredentials property is shortened for readability.</span></span> <span data-ttu-id="02f79-227">Значение представлено в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="02f79-227">The value is base 64 encoded.</span></span> <span data-ttu-id="02f79-228">Для закрытого ключа свойство `usage` имеет значение "Sign".</span><span class="sxs-lookup"><span data-stu-id="02f79-228">For the private key the property `usage` is "Sign".</span></span> <span data-ttu-id="02f79-229">Для открытого ключа свойство `usage` имеет значение "Verify".</span><span class="sxs-lookup"><span data-stu-id="02f79-229">For the public key the property `usage` is "Verify".</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: servicePrincipals/json

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

#### <a name="response"></a><span data-ttu-id="02f79-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f79-230">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a><span data-ttu-id="02f79-231">Активация пользовательского ключа подписывания</span><span class="sxs-lookup"><span data-stu-id="02f79-231">Activate the custom signing key</span></span>

<span data-ttu-id="02f79-232">Вам нужно задать для свойства `preferredTokenSigningKeyThumbprint` значение отпечатка сертификата, с помощью которого Azure AD будет подписывать ответ SAML.</span><span class="sxs-lookup"><span data-stu-id="02f79-232">You need to set the `preferredTokenSigningKeyThumbprint` property to the thumbprint of the certificate you want Azure AD to use to sign the SAML response.</span></span> 

#### <a name="request"></a><span data-ttu-id="02f79-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f79-233">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: servicePrincipals/json

{
    "preferredTokenSigningKeyThumbprint": "AC09FEF18DDE6983EE2A164FBA3C4DD7518BD787"
}
```

#### <a name="response"></a><span data-ttu-id="02f79-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f79-234">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```
## <a name="step-5-assign-users"></a><span data-ttu-id="02f79-235">Шаг 5. Назначение пользователей</span><span class="sxs-lookup"><span data-stu-id="02f79-235">Step 5: Assign users</span></span>

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="02f79-236">Назначение пользователей и групп для приложения</span><span class="sxs-lookup"><span data-stu-id="02f79-236">Assign users and groups to the application</span></span>

<span data-ttu-id="02f79-237">Назначьте субъекту-службе следующего пользователя и роль AWS_Role1.</span><span class="sxs-lookup"><span data-stu-id="02f79-237">Assign the following user to the service principal and assign the AWS_Role1.</span></span> 

| <span data-ttu-id="02f79-238">Имя</span><span class="sxs-lookup"><span data-stu-id="02f79-238">Name</span></span>  | <span data-ttu-id="02f79-239">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="02f79-239">ID</span></span>  |
|---------|---------|
| <span data-ttu-id="02f79-240">Идентификатор пользователя (principalId)</span><span class="sxs-lookup"><span data-stu-id="02f79-240">User ID (principalId)</span></span> | <span data-ttu-id="02f79-241">6cad4079-4e79-4a3f-9efb-ea30a14bdb26</span><span class="sxs-lookup"><span data-stu-id="02f79-241">6cad4079-4e79-4a3f-9efb-ea30a14bdb26</span></span> |
| <span data-ttu-id="02f79-242">Тип (principalType)</span><span class="sxs-lookup"><span data-stu-id="02f79-242">Type (principalType)</span></span> | <span data-ttu-id="02f79-243">Пользователь</span><span class="sxs-lookup"><span data-stu-id="02f79-243">User</span></span> |
| <span data-ttu-id="02f79-244">Идентификатор роли приложения (appRoleId)</span><span class="sxs-lookup"><span data-stu-id="02f79-244">App role ID (appRoleId)</span></span> | <span data-ttu-id="02f79-245">454dc4c2-8176-498e-99df-8c4efcde41ef</span><span class="sxs-lookup"><span data-stu-id="02f79-245">454dc4c2-8176-498e-99df-8c4efcde41ef</span></span> |
| <span data-ttu-id="02f79-246">Идентификатор субъекта-службы (resourceId)</span><span class="sxs-lookup"><span data-stu-id="02f79-246">servicePrincipalID (resourceId)</span></span> | <span data-ttu-id="02f79-247">f47a6776-bca7-4f2e-bc6c-eec59d058e3e</span><span class="sxs-lookup"><span data-stu-id="02f79-247">f47a6776-bca7-4f2e-bc6c-eec59d058e3e</span></span> |

#### <a name="request"></a><span data-ttu-id="02f79-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f79-248">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
  "principalType": "User",
  "appRoleId":"454dc4c2-8176-498e-99df-8c4efcde41ef",
  "resourceId":"f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```
#### <a name="response"></a><span data-ttu-id="02f79-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f79-249">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 201 
Content-type: appRoleAssignments/json

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

<span data-ttu-id="02f79-250">Дополнительные сведения см. в документации по типу ресурса [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="02f79-250">For more information, see [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-1.0) resource type.</span></span>

## <a name="step-6-configure-the-application-side"></a><span data-ttu-id="02f79-251">Шаг 6. Настройка на стороне приложения</span><span class="sxs-lookup"><span data-stu-id="02f79-251">Step 6: Configure the application side</span></span>

### <a name="get-azure-ad-saml-metadata"></a><span data-ttu-id="02f79-252">Получение метаданных SAML из Azure AD</span><span class="sxs-lookup"><span data-stu-id="02f79-252">Get Azure AD SAML metadata</span></span>

<span data-ttu-id="02f79-253">Используйте следующий URL-адрес, чтобы получить метаданные SAML из Azure AD для конкретного настроенного приложения.</span><span class="sxs-lookup"><span data-stu-id="02f79-253">Use the following URL to get the Azure AD SAML metadata for the specific configured application.</span></span> <span data-ttu-id="02f79-254">Эти метаданные содержат такие сведения, как сертификат для подписи, идентификатор сущности Azure AD (entityID), служба единого входа Azure AD (SingleSignOnService) и т. д.</span><span class="sxs-lookup"><span data-stu-id="02f79-254">The metadata contains information such as the signing certificate, Azure AD entityID, and Azure AD SingleSignOnService, among others.</span></span>

https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}

## <a name="next-steps"></a><span data-ttu-id="02f79-255">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="02f79-255">Next steps</span></span>
- [<span data-ttu-id="02f79-256">Настройка подготовки пользователей с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="02f79-256">Use Microsoft Graph APIs to configure user provisioning</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api)
- [<span data-ttu-id="02f79-257">Использование отчета о действиях приложения AD FS для миграции приложений в Azure AD</span><span class="sxs-lookup"><span data-stu-id="02f79-257">Use the AD FS application activity report to migrate applications to Azure AD</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-application-activity)
