---
title: Предоставление appRoleAssignment субъекту-службе
description: Предоставление назначения роли приложения субъекту-службе
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 615eb0555f1f262cb399e11b844425eb8b370aa0
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223510"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a><span data-ttu-id="cc8d3-103">Предоставление appRoleAssignment субъекту-службе</span><span class="sxs-lookup"><span data-stu-id="cc8d3-103">Grant an appRoleAssignment to a service principal</span></span>

<span data-ttu-id="cc8d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc8d3-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="cc8d3-105">Назначьте роль приложения субъекту-службе клиента.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-105">Assign an app role to a client service principal.</span></span>

<span data-ttu-id="cc8d3-106">Роли приложений, назначаемые субъектам-службам, также называются [разрешениями приложений](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="cc8d3-106">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="cc8d3-107">Разрешения приложения можно предоставлять непосредственно в назначениях ролей приложений, а также с помощью [интерфейса согласия](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="cc8d3-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="cc8d3-108">Чтобы предоставить назначение роли приложения субъекту-службе клиента, нужны три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="cc8d3-108">To grant an app role assignment to a client service principal, you need three identifiers:</span></span>

- <span data-ttu-id="cc8d3-109">`principalId`: `id` субъекта-службы клиента, которой нужно назначить роль приложения.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-109">`principalId`: The `id` of the client service principal to which you are assigning the app role.</span></span>
- <span data-ttu-id="cc8d3-110">`resourceId`: `id` ресурса `servicePrincipal` (API), в которых определена роль приложения (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="cc8d3-110">`resourceId`: The `id` of the resource `servicePrincipal` (the API) which has defined the app role (the application permission).</span></span>
- <span data-ttu-id="cc8d3-111">`appRoleId`: `id` объекта `appRole` (определенного в субъекте-службе ресурса) для назначения субъекту-службе клиента.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-111">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the client service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc8d3-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc8d3-112">Permissions</span></span>

<span data-ttu-id="cc8d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc8d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc8d3-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc8d3-115">Permission type</span></span>      | <span data-ttu-id="cc8d3-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc8d3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc8d3-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc8d3-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cc8d3-118">AppRoleAssignment.ReadWrite.All,Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc8d3-118">AppRoleAssignment.ReadWrite.All,Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cc8d3-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc8d3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc8d3-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-120">Not supported.</span></span>    |
|<span data-ttu-id="cc8d3-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc8d3-121">Application</span></span> | <span data-ttu-id="cc8d3-122">AppRoleAssignment.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="cc8d3-122">AppRoleAssignment.ReadWrite.All,</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc8d3-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc8d3-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="cc8d3-124">Рекомендуется создавать назначения ролей приложения, используя [`appRoleAssignedTo`отношение _ресурса_ субъекта-службы](serviceprincipal-post-approleassignedto.md) вместо `appRoleAssignments`отношения назначенного пользователя, группы или субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-124">As a best practice, we recommend creating app role assignments through the [`appRoleAssignedTo` relationship of the _resource_ service principal](serviceprincipal-post-approleassignedto.md), instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc8d3-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc8d3-125">Request headers</span></span>

| <span data-ttu-id="cc8d3-126">Имя</span><span class="sxs-lookup"><span data-stu-id="cc8d3-126">Name</span></span>       | <span data-ttu-id="cc8d3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="cc8d3-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="cc8d3-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc8d3-128">Authorization</span></span> | <span data-ttu-id="cc8d3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc8d3-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc8d3-131">Content-type</span></span> | <span data-ttu-id="cc8d3-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc8d3-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc8d3-134">Request body</span></span>

<span data-ttu-id="cc8d3-135">В тексте запроса укажите представление JSON для объекта [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cc8d3-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cc8d3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc8d3-136">Response</span></span>

<span data-ttu-id="cc8d3-137">В случае успеха этот метод возвращает в тексте отклика код отклика `201 Created` и объект [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cc8d3-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc8d3-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc8d3-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc8d3-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc8d3-139">Request</span></span>

<span data-ttu-id="cc8d3-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc8d3-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc8d3-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="cc8d3-142">C#</span><span class="sxs-lookup"><span data-stu-id="cc8d3-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc8d3-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc8d3-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc8d3-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc8d3-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc8d3-145">Java</span><span class="sxs-lookup"><span data-stu-id="cc8d3-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="cc8d3-146">В этом примере `{id}` и `{principalId-value}` оба будут `id` назначенного субъекта-службы клиента, а `{resourceId}` будет `id` субъектом-службой ресурса (API).</span><span class="sxs-lookup"><span data-stu-id="cc8d3-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned client service principal, and `{resourceId}` would be the `id` of the resource service principal (the API).</span></span>

### <a name="response"></a><span data-ttu-id="cc8d3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc8d3-147">Response</span></span>

<span data-ttu-id="cc8d3-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-148">Here is an example of the response.</span></span> 

> <span data-ttu-id="cc8d3-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

