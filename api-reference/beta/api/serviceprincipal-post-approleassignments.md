---
title: Предоставление appRoleAssignment субъекту-службе
description: Предоставление назначения роли приложения субъекту-службе
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: ca0f3a2837062bacf592c100c4f92532483a8399
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076806"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a><span data-ttu-id="7cf62-103">Предоставление appRoleAssignment субъекту-службе</span><span class="sxs-lookup"><span data-stu-id="7cf62-103">Grant an appRoleAssignment to a service principal</span></span>

<span data-ttu-id="7cf62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cf62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7cf62-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cf62-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cf62-106">Назначьте роль приложения субъекту-службе клиента.</span><span class="sxs-lookup"><span data-stu-id="7cf62-106">Assign an app role to a client service principal.</span></span>

<span data-ttu-id="7cf62-107">Роли приложений, назначаемые субъектам-службам, также называются [разрешениями приложений](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="7cf62-107">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="7cf62-108">Разрешения приложения можно предоставлять непосредственно в назначениях ролей приложений, а также с помощью [интерфейса согласия](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="7cf62-108">Application permissions can be granted directly with app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="7cf62-109">Чтобы предоставить назначение роли приложения субъекту-службе клиента, нужны три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="7cf62-109">To grant an app role assignment to a client service principal, you need three identifiers:</span></span>

- <span data-ttu-id="7cf62-110">`principalId`: `id` субъекта-службы клиента, которой нужно назначить роль приложения.</span><span class="sxs-lookup"><span data-stu-id="7cf62-110">`principalId`: The `id` of the client service principal to which you are assigning the app role.</span></span>
- <span data-ttu-id="7cf62-111">`resourceId`: `id` ресурса `servicePrincipal` (API), в которых определена роль приложения (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="7cf62-111">`resourceId`: The `id` of the resource `servicePrincipal` (the API) which has defined the app role (the application permission).</span></span>
- <span data-ttu-id="7cf62-112">`appRoleId`: `id` объекта `appRole` (определенного в субъекте-службе ресурса) для назначения субъекту-службе клиента.</span><span class="sxs-lookup"><span data-stu-id="7cf62-112">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the client service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cf62-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7cf62-113">Permissions</span></span>

<span data-ttu-id="7cf62-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cf62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cf62-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cf62-116">Permission type</span></span>      | <span data-ttu-id="7cf62-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cf62-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cf62-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cf62-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7cf62-119">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7cf62-119">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7cf62-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cf62-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cf62-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cf62-121">Not supported.</span></span>    |
|<span data-ttu-id="7cf62-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cf62-122">Application</span></span> | <span data-ttu-id="7cf62-123">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf62-123">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cf62-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cf62-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="7cf62-125">Рекомендуется создавать назначения ролей приложения, используя [`appRoleAssignedTo`отношение _ресурса_ субъекта-службы](serviceprincipal-post-approleassignedto.md) вместо `appRoleAssignments`отношения назначенного пользователя, группы или субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="7cf62-125">As a best practice, we recommend creating app role assignments through the [`appRoleAssignedTo` relationship of the _resource_ service principal](serviceprincipal-post-approleassignedto.md), instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7cf62-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cf62-126">Request headers</span></span>

| <span data-ttu-id="7cf62-127">Имя</span><span class="sxs-lookup"><span data-stu-id="7cf62-127">Name</span></span>       | <span data-ttu-id="7cf62-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7cf62-128">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7cf62-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7cf62-129">Authorization</span></span> | <span data-ttu-id="7cf62-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cf62-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7cf62-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7cf62-132">Content-type</span></span> | <span data-ttu-id="7cf62-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cf62-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cf62-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cf62-135">Request body</span></span>

<span data-ttu-id="7cf62-136">В тексте запроса укажите представление JSON объекта [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7cf62-136">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7cf62-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cf62-137">Response</span></span>

<span data-ttu-id="7cf62-138">В случае успеха этот метод возвращает код отклика `201 Created` и объект [appRoleAssignment](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7cf62-138">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7cf62-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="7cf62-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7cf62-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cf62-140">Request</span></span>

<span data-ttu-id="7cf62-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cf62-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7cf62-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf62-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7cf62-143">C#</span><span class="sxs-lookup"><span data-stu-id="7cf62-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cf62-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cf62-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cf62-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cf62-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="7cf62-146">В этом примере `{id}` и `{principalId-value}` оба будут `id` назначенного субъекта-службы клиента, а `{resoruceId}` будет `id` субъектом-службой ресурса (API).</span><span class="sxs-lookup"><span data-stu-id="7cf62-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned client service principal, and `{resoruceId}` would be the `id` of the resource service principal (the API).</span></span>

### <a name="response"></a><span data-ttu-id="7cf62-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cf62-147">Response</span></span>

<span data-ttu-id="7cf62-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7cf62-148">Here is an example of the response.</span></span> 

> <span data-ttu-id="7cf62-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7cf62-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


