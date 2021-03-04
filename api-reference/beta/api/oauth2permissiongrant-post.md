---
title: Создание oAuth2PermissionGrant
description: Создайте объект oAuth2PermissionGrant, представляющий делегированную выдачу разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: e97cadee5e116104beb158a9977ab02c159eb43b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447960"
---
# <a name="create-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="0ad1f-103">Создание делегированного разрешения (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="0ad1f-103">Create a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="0ad1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ad1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ad1f-105">Создание делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="0ad1f-105">Create a delegated permission grant.</span></span> <span data-ttu-id="0ad1f-106">Делегированная выдача разрешений представлена объектом [oAuth2PermissionGrant.](../resources/oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="0ad1f-106">A delegated permission grant is represented by an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

<span data-ttu-id="0ad1f-107">Делегированная выдача разрешений разрешает директору клиентской службы (представляющим клиентскую заявку) получать доступ к директору службы ресурсов (представляющим API) от имени подписанного пользователя, для уровня доступа, ограниченного делегированных разрешений, которые были предоставлены.</span><span class="sxs-lookup"><span data-stu-id="0ad1f-107">A delegated permission grant authorizes a client service principal (representing a client application) to access a resource service principal (representing an API), on behalf of a signed-in user, for the level of access limited by the delegated permissions which were granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ad1f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ad1f-108">Permissions</span></span>

<span data-ttu-id="0ad1f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ad1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ad1f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ad1f-111">Permission type</span></span>      | <span data-ttu-id="0ad1f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ad1f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ad1f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ad1f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0ad1f-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ad1f-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0ad1f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ad1f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ad1f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ad1f-116">Not supported.</span></span>    |
|<span data-ttu-id="0ad1f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ad1f-117">Application</span></span> | <span data-ttu-id="0ad1f-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ad1f-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ad1f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ad1f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a><span data-ttu-id="0ad1f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ad1f-120">Request headers</span></span>

| <span data-ttu-id="0ad1f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0ad1f-121">Name</span></span>       | <span data-ttu-id="0ad1f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="0ad1f-122">Type</span></span> | <span data-ttu-id="0ad1f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0ad1f-123">Description</span></span> |
|:-----------|:------|:----------|
| <span data-ttu-id="0ad1f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ad1f-124">Authorization</span></span>  | <span data-ttu-id="0ad1f-125">string</span><span class="sxs-lookup"><span data-stu-id="0ad1f-125">string</span></span>  | <span data-ttu-id="0ad1f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ad1f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ad1f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ad1f-128">Request body</span></span>

<span data-ttu-id="0ad1f-129">В теле запроса поставляем представление JSON объекта [oAuth2PermissionGrant.](../resources/oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="0ad1f-129">In the request body, supply a JSON representation of an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0ad1f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ad1f-130">Response</span></span>

<span data-ttu-id="0ad1f-131">В случае успешной работы этот метод возвращает код отклика 200-й серии и новый [объект oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ad1f-131">If successful, this method returns a 200-series response code and a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ad1f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0ad1f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ad1f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ad1f-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0ad1f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ad1f-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0ad1f-135">C#</span><span class="sxs-lookup"><span data-stu-id="0ad1f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ad1f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ad1f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ad1f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ad1f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ad1f-138">Java</span><span class="sxs-lookup"><span data-stu-id="0ad1f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0ad1f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ad1f-139">Response</span></span>

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


