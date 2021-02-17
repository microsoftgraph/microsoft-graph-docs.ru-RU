---
title: Обзор API синхронизации Azure AD
description: Автоматизация предоставления удостоверений из систем управления персоналом, Active Directory и Azure Active Directory в облачные приложения.
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 2c0cbfae55ca02743d1b8e10777580e431529103
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272516"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="673b6-103">Обзор API синхронизации Azure AD</span><span class="sxs-lookup"><span data-stu-id="673b6-103">Azure AD synchronization API overview</span></span>

<span data-ttu-id="673b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="673b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="673b6-105">Синхронизация удостоверений Azure Active Directory (Azure AD) (также называемая "подготовка") позволяет автоматизировать подготовка (создание, обслуживание) и отмену (удаление) удостоверений из любого из следующих систем:</span><span class="sxs-lookup"><span data-stu-id="673b6-105">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the provisioning (creation, maintenance) and de-provisioning (removal) of identities from any of the following:</span></span>
- <span data-ttu-id="673b6-106">Из Active Directory в Azure AD</span><span class="sxs-lookup"><span data-stu-id="673b6-106">Active Directory to Azure AD</span></span>
- <span data-ttu-id="673b6-107">Рабочий день в Azure AD</span><span class="sxs-lookup"><span data-stu-id="673b6-107">Workday to Azure AD</span></span>
- <span data-ttu-id="673b6-108">Azure AD для облачных приложений, таких как Dropbox, Salesforce, ServiceNow и другие</span><span class="sxs-lookup"><span data-stu-id="673b6-108">Azure AD to cloud applications such as Dropbox, Salesforce, ServiceNow, and more</span></span> 

<span data-ttu-id="673b6-109">Можно воспользоваться интерфейсами API синхронизации в Microsoft Graph для управления синхронизацией удостоверений программными средствами, в том числе для:</span><span class="sxs-lookup"><span data-stu-id="673b6-109">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="673b6-110">создания, запуска и остановки заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="673b6-110">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="673b6-111">изменения схемы синхронизации для заданий</span><span class="sxs-lookup"><span data-stu-id="673b6-111">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="673b6-112">проверки текущего состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="673b6-112">Verify the current synchronization status</span></span>

<span data-ttu-id="673b6-113">Дополнительные сведения о синхронизации в Azure AD см. в:</span><span class="sxs-lookup"><span data-stu-id="673b6-113">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="673b6-114">Автоматизация пользовательской подготовка и подготовка к приложениям SaaS с помощью Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="673b6-114">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="673b6-115">Управление подготовкаю учетных записей пользователей для корпоративных приложений на портале Azure</span><span class="sxs-lookup"><span data-stu-id="673b6-115">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="673b6-116">Вы также можете попробовать API в обозревателе [Graph](https://developer.microsoft.com/graph/graph-explorer) в примере клиента или собственном клиенте.</span><span class="sxs-lookup"><span data-stu-id="673b6-116">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="673b6-117">Задание синхронизации</span><span class="sxs-lookup"><span data-stu-id="673b6-117">Synchronization job</span></span>

<span data-ttu-id="673b6-118">Задания синхронизации выполняют синхронизацию, периодически работая в фоновом режиме, выполняя опрос изменений в одном каталоге и перенажимая их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="673b6-118">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="673b6-119">Задание синхронизации всегда является специфическим для конкретного экземпляра приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="673b6-119">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="673b6-120">В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге и настроить схему синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="673b6-120">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="673b6-121">Дополнительные сведения см. [в заданиях синхронизации.](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="673b6-121">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="673b6-122">Схема синхронизации</span><span class="sxs-lookup"><span data-stu-id="673b6-122">Synchronization schema</span></span>

<span data-ttu-id="673b6-123">Схема синхронизации определяет, какие объекты будут синхронизироваться и как они будут синхронизироваться.</span><span class="sxs-lookup"><span data-stu-id="673b6-123">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="673b6-124">Схема синхронизации содержит большую часть сведений об установке для конкретного задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="673b6-124">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="673b6-125">Как правило, некоторые сопоставления [](synchronization-attributemapping.md)атрибутов настраиваются или [](synchronization-filter.md) добавляются фильтры области для синхронизации только объектов, удовлетворяющих определенному условию.</span><span class="sxs-lookup"><span data-stu-id="673b6-125">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="673b6-126">Схема синхронизации включает следующие компоненты:</span><span class="sxs-lookup"><span data-stu-id="673b6-126">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="673b6-127">Определения каталогов</span><span class="sxs-lookup"><span data-stu-id="673b6-127">Directory definitions</span></span>
- <span data-ttu-id="673b6-128">Правила синхронизации</span><span class="sxs-lookup"><span data-stu-id="673b6-128">Synchronization rules</span></span>
- <span data-ttu-id="673b6-129">Сопоставления объектов</span><span class="sxs-lookup"><span data-stu-id="673b6-129">Object mappings</span></span>

<span data-ttu-id="673b6-130">Дополнительные сведения см. [в схеме синхронизации.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="673b6-130">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="673b6-131">Шаблон синхронизации</span><span class="sxs-lookup"><span data-stu-id="673b6-131">Synchronization template</span></span>

<span data-ttu-id="673b6-132">Шаблон синхронизации предоставляет предварительно настроенные параметры синхронизации для конкретного приложения.</span><span class="sxs-lookup"><span data-stu-id="673b6-132">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="673b6-133">Эти параметры (что самое важное, схема синхронизации) [](synchronization-synchronizationjob.md) будут использоваться по умолчанию для любого задания синхронизации, основанного на шаблоне. [](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="673b6-133">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="673b6-134">Шаблоны заданы разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="673b6-134">Templates are specified by the application developer.</span></span>

<span data-ttu-id="673b6-135">Дополнительные сведения см. [в шаблоне синхронизации.](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="673b6-135">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="673b6-136">Работа с API синхронизации</span><span class="sxs-lookup"><span data-stu-id="673b6-136">Working with the synchronization API</span></span>

<span data-ttu-id="673b6-137">Работа с API синхронизации в основном включает доступ к ресурсам [synchronizationJob](synchronization-synchronizationjob.md) и [synchronizationSchema.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="673b6-137">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="673b6-138">Чтобы найти ресурс [synchronizationJob,](synchronization-synchronizationjob.md) необходимо знать ИД объекта-службы, к которой принадлежит задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="673b6-138">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="673b6-139">В следующих примерах покажем, как работать с **ресурсами synchronizationJob** и **synchronizationSchema.**</span><span class="sxs-lookup"><span data-stu-id="673b6-139">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="673b6-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="673b6-140">Authorization</span></span>

<span data-ttu-id="673b6-141">Для авторизации API синхронизации Azure AD использует OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="673b6-141">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="673b6-142">Прежде чем делать запросы к API, необходимо получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="673b6-142">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="673b6-143">Дополнительные сведения см. в сведениях о [том, как получить маркеры доступа для вызова Microsoft Graph.](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="673b6-143">For more information, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span> <span data-ttu-id="673b6-144">Для доступа к ресурсам синхронизации приложению необходимы разрешения Directory.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="673b6-144">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="673b6-145">Дополнительные сведения [см. в сведениях о разрешениях для каталогов.](/graph/permissions-reference#directory-permissions)</span><span class="sxs-lookup"><span data-stu-id="673b6-145">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="673b6-146">Поиск объекта-службы по отображаемой имени</span><span class="sxs-lookup"><span data-stu-id="673b6-146">Find the service principal object by display name</span></span>

<span data-ttu-id="673b6-147">В следующем примере показано, как найти объект-службу по отображаемой имени.</span><span class="sxs-lookup"><span data-stu-id="673b6-147">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="673b6-148">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="673b6-148">**Request**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="673b6-149">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="673b6-149">**Response**</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK

{
   "value":[
      {
         "id":"bc0dc311-87df-48ac-91b1-259bd2c3a31c",
         "appId":"f7808c5e-cb57-4e37-8094-406d302c0f8d",
         "displayName":"Salesforce"
      },
      {
         "id":"d813d7d7-0f41-4edc-b284-d0dfaf399d15",
         "appId":"219561ee-1480-4c67-9aa6-63d861fae3ef",
         "displayName":"salesforce 3"
      }
   ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="673b6-150">Поиск объекта-службы по ИД приложения</span><span class="sxs-lookup"><span data-stu-id="673b6-150">Find the service principal object by app ID</span></span>

<span data-ttu-id="673b6-151">В следующем примере показано, как найти объект-службу по ИД приложения.</span><span class="sxs-lookup"><span data-stu-id="673b6-151">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="673b6-152">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="673b6-152">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="673b6-153">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="673b6-153">**Response**</span></span>
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

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="673b6-154">Список существующих заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="673b6-154">List existing synchronization jobs</span></span>

<span data-ttu-id="673b6-155">В следующем примере показано, как перечислить существующие задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="673b6-155">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="673b6-156">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="673b6-156">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="673b6-157">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="673b6-157">**Response**</span></span>
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

### <a name="get-synchronization-job-status"></a><span data-ttu-id="673b6-158">Получить состояние задания синхронизации</span><span class="sxs-lookup"><span data-stu-id="673b6-158">Get synchronization job status</span></span>
<span data-ttu-id="673b6-159">В следующем примере показано, как получить состояние задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="673b6-159">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="673b6-160">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="673b6-160">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="673b6-161">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="673b6-161">**Response**</span></span>
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

### <a name="get-synchronization-schema"></a><span data-ttu-id="673b6-162">Получить схему синхронизации</span><span class="sxs-lookup"><span data-stu-id="673b6-162">Get synchronization schema</span></span>
<span data-ttu-id="673b6-163">В следующем примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="673b6-163">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="673b6-164">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="673b6-164">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="673b6-165">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="673b6-165">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK

{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="673b6-166">См. также</span><span class="sxs-lookup"><span data-stu-id="673b6-166">See also</span></span>

* [<span data-ttu-id="673b6-167">Настройка синхронизации с атрибутами расширения каталога</span><span class="sxs-lookup"><span data-stu-id="673b6-167">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="673b6-168">Настройка синхронизации с настраиваемых целевых атрибутов</span><span class="sxs-lookup"><span data-stu-id="673b6-168">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)
