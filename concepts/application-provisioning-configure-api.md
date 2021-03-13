---
title: 'Настройка подготовки с помощью интерфейсов API Microsoft Graph:'
description: Узнайте, как сэкономить время с помощью API Microsoft Graph для автоматизации конфигурации автоматического обеспечения.
author: kenwith
ms.topic: conceptual
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 626593ada6c45de18bb24f9ec107fca7d077fb67
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761865"
---
# <a name="configure-provisioning-using-microsoft-graph-apis"></a><span data-ttu-id="9ab96-103">Настройка подготовки с помощью интерфейсов API Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="9ab96-103">Configure provisioning using Microsoft Graph APIs</span></span>

<span data-ttu-id="9ab96-104">Портал Azure — это удобный способ настроить подготовка для отдельных приложений по одному.</span><span class="sxs-lookup"><span data-stu-id="9ab96-104">The Azure portal is a convenient way to configure provisioning for individual apps one at a time.</span></span> <span data-ttu-id="9ab96-105">Но если вы создаете несколько или даже сотни экземпляров приложения, можно проще автоматизировать создание и конфигурацию приложений с API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9ab96-105">But if you're creating several—or even hundreds—of instances of an application, it can be easier to automate app creation and configuration with the Microsoft Graph APIs.</span></span> <span data-ttu-id="9ab96-106">В этой статье описано, как автоматизировать конфигурацию подготовка с помощью API.</span><span class="sxs-lookup"><span data-stu-id="9ab96-106">This article outlines how to automate provisioning configuration through APIs.</span></span> <span data-ttu-id="9ab96-107">Этот метод обычно используется для таких приложений, как [Amazon Web Services.](/azure/active-directory/saas-apps/amazon-web-service-tutorial#configure-azure-ad-sso)</span><span class="sxs-lookup"><span data-stu-id="9ab96-107">This method is commonly used for applications like [Amazon Web Services](/azure/active-directory/saas-apps/amazon-web-service-tutorial#configure-azure-ad-sso).</span></span>

<span data-ttu-id="9ab96-108">**Обзор действий по использованию API Microsoft Graph для автоматизации конфигурации подготовка**</span><span class="sxs-lookup"><span data-stu-id="9ab96-108">**Overview of steps for using Microsoft Graph APIs to automate provisioning configuration**</span></span>


|<span data-ttu-id="9ab96-109">Шаг</span><span class="sxs-lookup"><span data-stu-id="9ab96-109">Step</span></span>  |<span data-ttu-id="9ab96-110">Сведения</span><span class="sxs-lookup"><span data-stu-id="9ab96-110">Details</span></span>  |
|---------|---------|
|[<span data-ttu-id="9ab96-111">Шаг 1. Создание приложения галереи</span><span class="sxs-lookup"><span data-stu-id="9ab96-111">Step 1. Create the gallery application</span></span>](#step-1-create-the-gallery-application)     |<span data-ttu-id="9ab96-112">Вход в клиент API</span><span class="sxs-lookup"><span data-stu-id="9ab96-112">Sign-in to the API client</span></span> <br> <span data-ttu-id="9ab96-113">Получение шаблона приложения галереи</span><span class="sxs-lookup"><span data-stu-id="9ab96-113">Retrieve the gallery application template</span></span> <br> <span data-ttu-id="9ab96-114">Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="9ab96-114">Create the gallery application</span></span>         |
|[<span data-ttu-id="9ab96-115">Шаг 2. Создание задания по подготовкам на основе шаблона</span><span class="sxs-lookup"><span data-stu-id="9ab96-115">Step 2. Create provisioning job based on template</span></span>](#step-2-create-the-provisioning-job-based-on-the-template)     |<span data-ttu-id="9ab96-116">Извлечение шаблона для соединиттеля подготовка</span><span class="sxs-lookup"><span data-stu-id="9ab96-116">Retrieve the template for the provisioning connector</span></span> <br> <span data-ttu-id="9ab96-117">Создание задания по подготовкам</span><span class="sxs-lookup"><span data-stu-id="9ab96-117">Create the provisioning job</span></span>         |
|[<span data-ttu-id="9ab96-118">Шаг 3. Авторизировать доступ</span><span class="sxs-lookup"><span data-stu-id="9ab96-118">Step 3. Authorize access</span></span>](#step-3-authorize-access)     |<span data-ttu-id="9ab96-119">Проверка подключения к приложению</span><span class="sxs-lookup"><span data-stu-id="9ab96-119">Test the connection to the application</span></span> <br> <span data-ttu-id="9ab96-120">Сохранение учетных данных</span><span class="sxs-lookup"><span data-stu-id="9ab96-120">Save the credentials</span></span>         |
|[<span data-ttu-id="9ab96-121">Шаг 4. Начало задания по подготовкам</span><span class="sxs-lookup"><span data-stu-id="9ab96-121">Step 4. Start provisioning job</span></span>](#step-4-start-the-provisioning-job)     |<span data-ttu-id="9ab96-122">Запуск задания</span><span class="sxs-lookup"><span data-stu-id="9ab96-122">Start the job</span></span>         |
|[<span data-ttu-id="9ab96-123">Шаг 5. Мониторинг подготовка</span><span class="sxs-lookup"><span data-stu-id="9ab96-123">Step 5. Monitor provisioning</span></span>](#step-5-monitor-provisioning)     |<span data-ttu-id="9ab96-124">Проверка состояния задания подготовка</span><span class="sxs-lookup"><span data-stu-id="9ab96-124">Check the status of the provisioning job</span></span> <br> <span data-ttu-id="9ab96-125">Извлечение журналов подготовка</span><span class="sxs-lookup"><span data-stu-id="9ab96-125">Retrieve the provisioning logs</span></span>         |

## <a name="step-1-create-the-gallery-application"></a><span data-ttu-id="9ab96-126">Шаг 1. Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="9ab96-126">Step 1: Create the gallery application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="9ab96-127">Вход в песочницу Microsoft Graph (рекомендуется), Postman или любой другой используемый клиент API</span><span class="sxs-lookup"><span data-stu-id="9ab96-127">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="9ab96-128">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="9ab96-128">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
1. <span data-ttu-id="9ab96-129">Выберите кнопку "Вход с Microsoft" и впишитесь с помощью глобального администратора Azure AD или учетных данных администратора приложений.</span><span class="sxs-lookup"><span data-stu-id="9ab96-129">Select the "Sign-In with Microsoft" button and sign in using Azure AD global administrator or App Admin credentials.</span></span>

    ![Вход в граф](./images/application-provisioning-configure-api/wd_export_02.png)

1. <span data-ttu-id="9ab96-131">После успешного входа вы увидите данные учетной записи пользователя на панели слева.</span><span class="sxs-lookup"><span data-stu-id="9ab96-131">Upon successful sign-in, you'll see the user account details in the left-hand pane.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="9ab96-132">Получение идентификатора шаблона для приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="9ab96-132">Retrieve the gallery application template identifier</span></span>
<span data-ttu-id="9ab96-133">У каждого приложения в коллекции приложений Azure AD есть [шаблон](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta), описывающий метаданные для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9ab96-133">Applications in the Azure AD application gallery each have an [application template](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta) that describes the metadata for that application.</span></span> <span data-ttu-id="9ab96-134">По этому шаблону вы можете создать экземпляр приложения и субъект-службу в клиенте для управления им.</span><span class="sxs-lookup"><span data-stu-id="9ab96-134">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span>

#### <a name="request"></a><span data-ttu-id="9ab96-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9ab96-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab96-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="9ab96-137">C#</span><span class="sxs-lookup"><span data-stu-id="9ab96-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ab96-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ab96-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ab96-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ab96-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ab96-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab96-140">Response</span></span>

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

### <a name="create-the-gallery-application"></a><span data-ttu-id="9ab96-141">Создание приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="9ab96-141">Create the gallery application</span></span>

<span data-ttu-id="9ab96-142">На последнем шаге используйте ИД шаблона, [](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta) извлеченный для приложения, чтобы создать экземпляр основного приложения и службы в клиенте.</span><span class="sxs-lookup"><span data-stu-id="9ab96-142">Use the template ID retrieved for your application in the last step to [create an instance](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta) of the application and service principal in your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="9ab96-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9ab96-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab96-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9ab96-145">C#</span><span class="sxs-lookup"><span data-stu-id="9ab96-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ab96-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ab96-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ab96-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ab96-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ab96-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab96-148">Response</span></span>


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

## <a name="step-2-create-the-provisioning-job-based-on-the-template"></a><span data-ttu-id="9ab96-149">Шаг 2. Создание задания подготовка на основе шаблона</span><span class="sxs-lookup"><span data-stu-id="9ab96-149">Step 2: Create the provisioning job based on the template</span></span>

### <a name="retrieve-the-template-for-the-provisioning-connector"></a><span data-ttu-id="9ab96-150">Извлечение шаблона для соединиттеля подготовка</span><span class="sxs-lookup"><span data-stu-id="9ab96-150">Retrieve the template for the provisioning connector</span></span>

<span data-ttu-id="9ab96-151">Приложения в галерее, которые включены для подготовка, имеют шаблоны для оптимизации конфигурации.</span><span class="sxs-lookup"><span data-stu-id="9ab96-151">Applications in the gallery that are enabled for provisioning have templates to streamline configuration.</span></span> <span data-ttu-id="9ab96-152">Чтобы получить шаблон для конфигурации подготовка, используйте приведенную ниже [просьбу.](/graph/api/synchronization-synchronizationtemplate-list?tabs=http&view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="9ab96-152">Use the request below to [retrieve the template for the provisioning configuration](/graph/api/synchronization-synchronizationtemplate-list?tabs=http&view=graph-rest-beta).</span></span> <span data-ttu-id="9ab96-153">Обратите внимание, что необходимо предоставить ID.</span><span class="sxs-lookup"><span data-stu-id="9ab96-153">Note that you will need to provide the ID.</span></span> <span data-ttu-id="9ab96-154">ID относится к предыдущему ресурсу, который в данном случае является ресурсом servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="9ab96-154">The ID refers to the preceding resource, which in this case is the servicePrincipal resource.</span></span> 

#### <a name="request"></a><span data-ttu-id="9ab96-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9ab96-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab96-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="c"></a>[<span data-ttu-id="9ab96-157">C#</span><span class="sxs-lookup"><span data-stu-id="9ab96-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ab96-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ab96-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ab96-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ab96-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="9ab96-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab96-160">Response</span></span>
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

### <a name="create-the-provisioning-job"></a><span data-ttu-id="9ab96-161">Создание задания по подготовкам</span><span class="sxs-lookup"><span data-stu-id="9ab96-161">Create the provisioning job</span></span>
<span data-ttu-id="9ab96-162">Чтобы включить подготовка, сначала необходимо [создать задание.](/graph/api/synchronization-synchronizationjob-post?tabs=http&view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="9ab96-162">To enable provisioning, you'll first need to [create a job](/graph/api/synchronization-synchronizationjob-post?tabs=http&view=graph-rest-beta).</span></span> <span data-ttu-id="9ab96-163">Чтобы создать задание по подготовкам, используйте следующий запрос.</span><span class="sxs-lookup"><span data-stu-id="9ab96-163">Use the following request to create a provisioning job.</span></span> <span data-ttu-id="9ab96-164">Используйте templateId с предыдущего шага при указании шаблона, который будет использоваться для задания.</span><span class="sxs-lookup"><span data-stu-id="9ab96-164">Use the templateId from the previous step when specifying the template to be used for the job.</span></span>

#### <a name="request"></a><span data-ttu-id="9ab96-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-165">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9ab96-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab96-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9ab96-167">C#</span><span class="sxs-lookup"><span data-stu-id="9ab96-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ab96-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ab96-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ab96-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ab96-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ab96-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab96-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 201 OK
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

## <a name="step-3-authorize-access"></a><span data-ttu-id="9ab96-171">Шаг 3. Авторизованный доступ</span><span class="sxs-lookup"><span data-stu-id="9ab96-171">Step 3: Authorize access</span></span>

### <a name="test-the-connection-to-the-application"></a><span data-ttu-id="9ab96-172">Проверка подключения к приложению</span><span class="sxs-lookup"><span data-stu-id="9ab96-172">Test the connection to the application</span></span>

<span data-ttu-id="9ab96-173">Проверьте подключение к стороне приложения.</span><span class="sxs-lookup"><span data-stu-id="9ab96-173">Test the connection with the third-party application.</span></span> <span data-ttu-id="9ab96-174">Ниже приводится пример приложения, которое требует секрета клиента и секретного маркера.</span><span class="sxs-lookup"><span data-stu-id="9ab96-174">The following example is for an application that requires a client secret and secret token.</span></span> <span data-ttu-id="9ab96-175">Каждое приложение имеет свои требования.</span><span class="sxs-lookup"><span data-stu-id="9ab96-175">Each application has its own requirements.</span></span> <span data-ttu-id="9ab96-176">Приложения часто используют базовый адрес, а не клиентскую тайну.</span><span class="sxs-lookup"><span data-stu-id="9ab96-176">Applications often use a base address in place of a client secret.</span></span> <span data-ttu-id="9ab96-177">Чтобы определить, какие учетные данные требуются вашему приложению, перейдите на страницу конфигурации подготовка для приложения, а в режиме разработчика щелкните **тестовую подключение.**</span><span class="sxs-lookup"><span data-stu-id="9ab96-177">To determine what credentials your app requires, go to the provisioning configuration page for your application, and in developer mode, click **test connection**.</span></span> <span data-ttu-id="9ab96-178">В сетевом трафике покажут параметры, используемые для учетных данных.</span><span class="sxs-lookup"><span data-stu-id="9ab96-178">The network traffic will show the parameters used for credentials.</span></span> <span data-ttu-id="9ab96-179">Полный список учетных данных см. в [синхронизацииJob: validateCredentials.](/graph/api/synchronization-synchronizationjob-validatecredentials?tabs=http&view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="9ab96-179">For a full list of credentials, see [synchronizationJob: validateCredentials](/graph/api/synchronization-synchronizationjob-validatecredentials?tabs=http&view=graph-rest-beta).</span></span> <span data-ttu-id="9ab96-180">Большинство приложений, например Azure Databricks, используют BaseAddress и SecretToken.</span><span class="sxs-lookup"><span data-stu-id="9ab96-180">Most applications, such as Azure Databricks, rely on a BaseAddress and SecretToken.</span></span> <span data-ttu-id="9ab96-181">BaseAddress ссылаются на URL-адрес клиента на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9ab96-181">The BaseAddress is refered to as a tenant URL in the Azure Portal.</span></span> 

#### <a name="request"></a><span data-ttu-id="9ab96-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-182">Request</span></span>
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials
{ 
    "credentials": [ 
        { "key": "ClientSecret", "value": "xxxxxxxxxxxxxxxxxxxxx" },
        { "key": "SecretToken", "value": "xxxxxxxxxxxxxxxxxxxxx" }
    ]
}
```
#### <a name="response"></a><span data-ttu-id="9ab96-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ab96-183">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="save-your-credentials"></a><span data-ttu-id="9ab96-184">Сохранение учетных данных</span><span class="sxs-lookup"><span data-stu-id="9ab96-184">Save your credentials</span></span>

<span data-ttu-id="9ab96-185">Настройка подготовка требует установления доверия между Azure AD и приложением.</span><span class="sxs-lookup"><span data-stu-id="9ab96-185">Configuring provisioning requires establishing a trust between Azure AD and the application.</span></span> <span data-ttu-id="9ab96-186">Авторизузить доступ к сторонним приложениям.</span><span class="sxs-lookup"><span data-stu-id="9ab96-186">Authorize access to the third-party application.</span></span> <span data-ttu-id="9ab96-187">Ниже приводится пример приложения, которое требует секрета клиента и секретного маркера.</span><span class="sxs-lookup"><span data-stu-id="9ab96-187">The following example is for an application that requires a client secret and a secret token.</span></span> <span data-ttu-id="9ab96-188">Каждое приложение имеет свои требования.</span><span class="sxs-lookup"><span data-stu-id="9ab96-188">Each application has its own requirements.</span></span> <span data-ttu-id="9ab96-189">Просмотрите [документацию по API,](/graph/api/synchronization-synchronizationjob-validatecredentials?tabs=http&view=graph-rest-beta) чтобы просмотреть доступные варианты.</span><span class="sxs-lookup"><span data-stu-id="9ab96-189">Review the [API documentation](/graph/api/synchronization-synchronizationjob-validatecredentials?tabs=http&view=graph-rest-beta) to see the available options.</span></span> 

#### <a name="request"></a><span data-ttu-id="9ab96-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-190">Request</span></span>
```msgraph-interactive
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/secrets 
 
{ 
    "value": [ 
        { "key": "ClientSecret", "value": "xxxxxxxxxxxxxxxxxxxxx" },
        { "key": "SecretToken", "value": "xxxxxxxxxxxxxxxxxxxxx" }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="9ab96-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ab96-191">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="step-4-start-the-provisioning-job"></a><span data-ttu-id="9ab96-192">Шаг 4. Запуск задания по подготовкам</span><span class="sxs-lookup"><span data-stu-id="9ab96-192">Step 4: Start the provisioning job</span></span>
<span data-ttu-id="9ab96-193">Теперь, когда задание подготовка настроено, для запуска задания используйте следующую [команду.](/graph/api/synchronization-synchronizationjob-start?tabs=http&view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="9ab96-193">Now that the provisioning job is configured, use the following command to [start the job](/graph/api/synchronization-synchronizationjob-start?tabs=http&view=graph-rest-beta).</span></span> 


#### <a name="request"></a><span data-ttu-id="9ab96-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-194">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9ab96-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab96-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="9ab96-196">C#</span><span class="sxs-lookup"><span data-stu-id="9ab96-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ab96-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ab96-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ab96-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ab96-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ab96-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab96-199">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


## <a name="step-5-monitor-provisioning"></a><span data-ttu-id="9ab96-200">Шаг 5. Мониторинг подготовка</span><span class="sxs-lookup"><span data-stu-id="9ab96-200">Step 5: Monitor provisioning</span></span>

### <a name="monitor-the-provisioning-job-status"></a><span data-ttu-id="9ab96-201">Мониторинг состояния задания по подготовкам</span><span class="sxs-lookup"><span data-stu-id="9ab96-201">Monitor the provisioning job status</span></span>

<span data-ttu-id="9ab96-202">Теперь, когда задание по подготовкам запущено, используйте следующую команду для отслеживания хода текущего цикла подготовка, а также статистики на сегодняшний день, таких как количество пользователей и групп, созданных в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="9ab96-202">Now that the provisioning job is running, use the following command to track the progress of the current provisioning cycle as well as statistics to date such as the number of users and groups that have been created in the target system.</span></span> 

#### <a name="request"></a><span data-ttu-id="9ab96-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-203">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9ab96-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab96-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="9ab96-205">C#</span><span class="sxs-lookup"><span data-stu-id="9ab96-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ab96-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ab96-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ab96-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ab96-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ab96-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab96-208">Response</span></span>
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


### <a name="monitor-provisioning-events-using-the-provisioning-logs"></a><span data-ttu-id="9ab96-209">Мониторинг событий подготовка с помощью журналов подготовка</span><span class="sxs-lookup"><span data-stu-id="9ab96-209">Monitor provisioning events using the provisioning logs</span></span>
<span data-ttu-id="9ab96-210">В дополнение к мониторингу состояния задания подготовка, [](/graph/api/provisioningobjectsummary-list?tabs=http&view=graph-rest-beta) вы можете использовать журналы подготовка для запроса для всех событий, которые происходят.</span><span class="sxs-lookup"><span data-stu-id="9ab96-210">In addition to monitoring the status of the provisioning job, you can use the [provisioning logs](/graph/api/provisioningobjectsummary-list?tabs=http&view=graph-rest-beta) to query for all the events that are occurring.</span></span> <span data-ttu-id="9ab96-211">Например, запрос для конкретного пользователя и определите, были ли они успешно заданной.</span><span class="sxs-lookup"><span data-stu-id="9ab96-211">For example, query for a particular user and determine if they were successfully provisioned.</span></span>

#### <a name="request"></a><span data-ttu-id="9ab96-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-212">Request</span></span>
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
#### <a name="response"></a><span data-ttu-id="9ab96-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ab96-213">Response</span></span>
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
## <a name="see-also"></a><span data-ttu-id="9ab96-214">См. также</span><span class="sxs-lookup"><span data-stu-id="9ab96-214">See also</span></span>

- [<span data-ttu-id="9ab96-215">Просмотрите документацию по синхронизации Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9ab96-215">Review the synchronization Microsoft Graph documentation</span></span>](/graph/api/resources/synchronization-overview?view=graph-rest-beta)
- [<span data-ttu-id="9ab96-216">Интеграция настраиваемого приложения SCIM с Azure AD</span><span class="sxs-lookup"><span data-stu-id="9ab96-216">Integrating a custom SCIM app with Azure AD</span></span>](/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups)
