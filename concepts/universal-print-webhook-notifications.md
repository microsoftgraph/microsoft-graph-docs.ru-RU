---
title: Подписка на уведомления об изменениях из API облачной печати с использованием Microsoft Graph
description: Узнайте, как подписаться на уведомления об изменениях событий печати с помощью API Microsoft Graph.
author: jahsu
localization_priority: Priority
ms.prod: cloud-printing
ms.custom: scenarios:getting-started
ms.openlocfilehash: d7b4aa230e3f3b93997de51e014c52581d5f9f8b
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920392"
---
# <a name="subscribe-to-change-notifications-from-cloud-printing-apis-using-microsoft-graph"></a><span data-ttu-id="ac03a-103">Подписка на уведомления об изменениях из API облачной печати с использованием Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ac03a-103">Subscribe to change notifications from cloud printing APIs using Microsoft Graph</span></span>

<span data-ttu-id="ac03a-104">Универсальная печать помогает пользователям переносить инфраструктуру печати в облако и является частью надежной экосистемы партнерских решений, предлагающих расширенные возможности печати.</span><span class="sxs-lookup"><span data-stu-id="ac03a-104">Universal Print helps customers move their print infrastructure to the cloud, and is part of a robust ecosystem of partner solutions that offer advanced print functionality.</span></span> <span data-ttu-id="ac03a-105">Эти решения могут быть еще эффективнее, если использовать API облачной печати в Microsoft Graph для интеграции с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="ac03a-105">These solutions can become even more powerful when you use the cloud printing APIs in Microsoft Graph to integrate with Universal Print.</span></span>

<span data-ttu-id="ac03a-106">Многие партнерские решения должны обрабатывать задания печати в режиме реального времени при их отправке с устройств пользователей на принтеры. Это означает, что они должны получать уведомления, когда задания печати доступны для обработки.</span><span class="sxs-lookup"><span data-stu-id="ac03a-106">Many partner solutions need to process print jobs in real time as they're sent from users' devices to printers, which means they need to be notified when print jobs are available for processing.</span></span> <span data-ttu-id="ac03a-107">Универсальная печать предоставляет обработчики для уведомления решений поставщиков печати, когда задания перемещаются в облаке, а также API, позволяющие управлять принтерами и заданиями печати.</span><span class="sxs-lookup"><span data-stu-id="ac03a-107">Universal Print provides hooks for print vendor solutions to be notified as jobs move through the cloud, and APIs that enable management of printers and print jobs.</span></span>

<span data-ttu-id="ac03a-108">В этой статье объясняется, как подписаться на уведомления о различных событиях заданий печати.</span><span class="sxs-lookup"><span data-stu-id="ac03a-108">This article describes how to subscribe to notifications for various print job events.</span></span>


## <a name="get-started-with-change-notifications"></a><span data-ttu-id="ac03a-109">Начало работы с уведомлениями об изменениях</span><span class="sxs-lookup"><span data-stu-id="ac03a-109">Get started with change notifications</span></span>

<span data-ttu-id="ac03a-110">Чтобы использовать уведомления об изменениях посредством Microsoft Graph, вы должны [зарегистрировать свое приложение в Azure](/azure/active-directory/develop/howto-create-service-principal-portal#register-an-application-with-azure-ad-and-create-a-service-principal) и подготовить приложение в клиенте Azure Active Directory (Azure AD) пользователей.</span><span class="sxs-lookup"><span data-stu-id="ac03a-110">Before you can take advantage of change notifications via Microsoft Graph, you must [register your application in Azure](/azure/active-directory/develop/howto-create-service-principal-portal#register-an-application-with-azure-ad-and-create-a-service-principal) and provision your application in the customers Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="ac03a-111">Включите требуемые области разрешений для приложения, как описано далее в этой статье.</span><span class="sxs-lookup"><span data-stu-id="ac03a-111">Make sure that the application has the required permission scopes enabled, as described later in this article.</span></span>


### <a name="notifications-and-subscriptions"></a><span data-ttu-id="ac03a-112">Уведомления и подписки</span><span class="sxs-lookup"><span data-stu-id="ac03a-112">Notifications and subscriptions</span></span>

<span data-ttu-id="ac03a-113">В настоящее время универсальная печать поддерживает уведомления для двух сценариев, связанных с заданиями печати.</span><span class="sxs-lookup"><span data-stu-id="ac03a-113">Universal Print currently supports notifications for two scenarios related to print jobs:</span></span>

* <span data-ttu-id="ac03a-114">Инициирована задача PrintTask (JobStarted): приложение может подписаться на получение уведомлений при инициировании printTask(hook).</span><span class="sxs-lookup"><span data-stu-id="ac03a-114">PrintTask is triggered (JobStarted): An application can subscribe to receive notifications when their printTask(hook) is triggered.</span></span>
<span data-ttu-id="ac03a-115">Дополнительные сведения о том, как инициировать задачу, см. в разделе [Расширение универсальной печати для поддержки печати по запросу](./universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="ac03a-115">For details about how to trigger a task, see [Extending Universal Print to support pull printing](./universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing).</span></span> <span data-ttu-id="ac03a-116">В настоящее задачу printTask можно инициировать только для события JobStarted.</span><span class="sxs-lookup"><span data-stu-id="ac03a-116">Currently, a printTask can be triggered only for a JobStarted event.</span></span> <span data-ttu-id="ac03a-117">Событие JobStarted возникает, когда создано задание печати, загружены его полезные данные и запущена обработка задания.</span><span class="sxs-lookup"><span data-stu-id="ac03a-117">A JobStarted event is raised when a print job has been successfully created, its payload has been uploaded, and job processing has started.</span></span>  

* <span data-ttu-id="ac03a-118">JobFetchable: после запуска задания сторонние приложения печати или универсальная печать могут выполнять некоторую обработку (например, преобразовать полезные данные XPS в формат PDF для принтера PDF).</span><span class="sxs-lookup"><span data-stu-id="ac03a-118">JobFetchable: After the job has started, third-party print applications or Universal Print might do some processing (like converting XPS payload to PDF for a PDF printer).</span></span> <span data-ttu-id="ac03a-119">После завершения обработки и готовности полезных данных к загрузке принтером возникает событие JobFetchable для соответствующего задания печати.</span><span class="sxs-lookup"><span data-stu-id="ac03a-119">After processing is complete and the payload is ready to be downloaded by a printer, a JobFetchable event is raised for the corresponding print job.</span></span>

>[!NOTE]
><span data-ttu-id="ac03a-120">Чтобы прослушивать уведомления об изменениях для события JobFetchable, не требуется ресурс **printTaskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="ac03a-120">For listening to the change notifications for JobFetchable event, a **printTaskDefinition** resource is not required.</span></span>

### <a name="create-an-application-to-listen-to-notifications"></a><span data-ttu-id="ac03a-121">Создание приложения для прослушивания уведомлений</span><span class="sxs-lookup"><span data-stu-id="ac03a-121">Create an application to listen to notifications</span></span>

<span data-ttu-id="ac03a-122">Сведения о том, как прослушивать уведомления Microsoft Graph, см. в разделах [Использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges/) и [Настройка уведомлений об изменениях пользовательских данных — примеры кода](./webhooks.md#code-samples).</span><span class="sxs-lookup"><span data-stu-id="ac03a-122">For information about how to listen for Microsoft Graph notifications, see [Use change notifications and track changes with Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges/) and [Set up notifications for changes in user data – Code Samples](./webhooks.md#code-samples).</span></span>


### <a name="scopes"></a><span data-ttu-id="ac03a-123">Области</span><span class="sxs-lookup"><span data-stu-id="ac03a-123">Scopes</span></span>

<span data-ttu-id="ac03a-124">Чтобы подписаться на уведомления о заданиях печати, для приложений должны быть утверждены следующие области разрешений в клиенте Azure AD пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac03a-124">To subscribe to notifications for print jobs, applications must have the following permission scopes approved in the customer’s Azure AD tenant:</span></span> 

* <span data-ttu-id="ac03a-125">Для инициированного события printTask (JobStarted) разрешения перечислены в статье [Получение taskDefinition](/graph/api/printtaskdefinition-get?view=graph-rest-v1.0&tabs=http%22%20%5Cl%20%22permissions%22%20%5C).</span><span class="sxs-lookup"><span data-stu-id="ac03a-125">For printTask triggered (JobStarted) event, the permissions listed in [Get taskDefinition](/graph/api/printtaskdefinition-get?view=graph-rest-v1.0&tabs=http%22%20%5Cl%20%22permissions%22%20%5C).</span></span> 

* <span data-ttu-id="ac03a-126">Для события JobFetchable разрешения перечислены в статье [Создание подписки](/graph/api/subscription-post-subscriptions?view=graph-rest-v1.0&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="ac03a-126">For JobFetchable event, the permissions listed in [Create subscription](/graph/api/subscription-post-subscriptions?view=graph-rest-v1.0&tabs=http).</span></span>

<span data-ttu-id="ac03a-127">Приложения должны [создавать и использовать маркер безопасности Azure AD](/graph/auth-v2-service?context=graph%2Fapi%2F1.0) в заголовке запроса API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ac03a-127">Applications must [generate and use the Azure AD security token](/graph/auth-v2-service?context=graph%2Fapi%2F1.0) in the Microsoft Graph API request header.</span></span> <span data-ttu-id="ac03a-128">Маркер безопасности содержит утверждения согласно областям, одобренным администратором для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ac03a-128">The security token contains the claims as per the scopes approved for the customer’s Azure AD tenant by its administrator.</span></span>  


## <a name="create-subscription-printtask-triggered-jobstarted-event"></a><span data-ttu-id="ac03a-129">Создание подписки: инициировано событие printTask (JobStarted)</span><span class="sxs-lookup"><span data-stu-id="ac03a-129">Create subscription: printTask triggered (JobStarted) event</span></span> 

<span data-ttu-id="ac03a-130">Некоторые приложения отслеживают очереди печати для входящих заданий и хотят получать уведомления сразу при появлении действительного задания в очереди.</span><span class="sxs-lookup"><span data-stu-id="ac03a-130">Some applications monitor print queues for incoming jobs and want to be notified as soon as there is a valid job in the queue.</span></span> <span data-ttu-id="ac03a-131">После уведомления они могут собирать соответствующие метаданные задания или даже вносить изменения в задание печати, включая отмену задания или его перенаправление из текущей очереди печати в другую очередь после соответствующего изменения атрибутов задания.</span><span class="sxs-lookup"><span data-stu-id="ac03a-131">After they're notified, they can collect the relevant job metadata or even perform modifications in the print job – including aborting the job or redirecting the job from the current print queue to another queue after modifying the job attributes accordingly.</span></span> 

<span data-ttu-id="ac03a-132">Перед созданием уведомления для инициированного события **printTask**, убедитесь, что приложение создало следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ac03a-132">Before creating a notification for a **printTask**-triggered event, ensure that application has created the following:</span></span> 

- <span data-ttu-id="ac03a-133">[printTaskDefinition](/graph/api/print-post-taskdefinitions?view=graph-rest-v1.0&tabs=http)  для клиента Azure AD пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac03a-133">A [printTaskDefinition](/graph/api/print-post-taskdefinitions?view=graph-rest-v1.0&tabs=http) for the customer’s Azure AD tenant.</span></span> <span data-ttu-id="ac03a-134">Одно определение задачи можно связать с одним или несколькими принтерами в одном клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ac03a-134">A single task definition can be associated with one or more printers within the same Azure AD tenant.</span></span> 

- <span data-ttu-id="ac03a-135">[printTaskTrigger](/graph/api/printer-post-tasktriggers?view=graph-rest-v1.0&tabs=http) для всех очередей принтеров, для которых партнер хочет получать уведомление при запуске нового задания печати.</span><span class="sxs-lookup"><span data-stu-id="ac03a-135">A [printTaskTrigger](/graph/api/printer-post-tasktriggers?view=graph-rest-v1.0&tabs=http) for each of the printer queues for which the partner wants to receive a notification when a new print job starts.</span></span> <span data-ttu-id="ac03a-136">**printTaskTrigger** требуется связать с **printTaskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="ac03a-136">The **printTaskTrigger** needs to be bound to the **printTaskDefinition**.</span></span> 

>[!NOTE]
><span data-ttu-id="ac03a-137">Один принтер можно связать только с одним объектом **printTaskTrigger**, а один объект **printTaskTrigger** можно связать только с одним элементом **printTaskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="ac03a-137">One printer can be associated with only one **printTaskTrigger** and one **printTaskTrigger** can be associated with only one **printTaskDefinition**.</span></span> <span data-ttu-id="ac03a-138">Однако один элемент **printTaskDefinition** можно связать с несколькими объектами **printTaskTriggers**.</span><span class="sxs-lookup"><span data-stu-id="ac03a-138">However, one **printTaskDefinition** can have one or more **printTaskTriggers** associated with it.</span></span> 

<span data-ttu-id="ac03a-139">С помощью элемента **printTaskDefinition**, существующего для клиента Azure AD пользователя, приложение может [создать подписку на инициированное событие printTask (JobStarted) с помощью printTaskDefinition](/graph/api/subscription-post-subscriptions?view=graph-rest-v1.0&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="ac03a-139">With the **printTaskDefinition** that exists for customer’s Azure AD tenant, the application can [create a subscription for a printTask triggered (JobStarted) event using the printTaskDefinition](/graph/api/subscription-post-subscriptions?view=graph-rest-v1.0&tabs=http).</span></span> <span data-ttu-id="ac03a-140">При создании подписки:</span><span class="sxs-lookup"><span data-stu-id="ac03a-140">While creating the subscription:</span></span>  

* <span data-ttu-id="ac03a-141">Полю `resource` требуется присвоить значение `print/taskDefinitions/{printTaskDefinition ID}/tasks`.</span><span class="sxs-lookup"><span data-stu-id="ac03a-141">The `resource` field needs to be set as `print/taskDefinitions/{printTaskDefinition ID}/tasks`.</span></span> 
* <span data-ttu-id="ac03a-142">Полю `changeType` требуется присвоить значение `created`.</span><span class="sxs-lookup"><span data-stu-id="ac03a-142">The `changeType` field needs to be set as `created`.</span></span> 
* <span data-ttu-id="ac03a-143">Поле `expirationDateTime` не должное превышать [максимальный срок действия](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="ac03a-143">The `expirationDateTime` field needs to be less than the [maximum expiration time](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type).</span></span> 

<span data-ttu-id="ac03a-144">Дополнительные сведения см. в разделе [Свойства типа ресурса subscription](/graph/api/resources/subscription?view=graph-rest-v1.0#properties).</span><span class="sxs-lookup"><span data-stu-id="ac03a-144">For more details, see [Subscription resource type properties](/graph/api/resources/subscription?view=graph-rest-v1.0#properties).</span></span>

<span data-ttu-id="ac03a-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac03a-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/v1.0/subscriptions 
Content-Type: application/json
{ 
    "changeType":"created", 
    "resource":"print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "clientState":"secret", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "expirationDateTime":"2020-01-30T22:42:09Z" 
} 
```

### <a name="response"></a><span data-ttu-id="ac03a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac03a-146">Response</span></span>

<span data-ttu-id="ac03a-147">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac03a-147">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity", 
    "id": "{Subscription ID}", 
    "resource": "print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "applicationId": "{application ID}", 
    "changeType": "created", 
    "clientState": "secret", 
    "notificationUrl": "{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "notificationQueryOptions": null, 
    "lifecycleNotificationUrl": null, 
    "expirationDateTime": "2020-12-30T22:42:09Z", 
    "creatorId": "{Creator ID}", 
    "includeResourceData": null, 
    "latestSupportedTlsVersion": "v1_2", 
    "encryptionCertificate": null, 
    "encryptionCertificateId": null 
}
```


## <a name="create-subscription-jobfetchable-event"></a><span data-ttu-id="ac03a-148">Создание подписки: событие JobFetchable</span><span class="sxs-lookup"><span data-stu-id="ac03a-148">Create subscription: JobFetchable event</span></span> 
<span data-ttu-id="ac03a-149">Некоторым облачным приложениям требуется скачивать задания печати из универсальной печати, когда они будут готовы.</span><span class="sxs-lookup"><span data-stu-id="ac03a-149">Some cloud applications need to download print jobs from Universal Print when they are ready.</span></span> <span data-ttu-id="ac03a-150">Так как такие приложения, работающие в облаке, находятся вне границ брандмауэра пользователя, они могут использовать уведомления об изменениях Microsoft Graph, чтобы узнавать о готовности заданий печати к скачиванию.</span><span class="sxs-lookup"><span data-stu-id="ac03a-150">Because these applications running in the cloud are not behind the customer's firewall, they can use Microsoft Graph change notifications to be notified when a print job is ready to be downloaded.</span></span>

>[!NOTE]
><span data-ttu-id="ac03a-151">Задания печати нельзя изменить после их перехода в состояние JobFetchable.</span><span class="sxs-lookup"><span data-stu-id="ac03a-151">Print jobs can't be modified when they enter the JobFetchable state.</span></span>
<span data-ttu-id="ac03a-152">Уведомление JobFetchable требуется создавать для каждой очереди принтера.</span><span class="sxs-lookup"><span data-stu-id="ac03a-152">A JobFetchable notification needs to be created for each printer queue.</span></span> <span data-ttu-id="ac03a-153">При создании подписки:</span><span class="sxs-lookup"><span data-stu-id="ac03a-153">While creating the subscription:</span></span>
* <span data-ttu-id="ac03a-154">Полю `resource` требуется присвоить значение "print/printers/{printer id}/jobs".</span><span class="sxs-lookup"><span data-stu-id="ac03a-154">The `resource` field needs to be set as 'print/printers/{printer id}/jobs'.</span></span> 
* <span data-ttu-id="ac03a-155">Полю `changeType` требуется присвоить значение `updated`.</span><span class="sxs-lookup"><span data-stu-id="ac03a-155">The `changeType` field needs to be set as `updated`.</span></span> 
* <span data-ttu-id="ac03a-156">Полю `notificationQueryOptions` требуется присвоить значение `$filter = isFetchable eq true`.</span><span class="sxs-lookup"><span data-stu-id="ac03a-156">The `notificationQueryOptions` field needs to be set as `$filter = isFetchable eq true`.</span></span> 
* <span data-ttu-id="ac03a-157">Поле `expirationDateTime` не должное превышать [максимальный срок действия](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="ac03a-157">The `expirationDateTime` field needs to be less than the [maximum expiration time](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type).</span></span> 

<span data-ttu-id="ac03a-158">Дополнительные сведения см. в разделе [Свойства типа ресурса subscription](/graph/api/resources/subscription?view=graph-rest-v1.0#properties).</span><span class="sxs-lookup"><span data-stu-id="ac03a-158">For more details, see [Subscription resource type properties](/graph/api/resources/subscription?view=graph-rest-v1.0#properties).</span></span>

<span data-ttu-id="ac03a-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac03a-159">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
    "changeType":"updated",
    "resource":"print/printers/{printer id}/jobs",
    "notificationQueryOptions": "$filter = isFetchable eq true", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}",
    "expirationDateTime":"2020-12-30T22:42:09Z",
    "clientState":"mysecret"
} 
```

### <a name="response"></a><span data-ttu-id="ac03a-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac03a-160">Response</span></span>

<span data-ttu-id="ac03a-161">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac03a-161">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity", 
    "id": "{Subscription ID}", 
    "resource": "print/printers/{printer ID}/jobs", 
    "applicationId": "{Application ID}", 
    "changeType": "updated", 
    "clientState": "mysecret", 
    "notificationUrl": "{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "notificationQueryOptions": "$filter = isFetchable eq true", 
    "lifecycleNotificationUrl": null, 
    "expirationDateTime": "2020-12-30T22:42:09Z", 
    "creatorId": "{Creator ID}", 
    "includeResourceData": null, 
    "latestSupportedTlsVersion": "v1_2", 
    "encryptionCertificate": null, 
    "encryptionCertificateId": null
}
```


## <a name="renewing-a-notification-subscription"></a><span data-ttu-id="ac03a-162">Возобновление подписки на уведомления</span><span class="sxs-lookup"><span data-stu-id="ac03a-162">Renewing a notification subscription</span></span>

<span data-ttu-id="ac03a-163">В Microsoft Graph срок действия ограничен.</span><span class="sxs-lookup"><span data-stu-id="ac03a-163">Microsoft Graph has a limit on the expiration time.</span></span> <span data-ttu-id="ac03a-164">Дополнительные сведения см. в разделе о [максимальном сроке действия](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="ac03a-164">For details, see [maximum expiration time](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type).</span></span> <span data-ttu-id="ac03a-165">Чтобы продолжать получать уведомления, подписку требуется периодически обновлять с помощью [API обновления подписки](/graph/api/subscription-update?view=graph-rest-v1.0&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="ac03a-165">To continue receiving notifications, the subscription needs to be renewed periodically by using the [Update subscription API](/graph/api/subscription-update?view=graph-rest-v1.0&tabs=http).</span></span> 

## <a name="other-operations-on-notification-subscriptions"></a><span data-ttu-id="ac03a-166">Другие операции с подпиской на уведомления</span><span class="sxs-lookup"><span data-stu-id="ac03a-166">Other operations on notification subscriptions</span></span> 

<span data-ttu-id="ac03a-167">Приложения могут [получать](/graph/api/subscription-get?view=graph-rest-v1.0&tabs=http) сведения о подписке или [удалять](/graph/api/subscription-delete?view=graph-rest-v1.0&tabs=http) подписку при необходимости.</span><span class="sxs-lookup"><span data-stu-id="ac03a-167">Applications can [get](/graph/api/subscription-get?view=graph-rest-v1.0&tabs=http) details of the subscription or can [delete](/graph/api/subscription-delete?view=graph-rest-v1.0&tabs=http) a subscription when required.</span></span> <span data-ttu-id="ac03a-168">Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](/graph/api/resources/webhooks?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="ac03a-168">For details, see [Use the Microsoft Graph API to get change notifications](/graph/api/resources/webhooks?view=graph-rest-v1.0).</span></span>


## <a name="faqs"></a><span data-ttu-id="ac03a-169">Вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="ac03a-169">FAQs</span></span>
### <a name="how-does-microsoft-graph-validate-notification-urls"></a><span data-ttu-id="ac03a-170">Как Microsoft Graph проверяет URL-адреса уведомлений?</span><span class="sxs-lookup"><span data-stu-id="ac03a-170">How does Microsoft Graph validate notification URLs?</span></span>
<span data-ttu-id="ac03a-171">Прежде чем создать подписку, Microsoft Graph проверяет конечную точку уведомлений в свойстве **notificationUrl** запроса подписки.</span><span class="sxs-lookup"><span data-stu-id="ac03a-171">Microsoft Graph validates the notification endpoint provided in the **notificationUrl** property of the subscription request before creating the subscription.</span></span>
<span data-ttu-id="ac03a-172">Подробности см. в разделе [Проверка конечной точки уведомлений](./webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="ac03a-172">For details, see [Notification endpoint validation](./webhooks.md#notification-endpoint-validation).</span></span>

### <a name="what-are-applications-expected-to-do-after-receiving-a-change-notification"></a><span data-ttu-id="ac03a-173">Каковы предполагаемые действия приложений после получения уведомления об изменении?</span><span class="sxs-lookup"><span data-stu-id="ac03a-173">What are applications expected to do after receiving a change notification?</span></span>
<span data-ttu-id="ac03a-174">Приложения должны обрабатывать и подтверждать каждое полученное уведомление об изменении.</span><span class="sxs-lookup"><span data-stu-id="ac03a-174">Applications should process and acknowledge every change notification they receive.</span></span> <span data-ttu-id="ac03a-175">Подробности см. в разделе [Обработка уведомлений об изменениях](./webhooks.md#processing-the-change-notification).</span><span class="sxs-lookup"><span data-stu-id="ac03a-175">For details, see [Processing the change notification](./webhooks.md#processing-the-change-notification).</span></span>

### <a name="how-can-i-get-a-list-of-active-subscriptions"></a><span data-ttu-id="ac03a-176">Как получить список активных подписок?</span><span class="sxs-lookup"><span data-stu-id="ac03a-176">How can I get a list of active subscriptions?</span></span>
<span data-ttu-id="ac03a-177">Сведения о том, как получить список подписок на веб-перехватчики, см. в разделе [Перечисление подписок](/graph/api/subscription-list?view=graph-rest-v1.0&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="ac03a-177">For details about how to retrieve a list of webhook subscriptions, see [List subscriptions](/graph/api/subscription-list?view=graph-rest-v1.0&tabs=http).</span></span>


## <a name="see-also"></a><span data-ttu-id="ac03a-178">См. также</span><span class="sxs-lookup"><span data-stu-id="ac03a-178">See also</span></span>

- <span data-ttu-id="ac03a-179">Дополнительные сведения об API облачной печати в Microsoft Graph см. в статье [Обзор API облачной среды универсальной печати](/graph/universal-print-concept-overview).</span><span class="sxs-lookup"><span data-stu-id="ac03a-179">To learn more about the cloud printing API in Microsoft Graph, see [Universal Print cloud printing API overview](/graph/universal-print-concept-overview).</span></span> 
- <span data-ttu-id="ac03a-180">Чтобы отправить предложения и отзывы об API облачной печати в Microsoft Graph, перейдите в [техническое сообщество универсальной печати](https://aka.ms/community/UniversalPrint).</span><span class="sxs-lookup"><span data-stu-id="ac03a-180">For suggestions or feedback about the cloud printing API in Microsoft Graph, visit the [Universal Print tech community](https://aka.ms/community/UniversalPrint).</span></span>
