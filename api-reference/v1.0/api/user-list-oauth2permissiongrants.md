---
title: Перечисление oauth2PermissionGrants
description: Извлечение списка объектов oAuth2PermissionGrant, представляющих предоставленные делегированные разрешения.
localization_priority: Priority
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 412fd819e460b83eaed8ad789bd3a3ded6aa58d6
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232083"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="4f8e8-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="4f8e8-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="4f8e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f8e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f8e8-105">Извлечение списка объектов [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md), представляющих делегированные разрешения, предоставленные клиентскому приложению для доступа к API от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, which represent delegated permissions granted to enable a client application to access an API on behalf of the user.</span></span>

> [!NOTE]
> <span data-ttu-id="4f8e8-106">При запросе предоставленных делегированных разрешений для пользователя будут возвращаться только предоставленные делегированные разрешения, предназначенные для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-106">Querying the delegated permission grants for a user will only return delegated permissions grants that are specifically for the given user.</span></span> <span data-ttu-id="4f8e8-107">Делегированные разрешения, предоставленные от имени всех пользователей в организации, _не_ включаются в ответ.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-107">Delegated permissions granted on behalf of all users in the organization are _not_ included in the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4f8e8-108">При запросе могут происходить задержки репликации для предоставленных делегированных разрешений, которые были недавно созданы, обновлены или удалены.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-108">This request might have replication delays for delegated permission grants that were recently created, updated, or deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f8e8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f8e8-109">Permissions</span></span>

<span data-ttu-id="4f8e8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f8e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f8e8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f8e8-112">Permission type</span></span>      | <span data-ttu-id="4f8e8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f8e8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f8e8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f8e8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4f8e8-115">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4f8e8-115">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="4f8e8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f8e8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f8e8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-117">Not supported.</span></span>    |
|<span data-ttu-id="4f8e8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f8e8-118">Application</span></span> | <span data-ttu-id="4f8e8-119">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f8e8-119">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f8e8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f8e8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/oauth2PermissionGrants
GET /users/{id | userPrincipalName}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f8e8-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f8e8-121">Optional query parameters</span></span>

<span data-ttu-id="4f8e8-122">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f8e8-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f8e8-123">Request headers</span></span>

| <span data-ttu-id="4f8e8-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4f8e8-124">Name</span></span>           | <span data-ttu-id="4f8e8-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4f8e8-125">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="4f8e8-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f8e8-126">Authorization</span></span>  | <span data-ttu-id="4f8e8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f8e8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f8e8-129">Request body</span></span>

<span data-ttu-id="4f8e8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f8e8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f8e8-131">Response</span></span>

<span data-ttu-id="4f8e8-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-132">If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f8e8-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="4f8e8-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f8e8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f8e8-134">Request</span></span>

<span data-ttu-id="4f8e8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-135">Here is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="4f8e8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f8e8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="4f8e8-137">C#</span><span class="sxs-lookup"><span data-stu-id="4f8e8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f8e8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f8e8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f8e8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f8e8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f8e8-140">Java</span><span class="sxs-lookup"><span data-stu-id="4f8e8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f8e8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f8e8-141">Response</span></span>

<span data-ttu-id="4f8e8-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-142">Here is an example of the response.</span></span> 

> <span data-ttu-id="4f8e8-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f8e8-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "clientId": "85477313-ea43-4c7d-b8a4-54fed35d0b60",
      "consentType": "Principal",
      "id": "E3NHhUPqfUy4pFT-010LYFo5-ycA-_5Fhl7nHbaJ7qACy1R9o6oWQJ-cpLSUIt2b",
      "principalId": "7d54cb02-aaa3-4016-9f9c-a4b49422dd9b",
      "resourceId": "27fb395a-fb00-45fe-865e-e71db689eea0",
      "scope": " Contacts.ReadWrite openid profile"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

