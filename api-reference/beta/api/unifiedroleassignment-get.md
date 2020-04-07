---
title: Получение Унифиедролеассигнмент
description: Получение свойств и связей объекта Унифиедролеассигнмент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9e041e30eefdcf10792bf652176c9d35ba1687c5
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160242"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="341a4-103">Получение Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="341a4-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="341a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="341a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="341a4-105">Получение свойств и связей объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="341a4-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="341a4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="341a4-106">Permissions</span></span>

<span data-ttu-id="341a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="341a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="341a4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="341a4-109">Permission type</span></span>      | <span data-ttu-id="341a4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="341a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="341a4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="341a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="341a4-112">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="341a4-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="341a4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="341a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="341a4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="341a4-114">Not supported.</span></span>    |
|<span data-ttu-id="341a4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="341a4-115">Application</span></span> | <span data-ttu-id="341a4-116">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="341a4-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="341a4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="341a4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="341a4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="341a4-118">Optional query parameters</span></span>

<span data-ttu-id="341a4-119">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="341a4-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="341a4-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="341a4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="341a4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="341a4-121">Request headers</span></span>

| <span data-ttu-id="341a4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="341a4-122">Name</span></span>      |<span data-ttu-id="341a4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="341a4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="341a4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="341a4-124">Authorization</span></span> | <span data-ttu-id="341a4-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="341a4-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="341a4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="341a4-126">Request body</span></span>

<span data-ttu-id="341a4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="341a4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="341a4-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="341a4-128">Response</span></span>

<span data-ttu-id="341a4-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="341a4-129">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="341a4-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="341a4-130">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="341a4-131">Пример 1: получение сведений о назначении роли</span><span class="sxs-lookup"><span data-stu-id="341a4-131">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="341a4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="341a4-132">Request</span></span>

<span data-ttu-id="341a4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="341a4-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```

#### <a name="response"></a><span data-ttu-id="341a4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="341a4-134">Response</span></span>

<span data-ttu-id="341a4-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="341a4-135">The following is an example of the response.</span></span>

> <span data-ttu-id="341a4-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="341a4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0"
}
```

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="341a4-138">Пример 2: получение сведений о назначении роли с помощью`$expand`</span><span class="sxs-lookup"><span data-stu-id="341a4-138">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="341a4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="341a4-139">Request</span></span>

<span data-ttu-id="341a4-140">Ниже приведен пример запроса с параметром `$expand` Query.</span><span class="sxs-lookup"><span data-stu-id="341a4-140">The following is an example of the request with the `$expand` query parameter.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```

#### <a name="response"></a><span data-ttu-id="341a4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="341a4-141">Response</span></span>

<span data-ttu-id="341a4-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="341a4-142">The following is an example of the response.</span></span>
> <span data-ttu-id="341a4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="341a4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "roleDefinition": {
      "id": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
      "displayName": "Billing Administrator",
      "description": "Can perform common billing related tasks like updating payment information.",
      "rolePermissions": [
        {
          "allowedResourceActions": [
            "microsoft.commerce.billing/allEntities/allTasks",
            "microsoft.directory/organization/basic/update",
          ],
          "excludedResourceActions": []
        }],
      "isEnabled": true,
      },
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "principal": {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
      "id": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d ",
      "userPrincipalName": "alice@contoso.com",
      "displayName": "Alice Smith"
    },
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScope": {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization/$entity",
      "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Contoso_Seattle_Admins"
    }
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->