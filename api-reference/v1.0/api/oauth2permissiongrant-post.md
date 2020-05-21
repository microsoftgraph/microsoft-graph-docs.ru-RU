---
title: Создание oAuth2PermissionGrant
description: Создание объекта oAuth2PermissionGrant, представляющего делегированное предоставление разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: f9648cf3ef2635a0cbb838080c01249eb0a526a0
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334492"
---
# <a name="create-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="6becf-103">Создание делегированного предоставления разрешений (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="6becf-103">Create a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="6becf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6becf-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="6becf-105">Создайте делегированное предоставление разрешений.</span><span class="sxs-lookup"><span data-stu-id="6becf-105">Create a delegated permission grant.</span></span> <span data-ttu-id="6becf-106">Делегированное предоставление разрешений представлено объектом [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .</span><span class="sxs-lookup"><span data-stu-id="6becf-106">A delegated permission grant is represented by an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

<span data-ttu-id="6becf-107">Делегированное разрешение предоставляет субъекту-клиенту (представляющему клиентское приложение) доступ к субъекту-службе ресурсов (представляющему API), от имени пользователя, выполнившего вход, для уровня доступа, ограниченного делегированными разрешениями, которые были предоставлены.</span><span class="sxs-lookup"><span data-stu-id="6becf-107">A delegated permission grant authorizes a client service principal (representing a client application) to access a resource service principal (representing an API), on behalf of a signed-in user, for the level of access limited by the delegated permissions which were granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="6becf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6becf-108">Permissions</span></span>

<span data-ttu-id="6becf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6becf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6becf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6becf-111">Permission type</span></span>      | <span data-ttu-id="6becf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6becf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6becf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6becf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6becf-114">Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="6becf-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6becf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6becf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6becf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6becf-116">Not supported.</span></span>    |
|<span data-ttu-id="6becf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6becf-117">Application</span></span> | <span data-ttu-id="6becf-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6becf-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6becf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6becf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a><span data-ttu-id="6becf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6becf-120">Request headers</span></span>

| <span data-ttu-id="6becf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6becf-121">Name</span></span>       | <span data-ttu-id="6becf-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6becf-122">Type</span></span> | <span data-ttu-id="6becf-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6becf-123">Description</span></span> |
|:-----------|:------|:----------|
| <span data-ttu-id="6becf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6becf-124">Authorization</span></span>  | <span data-ttu-id="6becf-125">string</span><span class="sxs-lookup"><span data-stu-id="6becf-125">string</span></span>  | <span data-ttu-id="6becf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6becf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6becf-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6becf-128">Request body</span></span>

<span data-ttu-id="6becf-129">В тексте запроса добавьте представление объекта [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6becf-129">In the request body, supply a JSON representation of an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6becf-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6becf-130">Response</span></span>

<span data-ttu-id="6becf-131">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6becf-131">If successful, this method returns a 200-series response code and a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6becf-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6becf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6becf-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6becf-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6becf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6becf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_oAuth2PermissionGrant"
}-->

```http
POST https://graph.microsoft.com/v1.0/oauth2PermissionGrants
Content-Type: application/json
Content-Length: 30

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6becf-135">C#</span><span class="sxs-lookup"><span data-stu-id="6becf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6becf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6becf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6becf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6becf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6becf-138">Java</span><span class="sxs-lookup"><span data-stu-id="6becf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6becf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6becf-139">Response</span></span>

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
  "scope": "scope-value"
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
