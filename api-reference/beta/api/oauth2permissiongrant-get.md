---
title: Получить oAuth2PermissionGrant
description: Извлечение свойств и связей одного oAuth2PermissionGrant, представляющего делегированную лицензию.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 05a21be27e0df9c408134556b38aa509b1881350
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038364"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="a5f78-103">Получить делегированную субсидию разрешений (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="a5f78-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="a5f78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5f78-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5f78-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5f78-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5f78-106">Извлечение свойств одного [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="a5f78-106">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="a5f78-107">**OAuth2PermissionGrant** представляет делегированную разрешений, которые были предоставлены для клиентского приложения для доступа к API от имени подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5f78-107">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5f78-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5f78-108">Permissions</span></span>

<span data-ttu-id="a5f78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5f78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5f78-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5f78-111">Permission type</span></span>      | <span data-ttu-id="a5f78-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5f78-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5f78-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5f78-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a5f78-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5f78-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5f78-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5f78-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5f78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5f78-116">Not supported.</span></span>    |
|<span data-ttu-id="a5f78-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5f78-117">Application</span></span> | <span data-ttu-id="a5f78-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f78-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5f78-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5f78-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5f78-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a5f78-120">Optional query parameters</span></span>

<span data-ttu-id="a5f78-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a5f78-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5f78-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5f78-122">Request headers</span></span>

| <span data-ttu-id="a5f78-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a5f78-123">Name</span></span>       | <span data-ttu-id="a5f78-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a5f78-124">Type</span></span> | <span data-ttu-id="a5f78-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a5f78-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5f78-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5f78-126">Authorization</span></span>  | <span data-ttu-id="a5f78-127">string</span><span class="sxs-lookup"><span data-stu-id="a5f78-127">string</span></span>  | <span data-ttu-id="a5f78-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5f78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5f78-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5f78-130">Request body</span></span>

<span data-ttu-id="a5f78-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5f78-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5f78-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5f78-132">Response</span></span>

<span data-ttu-id="a5f78-133">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5f78-133">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5f78-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a5f78-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5f78-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5f78-135">Request</span></span>

<span data-ttu-id="a5f78-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5f78-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5f78-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5f78-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2PermissionGrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="a5f78-138">C#</span><span class="sxs-lookup"><span data-stu-id="a5f78-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5f78-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5f78-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5f78-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5f78-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5f78-141">Java</span><span class="sxs-lookup"><span data-stu-id="a5f78-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a5f78-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5f78-142">Response</span></span>

<span data-ttu-id="a5f78-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5f78-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="a5f78-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5f78-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 200

{
  "id": "id-value",
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value",
  "startTime": "2016-10-19T10:37:00Z",
  "expiryTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


