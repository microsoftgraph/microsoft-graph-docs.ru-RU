---
title: Предоставление appRoleAssignment субъекту-службе
description: Предоставление назначения роли приложения субъекту-службе
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 67faa1ea6448562ba4db66fd15baa46f21a71d9e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132911"
---
# <a name="grant-an-approleassignment-for-a-service-principal"></a><span data-ttu-id="6fa7a-103">Предоставление appRoleAssignment субъекту-службе</span><span class="sxs-lookup"><span data-stu-id="6fa7a-103">Grant an appRoleAssignment for a service principal</span></span>

<span data-ttu-id="6fa7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fa7a-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="6fa7a-105">Назначение роли приложения для этого субъекта-службы пользователю, группе или субъекту-службе клиента.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-105">Assign an app role for a resource service principal, to a user, group, or client service principal.</span></span>

<span data-ttu-id="6fa7a-106">Роли приложений, назначаемые субъектам-службам, также называются [разрешениями приложений](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="6fa7a-106">App roles that are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="6fa7a-107">Разрешения приложений можно предоставлять непосредственно в назначениях ролей приложений, а также с помощью [интерфейса согласия](/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="6fa7a-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="6fa7a-108">Чтобы предоставить назначение роли приложения, нужны три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="6fa7a-108">To grant an app role assignment, you need three identifiers:</span></span>

- <span data-ttu-id="6fa7a-109">`principalId`: `id` **пользователя**, **группы** или объекта **servicePrincipal** клиента, которому назначается роль приложения.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-109">`principalId`: The `id` of the **user**, **group** or client **servicePrincipal** to which you are assigning the app role.</span></span>
- <span data-ttu-id="6fa7a-110">`resourceId`: `id` ресурса **servicePrincipal**, определяющий роль приложения.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-110">`resourceId`: The `id` of the resource **servicePrincipal** which has defined the app role.</span></span>
- <span data-ttu-id="6fa7a-111">`appRoleId`: `id` объекта **appRole** (определенного в субъекте-службе ресурса) для назначения пользователю, группе или субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-111">`appRoleId`: The `id` of the **appRole** (defined on the resource service principal) to assign to a user, group, or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fa7a-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6fa7a-112">Permissions</span></span>

<span data-ttu-id="6fa7a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fa7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fa7a-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fa7a-115">Permission type</span></span>      | <span data-ttu-id="6fa7a-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fa7a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fa7a-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fa7a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="6fa7a-118">AppRoleAssignment.ReadWrite.All,Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6fa7a-118">AppRoleAssignment.ReadWrite.All,Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6fa7a-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fa7a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fa7a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-120">Not supported.</span></span>    |
|<span data-ttu-id="6fa7a-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fa7a-121">Application</span></span> | <span data-ttu-id="6fa7a-122">AppRoleAssignment.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="6fa7a-122">AppRoleAssignment.ReadWrite.All,</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fa7a-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fa7a-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="request-headers"></a><span data-ttu-id="6fa7a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fa7a-124">Request headers</span></span>

| <span data-ttu-id="6fa7a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="6fa7a-125">Name</span></span>       | <span data-ttu-id="6fa7a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6fa7a-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="6fa7a-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6fa7a-127">Authorization</span></span> | <span data-ttu-id="6fa7a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6fa7a-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6fa7a-130">Content-type</span></span> | <span data-ttu-id="6fa7a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fa7a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6fa7a-133">Request body</span></span>

<span data-ttu-id="6fa7a-134">В тексте запроса укажите представление JSON для объекта [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6fa7a-134">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6fa7a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fa7a-135">Response</span></span>

<span data-ttu-id="6fa7a-136">В случае успеха этот метод возвращает в тексте отклика код отклика `201 Created` и объект [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6fa7a-136">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6fa7a-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="6fa7a-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6fa7a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fa7a-138">Request</span></span>

<span data-ttu-id="6fa7a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6fa7a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fa7a-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6fa7a-141">C#</span><span class="sxs-lookup"><span data-stu-id="6fa7a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fa7a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fa7a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fa7a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fa7a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fa7a-144">Java</span><span class="sxs-lookup"><span data-stu-id="6fa7a-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="6fa7a-145">В этом примере `{id}` и `{resourceId-value}` оба будут `id` субъекта-службы ресурса, а `{principalId}` будет `id` назначенного пользователя, группы или субъекта-службы клиента.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-145">In this example, `{id}` and `{resourceId-value}` would both be the `id` of the resource service principal, and `{principalId}` would be the `id` of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="6fa7a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fa7a-146">Response</span></span>

<span data-ttu-id="6fa7a-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-147">Here is an example of the response.</span></span> 

> <span data-ttu-id="6fa7a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
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
