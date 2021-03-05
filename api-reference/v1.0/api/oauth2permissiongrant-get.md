---
title: Получить oAuth2PermissionGrant
description: Извлечение свойств и связей одного oAuth2PermissionGrant, представляющего делегированную лицензию.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 5a268a5801ee5202bd6621b4f7f05aac39a0fb86
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448216"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="18989-103">Получить делегированную субсидию разрешений (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="18989-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="18989-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18989-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18989-105">Извлечение свойств одного [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="18989-105">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="18989-106">**OAuth2PermissionGrant** представляет делегированную разрешений, которые были предоставлены для клиентского приложения для доступа к API от имени подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="18989-106">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="18989-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18989-107">Permissions</span></span>

<span data-ttu-id="18989-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18989-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18989-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18989-110">Permission type</span></span>      | <span data-ttu-id="18989-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18989-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18989-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18989-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18989-113">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18989-113">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="18989-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18989-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18989-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18989-115">Not supported.</span></span>    |
|<span data-ttu-id="18989-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18989-116">Application</span></span> | <span data-ttu-id="18989-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18989-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18989-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18989-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18989-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18989-119">Optional query parameters</span></span>

<span data-ttu-id="18989-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="18989-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18989-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18989-121">Request headers</span></span>

| <span data-ttu-id="18989-122">Имя</span><span class="sxs-lookup"><span data-stu-id="18989-122">Name</span></span>       | <span data-ttu-id="18989-123">Тип</span><span class="sxs-lookup"><span data-stu-id="18989-123">Type</span></span> | <span data-ttu-id="18989-124">Описание</span><span class="sxs-lookup"><span data-stu-id="18989-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="18989-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="18989-125">Authorization</span></span>  | <span data-ttu-id="18989-126">string</span><span class="sxs-lookup"><span data-stu-id="18989-126">string</span></span>  | <span data-ttu-id="18989-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18989-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18989-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18989-129">Request body</span></span>

<span data-ttu-id="18989-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18989-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18989-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="18989-131">Response</span></span>

<span data-ttu-id="18989-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="18989-132">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18989-133">Пример</span><span class="sxs-lookup"><span data-stu-id="18989-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="18989-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="18989-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="18989-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="18989-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
```
# <a name="c"></a>[<span data-ttu-id="18989-136">C#</span><span class="sxs-lookup"><span data-stu-id="18989-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18989-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18989-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18989-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18989-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18989-139">Java</span><span class="sxs-lookup"><span data-stu-id="18989-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18989-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="18989-140">Response</span></span>

> <span data-ttu-id="18989-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18989-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "scope": "scope-value"
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

