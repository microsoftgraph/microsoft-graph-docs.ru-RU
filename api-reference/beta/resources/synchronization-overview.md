---
title: Общие сведения об API синхронизации Azure AD
description: Автоматизируйте подготовку удостоверений от систем отдела кадров, Active Directory и Azure Active Directory к облачным приложениям.
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d1a2de9dcac9765899fa3eaff6173a3791984ade
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630321"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="d3bf8-103">Общие сведения об API синхронизации Azure AD</span><span class="sxs-lookup"><span data-stu-id="d3bf8-103">Azure AD synchronization API overview</span></span>

<span data-ttu-id="d3bf8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3bf8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3bf8-105">Служба синхронизации удостоверений Azure Active Directory (также называется "подготовкам") позволяет автоматизировать подготовку (создание, обслуживание) и отмену (удаление) удостоверений из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="d3bf8-105">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the provisioning (creation, maintenance) and de-provisioning (removal) of identities from any of the following:</span></span>
- <span data-ttu-id="d3bf8-106">Active Directory для Azure AD</span><span class="sxs-lookup"><span data-stu-id="d3bf8-106">Active Directory to Azure AD</span></span>
- <span data-ttu-id="d3bf8-107">Рабочий день в Azure AD</span><span class="sxs-lookup"><span data-stu-id="d3bf8-107">Workday to Azure AD</span></span>
- <span data-ttu-id="d3bf8-108">Azure AD to Cloud Applications, например Dropbox, Salesforce, ServiceNow и т. д.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-108">Azure AD to cloud applications such as Dropbox, Salesforce, ServiceNow, and more</span></span> 

<span data-ttu-id="d3bf8-109">С помощью API синхронизации в Microsoft Graph можно управлять синхронизацией удостоверений программным способом, в том числе:</span><span class="sxs-lookup"><span data-stu-id="d3bf8-109">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="d3bf8-110">Создание, запуск и остановка заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="d3bf8-110">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="d3bf8-111">Внесение изменений в схему синхронизации для заданий</span><span class="sxs-lookup"><span data-stu-id="d3bf8-111">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="d3bf8-112">Проверка текущего состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="d3bf8-112">Verify the current synchronization status</span></span>

<span data-ttu-id="d3bf8-113">Дополнительные сведения о синхронизации в Azure AD приведены в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="d3bf8-113">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="d3bf8-114">Автоматизация подготовки пользователей и их отмена в приложениях SaaS с помощью Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="d3bf8-114">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="d3bf8-115">Управление предоставлением учетных записей пользователей для корпоративных приложений на портале Azure</span><span class="sxs-lookup"><span data-stu-id="d3bf8-115">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="d3bf8-116">Вы также можете попробовать API в [проводнике Graph](https://developer.microsoft.com/graph/graph-explorer) в образце клиента или в собственном клиенте.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-116">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="d3bf8-117">Задание синхронизации</span><span class="sxs-lookup"><span data-stu-id="d3bf8-117">Synchronization job</span></span>

<span data-ttu-id="d3bf8-118">Задания синхронизации выполняют синхронизацию, периодически запуская в фоновом режиме, запрашивают изменения в одном каталоге и отправляют их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-118">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="d3bf8-119">Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-119">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="d3bf8-120">В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-120">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="d3bf8-121">Более подробную информацию можно узнать в статье [Задание синхронизации](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="d3bf8-121">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="d3bf8-122">Схема синхронизации</span><span class="sxs-lookup"><span data-stu-id="d3bf8-122">Synchronization schema</span></span>

<span data-ttu-id="d3bf8-123">Схема синхронизации определяет объекты, которые будут синхронизированы и как они будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-123">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="d3bf8-124">Схема синхронизации содержит большую часть сведений о настройке для определенного задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-124">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="d3bf8-125">Как правило, вы настраиваете некоторые [сопоставления атрибутов](synchronization-attributemapping.md)или добавляете [Фильтр областей](synchronization-filter.md) для синхронизации только объектов, удовлетворяющих определенному условию.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-125">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="d3bf8-126">Схема синхронизации включает в себя следующие компоненты:</span><span class="sxs-lookup"><span data-stu-id="d3bf8-126">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="d3bf8-127">Определения каталогов</span><span class="sxs-lookup"><span data-stu-id="d3bf8-127">Directory definitions</span></span>
- <span data-ttu-id="d3bf8-128">Правила синхронизации</span><span class="sxs-lookup"><span data-stu-id="d3bf8-128">Synchronization rules</span></span>
- <span data-ttu-id="d3bf8-129">Сопоставления объектов</span><span class="sxs-lookup"><span data-stu-id="d3bf8-129">Object mappings</span></span>

<span data-ttu-id="d3bf8-130">Более подробную информацию можно узнать в статье [схема синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="d3bf8-130">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="d3bf8-131">Шаблон синхронизации</span><span class="sxs-lookup"><span data-stu-id="d3bf8-131">Synchronization template</span></span>

<span data-ttu-id="d3bf8-132">Шаблон синхронизации предоставляет предварительно настроенные параметры синхронизации для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-132">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="d3bf8-133">Эти параметры (наиболее важное, [схема синхронизации](synchronization-synchronizationschema.md)) будут использоваться по умолчанию для всех [заданий синхронизации](synchronization-synchronizationjob.md) , основанных на этом шаблоне.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-133">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="d3bf8-134">Шаблоны задаются разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-134">Templates are specified by the application developer.</span></span>

<span data-ttu-id="d3bf8-135">Для получения дополнительных сведений см [шаблон синхронизации](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d3bf8-135">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="d3bf8-136">Работа с API синхронизации</span><span class="sxs-lookup"><span data-stu-id="d3bf8-136">Working with the synchronization API</span></span>

<span data-ttu-id="d3bf8-137">Работа с API синхронизации в основном включает доступ к ресурсам [синчронизатионжоб](synchronization-synchronizationjob.md) и [синчронизатионсчема](synchronization-synchronizationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="d3bf8-137">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="d3bf8-138">Чтобы найти ресурс [синчронизатионжоб](synchronization-synchronizationjob.md) , необходимо знать идентификатор объекта участника службы, к которому относится задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-138">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="d3bf8-139">В приведенных ниже примерах показано, как работать с ресурсами **синчронизатионжоб** и **синчронизатионсчема** .</span><span class="sxs-lookup"><span data-stu-id="d3bf8-139">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="d3bf8-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3bf8-140">Authorization</span></span>

<span data-ttu-id="d3bf8-141">API синхронизации Azure AD использует OAuth 2,0 для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-141">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="d3bf8-142">Перед выполнением запросов к API необходимо получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-142">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="d3bf8-143">Дополнительные сведения [можно найти в статье получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="d3bf8-143">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="d3bf8-144">Для доступа к ресурсам синхронизации приложению требуются разрешения Directory. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-144">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="d3bf8-145">Для получения дополнительных сведений ознакомьтесь с [разрешениями для каталогов](/graph/permissions-reference#directory-permissions).</span><span class="sxs-lookup"><span data-stu-id="d3bf8-145">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="d3bf8-146">Поиск объекта субъекта службы по отображаемому имени</span><span class="sxs-lookup"><span data-stu-id="d3bf8-146">Find the service principal object by display name</span></span>

<span data-ttu-id="d3bf8-147">В приведенном ниже примере показано, как найти объект участника службы по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-147">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="d3bf8-148">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="d3bf8-148">**Request**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="d3bf8-149">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="d3bf8-149">**Response**</span></span>

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

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="d3bf8-150">Поиск объекта субъекта службы по ИДЕНТИФИКАТОРу приложения</span><span class="sxs-lookup"><span data-stu-id="d3bf8-150">Find the service principal object by app ID</span></span>

<span data-ttu-id="d3bf8-151">В приведенном ниже примере показано, как найти объект субъекта службы по ИДЕНТИФИКАТОРу приложения.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-151">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="d3bf8-152">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="d3bf8-152">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="d3bf8-153">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="d3bf8-153">**Response**</span></span>
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

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="d3bf8-154">Перечисление существующих заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="d3bf8-154">List existing synchronization jobs</span></span>

<span data-ttu-id="d3bf8-155">В приведенном ниже примере показано, как перечислить существующие задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-155">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="d3bf8-156">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="d3bf8-156">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="d3bf8-157">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="d3bf8-157">**Response**</span></span>
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

### <a name="get-synchronization-job-status"></a><span data-ttu-id="d3bf8-158">Получение состояния задания синхронизации</span><span class="sxs-lookup"><span data-stu-id="d3bf8-158">Get synchronization job status</span></span>
<span data-ttu-id="d3bf8-159">В приведенном ниже примере показано, как получить состояние задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-159">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="d3bf8-160">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="d3bf8-160">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="d3bf8-161">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="d3bf8-161">**Response**</span></span>
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

### <a name="get-synchronization-schema"></a><span data-ttu-id="d3bf8-162">Получение схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="d3bf8-162">Get synchronization schema</span></span>
<span data-ttu-id="d3bf8-163">В приведенном ниже примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3bf8-163">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="d3bf8-164">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="d3bf8-164">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="d3bf8-165">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="d3bf8-165">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="d3bf8-166">См. также</span><span class="sxs-lookup"><span data-stu-id="d3bf8-166">See also</span></span>

* [<span data-ttu-id="d3bf8-167">Настройка синхронизации с атрибутами расширения каталога</span><span class="sxs-lookup"><span data-stu-id="d3bf8-167">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="d3bf8-168">Настройка синхронизации с пользовательскими целевыми атрибутами</span><span class="sxs-lookup"><span data-stu-id="d3bf8-168">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



