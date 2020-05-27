---
title: Предоставление Аппролеассигнмент участнику службы
description: Предоставьте участнику службы назначение роли приложения.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 8e8bc455f8b04e4a78bfcad1795917350ec8b86b
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44382666"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a><span data-ttu-id="5eae5-103">Предоставление Аппролеассигнмент участнику службы</span><span class="sxs-lookup"><span data-stu-id="5eae5-103">Grant an appRoleAssignment to a service principal</span></span>

<span data-ttu-id="5eae5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eae5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5eae5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eae5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eae5-106">Назначьте роль приложения участнику клиентской службы.</span><span class="sxs-lookup"><span data-stu-id="5eae5-106">Assign an app role to a client service principal.</span></span>

<span data-ttu-id="5eae5-107">Роли приложений, назначенные субъектам служб, также называются [разрешениями приложений](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="5eae5-107">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="5eae5-108">Разрешения приложения могут быть предоставлены непосредственно с назначениями ролей приложения или с помощью [согласия пользователя](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="5eae5-108">Application permissions can be granted directly with app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="5eae5-109">Чтобы назначить роль приложения для участника клиентской службы, необходимы три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="5eae5-109">To grant an app role assignment to a client service principal, you need three identifiers:</span></span>

- <span data-ttu-id="5eae5-110">`principalId`: `id` Клиент службы, которому назначается роль приложения.</span><span class="sxs-lookup"><span data-stu-id="5eae5-110">`principalId`: The `id` of the client service principal to which you are assigning the app role.</span></span>
- <span data-ttu-id="5eae5-111">`resourceId`: `id` Ресурс `servicePrincipal` (API), в котором определена роль приложения (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="5eae5-111">`resourceId`: The `id` of the resource `servicePrincipal` (the API) which has defined the app role (the application permission).</span></span>
- <span data-ttu-id="5eae5-112">`appRoleId`: Значение `id` `appRole` (заданное для субъекта-службы ресурса), которое необходимо назначить участнику клиентской службы.</span><span class="sxs-lookup"><span data-stu-id="5eae5-112">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the client service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eae5-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5eae5-113">Permissions</span></span>

<span data-ttu-id="5eae5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eae5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eae5-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5eae5-116">Permission type</span></span>      | <span data-ttu-id="5eae5-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5eae5-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eae5-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5eae5-118">Delegated (work or school account)</span></span> | <span data-ttu-id="5eae5-119">Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="5eae5-119">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5eae5-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5eae5-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eae5-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eae5-121">Not supported.</span></span>    |
|<span data-ttu-id="5eae5-122">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="5eae5-122">Application</span></span> | <span data-ttu-id="5eae5-123">Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5eae5-123">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eae5-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5eae5-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="5eae5-125">Рекомендуется создавать назначения ролей приложений с помощью [ `appRoleAssignedTo` отношения между субъектом службы _ресурсов_ ](serviceprincipal-post-approleassignedto.md), а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="5eae5-125">As a best practice, we recommend creating app role assignments through the [`appRoleAssignedTo` relationship of the _resource_ service principal](serviceprincipal-post-approleassignedto.md), instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5eae5-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5eae5-126">Request headers</span></span>

| <span data-ttu-id="5eae5-127">Имя</span><span class="sxs-lookup"><span data-stu-id="5eae5-127">Name</span></span>       | <span data-ttu-id="5eae5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5eae5-128">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5eae5-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5eae5-129">Authorization</span></span> | <span data-ttu-id="5eae5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5eae5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5eae5-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5eae5-132">Content-type</span></span> | <span data-ttu-id="5eae5-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5eae5-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5eae5-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5eae5-135">Request body</span></span>

<span data-ttu-id="5eae5-136">В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5eae5-136">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5eae5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eae5-137">Response</span></span>

<span data-ttu-id="5eae5-138">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5eae5-138">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5eae5-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="5eae5-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5eae5-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5eae5-140">Request</span></span>

<span data-ttu-id="5eae5-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5eae5-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5eae5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5eae5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="5eae5-143">C#</span><span class="sxs-lookup"><span data-stu-id="5eae5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5eae5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5eae5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5eae5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5eae5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5eae5-146">В этом примере и то, `{id}` и другое — это `{principalId-value}` `id` назначенный субъект-службу клиента, и будет `{resoruceId}` иметь значение `id` субъекта-службы ресурсов (API).</span><span class="sxs-lookup"><span data-stu-id="5eae5-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned client service principal, and `{resoruceId}` would be the `id` of the resource service principal (the API).</span></span>

### <a name="response"></a><span data-ttu-id="5eae5-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eae5-147">Response</span></span>

<span data-ttu-id="5eae5-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5eae5-148">Here is an example of the response.</span></span> 

> <span data-ttu-id="5eae5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5eae5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
