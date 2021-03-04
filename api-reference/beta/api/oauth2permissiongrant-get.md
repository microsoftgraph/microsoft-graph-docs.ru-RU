---
title: Получить oAuth2PermissionGrant
description: Извлечение свойств и связей одного oAuth2PermissionGrant, представляющего делегированную лицензию.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 4919e2e664ba3af1d3b74c8af9f7f5047c915a16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442387"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="38a6a-103">Получить делегированную субсидию разрешений (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="38a6a-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="38a6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38a6a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38a6a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38a6a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a6a-106">Извлечение свойств одного [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="38a6a-106">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="38a6a-107">**OAuth2PermissionGrant** представляет делегированную разрешений, которые были предоставлены для клиентского приложения для доступа к API от имени подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="38a6a-107">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="38a6a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38a6a-108">Permissions</span></span>

<span data-ttu-id="38a6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38a6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38a6a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38a6a-111">Permission type</span></span>      | <span data-ttu-id="38a6a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38a6a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38a6a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38a6a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="38a6a-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="38a6a-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="38a6a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38a6a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38a6a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38a6a-116">Not supported.</span></span>    |
|<span data-ttu-id="38a6a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38a6a-117">Application</span></span> | <span data-ttu-id="38a6a-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38a6a-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38a6a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38a6a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38a6a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38a6a-120">Optional query parameters</span></span>

<span data-ttu-id="38a6a-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="38a6a-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38a6a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38a6a-122">Request headers</span></span>

| <span data-ttu-id="38a6a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="38a6a-123">Name</span></span>       | <span data-ttu-id="38a6a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="38a6a-124">Type</span></span> | <span data-ttu-id="38a6a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="38a6a-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="38a6a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="38a6a-126">Authorization</span></span>  | <span data-ttu-id="38a6a-127">string</span><span class="sxs-lookup"><span data-stu-id="38a6a-127">string</span></span>  | <span data-ttu-id="38a6a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38a6a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38a6a-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38a6a-130">Request body</span></span>

<span data-ttu-id="38a6a-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38a6a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38a6a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="38a6a-132">Response</span></span>

<span data-ttu-id="38a6a-133">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="38a6a-133">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38a6a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="38a6a-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="38a6a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="38a6a-135">Request</span></span>

<span data-ttu-id="38a6a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38a6a-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38a6a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="38a6a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2PermissionGrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="38a6a-138">C#</span><span class="sxs-lookup"><span data-stu-id="38a6a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38a6a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38a6a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38a6a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38a6a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38a6a-141">Java</span><span class="sxs-lookup"><span data-stu-id="38a6a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="38a6a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="38a6a-142">Response</span></span>

<span data-ttu-id="38a6a-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="38a6a-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="38a6a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38a6a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


