---
title: Список Унифиедроледефинитионс
description: Получение списка объектов Унифиедроледефинитион.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bde822dde2fa7b9a13a56fc3cc25faf46f387ce4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981112"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="def3c-103">Список Унифиедроледефинитионс</span><span class="sxs-lookup"><span data-stu-id="def3c-103">List unifiedRoleDefinitions</span></span>

<span data-ttu-id="def3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="def3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="def3c-105">Получение списка объектов [унифиедроледефинитион](../resources/unifiedroledefinition.md) для поставщика.</span><span class="sxs-lookup"><span data-stu-id="def3c-105">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="def3c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="def3c-106">Permissions</span></span>

<span data-ttu-id="def3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="def3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="def3c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="def3c-109">Permission type</span></span>      | <span data-ttu-id="def3c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="def3c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="def3c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="def3c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="def3c-112">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="def3c-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="def3c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="def3c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="def3c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="def3c-114">Not supported.</span></span>    |
|<span data-ttu-id="def3c-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="def3c-115">Application</span></span> | <span data-ttu-id="def3c-116">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="def3c-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="def3c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="def3c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="def3c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="def3c-118">Optional query parameters</span></span>
<span data-ttu-id="def3c-119">Этот метод поддерживает `$filter` `id` , `displayName` и `isBuiltIn` .</span><span class="sxs-lookup"><span data-stu-id="def3c-119">This method supports `$filter` on `id`, `displayName`, and `isBuiltIn`.</span></span> <span data-ttu-id="def3c-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="def3c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="def3c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="def3c-121">Request headers</span></span>

| <span data-ttu-id="def3c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="def3c-122">Name</span></span>      |<span data-ttu-id="def3c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="def3c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="def3c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="def3c-124">Authorization</span></span> | <span data-ttu-id="def3c-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="def3c-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="def3c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="def3c-126">Request body</span></span>

<span data-ttu-id="def3c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="def3c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="def3c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="def3c-128">Response</span></span>

<span data-ttu-id="def3c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="def3c-129">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="def3c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="def3c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="def3c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="def3c-131">Request</span></span>

<span data-ttu-id="def3c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="def3c-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="def3c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="def3c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="def3c-134">C#</span><span class="sxs-lookup"><span data-stu-id="def3c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="def3c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="def3c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="def3c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="def3c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="def3c-137">Java</span><span class="sxs-lookup"><span data-stu-id="def3c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="def3c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="def3c-138">Response</span></span>

<span data-ttu-id="def3c-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="def3c-139">The following is an example of the response.</span></span>

> <span data-ttu-id="def3c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="def3c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions",
    "value": [
        {
            "id": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "description": "Can reset passwords for non-administrators and Helpdesk Administrators.",
            "displayName": "Helpdesk Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/users/invalidateAllRefreshTokens",
                        "microsoft.directory/users/bitLockerRecoveryKeys/read",
                        "microsoft.directory/users/password/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('729827e3-9c14-49f7-bb1b-9608f156bbb8')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "f023fd81-a637-4b56-95fd-791ac0226033",
            "description": "Can read service health information and manage support tickets.",
            "displayName": "Service Support Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "f023fd81-a637-4b56-95fd-791ac0226033",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('f023fd81-a637-4b56-95fd-791ac0226033')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "description": "Can perform common billing related tasks like updating payment information.",
            "displayName": "Billing Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/organization/basic/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.commerce.billing/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('b0f54661-2d74-4c50-afa3-1ec803f12efe')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
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
  "description": "List roleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


