---
title: Создание oAuth2PermissionGrant
description: Создание объекта oAuth2PermissionGrant, представляющего делегированное предоставление разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: cde41b8193d535a4911c56464a539f518aca570f
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383667"
---
# <a name="create-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="c0b61-103">Создание делегированного предоставления разрешений (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="c0b61-103">Create a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="c0b61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0b61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0b61-105">Создайте делегированное предоставление разрешений.</span><span class="sxs-lookup"><span data-stu-id="c0b61-105">Create a delegated permission grant.</span></span> <span data-ttu-id="c0b61-106">Делегированное предоставление разрешений представлено объектом [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .</span><span class="sxs-lookup"><span data-stu-id="c0b61-106">A delegated permission grant is represented by an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

<span data-ttu-id="c0b61-107">Делегированное разрешение предоставляет субъекту-клиенту (представляющему клиентское приложение) доступ к субъекту-службе ресурсов (представляющему API), от имени пользователя, выполнившего вход, для уровня доступа, ограниченного делегированными разрешениями, которые были предоставлены.</span><span class="sxs-lookup"><span data-stu-id="c0b61-107">A delegated permission grant authorizes a client service principal (representing a client application) to access a resource service principal (representing an API), on behalf of a signed-in user, for the level of access limited by the delegated permissions which were granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0b61-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0b61-108">Permissions</span></span>

<span data-ttu-id="c0b61-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0b61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0b61-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0b61-111">Permission type</span></span>      | <span data-ttu-id="c0b61-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0b61-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0b61-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0b61-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c0b61-114">Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c0b61-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0b61-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0b61-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0b61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0b61-116">Not supported.</span></span>    |
|<span data-ttu-id="c0b61-117">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="c0b61-117">Application</span></span> | <span data-ttu-id="c0b61-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0b61-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0b61-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0b61-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a><span data-ttu-id="c0b61-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0b61-120">Request headers</span></span>

| <span data-ttu-id="c0b61-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c0b61-121">Name</span></span>       | <span data-ttu-id="c0b61-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c0b61-122">Type</span></span> | <span data-ttu-id="c0b61-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c0b61-123">Description</span></span> |
|:-----------|:------|:----------|
| <span data-ttu-id="c0b61-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0b61-124">Authorization</span></span>  | <span data-ttu-id="c0b61-125">string</span><span class="sxs-lookup"><span data-stu-id="c0b61-125">string</span></span>  | <span data-ttu-id="c0b61-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0b61-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0b61-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0b61-128">Request body</span></span>

<span data-ttu-id="c0b61-129">В тексте запроса добавьте представление объекта [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0b61-129">In the request body, supply a JSON representation of an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c0b61-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0b61-130">Response</span></span>

<span data-ttu-id="c0b61-131">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0b61-131">If successful, this method returns a 200-series response code and a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0b61-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c0b61-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0b61-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0b61-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c0b61-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0b61-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c0b61-135">C#</span><span class="sxs-lookup"><span data-stu-id="c0b61-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0b61-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0b61-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0b61-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0b61-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0b61-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0b61-138">Response</span></span>

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
