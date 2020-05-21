---
title: Предоставление Аппролеассигнмент участнику службы
description: Предоставьте участнику службы назначение роли приложения.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a7d25a23b1ad3281b7a22107ee16b20e9d39e60a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335124"
---
# <a name="grant-an-approleassignment-for-a-service-principal"></a><span data-ttu-id="bb94f-103">Предоставление Аппролеассигнмент для субъекта службы</span><span class="sxs-lookup"><span data-stu-id="bb94f-103">Grant an appRoleAssignment for a service principal</span></span>

<span data-ttu-id="bb94f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb94f-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="bb94f-105">Назначение роли приложения для субъекта службы ресурсов пользователю, группе или участнику клиентской службы.</span><span class="sxs-lookup"><span data-stu-id="bb94f-105">Assign an app role for a resource service principal, to a user, group, or client service principal.</span></span>

<span data-ttu-id="bb94f-106">Роли приложений, назначенные субъектам служб, также называются [разрешениями приложений](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="bb94f-106">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="bb94f-107">Разрешения приложения могут быть предоставлены непосредственно с назначениями ролей приложения или с помощью [согласия пользователя](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="bb94f-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="bb94f-108">Чтобы предоставить назначение роли приложения, вам потребуется три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="bb94f-108">To grant an app role assignment, you need three identifiers:</span></span>

- <span data-ttu-id="bb94f-109">`principalId`: `id` **Пользователь**, **Группа** или клиент **servicePrincipal** , которому назначается роль приложения.</span><span class="sxs-lookup"><span data-stu-id="bb94f-109">`principalId`: The `id` of the **user**, **group** or client **servicePrincipal** to which you are assigning the app role.</span></span>
- <span data-ttu-id="bb94f-110">`resourceId`: `id` Ресурс **servicePrincipal** , в котором определена роль приложения.</span><span class="sxs-lookup"><span data-stu-id="bb94f-110">`resourceId`: The `id` of the resource **servicePrincipal** which has defined the app role.</span></span>
- <span data-ttu-id="bb94f-111">`appRoleId`: Объект `id` **аппроле** (определенный для субъекта-службы ресурса), назначаемый пользователю, группе или субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="bb94f-111">`appRoleId`: The `id` of the **appRole** (defined on the resource service principal) to assign to a user, group, or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb94f-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb94f-112">Permissions</span></span>

<span data-ttu-id="bb94f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb94f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb94f-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb94f-115">Permission type</span></span>      | <span data-ttu-id="bb94f-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb94f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb94f-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb94f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="bb94f-118">Аппролеассигнмент. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="bb94f-118">AppRoleAssignment.ReadWrite.All,Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb94f-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb94f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb94f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb94f-120">Not supported.</span></span>    |
|<span data-ttu-id="bb94f-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb94f-121">Application</span></span> | <span data-ttu-id="bb94f-122">Аппролеассигнмент. ReadWrite. ALL,</span><span class="sxs-lookup"><span data-stu-id="bb94f-122">AppRoleAssignment.ReadWrite.All,</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb94f-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb94f-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="request-headers"></a><span data-ttu-id="bb94f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb94f-124">Request headers</span></span>

| <span data-ttu-id="bb94f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="bb94f-125">Name</span></span>       | <span data-ttu-id="bb94f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="bb94f-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="bb94f-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb94f-127">Authorization</span></span> | <span data-ttu-id="bb94f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb94f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bb94f-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb94f-130">Content-type</span></span> | <span data-ttu-id="bb94f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb94f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb94f-133">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb94f-133">Request body</span></span>

<span data-ttu-id="bb94f-134">В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb94f-134">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bb94f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb94f-135">Response</span></span>

<span data-ttu-id="bb94f-136">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb94f-136">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb94f-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="bb94f-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb94f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb94f-138">Request</span></span>

<span data-ttu-id="bb94f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb94f-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bb94f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb94f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_approleassignedto"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignedTo
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="bb94f-141">C#</span><span class="sxs-lookup"><span data-stu-id="bb94f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb94f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb94f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb94f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb94f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb94f-144">Java</span><span class="sxs-lookup"><span data-stu-id="bb94f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="bb94f-145">В этом примере `{id}` и будет `{resourceId-value}` `id` назначена субъектом службы ресурсов, и будет `{principalId}` `id` назначен участник службы, назначенный пользователю, группе или клиенту.</span><span class="sxs-lookup"><span data-stu-id="bb94f-145">In this example, `{id}` and `{resourceId-value}` would both be the `id` of the resource service principal, and `{principalId}` would be the `id` of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="bb94f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb94f-146">Response</span></span>

<span data-ttu-id="bb94f-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb94f-147">Here is an example of the response.</span></span> 

> <span data-ttu-id="bb94f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb94f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
