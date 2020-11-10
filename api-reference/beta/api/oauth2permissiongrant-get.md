---
title: Получение oAuth2PermissionGrant
description: Получение свойств и связей одного oAuth2PermissionGrant, представляющих делегированное предоставление разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 2a5a48b2a96717a749ca400c47ce56b5b807de80
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967574"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="7c3ec-103">Получение делегированного разрешения Grant (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="7c3ec-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="7c3ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c3ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c3ec-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c3ec-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c3ec-106">Получение свойств одного объекта [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="7c3ec-106">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="7c3ec-107">**OAuth2PermissionGrant** представляет делегированные разрешения, которые были предоставлены клиентскому приложению для доступа к API от имени пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="7c3ec-107">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c3ec-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c3ec-108">Permissions</span></span>

<span data-ttu-id="7c3ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c3ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c3ec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c3ec-111">Permission type</span></span>      | <span data-ttu-id="7c3ec-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c3ec-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c3ec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c3ec-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7c3ec-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7c3ec-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7c3ec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c3ec-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c3ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c3ec-116">Not supported.</span></span>    |
|<span data-ttu-id="7c3ec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c3ec-117">Application</span></span> | <span data-ttu-id="7c3ec-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c3ec-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c3ec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c3ec-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c3ec-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7c3ec-120">Optional query parameters</span></span>

<span data-ttu-id="7c3ec-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7c3ec-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c3ec-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c3ec-122">Request headers</span></span>

| <span data-ttu-id="7c3ec-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7c3ec-123">Name</span></span>       | <span data-ttu-id="7c3ec-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7c3ec-124">Type</span></span> | <span data-ttu-id="7c3ec-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7c3ec-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7c3ec-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c3ec-126">Authorization</span></span>  | <span data-ttu-id="7c3ec-127">string</span><span class="sxs-lookup"><span data-stu-id="7c3ec-127">string</span></span>  | <span data-ttu-id="7c3ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c3ec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c3ec-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c3ec-130">Request body</span></span>

<span data-ttu-id="7c3ec-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c3ec-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c3ec-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c3ec-132">Response</span></span>

<span data-ttu-id="7c3ec-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c3ec-133">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c3ec-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7c3ec-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c3ec-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c3ec-135">Request</span></span>

<span data-ttu-id="7c3ec-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c3ec-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c3ec-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c3ec-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2PermissionGrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="7c3ec-138">C#</span><span class="sxs-lookup"><span data-stu-id="7c3ec-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c3ec-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c3ec-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c3ec-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c3ec-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c3ec-141">Java</span><span class="sxs-lookup"><span data-stu-id="7c3ec-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="7c3ec-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c3ec-142">Response</span></span>

<span data-ttu-id="7c3ec-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7c3ec-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="7c3ec-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c3ec-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


