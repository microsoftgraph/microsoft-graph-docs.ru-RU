---
title: Общие сведения об API синхронизации Azure AD
description: ') позволяет автоматизировать создание, Обслуживание и удаление удостоверений в приложениях Cloud (программное обеспечение, в качестве службы или SaaS), таких как Dropbox, Salesforce, ServiceNow и т. д. С помощью API синхронизации в Microsoft Graph можно управлять синхронизацией удостоверений программным способом, в том числе:'
localization_priority: Normal
doc_type: conceptualPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62c127b632277a93312afd7682939049b1e9de68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520144"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="5cf29-104">Общие сведения об API синхронизации Azure AD</span><span class="sxs-lookup"><span data-stu-id="5cf29-104">Azure AD synchronization API overview</span></span>

<span data-ttu-id="5cf29-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5cf29-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cf29-106">Синхронизация удостоверений Azure Active Directory (также называемая "наполнением") позволяет автоматизировать создание, Обслуживание и удаление удостоверений в Cloud (программное обеспечение, в виде службы или SaaS), например Dropbox, Salesforce, ServiceNow и многое другое.</span><span class="sxs-lookup"><span data-stu-id="5cf29-106">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="5cf29-107">С помощью API синхронизации в Microsoft Graph можно управлять синхронизацией удостоверений программным способом, в том числе:</span><span class="sxs-lookup"><span data-stu-id="5cf29-107">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="5cf29-108">Создание, запуск и остановка заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="5cf29-108">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="5cf29-109">Внесение изменений в схему синхронизации для заданий</span><span class="sxs-lookup"><span data-stu-id="5cf29-109">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="5cf29-110">Проверка текущего состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="5cf29-110">Verify the current synchronization status</span></span>

<span data-ttu-id="5cf29-111">Дополнительные сведения о синхронизации в Azure AD приведены в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="5cf29-111">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="5cf29-112">Автоматизация подготовки пользователей и их отмена в приложениях SaaS с помощью Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="5cf29-112">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="5cf29-113">Управление предоставлением учетных записей пользователей для корпоративных приложений на портале Azure</span><span class="sxs-lookup"><span data-stu-id="5cf29-113">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="5cf29-114">Вы также можете попробовать API в [проводнике Graph](https://developer.microsoft.com/graph/graph-explorer) в образце клиента или в собственном клиенте.</span><span class="sxs-lookup"><span data-stu-id="5cf29-114">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="5cf29-115">Задание синхронизации</span><span class="sxs-lookup"><span data-stu-id="5cf29-115">Synchronization job</span></span>

<span data-ttu-id="5cf29-116">Задания синхронизации выполняют синхронизацию, периодически запуская в фоновом режиме, запрашивают изменения в одном каталоге и отправляют их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="5cf29-116">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="5cf29-117">Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5cf29-117">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="5cf29-118">В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="5cf29-118">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="5cf29-119">Более подробную информацию можно узнать в статье [Задание синхронизации](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="5cf29-119">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="5cf29-120">Схема синхронизации</span><span class="sxs-lookup"><span data-stu-id="5cf29-120">Synchronization schema</span></span>

<span data-ttu-id="5cf29-121">Схема синхронизации определяет объекты, которые будут синхронизированы и как они будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="5cf29-121">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="5cf29-122">Схема синхронизации содержит большую часть сведений о настройке для определенного задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5cf29-122">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="5cf29-123">Как правило, вы настраиваете некоторые [сопоставления атрибутов](synchronization-attributemapping.md)или добавляете [Фильтр областей](synchronization-filter.md) для синхронизации только объектов, удовлетворяющих определенному условию.</span><span class="sxs-lookup"><span data-stu-id="5cf29-123">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="5cf29-124">Схема синхронизации включает в себя следующие компоненты:</span><span class="sxs-lookup"><span data-stu-id="5cf29-124">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="5cf29-125">Определения каталогов</span><span class="sxs-lookup"><span data-stu-id="5cf29-125">Directory definitions</span></span>
- <span data-ttu-id="5cf29-126">Правила синхронизации</span><span class="sxs-lookup"><span data-stu-id="5cf29-126">Synchronization rules</span></span>
- <span data-ttu-id="5cf29-127">Сопоставления объектов</span><span class="sxs-lookup"><span data-stu-id="5cf29-127">Object mappings</span></span>

<span data-ttu-id="5cf29-128">Более подробную информацию можно узнать в статье [схема синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="5cf29-128">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="5cf29-129">Шаблон синхронизации</span><span class="sxs-lookup"><span data-stu-id="5cf29-129">Synchronization template</span></span>

<span data-ttu-id="5cf29-130">Шаблон синхронизации предоставляет предварительно настроенные параметры синхронизации для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="5cf29-130">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="5cf29-131">Эти параметры (наиболее важное, [схема синхронизации](synchronization-synchronizationschema.md)) будут использоваться по умолчанию для всех [заданий синхронизации](synchronization-synchronizationjob.md) , основанных на этом шаблоне.</span><span class="sxs-lookup"><span data-stu-id="5cf29-131">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="5cf29-132">Шаблоны задаются разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5cf29-132">Templates are specified by the application developer.</span></span>

<span data-ttu-id="5cf29-133">Для получения дополнительных сведений см [шаблон синхронизации](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="5cf29-133">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="5cf29-134">Работа с API синхронизации</span><span class="sxs-lookup"><span data-stu-id="5cf29-134">Working with the synchronization API</span></span>

<span data-ttu-id="5cf29-135">Работа с API синхронизации в основном включает доступ к ресурсам [синчронизатионжоб](synchronization-synchronizationjob.md) и [синчронизатионсчема](synchronization-synchronizationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="5cf29-135">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="5cf29-136">Чтобы найти ресурс [синчронизатионжоб](synchronization-synchronizationjob.md) , необходимо знать идентификатор объекта участника службы, к которому относится задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5cf29-136">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="5cf29-137">В приведенных ниже примерах показано, как работать с ресурсами **синчронизатионжоб** и **синчронизатионсчема** .</span><span class="sxs-lookup"><span data-stu-id="5cf29-137">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="5cf29-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cf29-138">Authorization</span></span>

<span data-ttu-id="5cf29-139">API синхронизации Azure AD использует OAuth 2,0 для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5cf29-139">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="5cf29-140">Перед выполнением запросов к API необходимо получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="5cf29-140">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="5cf29-141">Дополнительные сведения [можно найти в статье получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="5cf29-141">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="5cf29-142">Для доступа к ресурсам синхронизации приложению требуются разрешения Directory. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="5cf29-142">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="5cf29-143">Для получения дополнительных сведений ознакомьтесь с [разрешениями для каталогов](/graph/permissions-reference#directory-permissions).</span><span class="sxs-lookup"><span data-stu-id="5cf29-143">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="5cf29-144">Поиск объекта субъекта службы по отображаемому имени</span><span class="sxs-lookup"><span data-stu-id="5cf29-144">Find the service principal object by display name</span></span>

<span data-ttu-id="5cf29-145">В приведенном ниже примере показано, как найти объект участника службы по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="5cf29-145">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="5cf29-146">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="5cf29-146">**Request**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="5cf29-147">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="5cf29-147">**Response**</span></span>

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

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="5cf29-148">Поиск объекта субъекта службы по ИДЕНТИФИКАТОРу приложения</span><span class="sxs-lookup"><span data-stu-id="5cf29-148">Find the service principal object by app ID</span></span>

<span data-ttu-id="5cf29-149">В приведенном ниже примере показано, как найти объект субъекта службы по ИДЕНТИФИКАТОРу приложения.</span><span class="sxs-lookup"><span data-stu-id="5cf29-149">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="5cf29-150">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="5cf29-150">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="5cf29-151">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="5cf29-151">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
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

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="5cf29-152">Перечисление существующих заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="5cf29-152">List existing synchronization jobs</span></span>

<span data-ttu-id="5cf29-153">В приведенном ниже примере показано, как перечислить существующие задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5cf29-153">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="5cf29-154">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="5cf29-154">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="5cf29-155">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="5cf29-155">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
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

### <a name="get-synchronization-job-status"></a><span data-ttu-id="5cf29-156">Получение состояния задания синхронизации</span><span class="sxs-lookup"><span data-stu-id="5cf29-156">Get synchronization job status</span></span>
<span data-ttu-id="5cf29-157">В приведенном ниже примере показано, как получить состояние задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5cf29-157">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="5cf29-158">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="5cf29-158">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="5cf29-159">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="5cf29-159">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
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

### <a name="get-synchronization-schema"></a><span data-ttu-id="5cf29-160">Получение схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="5cf29-160">Get synchronization schema</span></span>
<span data-ttu-id="5cf29-161">В приведенном ниже примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5cf29-161">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="5cf29-162">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="5cf29-162">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="5cf29-163">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="5cf29-163">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="5cf29-164">См. также</span><span class="sxs-lookup"><span data-stu-id="5cf29-164">See also</span></span>

* [<span data-ttu-id="5cf29-165">Настройка синхронизации с атрибутами расширения каталога</span><span class="sxs-lookup"><span data-stu-id="5cf29-165">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="5cf29-166">Настройка синхронизации с пользовательскими целевыми атрибутами</span><span class="sxs-lookup"><span data-stu-id="5cf29-166">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



