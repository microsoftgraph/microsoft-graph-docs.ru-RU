---
title: Список Провисионингобжектсуммари
description: Получение всех событий подготовки, произошедших в клиенте.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce9ccfe4c5181b51f8ed006be6e5b32dcf56fe34
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394463"
---
# <a name="list-provisioningobjectsummary"></a><span data-ttu-id="07edf-103">Список Провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="07edf-103">List provisioningObjectSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07edf-104">Получение всех событий подготовки, произошедших в клиенте, таких как удаление группы в целевом приложении или создание пользователя при подготовке учетных записей пользователей из системы отдела кадров.</span><span class="sxs-lookup"><span data-stu-id="07edf-104">Get all provisioning events that occurred in your tenant, such as the deletion of a group in a target application or the creation of a user when provisioning user accounts from your HR system.</span></span> 

## <a name="permissions"></a><span data-ttu-id="07edf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07edf-105">Permissions</span></span>

<span data-ttu-id="07edf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07edf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07edf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07edf-108">Permission type</span></span>      | <span data-ttu-id="07edf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07edf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07edf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07edf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07edf-111">Аудитлог. Read. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="07edf-111">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="07edf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07edf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07edf-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="07edf-113">Not supported</span></span>   |
|<span data-ttu-id="07edf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07edf-114">Application</span></span> | <span data-ttu-id="07edf-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="07edf-115">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07edf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07edf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/provisioning
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07edf-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="07edf-117">Optional query parameters</span></span>

<span data-ttu-id="07edf-118">Этот метод поддерживает следующий параметр запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="07edf-118">This method supports the following OData query parameter to help customize the response.</span></span> <span data-ttu-id="07edf-119">Обратите внимание, что все фильтры, кроме состояния, зависят от регистра.</span><span class="sxs-lookup"><span data-stu-id="07edf-119">Note that the filters are all case sensitive except for status.</span></span> 

|<span data-ttu-id="07edf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="07edf-120">Name</span></span>     |<span data-ttu-id="07edf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="07edf-121">Description</span></span>                            |<span data-ttu-id="07edf-122">Пример</span><span class="sxs-lookup"><span data-stu-id="07edf-122">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="07edf-123">$filter</span><span class="sxs-lookup"><span data-stu-id="07edf-123">$filter</span></span>](/graph/query-parameters#filter-parameter)|<span data-ttu-id="07edf-124">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="07edf-124">Filters results (rows).</span></span> |/`auditLogs/provisioning?$filter=id eq '74c3b0ae-9cc5-850e-e0a5-7r6a4231de87'`

<span data-ttu-id="07edf-125">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="07edf-125">For general information, see [OData query parameters](/graph/query_parameters).</span></span>

### <a name="attributes-supported-by-the-filter-parameter"></a><span data-ttu-id="07edf-126">Атрибуты, поддерживаемые параметром $filter</span><span class="sxs-lookup"><span data-stu-id="07edf-126">Attributes supported by the $filter parameter</span></span>

|<span data-ttu-id="07edf-127">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="07edf-127">Attribute name</span></span> |<span data-ttu-id="07edf-128">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="07edf-128">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="07edf-129">id</span><span class="sxs-lookup"><span data-stu-id="07edf-129">id</span></span>| <span data-ttu-id="07edf-130">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-130">eq, contains</span></span>|
|<span data-ttu-id="07edf-131">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="07edf-131">activityDateTime</span></span>| <span data-ttu-id="07edf-132">eq</span><span class="sxs-lookup"><span data-stu-id="07edf-132">eq</span></span>|
|<span data-ttu-id="07edf-133">tenantid</span><span class="sxs-lookup"><span data-stu-id="07edf-133">tenantid</span></span>|<span data-ttu-id="07edf-134">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-134">eq, contains</span></span>|
|<span data-ttu-id="07edf-135">JOBID</span><span class="sxs-lookup"><span data-stu-id="07edf-135">jobid</span></span>|<span data-ttu-id="07edf-136">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-136">eq, contains</span></span>|
|<span data-ttu-id="07edf-137">чанжеид</span><span class="sxs-lookup"><span data-stu-id="07edf-137">changeid</span></span>|<span data-ttu-id="07edf-138">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-138">eq, contains</span></span>|
|<span data-ttu-id="07edf-139">циклеид</span><span class="sxs-lookup"><span data-stu-id="07edf-139">cycleid</span></span>|<span data-ttu-id="07edf-140">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-140">eq, contains</span></span>|
|<span data-ttu-id="07edf-141">action</span><span class="sxs-lookup"><span data-stu-id="07edf-141">action</span></span>|<span data-ttu-id="07edf-142">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-142">eq, contains</span></span>|
|<span data-ttu-id="07edf-143">Статусинфо/Status</span><span class="sxs-lookup"><span data-stu-id="07edf-143">statusInfo/status</span></span>|<span data-ttu-id="07edf-144">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-144">eq, contains</span></span>|
|<span data-ttu-id="07edf-145">Саурцесистем/displayName</span><span class="sxs-lookup"><span data-stu-id="07edf-145">sourceSystem/displayName</span></span>|<span data-ttu-id="07edf-146">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-146">eq, contains</span></span>|
|<span data-ttu-id="07edf-147">Таржетсистем/displayName</span><span class="sxs-lookup"><span data-stu-id="07edf-147">targetSystem/displayName</span></span>|<span data-ttu-id="07edf-148">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-148">eq, contains</span></span>|
|<span data-ttu-id="07edf-149">Саурцеидентити/Идентититипе</span><span class="sxs-lookup"><span data-stu-id="07edf-149">sourceIdentity/identityType</span></span>|<span data-ttu-id="07edf-150">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-150">eq, contains</span></span>|
|<span data-ttu-id="07edf-151">Таржетидентити/Идентититипе</span><span class="sxs-lookup"><span data-stu-id="07edf-151">targetIdentity/identityType</span></span>|<span data-ttu-id="07edf-152">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-152">eq, contains</span></span>|
|<span data-ttu-id="07edf-153">Саурцеидентити/ID</span><span class="sxs-lookup"><span data-stu-id="07edf-153">sourceIdentity/id</span></span>|<span data-ttu-id="07edf-154">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-154">eq, contains</span></span>|
|<span data-ttu-id="07edf-155">servicePrincipal/ID</span><span class="sxs-lookup"><span data-stu-id="07edf-155">servicePrincipal/id</span></span>|<span data-ttu-id="07edf-156">eq</span><span class="sxs-lookup"><span data-stu-id="07edf-156">eq</span></span>|
|<span data-ttu-id="07edf-157">servicePrincipal/Name</span><span class="sxs-lookup"><span data-stu-id="07edf-157">servicePrincipal/name</span></span>|<span data-ttu-id="07edf-158">eq</span><span class="sxs-lookup"><span data-stu-id="07edf-158">eq</span></span>|
|<span data-ttu-id="07edf-159">Таржетидентити/ID</span><span class="sxs-lookup"><span data-stu-id="07edf-159">targetIdentity/id</span></span>|<span data-ttu-id="07edf-160">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-160">eq, contains</span></span>|
|<span data-ttu-id="07edf-161">Саурцеидентити/displayName</span><span class="sxs-lookup"><span data-stu-id="07edf-161">sourceIdentity/displayName</span></span>|<span data-ttu-id="07edf-162">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-162">eq, contains</span></span>|
|<span data-ttu-id="07edf-163">Таржетидентити/displayName</span><span class="sxs-lookup"><span data-stu-id="07edf-163">targetIdentity/displayName</span></span>|<span data-ttu-id="07edf-164">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-164">eq, contains</span></span>|
|<span data-ttu-id="07edf-165">Инитиатедби/displayName</span><span class="sxs-lookup"><span data-stu-id="07edf-165">initiatedBy/displayName</span></span>|<span data-ttu-id="07edf-166">EQ содержит</span><span class="sxs-lookup"><span data-stu-id="07edf-166">eq, contains</span></span>|

## <a name="request-headers"></a><span data-ttu-id="07edf-167">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07edf-167">Request headers</span></span>

| <span data-ttu-id="07edf-168">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07edf-168">Header</span></span>        | <span data-ttu-id="07edf-169">Значение</span><span class="sxs-lookup"><span data-stu-id="07edf-169">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="07edf-170">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07edf-170">Authorization</span></span> | <span data-ttu-id="07edf-171">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="07edf-171">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07edf-172">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07edf-172">Request body</span></span>

<span data-ttu-id="07edf-173">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07edf-173">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07edf-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="07edf-174">Response</span></span>

<span data-ttu-id="07edf-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [провисионингобжектсуммари](../resources/provisioningobjectsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07edf-175">If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07edf-176">Примеры</span><span class="sxs-lookup"><span data-stu-id="07edf-176">Examples</span></span>

### <a name="example-1-successful-request"></a><span data-ttu-id="07edf-177">Пример 1: успешный запрос</span><span class="sxs-lookup"><span data-stu-id="07edf-177">Example 1: Successful request</span></span>

### <a name="request"></a><span data-ttu-id="07edf-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="07edf-178">Request</span></span>

<span data-ttu-id="07edf-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07edf-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07edf-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="07edf-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
# <a name="c"></a>[<span data-ttu-id="07edf-181">C#</span><span class="sxs-lookup"><span data-stu-id="07edf-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07edf-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07edf-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07edf-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07edf-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="07edf-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="07edf-184">Response</span></span>

<span data-ttu-id="07edf-185">Ниже приведен пример ответа на успешное выполнение события.</span><span class="sxs-lookup"><span data-stu-id="07edf-185">The following is an example of the response for a successful event.</span></span>

><span data-ttu-id="07edf-186">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="07edf-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="07edf-187">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07edf-187">All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-error-reponse"></a><span data-ttu-id="07edf-188">Пример 2: ответ на сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="07edf-188">Example 2: Error reponse</span></span>

### <a name="request"></a><span data-ttu-id="07edf-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="07edf-189">Request</span></span>

<span data-ttu-id="07edf-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07edf-190">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07edf-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="07edf-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary_error"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
# <a name="c"></a>[<span data-ttu-id="07edf-192">C#</span><span class="sxs-lookup"><span data-stu-id="07edf-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07edf-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07edf-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07edf-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07edf-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="07edf-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="07edf-195">Response</span></span>

<span data-ttu-id="07edf-196">Ниже приведен пример ответа на сообщение о неудачной подготовке.</span><span class="sxs-lookup"><span data-stu-id="07edf-196">The following is an example of the response for a failed provisioning event.</span></span>

><span data-ttu-id="07edf-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07edf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
