---
title: Предоставление appRoleAssignment субъекту-службе
description: Предоставляйте назначение роли приложения субъекту-службе.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 2f664742481dd289582f017b83142ec5db10918f
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060472"
---
# <a name="grant-an-approleassignment-for-a-service-principal"></a><span data-ttu-id="41e8f-103">Предоставление appRoleAssignment субъекту-службе</span><span class="sxs-lookup"><span data-stu-id="41e8f-103">Grant an appRoleAssignment for a service principal</span></span>

<span data-ttu-id="41e8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41e8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41e8f-105">Назначение роли приложения для этого субъекта-службы пользователю, группе или субъекту-службе клиента.</span><span class="sxs-lookup"><span data-stu-id="41e8f-105">Assign an app role for a resource service principal, to a user, group, or client service principal.</span></span>

<span data-ttu-id="41e8f-106">Роли приложений, назначаемые субъектам-службам, также называются [разрешениями приложений](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="41e8f-106">App roles that are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="41e8f-107">Разрешения приложений можно предоставлять непосредственно в назначениях ролей приложений, а также с помощью [интерфейса согласия](/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="41e8f-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="41e8f-108">Чтобы предоставить назначение роли приложения, нужны три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="41e8f-108">To grant an app role assignment, you need three identifiers:</span></span>

- <span data-ttu-id="41e8f-109">`principalId`: `id` **пользователя**, **группы** или объекта **servicePrincipal** клиента, которому назначается роль приложения.</span><span class="sxs-lookup"><span data-stu-id="41e8f-109">`principalId`: The `id` of the **user**, **group** or client **servicePrincipal** to which you are assigning the app role.</span></span>
- <span data-ttu-id="41e8f-110">`resourceId`: `id` ресурса **servicePrincipal**, определяющий роль приложения.</span><span class="sxs-lookup"><span data-stu-id="41e8f-110">`resourceId`: The `id` of the resource **servicePrincipal** which has defined the app role.</span></span>
- <span data-ttu-id="41e8f-111">`appRoleId`: `id` объекта **appRole** (определенного в субъекте-службе ресурса) для назначения пользователю, группе или субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="41e8f-111">`appRoleId`: The `id` of the **appRole** (defined on the resource service principal) to assign to a user, group, or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="41e8f-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41e8f-112">Permissions</span></span>

<span data-ttu-id="41e8f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41e8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41e8f-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41e8f-115">Permission type</span></span>      | <span data-ttu-id="41e8f-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41e8f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41e8f-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41e8f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="41e8f-118">AppRoleAssignment.ReadWrite.All и Application.Read.All, AppRoleAssignment.ReadWrite.All и Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41e8f-118">AppRoleAssignment.ReadWrite.All and Application.Read.All, AppRoleAssignment.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41e8f-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41e8f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41e8f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41e8f-120">Not supported.</span></span>    |
|<span data-ttu-id="41e8f-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="41e8f-121">Application</span></span> | <span data-ttu-id="41e8f-122">AppRoleAssignment.ReadWrite.All и Application.Read.All, AppRoleAssignment.ReadWrite.All и Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41e8f-122">AppRoleAssignment.ReadWrite.All and Application.Read.All, AppRoleAssignment.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41e8f-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41e8f-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="request-headers"></a><span data-ttu-id="41e8f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41e8f-124">Request headers</span></span>

| <span data-ttu-id="41e8f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="41e8f-125">Name</span></span>       | <span data-ttu-id="41e8f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="41e8f-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="41e8f-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41e8f-127">Authorization</span></span> | <span data-ttu-id="41e8f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41e8f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="41e8f-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41e8f-130">Content-type</span></span> | <span data-ttu-id="41e8f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41e8f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41e8f-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41e8f-133">Request body</span></span>

<span data-ttu-id="41e8f-134">В тексте запроса укажите представление JSON для объекта [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="41e8f-134">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="41e8f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="41e8f-135">Response</span></span>

<span data-ttu-id="41e8f-136">В случае успеха этот метод возвращает в тексте отклика код отклика `201 Created` и объект [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="41e8f-136">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41e8f-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="41e8f-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41e8f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="41e8f-138">Request</span></span>

<span data-ttu-id="41e8f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41e8f-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="41e8f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="41e8f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_approleassignedto"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignedTo
Content-Type: application/json

{
  "principalId": "33ad69f9-da99-4bed-acd0-3f24235cb296",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7"
}
```
# <a name="c"></a>[<span data-ttu-id="41e8f-141">C#</span><span class="sxs-lookup"><span data-stu-id="41e8f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41e8f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41e8f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41e8f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41e8f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41e8f-144">Java</span><span class="sxs-lookup"><span data-stu-id="41e8f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="41e8f-145">В этом примере `{id}` и `{resourceId-value}` оба будут `id` субъекта-службы ресурса, а `{principalId}` будет `id` назначенного пользователя, группы или субъекта-службы клиента.</span><span class="sxs-lookup"><span data-stu-id="41e8f-145">In this example, `{id}` and `{resourceId-value}` would both be the `id` of the resource service principal, and `{principalId}` would be the `id` of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="41e8f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="41e8f-146">Response</span></span>

<span data-ttu-id="41e8f-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="41e8f-147">Here is an example of the response.</span></span> 

> <span data-ttu-id="41e8f-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="41e8f-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('9028d19c-26a9-4809-8e3f-20ff73e2d75e')/appRoleAssignedTo/$entity",
  "id": "-WmtM5na7Uus0D8kI1yylpU9Mdo0Pb9OoBJvd3T5eKc",
  "deletedDateTime": null,
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7",
  "creationTimestamp": "2021-02-15T16:14:59.8643039Z",
  "principalDisplayName": "Parents of Contoso",
  "principalId": "33ad69f9-da99-4bed-acd0-3f24235cb296",
  "principalType": "Group",
  "resourceDisplayName": "Fabrikam App",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
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
