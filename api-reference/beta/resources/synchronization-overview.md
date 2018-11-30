---
title: Обзор синхронизации API Azure AD
description: ') позволяет автоматизировать создания, обслуживания и удаления удостоверений в облако (программное обеспечение как службы или SaaS) приложениями, такими как общего банка данных, Salesforce, ServiceNow и многое другое. API синхронизации можно использовать в Microsoft Graph для управления синхронизацией identity программным путем, включая:'
ms.openlocfilehash: ff3acb00801c9b04b8257345b06100297e11710c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081460"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="4e5d1-104">Обзор синхронизации API Azure AD</span><span class="sxs-lookup"><span data-stu-id="4e5d1-104">Azure AD synchronization API overview</span></span>

> <span data-ttu-id="4e5d1-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e5d1-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e5d1-107">Azure (Azure AD) удостоверений синхронизации с Active Directory (также называемая «Подготовка») позволяет автоматизировать создания, обслуживания и удаления удостоверений в облаке (программное обеспечение как службы или SaaS) приложениями, такими как общего банка данных, Salesforce, ServiceNow, и многое другое.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-107">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="4e5d1-108">API синхронизации можно использовать в Microsoft Graph для управления синхронизацией identity программным путем, включая:</span><span class="sxs-lookup"><span data-stu-id="4e5d1-108">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="4e5d1-109">Создание, запуск и остановка задания синхронизации</span><span class="sxs-lookup"><span data-stu-id="4e5d1-109">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="4e5d1-110">Вносить изменения в схеме синхронизации для задания</span><span class="sxs-lookup"><span data-stu-id="4e5d1-110">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="4e5d1-111">Проверка текущего состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="4e5d1-111">Verify the current synchronization status</span></span> 

<span data-ttu-id="4e5d1-112">Дополнительные сведения о синхронизации в Azure AD см.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-112">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="4e5d1-113">Автоматизировать пользователя обеспечение и Отмена обеспечения SaaS приложений с помощью Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4e5d1-113">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="4e5d1-114">Управление для корпоративных приложений в портале Azure при подготовке учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="4e5d1-114">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="4e5d1-115">Можно также попробовать API в [Обозревателе график](https://developer.microsoft.com/graph/graph-explorer) в пример клиента или собственного клиента.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-115">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="4e5d1-116">Задание синхронизации</span><span class="sxs-lookup"><span data-stu-id="4e5d1-116">Synchronization job</span></span>

<span data-ttu-id="4e5d1-117">Задания синхронизации для выполнения синхронизации периодически выполняется в фоновом режиме, опроса для изменения в один каталог и помещает их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-117">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="4e5d1-118">Задание синхронизации всегда специально для конкретного экземпляра приложения клиента.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-118">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="4e5d1-119">Как часть процесса установки задания синхронизации необходимо предоставить разрешение на чтение и запись в целевом каталоге объекты и настройке задания синхронизации схемы.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-119">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="4e5d1-120">Для получения дополнительных сведений см [Задание синхронизации](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="4e5d1-120">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="4e5d1-121">Схема синхронизации</span><span class="sxs-lookup"><span data-stu-id="4e5d1-121">Synchronization schema</span></span>

<span data-ttu-id="4e5d1-122">Схема синхронизации определяет объекты, которые будут синхронизированы и как они будут синхронизироваться.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-122">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="4e5d1-123">Схема синхронизации содержит основные сведения об установке для задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-123">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="4e5d1-124">Как правило будет настроить некоторые [атрибут сопоставления](synchronization-attributemapping.md)или добавить [области видимости фильтров](synchronization-filter.md) синхронизировать только объекты, удовлетворяющие определенному условию.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-124">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="4e5d1-125">Схема синхронизации включает в себя следующие компоненты:</span><span class="sxs-lookup"><span data-stu-id="4e5d1-125">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="4e5d1-126">Определения каталогов</span><span class="sxs-lookup"><span data-stu-id="4e5d1-126">Directory definitions</span></span>
- <span data-ttu-id="4e5d1-127">Правила синхронизации</span><span class="sxs-lookup"><span data-stu-id="4e5d1-127">Synchronization rules</span></span>
- <span data-ttu-id="4e5d1-128">Объект сопоставления</span><span class="sxs-lookup"><span data-stu-id="4e5d1-128">Object mappings</span></span>

<span data-ttu-id="4e5d1-129">Для получения дополнительных сведений см [синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="4e5d1-129">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="4e5d1-130">Шаблон синхронизации</span><span class="sxs-lookup"><span data-stu-id="4e5d1-130">Synchronization template</span></span>

<span data-ttu-id="4e5d1-131">Шаблон синхронизации предоставляет параметры предварительно настроенным синхронизации для конкретного приложения.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-131">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="4e5d1-132">Эти параметры (важнее, [синхронизации схемы](synchronization-synchronizationschema.md)) будет использоваться по умолчанию для любое [Задание синхронизации](synchronization-synchronizationjob.md) , основанный на шаблоне.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-132">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="4e5d1-133">Шаблоны задаются разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-133">Templates are specified by the application developer.</span></span>

<span data-ttu-id="4e5d1-134">Для получения дополнительных сведений см [шаблон синхронизации](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="4e5d1-134">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="4e5d1-135">Работа с API синхронизации</span><span class="sxs-lookup"><span data-stu-id="4e5d1-135">Working with the synchronization API</span></span>

<span data-ttu-id="4e5d1-136">Работа с синхронизацией API в основном состоит из доступ к ресурсам [synchronizationJob](synchronization-synchronizationjob.md) и [synchronizationSchema](synchronization-synchronizationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="4e5d1-136">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="4e5d1-137">Чтобы найти [synchronizationJob](synchronization-synchronizationjob.md) ресурса, необходимо знать идентификатор объекта-участника службы, к которой принадлежит задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-137">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="4e5d1-138">В приведенных ниже примерах показано, как работать с ресурсами **synchronizationJob** и **synchronizationSchema** .</span><span class="sxs-lookup"><span data-stu-id="4e5d1-138">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="4e5d1-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e5d1-139">Authorization</span></span>

<span data-ttu-id="4e5d1-140">Интерфейс API синхронизации Azure AD для авторизации используется OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-140">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="4e5d1-141">Прежде чем вносить какие-либо запросы API-интерфейса, необходимо получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-141">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="4e5d1-142">Для получения дополнительных сведений см [маркеры доступа Get для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="4e5d1-142">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="4e5d1-143">Для доступа к ресурсам синхронизации, приложению Directory.ReadWrite.All разрешения.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-143">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="4e5d1-144">Для получения дополнительных сведений см [разрешения для каталога](/graph/permissions-reference#directory-permissions).</span><span class="sxs-lookup"><span data-stu-id="4e5d1-144">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="4e5d1-145">Найдите объект участника службы по отображаемому имени</span><span class="sxs-lookup"><span data-stu-id="4e5d1-145">Find the service principal object by display name</span></span>

<span data-ttu-id="4e5d1-146">Следующем примере показано, как для объекта-участника службы поиска по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-146">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="4e5d1-147">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="4e5d1-147">**Request**</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="4e5d1-148">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="4e5d1-148">**Response**</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="4e5d1-149">Найдите объект участника службы по Идентификатору приложения</span><span class="sxs-lookup"><span data-stu-id="4e5d1-149">Find the service principal object by app ID</span></span>

<span data-ttu-id="4e5d1-150">Следующем примере показано, как найти объекта участника-службы с идентификатором приложения.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-150">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="4e5d1-151">**Запрос** 
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4e5d1-151">**Request** 
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="4e5d1-152">**Ответа**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4e5d1-152">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="4e5d1-153">Список существующих заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="4e5d1-153">List existing synchronization jobs</span></span>

<span data-ttu-id="4e5d1-154">Следующем примере показано, как список существующих заданий синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-154">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="4e5d1-155">**Запрос**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4e5d1-155">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="4e5d1-156">**Ответа**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4e5d1-156">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a><span data-ttu-id="4e5d1-157">Получить сведения о состоянии задания синхронизации</span><span class="sxs-lookup"><span data-stu-id="4e5d1-157">Get synchronization job status</span></span>
<span data-ttu-id="4e5d1-158">Следующем примере показано, как получить сведения о состоянии задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-158">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="4e5d1-159">**Запрос**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4e5d1-159">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="4e5d1-160">**Ответа**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4e5d1-160">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a><span data-ttu-id="4e5d1-161">Получение схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="4e5d1-161">Get synchronization schema</span></span>
<span data-ttu-id="4e5d1-162">Следующем примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4e5d1-162">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="4e5d1-163">**Запрос**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4e5d1-163">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="4e5d1-164">**Ответа**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="4e5d1-164">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="4e5d1-165">См. также</span><span class="sxs-lookup"><span data-stu-id="4e5d1-165">See also</span></span>

* [<span data-ttu-id="4e5d1-166">Настройка синхронизации с расширением атрибутов каталога</span><span class="sxs-lookup"><span data-stu-id="4e5d1-166">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="4e5d1-167">Настройка синхронизации с помощью настраиваемого конечного атрибутов</span><span class="sxs-lookup"><span data-stu-id="4e5d1-167">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



