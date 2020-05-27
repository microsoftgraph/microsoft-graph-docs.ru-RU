---
title: Предоставление пользователю Аппролеассигнмент
description: Предоставьте пользователю назначение роли приложения.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: c60e1f584f8d4caacb4f0bd643494fed578f21a8
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383835"
---
# <a name="grant-an-approleassignment-to-a-user"></a><span data-ttu-id="c4cdf-103">Предоставление пользователю Аппролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="c4cdf-103">Grant an appRoleAssignment to a user</span></span>

<span data-ttu-id="c4cdf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4cdf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4cdf-105">Используйте этот API, чтобы назначить роль приложения пользователю.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-105">Use this API to assign an app role to a user.</span></span> <span data-ttu-id="c4cdf-106">Чтобы предоставить пользователю назначение роли приложения, вам потребуется три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="c4cdf-106">To grant an app role assignment to a user, you need three identifiers:</span></span>

- <span data-ttu-id="c4cdf-107">`principalId`— `id` Пользователь, которому назначается роль приложения.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-107">`principalId`: The `id` of the user to whom you are assigning the app role.</span></span>
- <span data-ttu-id="c4cdf-108">`resourceId`: `id` Ресурс, в котором `servicePrincipal` определена роль приложения.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-108">`resourceId`: The `id` of the resource `servicePrincipal` that has defined the app role.</span></span>
- <span data-ttu-id="c4cdf-109">`appRoleId`: Значение `id` `appRole` (определяется для субъекта-службы ресурсов), которое необходимо назначить пользователю.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-109">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4cdf-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4cdf-110">Permissions</span></span>

<span data-ttu-id="c4cdf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4cdf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4cdf-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4cdf-113">Permission type</span></span>      | <span data-ttu-id="c4cdf-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4cdf-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4cdf-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4cdf-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c4cdf-116">Аппролеассигнмент. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c4cdf-116">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4cdf-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4cdf-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4cdf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-118">Not supported.</span></span>    |
|<span data-ttu-id="c4cdf-119">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="c4cdf-119">Application</span></span> | <span data-ttu-id="c4cdf-120">Аппролеассигнмент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c4cdf-120">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4cdf-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4cdf-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="c4cdf-122">Рекомендуется создавать назначения ролей приложений с помощью `appRoleAssignedTo` отношения между субъектом службы _ресурсов_ , а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-122">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4cdf-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4cdf-123">Request headers</span></span>

| <span data-ttu-id="c4cdf-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c4cdf-124">Name</span></span>       | <span data-ttu-id="c4cdf-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c4cdf-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c4cdf-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4cdf-126">Authorization</span></span> | <span data-ttu-id="c4cdf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c4cdf-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4cdf-129">Content-Type</span></span> | <span data-ttu-id="c4cdf-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4cdf-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4cdf-132">Request body</span></span>

<span data-ttu-id="c4cdf-133">В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-133">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c4cdf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4cdf-134">Response</span></span>

<span data-ttu-id="c4cdf-135">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-135">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4cdf-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4cdf-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4cdf-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4cdf-137">Request</span></span>

<span data-ttu-id="c4cdf-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-138">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c4cdf-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4cdf-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c4cdf-140">C#</span><span class="sxs-lookup"><span data-stu-id="c4cdf-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4cdf-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4cdf-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4cdf-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4cdf-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c4cdf-143">В этом примере `{id}` и то, и `{principalId-value}` другое — это `id` назначенный пользователь.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-143">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned user.</span></span>

### <a name="response"></a><span data-ttu-id="c4cdf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4cdf-144">Response</span></span>

<span data-ttu-id="c4cdf-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-145">Here is an example of the response.</span></span> 

> <span data-ttu-id="c4cdf-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4cdf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "id": "id-value",
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalType": "principalType-value",
  "principalId": "principalId-value",
  "principalDisplayName": "principalDisplayName-value",
  "resourceId": "resourceId-value",
  "resourceDisplayName": "resourceDisplayName-value"
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
