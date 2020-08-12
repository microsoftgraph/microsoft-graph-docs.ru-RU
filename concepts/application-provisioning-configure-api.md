---
title: Настройка подготовки с помощью API Microsoft Graph
description: Узнайте, как сэкономить время с помощью API Microsoft Graph для автоматизации настройки автоматической подготовки.
author: kenwith
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a144f0dbc0c6b57fb48c87b4ad8f5c5c446618aa
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643864"
---
# <a name="configure-provisioning-using-microsoft-graph-apis"></a><span data-ttu-id="3f2ee-103">Настройка подготовки с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3f2ee-103">Configure provisioning using Microsoft Graph APIs</span></span>

<span data-ttu-id="3f2ee-104">Портал Azure — это удобный способ настройки подготовки для отдельных приложений по одному за раз.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-104">The Azure portal is a convenient way to configure provisioning for individual apps one at a time.</span></span> <span data-ttu-id="3f2ee-105">Но если вы создаете несколько или даже сотни экземпляров приложения, вы можете упростить процесс создания и настройки приложений с помощью API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-105">But if you're creating several—or even hundreds—of instances of an application, it can be easier to automate app creation and configuration with the Microsoft Graph APIs.</span></span> <span data-ttu-id="3f2ee-106">В этой статье рассказывается, как автоматизировать подготовку конфигурации с помощью API.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-106">This article outlines how to automate provisioning configuration through APIs.</span></span> <span data-ttu-id="3f2ee-107">Этот метод часто используется для таких приложений, как [веб-службы Amazon](https://docs.microsoft.com/azure/active-directory/saas-apps/amazon-web-service-tutorial#configure-azure-ad-sso).</span><span class="sxs-lookup"><span data-stu-id="3f2ee-107">This method is commonly used for applications like [Amazon Web Services](https://docs.microsoft.com/azure/active-directory/saas-apps/amazon-web-service-tutorial#configure-azure-ad-sso).</span></span>

<span data-ttu-id="3f2ee-108">**Обзор действий по использованию API Microsoft Graph для автоматизации настройки подготовки**</span><span class="sxs-lookup"><span data-stu-id="3f2ee-108">**Overview of steps for using Microsoft Graph APIs to automate provisioning configuration**</span></span>


|<span data-ttu-id="3f2ee-109">Шаг</span><span class="sxs-lookup"><span data-stu-id="3f2ee-109">Step</span></span>  |<span data-ttu-id="3f2ee-110">Сведения</span><span class="sxs-lookup"><span data-stu-id="3f2ee-110">Details</span></span>  |
|---------|---------|
|[<span data-ttu-id="3f2ee-111">Шаг 1. Создание приложения коллекции</span><span class="sxs-lookup"><span data-stu-id="3f2ee-111">Step 1. Create the gallery application</span></span>](#step-1-create-the-gallery-application)     |<span data-ttu-id="3f2ee-112">Вход в клиент API</span><span class="sxs-lookup"><span data-stu-id="3f2ee-112">Sign-in to the API client</span></span> <br> <span data-ttu-id="3f2ee-113">Получение шаблона приложения коллекции</span><span class="sxs-lookup"><span data-stu-id="3f2ee-113">Retrieve the gallery application template</span></span> <br> <span data-ttu-id="3f2ee-114">Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="3f2ee-114">Create the gallery application</span></span>         |
|[<span data-ttu-id="3f2ee-115">Шаг 2. Создание задания подготовки на основе шаблона</span><span class="sxs-lookup"><span data-stu-id="3f2ee-115">Step 2. Create provisioning job based on template</span></span>](#step-2-create-the-provisioning-job-based-on-the-template)     |<span data-ttu-id="3f2ee-116">Получение шаблона для соединителя подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-116">Retrieve the template for the provisioning connector</span></span> <br> <span data-ttu-id="3f2ee-117">Создание задания подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-117">Create the provisioning job</span></span>         |
|[<span data-ttu-id="3f2ee-118">Шаг 3. Авторизация доступа</span><span class="sxs-lookup"><span data-stu-id="3f2ee-118">Step 3. Authorize access</span></span>](#step-3-authorize-access)     |<span data-ttu-id="3f2ee-119">Проверка подключения к приложению</span><span class="sxs-lookup"><span data-stu-id="3f2ee-119">Test the connection to the application</span></span> <br> <span data-ttu-id="3f2ee-120">Сохранение учетных данных</span><span class="sxs-lookup"><span data-stu-id="3f2ee-120">Save the credentials</span></span>         |
|[<span data-ttu-id="3f2ee-121">Шаг 4. Запуск задания подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-121">Step 4. Start provisioning job</span></span>](#step-4-start-the-provisioning-job)     |<span data-ttu-id="3f2ee-122">Запуск задания</span><span class="sxs-lookup"><span data-stu-id="3f2ee-122">Start the job</span></span>         |
|[<span data-ttu-id="3f2ee-123">Шаг 5. Подготовка к работе с монитором</span><span class="sxs-lookup"><span data-stu-id="3f2ee-123">Step 5. Monitor provisioning</span></span>](#step-5-monitor-provisioning)     |<span data-ttu-id="3f2ee-124">Проверка состояния задания подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-124">Check the status of the provisioning job</span></span> <br> <span data-ttu-id="3f2ee-125">Получение журналов подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-125">Retrieve the provisioning logs</span></span>         |

## <a name="step-1-create-the-gallery-application"></a><span data-ttu-id="3f2ee-126">Шаг 1. Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="3f2ee-126">Step 1: Create the gallery application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="3f2ee-127">Вход в песочницу Microsoft Graph (рекомендуется), Postman или любой другой используемый клиент API</span><span class="sxs-lookup"><span data-stu-id="3f2ee-127">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="3f2ee-128">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="3f2ee-128">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
1. <span data-ttu-id="3f2ee-129">Нажмите кнопку "войти в Microsoft" и войдите, используя учетные данные глобального администратора Azure AD или администратора приложения.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-129">Select the "Sign-In with Microsoft" button and sign in using Azure AD global administrator or App Admin credentials.</span></span>

    ![Вход в граф](./images/application-provisioning-configure-api/wd_export_02.png)

1. <span data-ttu-id="3f2ee-131">После успешного входа вы увидите данные учетной записи пользователя на панели слева.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-131">Upon successful sign-in, you'll see the user account details in the left-hand pane.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="3f2ee-132">Получение идентификатора шаблона для приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="3f2ee-132">Retrieve the gallery application template identifier</span></span>
<span data-ttu-id="3f2ee-133">У каждого приложения в коллекции приложений Azure AD есть [шаблон](https://docs.microsoft.com/graph/api/applicationtemplate-list?view=graph-rest-beta&tabs=http), описывающий метаданные для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-133">Applications in the Azure AD application gallery each have an [application template](https://docs.microsoft.com/graph/api/applicationtemplate-list?view=graph-rest-beta&tabs=http) that describes the metadata for that application.</span></span> <span data-ttu-id="3f2ee-134">По этому шаблону вы можете создать экземпляр приложения и субъект-службу в клиенте для управления им.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-134">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span>

#### <a name="request"></a><span data-ttu-id="3f2ee-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f2ee-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3f2ee-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f2ee-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="3f2ee-137">C#</span><span class="sxs-lookup"><span data-stu-id="3f2ee-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f2ee-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f2ee-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f2ee-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f2ee-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3f2ee-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2ee-140">Response</span></span>

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

### <a name="create-the-gallery-application"></a><span data-ttu-id="3f2ee-141">Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="3f2ee-141">Create the gallery application</span></span>

<span data-ttu-id="3f2ee-142">Используйте идентификатор шаблона, полученный для приложения, на последнем этапе, чтобы [создать экземпляр](https://docs.microsoft.com/graph/api/applicationtemplate-instantiate?view=graph-rest-beta&tabs=http) приложения и участника службы в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-142">Use the template ID retrieved for your application in the last step to [create an instance](https://docs.microsoft.com/graph/api/applicationtemplate-instantiate?view=graph-rest-beta&tabs=http) of the application and service principal in your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="3f2ee-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f2ee-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3f2ee-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f2ee-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```
# <a name="c"></a>[<span data-ttu-id="3f2ee-145">C#</span><span class="sxs-lookup"><span data-stu-id="3f2ee-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f2ee-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f2ee-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f2ee-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f2ee-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3f2ee-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2ee-148">Response</span></span>


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

## <a name="step-2-create-the-provisioning-job-based-on-the-template"></a><span data-ttu-id="3f2ee-149">Шаг 2: создание задания подготовки на основе шаблона</span><span class="sxs-lookup"><span data-stu-id="3f2ee-149">Step 2: Create the provisioning job based on the template</span></span>

### <a name="retrieve-the-template-for-the-provisioning-connector"></a><span data-ttu-id="3f2ee-150">Получение шаблона для соединителя подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-150">Retrieve the template for the provisioning connector</span></span>

<span data-ttu-id="3f2ee-151">В приложениях в коллекции, поддерживающей подготовку, предусмотрены шаблоны для упрощения настройки.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-151">Applications in the gallery that are enabled for provisioning have templates to streamline configuration.</span></span> <span data-ttu-id="3f2ee-152">Используйте приведенный ниже запрос для [получения шаблона конфигурации подготовки](https://docs.microsoft.com/graph/api/synchronization-synchronizationtemplate-list?view=graph-rest-beta&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="3f2ee-152">Use the request below to [retrieve the template for the provisioning configuration](https://docs.microsoft.com/graph/api/synchronization-synchronizationtemplate-list?view=graph-rest-beta&tabs=http).</span></span> <span data-ttu-id="3f2ee-153">Обратите внимание, что вам потребуется указать идентификатор.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-153">Note that you will need to provide the ID.</span></span> <span data-ttu-id="3f2ee-154">ИДЕНТИФИКАТОР ссылается на предыдущий ресурс, который в данном случае является ресурсом servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-154">The ID refers to the preceding resource, which in this case is the servicePrincipal resource.</span></span> 

#### <a name="request"></a><span data-ttu-id="3f2ee-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f2ee-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3f2ee-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f2ee-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="c"></a>[<span data-ttu-id="3f2ee-157">C#</span><span class="sxs-lookup"><span data-stu-id="3f2ee-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f2ee-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f2ee-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f2ee-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f2ee-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="3f2ee-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2ee-160">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "aws",
            "factoryTag": "aws",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

### <a name="create-the-provisioning-job"></a><span data-ttu-id="3f2ee-161">Создание задания подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-161">Create the provisioning job</span></span>
<span data-ttu-id="3f2ee-162">Чтобы включить подготовку, сначала необходимо [создать задание](https://docs.microsoft.com/graph/api/synchronization-synchronizationjob-post?view=graph-rest-beta&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="3f2ee-162">To enable provisioning, you'll first need to [create a job](https://docs.microsoft.com/graph/api/synchronization-synchronizationjob-post?view=graph-rest-beta&tabs=http).</span></span> <span data-ttu-id="3f2ee-163">Используйте следующий запрос для создания задания подготовки.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-163">Use the following request to create a provisioning job.</span></span> <span data-ttu-id="3f2ee-164">Используйте templateId из предыдущего этапа при указании шаблона, который будет использоваться для задания.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-164">Use the templateId from the previous step when specifying the template to be used for the job.</span></span>

#### <a name="request"></a><span data-ttu-id="3f2ee-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f2ee-165">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3f2ee-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f2ee-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
Content-type: application/json

{ 
    "templateId": "aws"
}
```
# <a name="c"></a>[<span data-ttu-id="3f2ee-167">C#</span><span class="sxs-lookup"><span data-stu-id="3f2ee-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f2ee-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f2ee-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f2ee-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f2ee-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3f2ee-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2ee-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "{jobId}",
    "templateId": "aws",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "NotConfigured",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    }
}
```

## <a name="step-3-authorize-access"></a><span data-ttu-id="3f2ee-171">Шаг 3: авторизация доступа</span><span class="sxs-lookup"><span data-stu-id="3f2ee-171">Step 3: Authorize access</span></span>

### <a name="test-the-connection-to-the-application"></a><span data-ttu-id="3f2ee-172">Проверка подключения к приложению</span><span class="sxs-lookup"><span data-stu-id="3f2ee-172">Test the connection to the application</span></span>

<span data-ttu-id="3f2ee-173">Протестируйте подключение к стороннему приложению.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-173">Test the connection with the third-party application.</span></span> <span data-ttu-id="3f2ee-174">Следующий пример предназначен для приложения, для которого требуется секретный и секретный маркер клиента.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-174">The following example is for an application that requires a client secret and secret token.</span></span> <span data-ttu-id="3f2ee-175">Каждое приложение имеет свои требования.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-175">Each application has its own requirements.</span></span> <span data-ttu-id="3f2ee-176">В приложениях часто используется базовый адрес вместо секрета клиента.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-176">Applications often use a base address in place of a client secret.</span></span> <span data-ttu-id="3f2ee-177">Чтобы определить, какие учетные данные требуются вашему приложению, перейдите на страницу конфигурации подготовки для приложения и в режиме разработчика щелкните Проверить подключение.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-177">To determine what credentials your app requires, go to the provisioning configuration page for your application and in developer mode click test connection.</span></span> <span data-ttu-id="3f2ee-178">В сетевом трафике отобразятся параметры, используемые для учетных данных.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-178">The network traffic will show the parameters used for credentials.</span></span> <span data-ttu-id="3f2ee-179">Полный список учетных данных приведен в разделе [синчронизатионжоб: валидатекредентиалс](https://docs.microsoft.com/graph/api/synchronization-synchronizationjob-validatecredentials?view=graph-rest-beta&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="3f2ee-179">For a full list of credentials, see [synchronizationJob: validateCredentials](https://docs.microsoft.com/graph/api/synchronization-synchronizationjob-validatecredentials?view=graph-rest-beta&tabs=http).</span></span> 

#### <a name="request"></a><span data-ttu-id="3f2ee-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f2ee-180">Request</span></span>
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials
{ 
    credentials: [ 
        { key: "ClientSecret", value: "xxxxxxxxxxxxxxxxxxxxx" },
        { key: "SecretToken", value: "xxxxxxxxxxxxxxxxxxxxx" }
    ]
}
```
#### <a name="response"></a><span data-ttu-id="3f2ee-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2ee-181">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="save-your-credentials"></a><span data-ttu-id="3f2ee-182">Сохранение учетных данных</span><span class="sxs-lookup"><span data-stu-id="3f2ee-182">Save your credentials</span></span>

<span data-ttu-id="3f2ee-183">Настройка подготовки требует установления доверия между Azure AD и приложением.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-183">Configuring provisioning requires establishing a trust between Azure AD and the application.</span></span> <span data-ttu-id="3f2ee-184">Авторизовать доступ к стороннему приложению.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-184">Authorize access to the third-party application.</span></span> <span data-ttu-id="3f2ee-185">Следующий пример предназначен для приложения, для которого требуется секрет клиента и секретный маркер.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-185">The following example is for an application that requires a client secret and a secret token.</span></span> <span data-ttu-id="3f2ee-186">Каждое приложение имеет свои требования.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-186">Each application has its own requirements.</span></span> <span data-ttu-id="3f2ee-187">Просмотрите [документацию по API](https://docs.microsoft.com/graph/api/synchronization-synchronizationjob-validatecredentials?view=graph-rest-beta&tabs=http) , чтобы просмотреть доступные варианты.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-187">Review the [API documentation](https://docs.microsoft.com/graph/api/synchronization-synchronizationjob-validatecredentials?view=graph-rest-beta&tabs=http) to see the available options.</span></span> 

#### <a name="request"></a><span data-ttu-id="3f2ee-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f2ee-188">Request</span></span>
```msgraph-interactive
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/secrets 
 
{ 
    value: [ 
        { key: "ClientSecret", value: "xxxxxxxxxxxxxxxxxxxxx" },
        { key: "SecretToken", value: "xxxxxxxxxxxxxxxxxxxxx" }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="3f2ee-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2ee-189">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="step-4-start-the-provisioning-job"></a><span data-ttu-id="3f2ee-190">Шаг 4: запуск задания подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-190">Step 4: Start the provisioning job</span></span>
<span data-ttu-id="3f2ee-191">После настройки задания подготовки используйте следующую команду для [запуска задания](https://docs.microsoft.com/graph/api/synchronization-synchronizationjob-start?view=graph-rest-beta&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="3f2ee-191">Now that the provisioning job is configured, use the following command to [start the job](https://docs.microsoft.com/graph/api/synchronization-synchronizationjob-start?view=graph-rest-beta&tabs=http).</span></span> 


#### <a name="request"></a><span data-ttu-id="3f2ee-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f2ee-192">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3f2ee-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f2ee-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="3f2ee-194">C#</span><span class="sxs-lookup"><span data-stu-id="3f2ee-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f2ee-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f2ee-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f2ee-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f2ee-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3f2ee-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2ee-197">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


## <a name="step-5-monitor-provisioning"></a><span data-ttu-id="3f2ee-198">Шаг 5: мониторинг подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-198">Step 5: Monitor provisioning</span></span>

### <a name="monitor-the-provisioning-job-status"></a><span data-ttu-id="3f2ee-199">Отслеживание состояния задания подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-199">Monitor the provisioning job status</span></span>

<span data-ttu-id="3f2ee-200">Теперь, когда выполняется задание подготовки, выполните следующую команду, чтобы отслеживать ход выполнения текущего цикла подготовки, а также статистику по дате, например к количеству пользователей и групп, созданных в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-200">Now that the provisioning job is running, use the following command to track the progress of the current provisioning cycle as well as statistics to date such as the number of users and groups that have been created in the target system.</span></span> 

#### <a name="request"></a><span data-ttu-id="3f2ee-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f2ee-201">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3f2ee-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f2ee-202">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="3f2ee-203">C#</span><span class="sxs-lookup"><span data-stu-id="3f2ee-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f2ee-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f2ee-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f2ee-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f2ee-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3f2ee-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2ee-206">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2577

{
    "id": "{jobId}",
    "templateId": "aws",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "Paused",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "progress": [],
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    },
    "synchronizationJobSettings": [
      {
          "name": "QuarantineTooManyDeletesThreshold",
          "value": "500"
      }
    ]
}
```


### <a name="monitor-provisioning-events-using-the-provisioning-logs"></a><span data-ttu-id="3f2ee-207">Мониторинг событий подготовки с помощью журналов подготовки</span><span class="sxs-lookup"><span data-stu-id="3f2ee-207">Monitor provisioning events using the provisioning logs</span></span>
<span data-ttu-id="3f2ee-208">Помимо наблюдения за состоянием задания подготовки, можно использовать [журналы подготовки](https://docs.microsoft.com/graph/api/provisioningobjectsummary-list?view=graph-rest-beta&tabs=http) для запроса всех происходящих событий...</span><span class="sxs-lookup"><span data-stu-id="3f2ee-208">In addition to monitoring the status of the provisioning job, you can use the [provisioning logs](https://docs.microsoft.com/graph/api/provisioningobjectsummary-list?view=graph-rest-beta&tabs=http) to query for all the events that are occurring.</span></span> <span data-ttu-id="3f2ee-209">Например, запросите определенного пользователя и определите, были ли они успешно подготовлены.</span><span class="sxs-lookup"><span data-stu-id="3f2ee-209">For example, query for a particular user and determine if they were successfully provisioned.</span></span>

#### <a name="request"></a><span data-ttu-id="3f2ee-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f2ee-210">Request</span></span>
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
#### <a name="response"></a><span data-ttu-id="3f2ee-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2ee-211">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "name": "list_provisioningobjectsummary_error"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/provisioning",
    "value": [
        {
            "id": "gc532ff9-r265-ec76-861e-42e2970a8218",
            "activityDateTime": "2019-06-24T20:53:08Z",
            "tenantId": "7928d5b5-7442-4a97-ne2d-66f9j9972ecn",
            "jobId": "BoxOutDelta.7928d5b574424a97ne2d66f9j9972ecn",
            "cycleId": "44576n58-v14b-70fj-8404-3d22tt46ed93",
            "changeId": "eaad2f8b-e6e3-409b-83bd-e4e2e57177d5",
            "action": "Create",
            "durationInMilliseconds": 2785,
            "sourceSystem": {
                "id": "0404601d-a9c0-4ec7-bbcd-02660120d8c9",
                "displayName": "Azure Active Directory",
                "details": {}
            },
            "targetSystem": {
                "id": "cd22f60b-5f2d-1adg-adb4-76ef31db996b",
                "displayName": "Box",
                "details": {
                    "ApplicationId": "f2764360-e0ec-5676-711e-cd6fc0d4dd61",
                    "ServicePrincipalId": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                    "ServicePrincipalDisplayName": "Box"
                }
            },
            "initiatedBy": {
                "id": "",
                "displayName": "Azure AD Provisioning Service",
                "initiatorType": "system"
            },
            "sourceIdentity": {
                "id": "5e6c9rae-ab4d-5239-8ad0-174391d110eb",
                "displayName": "Self-service Pilot",
                "identityType": "Group",
                "details": {}
            },
            "targetIdentity": {
                "id": "",
                "displayName": "",
                "identityType": "Group",
                "details": {}
            },
            "statusInfo": {
                "@odata.type": "#microsoft.graph.statusDetails",
                "status": "failure",
                "errorCode": "BoxEntryConflict",
                "reason": "Message: Box returned an error response with the HTTP status code 409.  This response indicates that a user or a group already exisits with the same name. This can be avoided by identifying and removing the conflicting user from Box via the Box administrative user interface, or removing the current user from the scope of provisioning either by removing their assignment to the Box application in Azure Active Directory or adding a scoping filter to exclude the user.",
                "additionalDetails": null,
                "errorCategory": "NonServiceFailure",
                "recommendedAction": null
            },
            "provisioningSteps": [
                {
                    "name": "EntryImportAdd",
                    "provisioningStepType": "import",
                    "status": "success",
                    "description": "Received Group 'Self-service Pilot' change of type (Add) from Azure Active Directory",
                    "details": {}
                },
                {
                    "name": "EntrySynchronizationAdd",
                    "provisioningStepType": "matching",
                    "status": "success",
                    "description": "Group 'Self-service Pilot' will be created in Box (Group is active and assigned in Azure Active Directory, but no matching Group was found in Box)",
                    "details": {}
                },
                {
                    "name": "EntryExportAdd",
                    "provisioningStepType": "export",
                    "status": "failure",
                    "description": "Failed to create Group 'Self-service Pilot' in Box",
                    "details": {
                        "ReportableIdentifier": "Self-service Pilot"
                    }
                }
            ],
            "modifiedProperties": [
                {
                    "displayName": "objectId",
                    "oldValue": null,
                    "newValue": "5e0c9eae-ad3d-4139-5ad0-174391d110eb"
                },
                {
                    "displayName": "displayName",
                    "oldValue": null,
                    "newValue": "Self-service Pilot"
                },
                {
                    "displayName": "mailEnabled",
                    "oldValue": null,
                    "newValue": "False"
                },
                {
                    "displayName": "mailNickname",
                    "oldValue": null,
                    "newValue": "5ce25n9a-4c5f-45c9-8362-ef3da29c66c5"
                },
                {
                    "displayName": "securityEnabled",
                    "oldValue": null,
                    "newValue": "True"
                },
                {
                    "displayName": "Name",
                    "oldValue": null,
                    "newValue": "Self-service Pilot"
                }
            ]
       }
    ]
}

```
## <a name="see-also"></a><span data-ttu-id="3f2ee-212">См. также</span><span class="sxs-lookup"><span data-stu-id="3f2ee-212">See also</span></span>

- [<span data-ttu-id="3f2ee-213">Изучите документацию по синхронизации Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3f2ee-213">Review the synchronization Microsoft Graph documentation</span></span>](https://docs.microsoft.com/graph/api/resources/synchronization-overview?view=graph-rest-beta)
- [<span data-ttu-id="3f2ee-214">Интеграция настраиваемого приложения СЦИМ с Azure AD</span><span class="sxs-lookup"><span data-stu-id="3f2ee-214">Integrating a custom SCIM app with Azure AD</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups)
