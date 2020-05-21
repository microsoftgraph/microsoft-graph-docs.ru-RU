---
title: Создание oAuth2PermissionGrant
description: Создание объекта oAuth2PermissionGrant, представляющего делегированное предоставление разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: eda8ea061b8b36669ecfa9adf2f9c9da4ccfd0d9
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333693"
---
# <a name="create-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="e587f-103">Создание делегированного предоставления разрешений (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="e587f-103">Create a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="e587f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e587f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e587f-105">Создайте делегированное предоставление разрешений.</span><span class="sxs-lookup"><span data-stu-id="e587f-105">Create a delegated permission grant.</span></span> <span data-ttu-id="e587f-106">Делегированное предоставление разрешений представлено объектом [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .</span><span class="sxs-lookup"><span data-stu-id="e587f-106">A delegated permission grant is represented by an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

<span data-ttu-id="e587f-107">Делегированное разрешение предоставляет субъекту-клиенту (представляющему клиентское приложение) доступ к субъекту-службе ресурсов (представляющему API), от имени пользователя, выполнившего вход, для уровня доступа, ограниченного делегированными разрешениями, которые были предоставлены.</span><span class="sxs-lookup"><span data-stu-id="e587f-107">A delegated permission grant authorizes a client service principal (representing a client application) to access a resource service principal (representing an API), on behalf of a signed-in user, for the level of access limited by the delegated permissions which were granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="e587f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e587f-108">Permissions</span></span>

<span data-ttu-id="e587f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e587f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e587f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e587f-111">Permission type</span></span>      | <span data-ttu-id="e587f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e587f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e587f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e587f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e587f-114">Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="e587f-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e587f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e587f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e587f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e587f-116">Not supported.</span></span>    |
|<span data-ttu-id="e587f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e587f-117">Application</span></span> | <span data-ttu-id="e587f-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e587f-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e587f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e587f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a><span data-ttu-id="e587f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e587f-120">Request headers</span></span>

| <span data-ttu-id="e587f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e587f-121">Name</span></span>       | <span data-ttu-id="e587f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e587f-122">Type</span></span> | <span data-ttu-id="e587f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e587f-123">Description</span></span> |
|:-----------|:------|:----------|
| <span data-ttu-id="e587f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e587f-124">Authorization</span></span>  | <span data-ttu-id="e587f-125">string</span><span class="sxs-lookup"><span data-stu-id="e587f-125">string</span></span>  | <span data-ttu-id="e587f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e587f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e587f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e587f-128">Request body</span></span>

<span data-ttu-id="e587f-129">В тексте запроса добавьте представление объекта [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e587f-129">In the request body, supply a JSON representation of an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e587f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e587f-130">Response</span></span>

<span data-ttu-id="e587f-131">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e587f-131">If successful, this method returns a 200-series response code and a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e587f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e587f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e587f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e587f-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e587f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e587f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_oAuth2PermissionGrant"
}-->

```http
POST https://graph.microsoft.com/beta/oauth2PermissionGrants
Content-Type: application/json
Content-Length: 30

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value",
  "startTime": "2016-10-19T10:37:00Z",
  "expiryTime": "2016-10-19T10:37:00Z"
}
```
# <a name="c"></a>[<span data-ttu-id="e587f-135">C#</span><span class="sxs-lookup"><span data-stu-id="e587f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e587f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e587f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e587f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e587f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e587f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e587f-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

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
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
