---
title: Список Провисионингобжектсуммари
description: Получение всех событий подготовки, произошедших в клиенте.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 51375b2f83eeeb5755e3685a159a2338c34fa3fd
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123110"
---
# <a name="list-provisioningobjectsummary"></a><span data-ttu-id="dc0d2-103">Список Провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="dc0d2-103">List provisioningObjectSummary</span></span>

<span data-ttu-id="dc0d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc0d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc0d2-105">Получение всех событий подготовки, произошедших в клиенте, таких как удаление группы в целевом приложении или создание пользователя при подготовке учетных записей пользователей из системы отдела кадров.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-105">Get all provisioning events that occurred in your tenant, such as the deletion of a group in a target application or the creation of a user when provisioning user accounts from your HR system.</span></span> 

## <a name="permissions"></a><span data-ttu-id="dc0d2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc0d2-106">Permissions</span></span>

<span data-ttu-id="dc0d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc0d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc0d2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc0d2-109">Permission type</span></span> | <span data-ttu-id="dc0d2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc0d2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc0d2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc0d2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc0d2-112">Аудитлог. Read. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="dc0d2-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="dc0d2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc0d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc0d2-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc0d2-114">Not supported</span></span>   |
|<span data-ttu-id="dc0d2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc0d2-115">Application</span></span> | <span data-ttu-id="dc0d2-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc0d2-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc0d2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc0d2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/provisioning
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc0d2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dc0d2-118">Optional query parameters</span></span>

<span data-ttu-id="dc0d2-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="dc0d2-120">Обратите внимание, что все фильтры, кроме состояния, зависят от регистра.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-120">Note that the filters are all case sensitive except for status.</span></span> 

|<span data-ttu-id="dc0d2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dc0d2-121">Name</span></span>     |<span data-ttu-id="dc0d2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dc0d2-122">Description</span></span>                            |<span data-ttu-id="dc0d2-123">Пример</span><span class="sxs-lookup"><span data-stu-id="dc0d2-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="dc0d2-124">$filter</span><span class="sxs-lookup"><span data-stu-id="dc0d2-124">$filter</span></span>](/graph/query-parameters#filter-parameter)|<span data-ttu-id="dc0d2-125">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="dc0d2-125">Filters results (rows).</span></span> |/`auditLogs/provisioning?$filter=id eq '74c3b0ae-9cc5-850e-e0a5-7r6a4231de87'`
|[<span data-ttu-id="dc0d2-126">$top</span><span class="sxs-lookup"><span data-stu-id="dc0d2-126">$top</span></span>](/graph/query-parameters#top-parameter)|<span data-ttu-id="dc0d2-127">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-127">Sets the page size of results.</span></span>|`/auditLogs/provisioning?$top=20`|
|[<span data-ttu-id="dc0d2-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="dc0d2-128">$skiptoken</span></span>](/graph/query-parameters#skiptoken-parameter)|<span data-ttu-id="dc0d2-129">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-129">Retrieves the next page of results from result sets that span multiple pages.</span></span> <span data-ttu-id="dc0d2-130">Для создания маркера необходимо передать верхний фильтр в запросе.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-130">You must pass the top filter in the query to generate the token.</span></span> <span data-ttu-id="dc0d2-131">Невозможно указать число результатов, которые необходимо пропустить.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-131">You cannot specify the number of results to be skipped.</span></span>|`/auditLogs/provisioning?$top=20&$skiptoken=g822a72df43b19c8ce94b71d153981b680a08800bc3e35f239dffb378ff72c25"`|

<span data-ttu-id="dc0d2-132">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="dc0d2-132">For general information, see [OData query parameters](/graph/query_parameters).</span></span>

### <a name="attributes-supported-by-the-filter-parameter"></a><span data-ttu-id="dc0d2-133">Атрибуты, поддерживаемые параметром $filter</span><span class="sxs-lookup"><span data-stu-id="dc0d2-133">Attributes supported by the $filter parameter</span></span>

|<span data-ttu-id="dc0d2-134">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="dc0d2-134">Attribute name</span></span> |<span data-ttu-id="dc0d2-135">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="dc0d2-135">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="dc0d2-136">id</span><span class="sxs-lookup"><span data-stu-id="dc0d2-136">id</span></span>| <span data-ttu-id="dc0d2-137">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-137">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-138">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="dc0d2-138">activityDateTime</span></span>| <span data-ttu-id="dc0d2-139">eq</span><span class="sxs-lookup"><span data-stu-id="dc0d2-139">eq</span></span>|
|<span data-ttu-id="dc0d2-140">tenantid</span><span class="sxs-lookup"><span data-stu-id="dc0d2-140">tenantid</span></span>|<span data-ttu-id="dc0d2-141">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-141">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-142">JOBID</span><span class="sxs-lookup"><span data-stu-id="dc0d2-142">jobid</span></span>|<span data-ttu-id="dc0d2-143">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-143">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-144">чанжеид</span><span class="sxs-lookup"><span data-stu-id="dc0d2-144">changeid</span></span>|<span data-ttu-id="dc0d2-145">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-145">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-146">циклеид</span><span class="sxs-lookup"><span data-stu-id="dc0d2-146">cycleid</span></span>|<span data-ttu-id="dc0d2-147">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-147">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-148">action</span><span class="sxs-lookup"><span data-stu-id="dc0d2-148">action</span></span>|<span data-ttu-id="dc0d2-149">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-149">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-150">Статусинфо/Status</span><span class="sxs-lookup"><span data-stu-id="dc0d2-150">statusInfo/status</span></span>|<span data-ttu-id="dc0d2-151">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-151">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-152">Саурцесистем/displayName</span><span class="sxs-lookup"><span data-stu-id="dc0d2-152">sourceSystem/displayName</span></span>|<span data-ttu-id="dc0d2-153">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-153">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-154">Таржетсистем/displayName</span><span class="sxs-lookup"><span data-stu-id="dc0d2-154">targetSystem/displayName</span></span>|<span data-ttu-id="dc0d2-155">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-155">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-156">Саурцеидентити/Идентититипе</span><span class="sxs-lookup"><span data-stu-id="dc0d2-156">sourceIdentity/identityType</span></span>|<span data-ttu-id="dc0d2-157">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-157">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-158">Таржетидентити/Идентититипе</span><span class="sxs-lookup"><span data-stu-id="dc0d2-158">targetIdentity/identityType</span></span>|<span data-ttu-id="dc0d2-159">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-159">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-160">Саурцеидентити/ID</span><span class="sxs-lookup"><span data-stu-id="dc0d2-160">sourceIdentity/id</span></span>|<span data-ttu-id="dc0d2-161">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-161">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-162">servicePrincipal/ID</span><span class="sxs-lookup"><span data-stu-id="dc0d2-162">servicePrincipal/id</span></span>|<span data-ttu-id="dc0d2-163">eq</span><span class="sxs-lookup"><span data-stu-id="dc0d2-163">eq</span></span>|
|<span data-ttu-id="dc0d2-164">servicePrincipal/Name</span><span class="sxs-lookup"><span data-stu-id="dc0d2-164">servicePrincipal/name</span></span>|<span data-ttu-id="dc0d2-165">eq</span><span class="sxs-lookup"><span data-stu-id="dc0d2-165">eq</span></span>|
|<span data-ttu-id="dc0d2-166">Таржетидентити/ID</span><span class="sxs-lookup"><span data-stu-id="dc0d2-166">targetIdentity/id</span></span>|<span data-ttu-id="dc0d2-167">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-167">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-168">Саурцеидентити/displayName</span><span class="sxs-lookup"><span data-stu-id="dc0d2-168">sourceIdentity/displayName</span></span>|<span data-ttu-id="dc0d2-169">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-169">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-170">Таржетидентити/displayName</span><span class="sxs-lookup"><span data-stu-id="dc0d2-170">targetIdentity/displayName</span></span>|<span data-ttu-id="dc0d2-171">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-171">eq, contains</span></span>|
|<span data-ttu-id="dc0d2-172">Инитиатедби/displayName</span><span class="sxs-lookup"><span data-stu-id="dc0d2-172">initiatedBy/displayName</span></span>|<span data-ttu-id="dc0d2-173">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="dc0d2-173">eq, contains</span></span>|

## <a name="request-headers"></a><span data-ttu-id="dc0d2-174">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc0d2-174">Request headers</span></span>

| <span data-ttu-id="dc0d2-175">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc0d2-175">Header</span></span>        | <span data-ttu-id="dc0d2-176">Значение</span><span class="sxs-lookup"><span data-stu-id="dc0d2-176">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="dc0d2-177">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc0d2-177">Authorization</span></span> | <span data-ttu-id="dc0d2-178">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="dc0d2-178">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc0d2-179">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc0d2-179">Request body</span></span>

<span data-ttu-id="dc0d2-180">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-180">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc0d2-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc0d2-181">Response</span></span>

<span data-ttu-id="dc0d2-182">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [провисионингобжектсуммари](../resources/provisioningobjectsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-182">If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc0d2-183">Примеры</span><span class="sxs-lookup"><span data-stu-id="dc0d2-183">Examples</span></span>

### <a name="example-1-successful-request"></a><span data-ttu-id="dc0d2-184">Пример 1: успешный запрос</span><span class="sxs-lookup"><span data-stu-id="dc0d2-184">Example 1: Successful request</span></span>

### <a name="request"></a><span data-ttu-id="dc0d2-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc0d2-185">Request</span></span>

<span data-ttu-id="dc0d2-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-186">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc0d2-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc0d2-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
# <a name="c"></a>[<span data-ttu-id="dc0d2-188">C#</span><span class="sxs-lookup"><span data-stu-id="dc0d2-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc0d2-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc0d2-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc0d2-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc0d2-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dc0d2-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc0d2-191">Response</span></span>

<span data-ttu-id="dc0d2-192">Ниже приведен пример ответа на успешное выполнение события.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-192">The following is an example of the response for a successful event.</span></span>

><span data-ttu-id="dc0d2-193">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dc0d2-194">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-194">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "name": "list_provisioningobjectsummary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/provisioning",
    "value": [
         {
            "id": "75b5b0ae-9fc5-8d0e-e0a9-7y6a4728de56",
            "activityDateTime": "2019-05-04T03:00:54Z",
            "tenantId": "74beb175-3b80-7b63-b9d5-6f0b76082b16",
            "jobId": "aws.74beb1753b704b63b8d56f0b76082b16.10a7a801-7101-4c69-ae00-ce9f75f8460a",
            "cycleId": "b6502552-018d-79bd-8869-j47194dc65c1",
            "changeId": "b6502552-018d-89bd-9969-b49194dc65c1",
            "action": "EntryExportUpdate",
            "durationInMilliseconds": 3236,
            "statusInfo": {
                "status": "success"
            },
            "provisioningSteps": [
                {
                    "name": "EntryImport",
                    "provisioningStepType": "Import",
                    "status": "success",
                    "description": "Retrieved RolesCompound '10a7a801-7101-4c69-ae00-ce9f75f8460a' from Contoso",
                    "details": {}
                },
                {
                    "name": "EntryExportUpdate",
                    "provisioningStepType": "Export",
                    "status": "success",
                    "description": "RolesCompound '60a7a801-7101-4c69-ae00-ce9f75f8460a' was updated in Azure Active Directory",
                    "details": {
                        "ReportableIdentifier": "60a7a801-7101-4c69-ae00-ce9f75f8460a"
                    }
                }
            ],
            "modifiedProperties": [
                {
                    "displayName": "appId",
                    "oldValue": null,
                    "newValue": "60a7a801-7101-4c69-ae00-ce9f75f8460a"
                },
                {
                    "displayName": "Roles",
                    "oldValue": null,
                    "newValue": "jaws-prod-role2,jaws-prod-saml2, jayaws-role,jayaws-saml, TestRole,super-saml"
                },
                {
                    "displayName": "objectId",
                    "oldValue": null,
                    "newValue": "6nn37b93-185a-4485-a519-50c09549f3ad"
                },
                {
                    "displayName": "displayName",
                    "oldValue": null,
                    "newValue": "Contoso"
                },
                {
                    "displayName": "homepage",
                    "oldValue": null,
                    "newValue": "https://signin.contoso.com/saml?metadata=contoso|ISV9.1|primary|z"
                },
            ],
            "servicePrincipal": {
                "id": "6cc35b93-185a-4485-a519-50c09549g3ad",
                "displayName": "Contoso"
            },
            "sourceSystem": {
                "id": "d1e090e1-f2f4-4678-be44-6442ffff0621",
                "displayName": "Contoso",
                "details": {}
            },
            "targetSystem": {
                "id": "e69d4bd2-2da2-483e-bc49-aad4080b91b3",
                "displayName": "Azure Active Directory",
                "details": {
                    "ApplicationId": "bcf4d658-ac9f-408d-bf04-e86dc10328fb",
                    "ServicePrincipalId": "6nn35b93-185a-4485-a519-50c09549f3ad",
                    "ServicePrincipalDisplayName": "Contoso"
                }
            },
            "initiatedBy": {
                "initiatingType": "System",
                "id": "",
                "displayName": "Azure AD Provisioning Service"
            },
            "sourceIdentity": {
                "identityType": "RolesCompound",
                "id": "60a7a801-7101-4c69-ae00-ce9f75f8460a",
                "displayName": "",
                "details": {}
            },
            "targetIdentity": {
                "identityType": "ServicePrincipal",
                "id": "6nn35b93-185a-4485-a519-50c09549f3ad",
                "displayName": "",
                "details": {}
            }
          }
    ]
}

```
### <a name="example-2-error-reponse"></a><span data-ttu-id="dc0d2-195">Пример 2: ответ на сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="dc0d2-195">Example 2: Error reponse</span></span>

### <a name="request"></a><span data-ttu-id="dc0d2-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc0d2-196">Request</span></span>

<span data-ttu-id="dc0d2-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-197">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc0d2-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc0d2-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary_error"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
# <a name="c"></a>[<span data-ttu-id="dc0d2-199">C#</span><span class="sxs-lookup"><span data-stu-id="dc0d2-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc0d2-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc0d2-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc0d2-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc0d2-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dc0d2-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc0d2-202">Response</span></span>

<span data-ttu-id="dc0d2-203">Ниже приведен пример ответа на сообщение о неудачной подготовке.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-203">The following is an example of the response for a failed provisioning event.</span></span>

><span data-ttu-id="dc0d2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "jobId": "ContosoOutDelta.7928d5b574424a97ne2d66f9j9972ecn",
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
                "displayName": "Contoso",
                "details": {
                    "ApplicationId": "f2764360-e0ec-5676-711e-cd6fc0d4dd61",
                    "ServicePrincipalId": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                    "ServicePrincipalDisplayName": "Contoso"
                }
            },
            "initiatedBy": {
                "id": "",
                "displayName": "Azure AD Provisioning Service",
                "initiatorType": "system"
            },
            "servicePrincipal": {
                "id": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                "displayName": "Contoso"
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
                "errorCode": "ContosoEntryConflict",
                "reason": "Message: Contoso returned an error response with the HTTP status code 409.  This response indicates that a user or a group already exisits with the same name. This can be avoided by identifying and removing the conflicting user from Contoso via the Contoso administrative user interface, or removing the current user from the scope of provisioning either by removing their assignment to the Contoso application in Azure Active Directory or adding a scoping filter to exclude the user.",
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
                    "description": "Group 'Self-service Pilot' will be created in Contoso (Group is active and assigned in Azure Active Directory, but no matching Group was found in Contoso)",
                    "details": {}
                },
                {
                    "name": "EntryExportAdd",
                    "provisioningStepType": "export",
                    "status": "failure",
                    "description": "Failed to create Group 'Self-service Pilot' in Contoso",
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
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get provisioningObjectSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
