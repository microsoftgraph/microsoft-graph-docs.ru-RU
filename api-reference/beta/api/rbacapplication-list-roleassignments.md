---
title: Список Унифиедролеассигнментс
description: Получение списка объектов Унифиедролеассигнмент.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6586de66b1e56820427ca2d6e5c0cdf9d70cc0de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969307"
---
# <a name="list-unifiedroleassignments"></a><span data-ttu-id="f575f-103">Список Унифиедролеассигнментс</span><span class="sxs-lookup"><span data-stu-id="f575f-103">List unifiedRoleAssignments</span></span>

<span data-ttu-id="f575f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f575f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f575f-105">Получение списка объектов [унифиедролеассигнмент](../resources/unifiedroleassignment.md) для поставщика.</span><span class="sxs-lookup"><span data-stu-id="f575f-105">Get a list of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="f575f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f575f-106">Permissions</span></span>

<span data-ttu-id="f575f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f575f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f575f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f575f-109">Permission type</span></span>      | <span data-ttu-id="f575f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f575f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f575f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f575f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f575f-112">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="f575f-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f575f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f575f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f575f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f575f-114">Not supported.</span></span>    |
|<span data-ttu-id="f575f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f575f-115">Application</span></span> | <span data-ttu-id="f575f-116">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f575f-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f575f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f575f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f575f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f575f-118">Optional query parameters</span></span>

<span data-ttu-id="f575f-119">Для выполнения этой операции требуется `$filter` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="f575f-119">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="f575f-120">Вы можете отфильтровать `roleDefinitionId` по `principalId` свойствам или.</span><span class="sxs-lookup"><span data-stu-id="f575f-120">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="f575f-121">`roleDefinitionId`Свойство может быть идентификатором объекта Role или шаблоном роли.</span><span class="sxs-lookup"><span data-stu-id="f575f-121">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="f575f-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f575f-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f575f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f575f-123">Request headers</span></span>

| <span data-ttu-id="f575f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f575f-124">Name</span></span>      |<span data-ttu-id="f575f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f575f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f575f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f575f-126">Authorization</span></span> | <span data-ttu-id="f575f-127">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f575f-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f575f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f575f-128">Request body</span></span>

<span data-ttu-id="f575f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f575f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f575f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f575f-130">Response</span></span>

<span data-ttu-id="f575f-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f575f-131">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f575f-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="f575f-132">Examples</span></span>

### <a name="example-1-request-using-a-filter-on-role-definition-id"></a><span data-ttu-id="f575f-133">Пример 1: запрос с использованием фильтра по ИДЕНТИФИКАТОРу определения роли</span><span class="sxs-lookup"><span data-stu-id="f575f-133">Example 1: Request using a filter on role definition ID</span></span>

#### <a name="request"></a><span data-ttu-id="f575f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f575f-134">Request</span></span>

<span data-ttu-id="f575f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f575f-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f575f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f575f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'&$expand=principal
```
# <a name="c"></a>[<span data-ttu-id="f575f-137">C#</span><span class="sxs-lookup"><span data-stu-id="f575f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f575f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f575f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f575f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f575f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f575f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f575f-140">Response</span></span>

<span data-ttu-id="f575f-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f575f-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments(principal())",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEMmO4KwRqtpKkUWt3wOYIz4-1",
            "principalId": "ace08ec9-aa11-4ada-9145-addf0398233e",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "ace08ec9-aa11-4ada-9145-addf0398233e",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": "Redmond",
                "createdDateTime": "2019-02-22T20:29:07Z",
                "creationType": null,
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": "US",
                "department": "Office of the CEO",
                "displayName": "Joey Cruz",
                "employeeId": null,
                "faxNumber": null,
                "givenName": "Joey",
                "imAddresses": [
                    "joeyc@woodgrove.ms"
                ],
                "infoCatalogs": [],
                "isResourceAccount": null,
                "jobTitle": "Chief Security Officer",
                "legalAgeGroupClassification": null,
                "mail": "joeyc@woodgrove.ms",
                "mailNickname": "joeyc",
                "mobilePhone": null,
                "onPremisesDistinguishedName": null,
                "officeLocation": null,
                "userType": "Member",   

            }
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEC6Xh29-LklLmYDrOIi9z-E-1",
            "principalId": "6f87972e-2e7e-4b49-9980-eb3888bdcfe1",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "6f87972e-2e7e-4b49-9980-eb3888bdcfe1",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": null,
                "createdDateTime": "2019-07-18T01:38:36Z",
                "creationType": "Invitation",
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": null,
                "department": null,
                "displayName": "Kalyan Krishna",
                "employeeId": null,
                "faxNumber": null,
                "givenName": null,
                "imAddresses": [],
                "userType": "Guest",
    
            }
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEMgc_BA2rIZBuZsM-BSqLdU-1",
            "principalId": "10fc1cc8-ac36-4186-b99b-0cf814aa2dd5",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "10fc1cc8-ac36-4186-b99b-0cf814aa2dd5",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": null,
                "createdDateTime": "2019-11-13T21:54:27Z",
                "creationType": "Invitation",
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": null,
                "department": null,
                "displayName": "Markie Downing",
                "employeeId": null,
                "faxNumber": null,
                "givenName": null,
                "imAddresses": [],
                "userType": "Guest",
        
            }
        }
    ]
}
```

### <a name="example-2-request-using-a-filter-on-principal-id"></a><span data-ttu-id="f575f-142">Пример 2: запрос с использованием фильтра по ИДЕНТИФИКАТОРу субъекта</span><span class="sxs-lookup"><span data-stu-id="f575f-142">Example 2: Request using a filter on principal ID</span></span>

#### <a name="request"></a><span data-ttu-id="f575f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="f575f-143">Request</span></span>

<span data-ttu-id="f575f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f575f-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f575f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f575f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter = principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'
```
# <a name="c"></a>[<span data-ttu-id="f575f-146">C#</span><span class="sxs-lookup"><span data-stu-id="f575f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f575f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f575f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f575f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f575f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f575f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f575f-149">Response</span></span>

<span data-ttu-id="f575f-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f575f-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEHJ1hPGqSKpHlqMuxhkE9B8-1",
            "principalId": "f1847572-48aa-47aa-96a3-2ec61904f41f",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "LJnv8vs6uUa3z6Em7nTEUXJ1hPGqSKpHlqMuxhkE9B8-1",
            "principalId": "f1847572-48aa-47aa-96a3-2ec61904f41f",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


