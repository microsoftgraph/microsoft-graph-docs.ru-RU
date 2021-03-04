---
title: Предоставление appRoleAssignment пользователю
description: Предоставление назначения роли приложения пользователю.
localization_priority: Priority
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: 6c3ff85213332b5cc6a1585834d0b2a52c0c6fce
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444758"
---
# <a name="grant-an-approleassignment-to-a-user"></a><span data-ttu-id="ae74d-103">Предоставление appRoleAssignment пользователю</span><span class="sxs-lookup"><span data-stu-id="ae74d-103">Grant an appRoleAssignment to a user</span></span>

<span data-ttu-id="ae74d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae74d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae74d-105">Используйте этот API, чтобы назначить роль приложения пользователю.</span><span class="sxs-lookup"><span data-stu-id="ae74d-105">Use this API to assign an app role to a user.</span></span> <span data-ttu-id="ae74d-106">Чтобы предоставить назначение роли приложения пользователю, нужны три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="ae74d-106">To grant an app role assignment to a user, you need three identifiers:</span></span>

- <span data-ttu-id="ae74d-107">`principalId`: `id` пользователя, которому нужно назначить роль приложения.</span><span class="sxs-lookup"><span data-stu-id="ae74d-107">`principalId`: The `id` of the user to whom you are assigning the app role.</span></span>
- <span data-ttu-id="ae74d-108">`resourceId`: `id` ресурса `servicePrincipal`, который определяет роль приложения.</span><span class="sxs-lookup"><span data-stu-id="ae74d-108">`resourceId`: The `id` of the resource `servicePrincipal` that has defined the app role.</span></span>
- <span data-ttu-id="ae74d-109">`appRoleId`: `id` объекта `appRole` (определенного в субъекте-службе ресурса) для назначения пользователю.</span><span class="sxs-lookup"><span data-stu-id="ae74d-109">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae74d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae74d-110">Permissions</span></span>

<span data-ttu-id="ae74d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae74d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae74d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae74d-113">Permission type</span></span>      | <span data-ttu-id="ae74d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae74d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae74d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae74d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ae74d-116">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae74d-116">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae74d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae74d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae74d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae74d-118">Not supported.</span></span>    |
|<span data-ttu-id="ae74d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae74d-119">Application</span></span> | <span data-ttu-id="ae74d-120">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae74d-120">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae74d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae74d-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="ae74d-122">Рекомендуется создавать назначения ролей приложения, используя отношение `appRoleAssignedTo` _ресурса_ субъекта-службы вместо отношения `appRoleAssignments` назначенного пользователя, группы или субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ae74d-122">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae74d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae74d-123">Request headers</span></span>

| <span data-ttu-id="ae74d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ae74d-124">Name</span></span>       | <span data-ttu-id="ae74d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ae74d-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="ae74d-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae74d-126">Authorization</span></span> | <span data-ttu-id="ae74d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae74d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ae74d-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae74d-129">Content-Type</span></span> | <span data-ttu-id="ae74d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae74d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae74d-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae74d-132">Request body</span></span>

<span data-ttu-id="ae74d-133">В тексте запроса укажите представление JSON для объекта [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ae74d-133">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ae74d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae74d-134">Response</span></span>

<span data-ttu-id="ae74d-135">В случае успеха этот метод возвращает в тексте отклика код отклика `201 Created` и объект [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ae74d-135">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae74d-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae74d-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ae74d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae74d-137">Request</span></span>

<span data-ttu-id="ae74d-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae74d-138">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae74d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae74d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/users/cde330e5-2150-4c11-9c5b-14bfdc948c79/appRoleAssignments
Content-Type: application/json

{
  "principalId": "cde330e5-2150-4c11-9c5b-14bfdc948c79",
  "resourceId": "8e881353-1735-45af-af21-ee1344582a4d",
  "appRoleId": "00000000-0000-0000-0000-000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="ae74d-140">C#</span><span class="sxs-lookup"><span data-stu-id="ae74d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae74d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae74d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae74d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae74d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae74d-143">Java</span><span class="sxs-lookup"><span data-stu-id="ae74d-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ae74d-144">В этом примере `{id}` и `{principalId-value}` станут `id` назначенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae74d-144">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned user.</span></span>

### <a name="response"></a><span data-ttu-id="ae74d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae74d-145">Response</span></span>

<span data-ttu-id="ae74d-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae74d-146">Here is an example of the response.</span></span> 

> <span data-ttu-id="ae74d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae74d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('cde330e5-2150-4c11-9c5b-14bfdc948c79')/appRoleAssignments/$entity",
  "id": "5TDjzVAhEUycWxS_3JSMeY-oHkjrWvBKi7aIZwYGQzg",
  "deletedDateTime": null,
  "appRoleId": "00000000-0000-0000-0000-000000000000",
  "createdDateTime": "2021-02-15T10:31:53.5164841Z",
  "principalDisplayName": "Megan Bowen",
  "principalId": "cde330e5-2150-4c11-9c5b-14bfdc948c79",
  "principalType": "User",
  "resourceDisplayName": "dxprovisioning-graphapi-client",
  "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


